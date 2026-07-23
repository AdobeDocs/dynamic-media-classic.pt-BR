---
title: Práticas recomendadas para otimização da qualidade de imagens
description: Conheça as práticas recomendadas para otimizar a qualidade das suas imagens.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 3c50e706-b9ed-49db-8c08-f179de52b9cf
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T17:39:42.316Z'
TQID: 'https://experienceleague.adobe.com/kw-spdqv6ArVEWk8ID4mnQjYrS25RZntKOJ7-tESasY'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: bcc5edb5-84c3-4940-9f84-ed88b6c16274
  - id: cdd65e7e-8839-44a2-bc21-0e03623b5dd1
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: b29d7cc6962ca9e7724bb43987947b08af5cd4d7
workflow-type: tm+mt
source-wordcount: 1591
ht-degree: 0%

---

# Práticas recomendadas para otimização da qualidade de imagens{#best-practices-for-optimizing-the-quality-of-your-images}

A otimização da qualidade da imagem pode ser demorada. Muitos fatores contribuem para a obtenção de resultados aceitáveis. O resultado é parcialmente subjetivo porque os indivíduos percebem a qualidade da imagem de forma diferente. A experimentação estruturada é essencial.

O Adobe Dynamic Media Classic inclui mais de 100 comandos de veiculação de imagens para ajustar e otimizar imagens e renderizar resultados. As diretrizes a seguir podem ajudar você a simplificar o processo e obter bons resultados rapidamente usando alguns comandos essenciais e práticas recomendadas.

Consulte também [Imagem inteligente](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/dynamic/imaging-faq).

