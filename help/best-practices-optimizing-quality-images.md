---
title: Práticas recomendadas para otimização da qualidade de imagens
description: Conheça as práticas recomendadas para otimizar a qualidade de suas imagens.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 3c50e706-b9ed-49db-8c08-f179de52b9cf
source-git-commit: f3082fc6b66cf0903bf6cb1907a8615a12399fdc
workflow-type: tm+mt
source-wordcount: '1569'
ht-degree: 0%

---

# Práticas recomendadas para otimização da qualidade de imagens{#best-practices-for-optimizing-the-quality-of-your-images}

A otimização da qualidade da imagem pode ser um processo demorado, pois muitos fatores contribuem para a renderização de resultados aceitáveis. O resultado é parcialmente subjetivo porque os indivíduos percebem a qualidade da imagem de forma diferente. A experimentação estruturada é fundamental.

O Adobe Dynamic Media Classic inclui mais de 100 comandos de fornecimento de imagens para ajustar e otimizar imagens e resultados de renderização. As diretrizes a seguir podem ajudar você a simplificar o processo e obter bons resultados rapidamente usando alguns comandos essenciais e práticas recomendadas.

Consulte também [Imagem inteligente](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/imaging-faq.html#dynamic).

>[!TIP]
>
>Experimente e descubra os benefícios dos modificadores de imagem da Dynamic Media e do Smart Imaging, usando o Dynamic Media [_Instantâneo_](https://snapshot.scene7.com/).
>
> O Snapshot é uma ferramenta de demonstração visual, projetada para ilustrar o poder do Dynamic Media para a entrega de imagens otimizada e dinâmica. Experimente imagens de teste ou URLs do Dynamic Media para observar visualmente a saída de vários modificadores de imagem do Dynamic Media e otimizações de Smart Imaging para o seguinte:
>* Tamanho do arquivo (com entrega de WebP e AVIF)
>* Largura de banda de rede
>* DPR (Proporção de pixels do dispositivo)
>
>Para saber como é fácil usar o Snapshot, reproduza o [Vídeo de treinamento de instantâneo](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/dynamic-media/images/dynamic-media-snapshot.html?lang=en) (3 minutos e 17 segundos).


## Práticas recomendadas para o formato de imagem (&amp;fmt=) {#best-practices-for-image-format-fmt}

* JPG ou PNG são as melhores opções para fornecer imagens em boa qualidade e com tamanho e peso gerenciáveis.
* Se nenhum comando format for fornecido no URL, o Dynamic Media Image Serving assumirá JPG para entrega.
* O JPG comprime a uma proporção de 10:1 e geralmente produz tamanhos de arquivo de imagem menores. O PNG é compactado em uma proporção de cerca de 2:1, exceto às vezes quando as imagens contêm um plano de fundo vazio. Normalmente, porém, os tamanhos dos arquivos PNG são maiores que os arquivos JPG.
* O JPG usa compactação com perdas, o que significa que os elementos da imagem (pixels) são soltos durante a compactação. Por outro lado, o PNG usa compactação sem perdas.
* O JPG frequentemente compacta imagens fotográficas com mais fidelidade do que imagens sintéticas com bordas e contraste nítidos.
* Se suas imagens contêm transparência, use PNG porque o JPG não oferece suporte à transparência.

Como prática recomendada para o formato de imagem, comece com a configuração mais comum `&fmt=JPG`.

## Práticas recomendadas para o tamanho da imagem {#best-practices-for-image-size}

A redução dinâmica do tamanho da imagem é uma das tarefas mais comuns executadas pelo Dynamic Media Image Serving. Ela envolve especificar o tamanho e, opcionalmente, qual modo de diminuição da amostragem é usado para fazer o downscale da imagem.

* Para dimensionamento de imagem, a melhor e mais simples abordagem é usar `&wid=<value>` e `&hei=<value>` ou apenas `&hei=<value>`. Esses parâmetros definem automaticamente a largura da imagem de acordo com a proporção.
* `&resMode=<value>` controla o algoritmo usado para a resolução. Comece com `&resMode=sharp2`. Esse valor fornece a melhor qualidade de imagem. Ao usar o valor de amostragem decrescente `=bilin` for mais rápido, resultará frequentemente na aliasing de artefatos.

Como prática recomendada para dimensionar imagens, use `&wid=<value>&hei=<value>&resMode=sharp2` ou `&hei=<value>&resMode=sharp2`

## Práticas recomendadas para nitidez da imagem {#best-practices-for-image-sharpening}

A nitidez da imagem é o aspecto mais complexo do controle de imagens em seu site, e onde muitos erros são cometidos. Reserve tempo para saber mais sobre como a nitidez e o mascaramento em nitidez funcionam no Adobe Dynamic Media Classic, referindo-se aos seguintes recursos úteis:

White paper sobre práticas recomendadas [Nitidez de imagens no Adobe Dynamic Media Classic e no servidor de imagens](/help/assets/s7_sharpening_images.pdf).

<!-- Give a 404 See also [Sharpening an image with unsharp mask](https://helpx.adobe.com/photoshop/atv/cs6-tutorials/sharpening-an-image-with-unsharp-mask.html). -->

Com o Adobe Dynamic Media Classic, é possível aprimorar as imagens na assimilação, na entrega ou em ambas. No entanto, normalmente, as imagens são aprimoradas usando apenas um método ou o outro, mas não ambos. A nitidez de imagens na entrega, em um URL, normalmente fornece os melhores resultados.

Existem dois métodos de nitidez de imagem que você pode usar:

* Nitidez simples ( `&op_sharpen`) - Semelhante ao filtro de nitidez usado no Photoshop, a nitidez simples aplica nitidez básica à exibição final da imagem, após o redimensionamento dinâmico. No entanto, esse método não é configurável pelo usuário. A prática recomendada é não usar `&op_sharpen` exceto se necessário.
* Mascaramento nítido ( `&op_USM`) - O mascaramento com nitidez é um filtro padrão do setor para nitidez. A prática recomendada é aprimorar as imagens com máscara nítida seguindo as diretrizes abaixo. O mascaramento de nitidez permite controlar os três parâmetros a seguir:

   * `&op_sharpen=amount,radius,threshold`

      * `amount` (0-5, intensidade do efeito.)
      * `radius` (0-250, largura das &quot;linhas de nitidez&quot; desenhadas em torno do objeto com nitidez, conforme medida em pixels.)

         Lembre-se que os parâmetros `radius` e `amount` trabalhar um contra o outro. Redução `radius` pode ser compensada pelo aumento `amount`. `Radius` permite um controle mais fino como um valor mais baixo ajuste a nitidez apenas dos pixels da borda, enquanto um valor mais alto aumenta a nitidez de uma faixa maior de pixels.

      * `threshold` (0-255, sensibilidade do efeito.)

         Esse parâmetro determina como deve ser a diferença dos pixels com nitidez em relação à área ao redor antes de serem considerados pixels de borda e o filtro ajuste a nitidez deles. O limite ajuda a evitar áreas de nitidez excessiva com cores semelhantes, como tons de pele. Por exemplo, um valor limite de 12 ignora pequenas variações no brilho do tom da pele para evitar a adição de &quot;ruído&quot;, enquanto ainda adiciona o contraste da borda a áreas de alto contraste, como onde as pálpebras tocam a pele.

         Para obter mais informações sobre como você define esses três parâmetros, incluindo práticas recomendadas para usar com o filtro, consulte [Nitidez de imagens no Adobe Dynamic Media Classic e no servidor de imagens](/help/assets/s7_sharpening_images.pdf).

      * O Adobe Dynamic Media Classic também permite controlar um quarto parâmetro: monocromático ( `0,1`). Esse parâmetro determina se o mascaramento com nitidez é aplicado a cada componente de cor separadamente usando o valor `0` ou para o brilho/intensidade da imagem usando o valor `1`.

Como prática recomendada, comece com o parâmetro de raio da máscara de nitidez. As configurações de Raio que você pode começar são as seguintes:

* Sítio Web: 0,2-0,3 pixels
* Impressão fotográfica (250-300 ppi): 0,3-0,5 pixels
* Impressão offset (266-300 ppi): 0,7 a 1,0 pixels
* Impressão de tela (150 ppi): 1,5-2,0 pixels

Aumente gradualmente o montante de 1,75 para 4. Se a nitidez ainda não for a maneira desejada, aumente o raio em um ponto decimal e execute o valor novamente de 1,75 para 4. Repita conforme necessário.

Deixe a configuração do parâmetro monocromático em 0.

## Práticas recomendadas para compactação de JPEG (&amp;qlt=) {#best-practices-for-jpeg-compression-qlt}

* Esse parâmetro controla a qualidade da codificação de JPG. Um valor mais elevado significa uma imagem de qualidade superior, mas com um tamanho de ficheiro grande; como alternativa, um valor mais baixo significa uma imagem de qualidade mais baixa, mas com um tamanho de arquivo menor. O intervalo desse parâmetro é de 0 a 100.
* Para otimizar a qualidade, não defina o valor do parâmetro como 100. A diferença entre uma configuração de 90 ou 95 e 100 é quase imperceptível, mas 100 aumenta desnecessariamente o tamanho do arquivo de imagem. Portanto, para otimizar a qualidade, mas evitar que os arquivos de imagem fiquem muito grandes, defina a variável `qlt=` para 90 ou 95.
* Para otimizar para um pequeno tamanho de arquivo de imagem, mas manter a qualidade da imagem em um nível aceitável, defina a variável `qlt=` para 80. Valores inferiores a 70 a 75 resultam em degradação significativa da qualidade da imagem.
* Como prática recomendada, para permanecer no meio, defina a variável `qlt=` para 85 para ficar no meio.
* Uso do sinalizador de croma em `qlt=`

   * O `qlt=` tem uma segunda configuração que permite ativar a redução da amostragem de cromaticidade de RGB usando o valor normal `,0` (padrão), ou desative-o usando o valor `,1`.
   * Para simplificar, comece com a redução da amostragem de RGB para desativada ( `,1`). Essa configuração geralmente resulta em melhor qualidade de imagem, especialmente para imagens sintéticas com muitas bordas e contraste nítidos.

Como prática recomendada para o uso de compactação de JPG `&qlt=85,0`.

## Práticas recomendadas para dimensionamento de JPEG (&amp;jpegSize=) {#best-practices-for-jpeg-sizing-jpegsize}

O parâmetro `jpegSize` é útil se você quiser garantir que uma imagem não exceda um determinado tamanho para entrega em dispositivos com memória limitada.

* Esse parâmetro é definido em kilobytes ( `jpegSize=<size_in_kilobytes>`). Ela define o tamanho máximo permitido para a entrega de imagens.
* `&jpegSize=` interage com o parâmetro de compactação JPG `&qlt=`. Se a resposta JPG com o parâmetro de compactação JPG especificado ( `&qlt=`) não excede o `jpegSize` , a imagem é retornada com `&qlt=` conforme definido. Caso contrário, `&qlt=` diminui gradualmente até que a imagem se ajuste ao tamanho máximo permitido, ou até que o sistema determine que ela não se ajusta e retorne um erro.

Como prática recomendada, defina `&jpegSize=` e adicione o parâmetro `&qlt=` se estiver fornecendo imagens JPG para dispositivos com memória limitada.

## Resumo das práticas recomendadas {#best-practices-summary}

Como prática recomendada, para obter uma alta qualidade de imagem e um tamanho de arquivo pequeno, comece com a seguinte combinação de parâmetros:

`fmt=jpg&qlt=85,0&resMode=sharp2&op_usm=1.75,0.3,2,0`

Essa combinação de configurações de produtos é um excelente resultado na maioria das circunstâncias.

Se a imagem exigir mais otimização, ajuste gradualmente os parâmetros de nitidez (mascaramento com nitidez), começando com um raio definido como 0,2 ou 0,3. Em seguida, aumente gradualmente a quantidade de 1,75 para um máximo de 4 (equivalente a 400% no Photoshop). Verifique se o resultado desejado foi atingido.

Se os resultados de nitidez ainda não forem satisfatórios, aumente o raio em incrementos decimais. Para cada incremento decimal, reinicie o valor em 1,75 e aumente-o gradualmente para 4. Repita esse processo até atingir o resultado desejado. Embora os valores acima sejam uma abordagem que os estúdios criativos validaram, lembre-se de que é possível começar com outros valores e seguir outras estratégias. Se os resultados são ou não satisfatórios para si é uma questão subjetiva, por isso a experimentação estruturada é fundamental.

À medida que você experimenta, as seguintes sugestões gerais são úteis para otimizar seu fluxo de trabalho:

* Tente e teste diferentes parâmetros em tempo real, diretamente em um URL ou usando a funcionalidade de ajuste de imagem do Adobe Dynamic Media Classic. O último fornece visualizações em tempo real para operações de ajuste.
* Como prática recomendada, lembre-se de que é possível agrupar comandos do Dynamic Media Image Serving em uma predefinição de imagem. Uma predefinição de imagem é basicamente macros de comando de URL com nomes predefinidos personalizados, como `$thumb_low$` e `&product_high$`. O nome predefinido personalizado em um caminho de URL chama essas predefinições. Essa funcionalidade ajuda você a gerenciar comandos e configurações de qualidade para diferentes padrões de uso de imagens no seu site e reduz o tamanho geral dos URLs.
* O Adobe Dynamic Media Classic também oferece formas mais avançadas de ajustar a qualidade da imagem, como aplicar nitidez da imagem na assimilação. Para casos de uso avançado em que o ajuste e a otimização de resultados renderizados são uma opção, o Adobe Professional Services pode ajudá-lo com informações personalizadas e práticas recomendadas.
