---
title: Práticas recomendadas para otimizar a qualidade de suas imagens
seo-title: Práticas recomendadas para otimizar a qualidade de suas imagens
description: 'null'
seo-description: Saiba mais sobre as práticas recomendadas para otimizar a qualidade das suas imagens.
uuid: 102 e 83 fe-ee 2 a -443 b-ba 92-6 ad 5 cc 3 daef 0
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/master_ files
discoiquuid: 8164466 e -2520-482 a -88 ec -6191 fdc 77 ea 3
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Práticas recomendadas para otimizar a qualidade de suas imagens{#best-practices-for-optimizing-the-quality-of-your-images}

Otimizar a qualidade da imagem pode ser um processo demorado, pois muitos fatores contribuem para a renderização de resultados aceitáveis. O resultado é parcialmente subjetivo, pois os indivíduos percebem a qualidade da imagem de forma diferente. A experimentação estruturada é uma tecla.

O Dynamic Media Classic inclui mais de 100 comandos de disponibilização de imagens para ajustar e otimizar imagens e resultados de renderização. As orientações a seguir podem ajudá-lo a simplificar o processo e alcançar bons resultados rapidamente usando alguns comandos essenciais e práticas recomendadas.

Consulte também [Imagens inteligentes](https://helpx.adobe.com/experience-manager/6-3/assets/using/imaging-faq.html).

## Práticas recomendadas para o formato de imagem (&amp; fmt =) {#best-practices-for-image-format-fmt}

* JPG ou PNG são as melhores opções para fornecer imagens de boa qualidade e com tamanho e peso controláveis.
* Se nenhum comando de formato for fornecido no URL, o serviço de imagem de Dynamic Media assumirá como padrão o JPG para entrega.
* O JPG compacta em uma proporção de 10:1 e produz tamanhos de arquivo de imagem menores. O PNG compacta em uma proporção de aproximadamente 2:1, exceto em alguns casos, como quando as imagens contêm um plano de fundo branco. Normalmente, os tamanhos de arquivo PNG são maiores que os arquivos JPG.
* O JPG usa a compactação com perdas, o que significa que os elementos de imagem (pixels) são descartados durante a compactação. Por outro lado, o PNG usa compactação sem perdas.
* Com frequência, o JPG compacta imagens fotográficas com melhor fidelidade do que imagens sintéticas com bordas e contrastes nítidos.
* Se as imagens contiverem transparência, use PNG porque o JPG não suporta transparência.

Como prática recomendada para o formato de imagem, comece com a configuração `&fmt=JPG`mais comum.

## Práticas recomendadas para o tamanho da imagem {#best-practices-for-image-size}

Reduzir dinamicamente o tamanho da imagem é uma das tarefas mais comuns que o Serviço de imagem do Dynamic Media executa. Envolve especificar o tamanho e, opcionalmente, qual modo de redução de resolução é usado para diminuir a imagem.

* Para dimensionamento da imagem, a melhor e mais simples abordagem é usar `&wid=<value>` e `&hei=<value>` apenas `&hei=<value>`. Esses parâmetros definem automaticamente a largura da imagem de acordo com a proporção.
* `&resMode=<value>` controla o algoritmo usado para a diminuição da resolução. Comece `&resMode=sharp2`com. Esse valor fornece a melhor qualidade de imagem. Embora o valor de diminuição da resolução `=bilin` seja mais rápido, geralmente resulta na alias de artefatos.

Como prática recomendada para dimensionamento da imagem, use `&wid=<value>&hei=<value>&resMode=sharp2` ou `&hei=<value>&resMode=sharp2`

## Práticas recomendadas para a nitidez de imagens {#best-practices-for-image-sharpening}

A nitidez de imagens é o aspecto mais complexo do controle de imagens em seu site, e onde muitos erros são feitos. Aproveite o tempo para saber mais sobre como o ajuste de nitidez e a nitidez funciona no Dynamic Media Classic, fazendo referência aos seguintes recursos úteis:

Práticas recomendadas em papel de compartilhamento de [nitidez no Adobe Scene 7 Publishing System e no Servidor de imagens](https://marketing.adobe.com/resources/help/en_US/s7/sharpening/s7_sharpening_images.pdf).

Na Adobe TV, assista [a Nitidez de uma imagem com máscara de nitidez](https://tv.adobe.com/watch/visual-design-cs6/sharpening-an-image-with-unsharp-mask/).

Com o Dynamic Media Classic, é possível aumentar a nitidez de imagens em ingestão, na entrega ou em ambos. No entanto, na maioria dos casos, você deve ajustar as imagens usando apenas um método ou outro, mas não ambos. A nitidez de imagens na entrega, em um URL, geralmente oferece os melhores resultados.

Há dois métodos de nitidez de imagem que podem ser usados:

* Nitidez simples ( `&op_sharpen`) - Semelhante ao filtro de nitidez usado no Photoshop, a nitidez simples aplica nitidez básica à exibição final da imagem, após o redimensionamento dinâmico. No entanto, esse método não pode ser configurado pelo usuário. A prática recomendada não é usada `&op_sharpen` a menos que seja necessária.
* Máscara de nitidez ( `&op_USM`) - Máscara de nitidez é um filtro de nitidez padrão do setor. A melhor prática é aumentar a nitidez de imagens com máscara perfeita seguindo as orientações abaixo. A máscara de nitidez permite controlar os três parâmetros a seguir:

   * `&op_sharpen=amount,radius,threshold`

      * `amount` (0-5, força do efeito.)
      * `radius` (0-250, largura das "linhas de nitidez" desenhadas em torno do objeto com nitidez, conforme medido em pixels.)

         Lembre-se de que os parâmetros `radius` e `amount` trabalham uns com os outros. A redução `radius` pode ser compensada ao aumentar `amount`. `Radius` permite que controle mais fino como um valor mais baixo compartilhe apenas os pixels da borda, enquanto um valor mais alto aplica nitidez a uma banda maior de pixels.

      * `threshold` (0-255, sensibilidade do efeito.)

         Esse parâmetro determina como os pixels com nitidez devem ser provenientes da área circundante antes que sejam considerados pixels de borda, e o filtro compartilhe-os. O limite ajuda a evitar a nitidez de áreas com cores semelhantes, como tons de pele. Por exemplo, um valor limite de 12 ignora pequenas variações no brilho do tom de pele para evitar adicionar "barulho", ao mesmo tempo que adiciona contraste de borda a áreas de alto contraste, como quando as barras atendem a uma capa.
      Para obter mais informações sobre como você define esses três parâmetros, incluindo práticas recomendadas para usar com o filtro, consulte os seguintes recursos:

      Tópico de ajuda do Dynamic Media Classic na [nitidez de uma imagem](https://help.adobe.com/en_US/scene7/using/WS389B162D-2981-41e5-9253-15D22D2ECBC8.html).

      Práticas recomendadas em papel de compartilhamento de [nitidez no Adobe Scene 7 Publishing System e no Servidor de imagens](https://marketing.adobe.com/resources/help/en_US/s7/sharpening/s7_sharpening_images.pdf).

   * O Dynamic Media Classic também permite controlar um quarto parâmetro: monocromática ( `0,1`). Esse parâmetro determina se máscara unnítida é aplicada a cada componente de cor separadamente usando o valor `0` ou ao brilho/intensidade da imagem usando o valor `1`.


Como prática recomendada, comece com o parâmetro de raio da máscara de nitidez. As configurações de raio que podem ser iniciadas são:

* Site: 0.2-0.3 pixels
* Impressão fotográfica (250-300 ppi): 0.3-0.5 pixels
* Impressão offset (266-300 ppi): 0.7-1.0 pixels
* Impressão da tela de desenho (150 ppi): 1.5-2.0 pixels

Aumenta gradualmente a quantidade de 1.75 to para 4. Se a nitidez ainda não for da maneira desejada, aumente o raio por um ponto decimal e execute a quantia novamente de 1.75 para 4. Repita, conforme necessário.

Deixe a configuração do parâmetro monocromática em 0.

## Práticas recomendadas para compactação JPEG (&amp; qlt =) {#best-practices-for-jpeg-compression-qlt}

* Esse parâmetro controla a qualidade de codificação JPG. Um valor mais alto significa uma imagem de maior qualidade, mas um tamanho de arquivo grande; como alternativa, um valor menor significa uma imagem de qualidade menor, mas um tamanho de arquivo menor. O intervalo para esse parâmetro é de 0-100.
* Para otimizar a qualidade, não defina o valor do parâmetro como 100. A diferença entre uma configuração de 90 ou 95 e 100 é quase imperceptível, mas 100 aumenta o tamanho do arquivo de imagem. Portanto, para otimizar para qualidade, mas evitar que arquivos de imagem fiquem muito grandes, defina o `qlt=` valor como 90 ou 95.
* Para otimizar para um tamanho de arquivo de imagem pequeno, mas manter a qualidade da imagem em um nível aceitável, defina o `qlt=` valor como 80. Os valores abaixo de 70 a 75 resultam em uma degradação significativa de qualidade de imagens.
* Como prática recomendada, para permanecer no meio, defina o `qlt=` valor como 85 para permanecer no meio.
* Uso do sinalizador croma em `qlt=`

   * O `qlt=` parâmetro tem uma segunda configuração que permite ativar a diminuição da resolução de cromaticidade RGB usando o valor `,0` normal (padrão) ou desativá-la usando o valor `,1`.
   * Para mantê-la simples, comece com a diminuição da resolução de cromaticidade RGB desativada ( `,1`). Essa configuração geralmente resulta em melhor qualidade de imagem, especialmente para imagens sintéticas com muitas bordas e contrastes nítidos.

Como prática recomendada para uso `&qlt=85,0`de compressão JPG.

## Práticas recomendadas para dimensionamento JPEG (&amp; jpegsize =) {#best-practices-for-jpeg-sizing-jpegsize}

`jpegSize` é um parâmetro útil se você quiser garantir que uma imagem não exceda um determinado tamanho para a entrega em dispositivos com memória limitada.

* Esse parâmetro é definido em quilobytes ( `jpegSize=<size_in_kilobytes>`). Define o tamanho máximo permitido para a entrega de imagens.
* `&jpegSize=` interage com o parâmetro `&qlt=`de compactação JPG. Se a resposta JPG com o parâmetro de compactação JPG especificado ( `&qlt=`) não exceder o `jpegSize` valor, a imagem será retornada `&qlt=` como definido. Caso `&qlt=` contrário, diminua gradualmente até que a imagem se ajuste ao tamanho máximo permitido, ou até que o sistema a determine não se ajuste e retorne um erro.

Como prática recomendada, defina `&jpegSize=` e adicione o parâmetro `&qlt=` se estiver entregando imagens JPG a dispositivos com memória limitada.

## Resumo das práticas recomendadas {#best-practices-summary}

Como prática recomendada, para obter uma qualidade de imagem alta e tamanho de arquivo pequeno, comece com a seguinte combinação de parâmetros:

`fmt=jpg&qlt=85,0&resMode=sharp2&op_usm=1.75,0.3,2,0`

Essa combinação de configurações de produtos é excelente, na maioria das circunstâncias.

Se a imagem requer mais otimização, ajuste gradualmente os parâmetros de nitidez (máscara de nitidez), começando com um raio definido como 0.2 ou 0.3. Em seguida, aumenta gradualmente o valor de 1.75 para um máximo de 4 (equivalente a 400% no Photoshop). Verifique se o resultado desejado foi atingido.

Se os resultados de nitidez ainda não forem satisfatórios, aumente o raio em incrementos decimais. Para cada incremento decimal, reinicie a quantia em 1.75 e aumente gradualmente para 4. Repita esse processo até obter o resultado desejado. Embora os valores acima sejam uma abordagem que os estúdios criativos tenham validado, lembre-se de que você pode começar com outros valores e seguir outras estratégias. Se os resultados forem satisfatórios para você ou não for um assunto subjetivo, a realização de testes estruturados é importante.

Ao experimentar, você também pode encontrar as sugestões gerais a seguir úteis para otimizar seu fluxo de trabalho:

* Experimente e teste diferentes parâmetros em tempo real, diretamente em um URL de Dynamic Media clássica ou na funcionalidade de ajuste de imagem do Scene 7 Publishing System, que fornece visualizações em tempo real para operações de ajuste.
* Como prática recomendada, lembre-se de que você pode agrupar os comandos do Serviço de imagem do Dynamic Media em uma predefinição de imagens. Uma predefinição de imagens é basicamente um URL de comando com nomes predefinidos personalizados, como `$thumb_low$` e `&product_high$`. O nome predefinido personalizado em um caminho de URL faz uma chamada para essas predefinições. Essa funcionalidade ajuda a gerenciar comandos e configurações de qualidade para diferentes padrões de utilização de imagens no seu site e reduz o tamanho geral dos urls.
* O Dynamic Media Classic também fornece maneiras mais avançadas de ajustar a qualidade da imagem, como aplicar nitidez de imagens durante a ingestão. Para casos de uso avançados, onde pode ser uma opção para ajustar e otimizar ainda mais os resultados da renderização, o Adobe Professional Services pode ajudá-lo com informações e práticas recomendadas personalizadas.