>[!TIP]
>
>Experimente e descubra os benefícios dos modificadores de imagem do Dynamic Media e do Smart Imaging, usando o [_Snapshot_](https://snapshot.scene7.com/) do Dynamic Media.
>
> O Instantâneo é uma ferramenta de demonstração visual criada para ilustrar os recursos do Dynamic Media para entrega de imagens otimizadas e dinâmicas. Experimente com imagens de teste ou URLs do Dynamic Media, para que você possa observar visualmente a saída de vários modificadores de imagem do Dynamic Media e as otimizações de Imagem inteligente para o seguinte:
>
>* Tamanho do arquivo (com entrega WebP e AVIF)
>* Largura de banda de rede
>* DPR (Relação de pixels do dispositivo)
>
>Para aprender a usar o Instantâneo, assista ao [Vídeo de treinamento do Instantâneo](https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/dynamic-media/images/dynamic-media-snapshot) (3 minutos e 17 segundos).


## Práticas recomendadas para formato de imagem (&amp;fmt=) {#best-practices-for-image-format-fmt}

* JPG ou PNG são as melhores opções para fornecer imagens em boa qualidade e com tamanho e peso gerenciáveis.
* Se nenhum comando format for fornecido no URL, o Dynamic Media Image Serving assume o padrão JPG para entrega.
* O JPG é compactado a uma proporção de 10:1 e geralmente produz arquivos de imagem menores. O PNG é compactado em uma proporção de aproximadamente 2:1, exceto quando as imagens contêm planos de fundo transparentes. Normalmente, os tamanhos dos arquivos PNG são maiores que os arquivos JPG.
* O JPG usa compactação com perdas, o que significa que os elementos de imagem (pixels) são soltos durante a compactação. Por outro lado, o PNG usa compactação sem perdas.
* O JPG geralmente compacta imagens fotográficas com melhor fidelidade do que imagens sintéticas com bordas nítidas e contraste.
* Se as imagens contiverem transparência, use PNG, pois o JPG não oferece suporte a essa transparência.

Como prática recomendada para o formato de imagem, comece com a configuração mais comum `&fmt=JPG`.

## Práticas recomendadas para tamanho de imagem {#best-practices-for-image-size}

A redução dinâmica do tamanho da imagem é uma das tarefas mais comuns que o Dynamic Media Image Serving realiza. Envolve a especificação do tamanho e, opcionalmente, o modo de redução da resolução usado para diminuir a escala da imagem.

* Para dimensionamento de imagem, use `&wid=<value>` e `&hei=<value>`. Esses parâmetros definem automaticamente a largura da imagem de acordo com a taxa de proporção.
* `&resMode=<value>` Controla o algoritmo usado para redução da resolução. Comece com `&resMode=sharp2`. Esse valor fornece a melhor qualidade de imagem. Embora o uso do valor de redução de resolução `bilin` seja mais rápido, isso geralmente resulta em artefatos de suavização.

Como prática recomendada para dimensionamento de imagem, use `&wid=<value>&hei=<value>&resMode=sharp2`. `&hei=<value>&resMode=sharp2`

## Práticas recomendadas para nitidez de imagem {#best-practices-for-image-sharpening}

A nitidez de imagem é o aspecto mais complexo de controlar imagens no seu site e onde ocorrem muitos erros. Para saber mais sobre como a nitidez e o mascaramento sem nitidez funcionam no Adobe Dynamic Media Classic, consulte os seguintes recursos úteis:

O whitepaper de práticas recomendadas do PDF chamou [Nitidez de imagens no Adobe Dynamic Media Classic e no Servidor de imagens](/help/using/assets/s7_sharpening_images.pdf).

<!-- Give a 404 See also [Sharpening an image with unsharp mask](https://helpx.adobe.com/photoshop/atv/cs6-tutorials/sharpening-an-image-with-unsharp-mask.html). -->

No Adobe Dynamic Media Classic, você pode ajustar a nitidez das imagens durante a assimilação, a entrega ou ambas. No entanto, geralmente as imagens são mais nítidas usando um método, mas não ambos. A nitidez de imagens na entrega por meio de um URL geralmente oferece os melhores resultados.

Há dois métodos de nitidez de imagem que podem ser usados:

* Nitidez simples ( `&op_sharpen`): assim como o filtro de nitidez usado no Adobe Photoshop, a nitidez simples aplica a nitidez básica à exibição final da imagem após o redimensionamento dinâmico. No entanto, esse método não é configurável pelo usuário. A prática recomendada é evitar o uso de `&op_sharpen`, a menos que seja necessário.
* Mascaramento sem nitidez ( `&op_USM`): o mascaramento sem nitidez é um filtro padrão do setor para nitidez. A prática recomendada é tornar mais nítidas as imagens com mascaramento sem nitidez, seguindo as diretrizes abaixo. O mascaramento sem nitidez permite controlar os três parâmetros a seguir:

  * `&op_sharpen=amount,radius,threshold`

    * `amount` (0-5, intensidade do efeito.)
    * `radius` (0-250, largura das &quot;linhas de nitidez&quot; desenhadas ao redor do objeto com nitidez, conforme medido em pixels.)

      Observe que os parâmetros `radius` e `amount` têm uma relação inversa. A redução de `radius` pode ser compensada pelo aumento de `amount`. `Radius` permite um controle mais fino, pois um valor mais baixo aplica nitidez apenas aos pixels da borda, enquanto um valor mais alto aplica nitidez a um intervalo mais amplo de pixels.

    * `threshold` (0-255, sensibilidade de efeito.)

      Esse parâmetro determina como deve ser a diferença dos pixels com nitidez em relação à área ao redor antes de serem considerados pixels de borda e o filtro ajuste a nitidez deles. A opção Limiar ajuda a evitar áreas de nitidez excessiva com cores semelhantes, como tons de pele. Por exemplo, um valor limite de 12 ignora pequenas variações no brilho do tom da pele para evitar a adição de &quot;ruído&quot;, enquanto ainda adiciona o contraste da borda a áreas de alto contraste, como onde as pálpebras tocam a pele.

      Para obter mais informações sobre como você define esses três parâmetros, incluindo as práticas recomendadas a serem usadas com o filtro, consulte [Nitidez de imagens no Adobe Dynamic Media Classic e no Servidor de imagens](/help/using/assets/s7_sharpening_images.pdf).

    * O Adobe Dynamic Media Classic também permite controlar um quarto parâmetro: monocromático ( `0,1`). Este parâmetro determina se a máscara de nitidez é aplicada separadamente a cada componente de cor usando o valor `0` ou ao brilho/intensidade da imagem usando o valor `1`.

Como prática recomendada, comece com o parâmetro Tirar nitidez do raio da máscara. As configurações de raio com as quais você pode começar são as seguintes:

* Site: 0,2-0,3 pixels
* Impressão fotográfica (250-300 ppi): 0,3-0,5 pixels
* Impressão deslocada (266-300 ppi): 0,7-1,0 pixels
* Impressão da tela de desenho (150 ppi): 1,5 a 2,0 pixels

Aumente gradualmente a quantidade de 1,75 para 4. Se a nitidez ainda não for o resultado desejado, aumente o raio em um incremento decimal e defina a quantidade novamente de 1,75 para 4. Repita conforme necessário.

Deixe a configuração de parâmetro monocromático em 0.

## Práticas recomendadas para compactação JPEG (`&qlt=`) {#best-practices-for-jpeg-compression-qlt}

* Esse parâmetro controla a qualidade da codificação do JPG. Um valor mais alto significa uma imagem de qualidade superior, mas um tamanho de arquivo grande; como alternativa, um valor mais baixo significa uma imagem de qualidade inferior, mas um tamanho de arquivo menor. O intervalo desse parâmetro é de 0 a 100.
* Para otimizar a qualidade, não defina o valor do parâmetro como 100. A diferença entre um ajuste de 90 ou 95 e 100 é quase imperceptível. No entanto, 100 aumenta desnecessariamente o tamanho do arquivo de imagem. Portanto, para otimizar a qualidade, mas evitar que os arquivos de imagem fiquem muito grandes, defina o valor `qlt=` como 90 ou 95.
* Para otimizar um tamanho de arquivo de imagem pequeno, mas manter a qualidade da imagem em um nível aceitável, defina o valor `qlt=` como 80. Valores abaixo de 70 a 75 resultam em degradação significativa da qualidade da imagem.
* Para ficar no meio, defina o valor de `qlt=` como 85 como uma prática recomendada.
* Usando o sinalizador chroma `qlt=`

  * O parâmetro `qlt=` tem uma segunda configuração que permite ativar a redução de resolução de cromaticidade do RGB usando o valor normal `,0` (padrão), ou desativá-lo usando o valor `,1`.
  * Comece com a redução de resolução de cromaticidade do RGB desativada ( `,1`). Essa configuração geralmente resulta em melhor qualidade de imagem, especialmente para imagens sintéticas com muitas bordas e contraste nítidos.

Como prática recomendada para a compactação JPG, use `&qlt=85,0`.

## Práticas recomendadas para dimensionamento do JPEG (&amp;jpegSize=) {#best-practices-for-jpeg-sizing-jpegsize}

O parâmetro `jpegSize` é útil se você quiser garantir que uma imagem não exceda um determinado tamanho. Esse parâmetro é para dispositivos com memória limitada.

* Este parâmetro está definido em quilobytes ( `jpegSize=<size_in_kilobytes>`). Ele define o tamanho máximo permitido para a entrega de imagens.
* `&jpegSize=` Interage com o parâmetro de compactação JPG `&qlt=`. Se a resposta do JPG com o parâmetro de compactação JPG especificado ( `&qlt=`) não exceder o valor `jpegSize`, a imagem será retornada com `&qlt=` conforme definido. Caso contrário, `&qlt=` é diminuído gradualmente até que a imagem se ajuste ao tamanho máximo permitido. Como alternativa, o sistema retornará um erro se não conseguir ajustar a imagem.

Como prática recomendada, defina `&jpegSize=` e inclua o parâmetro `&qlt=` ao entregar imagens do JPG para dispositivos com memória limitada.

## Resumo de práticas recomendadas {#best-practices-summary}

Como prática recomendada, para atingir alta qualidade de imagem e um tamanho de arquivo pequeno, comece com a seguinte combinação de parâmetros:

`fmt=jpg&qlt=85,0&resMode=sharp2&op_usm=1.75,0.3,2,0`

Essa combinação de configurações produz excelentes resultados na maioria das circunstâncias.

Se a imagem exigir mais otimização, ajuste gradualmente os parâmetros de nitidez (mascaramento sem nitidez), começando com um raio definido como 0,2 ou 0,3. Em seguida, aumente gradualmente o valor de 1,75 para um máximo de 4 (equivalente a 400% em [!DNL Adobe Photoshop]). Verifique se o resultado desejado foi atingido.

Se os resultados da nitidez ainda não forem satisfatórios, aumente o raio em incrementos decimais. Para cada incremento decimal, redefina o valor para 1,75 e aumente-o gradualmente para 4. Repita esse processo até atingir o resultado desejado. Embora os valores acima sejam uma abordagem validada pelos estúdios de criação, observe que você pode usar outros valores e seguir outros procedimentos. Se os resultados são satisfatórios para você ou não é uma questão subjetiva; portanto, é necessária experimentação estruturada.

À medida que você experimenta, as seguintes sugestões gerais são úteis para otimizar seu fluxo de trabalho:

* Teste diferentes parâmetros em tempo real, diretamente em uma URL ou usando ferramentas de ajuste de imagem do [!DNL Adobe Dynamic Media Classic]. Este último fornece pré-visualizações em tempo real para operações de ajuste.
* Como prática recomendada, lembre-se de agrupar comandos do Servidor de imagens do Dynamic Media em uma Predefinição de imagem. Uma Predefinição de imagem é um conjunto de macros de comando de URL com nomes predefinidos personalizados, como `$thumb_low$` e `$product_high$`. O nome da predefinição personalizada em um caminho de URL chama essas predefinições. Essa funcionalidade ajuda a gerenciar comandos e configurações de qualidade para diferentes padrões de uso de imagens no site e reduz o comprimento geral dos URLs.
* O Adobe Dynamic Media Classic também oferece maneiras mais avançadas de ajustar a qualidade da imagem, como aplicar nitidez de imagem na assimilação. Para casos de uso avançados em que o ajuste e a otimização adicionais dos resultados renderizados são uma opção, a Adobe Professional Services pode ajudá-lo com práticas recomendadas e insight personalizadas.
