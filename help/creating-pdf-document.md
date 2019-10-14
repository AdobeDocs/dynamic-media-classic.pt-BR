---
title: Criação de um documento PDF
seo-title: Criação de um documento PDF
description: nulo
seo-description: Saiba como criar um documento PDF usando o processo de impressão da Web no Dynamic Media Classic.
uuid: 274fb06b-320b-40fa-8b61-c224d8aceaa1
contentOwner: admin
content-type: referência
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/category/template-publishing
discoiquuid: 87e91e8e-10a2-4fba-87c7-ad2bd798146
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Criação de um documento PDF {#creating-a-pdf-document}

A etapa final do processo Web-to-Print está gerando o PDF personalizado. Depois que os usuários finais personalizam o modelo usando o aplicativo da Web criado, eles criam um documento PDF final. Esse PDF final geralmente é enviado a um provedor de serviços de impressão para impressão em nível profissional. Para garantir que o PDF final seja impresso como esperado, os desenvolvedores usam o arquivo de opções de trabalho correto e configuram fontes, marcas de impressora e cores corretamente.

## Configuração de predefinições de PDF {#setting-up-pdf-presets}

Especifique o nível de compatibilidade do PDF e as configurações da impressora criando e fazendo upload de um arquivo de opções de trabalho do PDF para o servidor do Dynamic Media Classic. Por exemplo, você pode selecionar saída PDF compatível com PDF/X-4 (recomendado para fluxos de trabalho de publicação de impressão em PDF). Você pode criar o arquivo de opções de trabalho no software de criação (como o Adobe Illustrator) ou no Acrobat. Sempre verifique com sua impressora, que pode aconselhá-lo sobre as configurações de opção de trabalho apropriadas para seu trabalho de impressão.

Para obter mais informações sobre como criar arquivos de opções de trabalho e para obter informações sobre como criar um arquivo de opções de trabalho no Acrobat, consulte a Ajuda do Adobe Acrobat.

Para criar um arquivo de opções de trabalho no Illustrator:

1. Escolha Editar &gt; Predefinições de Adobe PDF.
1. Na caixa de diálogo, selecione a predefinição que deseja usar.

   As seguintes configurações de opção de trabalho são suportadas pelo Dynamic Media Classic:

   | Opção de trabalho | Descrição |
   |--- |--- |
   | Geral | <ul><li>Compatibilidade </li><li>Compactação no nível do objeto</li><li>Incorporar miniaturas</li><li>Otimizar para exibição rápida da Web</li></ul> |
   | Imagens | <ul><li>Diminuir resolução</li><li>Resolução</li><li>Limiar</li><li>Compactação para cor, cinza e mono</li></ul> |
   | Fontes | <ul><li>Incorporar todas as fontes (as fontes são incorporadas por padrão)</li><li>Incorporar fontes OpenType</li><li>Subconjunto de fontes incorporadas quando a porcentagem de caracteres usados for menor que:</li><li>Lista Sempre Incorporada</li><li>Nunca incorporar lista</li></ul> |
   | Cor | <ul><li>Estratégia de cor (a tag somente imagens é tratada como tag all)</li><li>Propósito de renderização do documento</li><li>Apenas os seguintes espaços de trabalho são suportados na seção 4.2.5. 4.3 permitirá que você use qualquer perfil fornecido pelo cliente que tenha sido carregado no IPS.</li><li>Como solução alternativa, você pode especificar o espaço de cor de destino para a arte-final a ser convertida usando os perfis de cor padrão da empresa.</li></ul> |
   | RGB | <ul><li>e-sRGB </li><li>scRGB com intervalo de codificação [-4.0, 4.0]</li><li>Lab D50</li><li>PCS XYZ</li><li>XYZ plano</li><li>ROMM-RGB linear</li><li>ROMM-RGB</li><li>sYCC de 8 bits</li><li>e-sYCC de 8 bits</li></ul> |
   | Cinza | <ul><li>Gama cinza 1.8</li><li>Gama cinza 2.2</li><li>Ganho de ponto 10%</li><li>Aumento de Ponto 15%</li><li>Ganho de ponto 20%</li><li>Ganho de ponto 25%</li><li>Ganho de ponto 30%</li><li>Cinza</li></ul> |
   | Preservar valores CMYK para espaços de cores CMYK calibrados |  |
   | Avançado | Preservar comentários OPI sempre é ativado |
   | Padrões | Padrão de conformidade |

   >[!NOTE]
   >
   >O Dynamic Media Classic ignora as configurações de marca de impressora no arquivo de opções de trabalho. Em vez disso, as marcas de impressora são configuradas por meio do uso de comandos de URL do Dynamic Media Classic.

1. Clique em Exportar, especifique um nome e um local e clique em Salvar.
1. Carregue o arquivo de opções de trabalho como um ativo no Scene7 Publishing System.

   Use-o com seu modelo publicado, fazendo referência a ele no URL.  Por exemplo:

   `https://yourpublishserver.scene7.com/is/agm/SiliconPublishing/PetNews?&fmt=pdf,cmyk&joboption=SPSfilenameid`

## Preparação do PDF para impressão {#preparing-the-pdf-for-print}

Antes de finalizar o PDF para impressão, siga as diretrizes desta seção.

**Imagens**

Verifique se todas as imagens em seu trabalho de publicação foram carregadas no servidor do Dynamic Media Classic e publicadas.

**Fontes**

Verifique se todas as fontes em seu trabalho de publicação foram carregadas no servidor do Dynamic Media Classic e publicadas. Certifique-se de que você tenha direitos legais para hospedar as fontes se planeja permitir que os usuários finais as alterem.

**Resolução da imagem (pixels por polegada)**

A resolução de imagens bitmap é preservada pelo servidor Dynamic Media Classic em PDFs prontos para impressão gerados. O Dynamic Media Classic atualiza a resolução da imagem, se necessário. Para obter resultados ideais, deixe a resolução no valor padrão (geralmente 72 dpi) ao visualizar na Web. A resolução padrão para todas as imagens em sua empresa é definida na janela Configurações de publicação/Servidor de imagens na seção Resolução de impressão padrão. Resoluções mais altas (como 300dpi) podem resultar em mais tempo de processamento e devem ser aplicadas somente a um PDF pronto para impressão. Use o comando imageRes= no URL para substituir manualmente a resolução padrão para trabalhos em PDF.

**Gerenciamento de cores**

O documento e as imagens podem usar tons de cinza, CMYK, cores especiais nomeadas, RGB ou modelos de cores Lab. Cada uma pode ser descalibrada ou calibrada usando um perfil de cor ICC. Para obter melhores resultados, incorpore o perfil ao PDF pronto para impressão gerado. O servidor Dynamic Media Classic faz isso por padrão. Verifique se todos os perfis de cores necessários foram carregados na plataforma Dynamic Media Classic. De preferência, verifique se as opções de gerenciamento de cores definidas no aplicativo de design correspondem àquelas definidas no servidor do Dynamic Media Classic:

* **** Configurações de gerenciamento de cores do aplicativo de design: Nas Configurações de cores do aplicativo de criação (como o Adobe Illustrator), especifique os perfis de cores RGB e CMYK na seção Espaços de trabalho.

* **** Configurações de gerenciamento de cores do Dynamic Media Classic: Normalmente, as configurações de gerenciamento de cores no aplicativo de design devem corresponder aos perfis de cores padrão no servidor do Dynamic Media Classic. Essas configurações podem ser encontradas na janela Instalação de publicação/Servidor de imagens.

## Exibição de marcas de impressora {#displaying-printer-marks}

Você pode criar um PDF para qualquer um destes casos:

* Um documento concluído
* Documento intermédio, como um filme ou chapa, que pode ser enviado a uma impressora para produção

Um documento intermediário pode conter conteúdo de produção adicional, como margens de sangria, marcas de impressora e assim por diante. Esse conteúdo geralmente é exibido fora dos limites da página finalizada.

Todas as marcas disponíveis na tela "Adicionar marcas de impressora" no Acrobat são suportadas. As marcas da impressora são controladas com o `printerMark` parâmetro. A sintaxe é `&printerMark=trim marks, bleed marks, registration marks, color bars, page information, style, line weight, layer embed`.

* marcas de aparagem = 0|1
* marcas de sangria = 0|1
* marcas de registro = 0|1
* barras de cores = 0|1
* informações da página = 0|1
* estilo = Illustrator| IllustratorJ| QuarkXPress
* espessura da linha = 0,125| 0,25| 0,50
* incorporação de camada = 0|1

Ao preparar um documento para a produção de impressão, podem ser necessárias marcas de impressão para ajudar o serviço de impressão a alinhar os filmes de separação para a produção de provas, medir a película para a calibração correta e a densidade de tinta, aparar filme para tamanho e assim por diante. As marcas de impressora indicam os limites de caixas de documentos, como caixas de aparagem e de sangria. O conteúdo relacionado à produção pode incluir:

* **Caixa** de mídia Os limites da mídia física na qual a página será impressa. O conteúdo fora da caixa de mídia pode ser descartado com segurança sem afetar o significado do arquivo.

* **Caixa de sangria** A região na qual o conteúdo da página é cortado quando é produzido em um ambiente de produção. A caixa de sangria pode incluir áreas necessárias para acomodar as limitações físicas dos equipamentos de corte, dobradura e aparagem. O valor padrão é a caixa de corte da página.

* **Caixa** de corteAs dimensões desejadas da página finalizada após a aparagem. A caixa de apara pode ser menor que a caixa de mídia para permitir conteúdo relacionado à produção, como instruções de impressão, marcas de corte e barras coloridas. O valor padrão é a caixa de corte da página.

* **Caixa** de arte A extensão do conteúdo significativo da página (incluindo o espaço em branco potencial) conforme pretendido pelo criador da página. O valor padrão é a caixa de corte da página.

Você pode usar os modificadores mostrados nesta tabela para replicar as marcas de impressora disponíveis no Adobe Illustrator, InDesign e Acrobat:

| Modificador/Valores | Descrição |
|--- |--- |
| bleedMargin=top,left,bottom,right | Especificado no Acrobat com a opção Definir caixas de página. Selecione BleedBox e especifique as margens com a opção Controles de margem.<br><br>Os valores representam a distância das bordas superior, esquerda, inferior e direita das bordas originais da arte-final (a caixa de mídia) que vai para dentro. Os valores (0-1000) estão em pontos.<br><br>Nova altura=altura original - (superior+inferior)<br><br>Nova largura= largura original - (esquerda+direita) |
| mediaMargin=top,left,bottom,right | Especificado no Acrobat com a opção Definir caixas de página. Modifique o Tamanho personalizado da página na opção Alterar tamanho da página.<br><br>Os valores representam a distância das bordas superior, esquerda, inferior e direita das bordas originais da arte-final (a caixa de mídia) que vai para fora. Os valores (0-1000) estão em pontos.<br><br>Nova altura=superior+inferior+<br><br>altura originalNova largura=superior+inferior+<br><br>largura originalOs novos valores de altura e largura determinam o novo tamanho de página do PDF gerado.<br><br>Quando uma nova Caixa de mídia é definida, todos os cálculos de margem de aparo e margem de sangria precisam considerar a nova Caixa de mídia como a borda da arte-final. |
| trimMargin=top,left,bottom,right | Especificado no Acrobat com a opção Definir caixas de página. Selecione Caixa de aparo e especifique as margens com a opção Controles de margem.<br><br>Os valores representam a distância das bordas superior, esquerda, inferior e direita das bordas originais da arte-final (a caixa de mídia) que vai para dentro. Os valores (0-1000) estão em pontos.<br><br>Nova altura=altura original - (superior+inferior)<br><br>Nova largura=largura original - (esquerda+direita) |
| printerMark= trim marks, sangramentos, marcas de registro, barras coloridas, informações da página, estilo, espessura da linha, incorporação da camada | Os valores são os seguintes:marcas de<br><br>aparo = 0,1 (o padrão é 0)marcas de<br><br>sangria = 0,1 (o padrão é 0)marcas de<br><br>registro = 0,1 (o padrão é 0)barras<br><br>coloridas = 0,1 (o padrão é 0)informações de<br><br>página = 0,1 (o padrão é 0)<br><br>estilo = Padrão, InDesignJ1, InDesignJ2, Illustrator, , QuarkXPress (o padrão é Padrão)<br><br>linha de peso= 0,125-0,2, ambos os valores inclusive (o padrão é 0,25)<br><br>camada incorporada = 0, 1, com 1 criando uma nova camada contendo todas as marcas de impressora (o padrão é 1)<br><br>Dependendo do estilo usado, as marcas e barras coloridas aparecem diferentes e correspondem aos estilos correspondentes usados pelo Acrobat. |

Observe o seguinte sobre as marcas de impressora:

* Especifique margens de sangria, margens de aparagem e margens de mídia por meio de chamadas de URL ao especificar marcas de impressora. A especificação de marcas de impressora sem especificar essas margens faz com que essas marcas apareçam fora da região visível do PDF gerado. Além disso, as marcas de aparagem e de sangria se sobrepõem.
* Especificar os mesmos valores de margem para a margem de aparagem e a margem de sangria resulta em marcas de aparagem e marcas de sangria sobrepostas quando ambos os sinalizadores estão definidos como 1 pol `&printerMark`.
* A especificação de formatos fmt=swf/image por meio de chamadas de URL resulta na saída sem marcas de impressora ou margens, pois esse recurso é específico para saída de PDF.
* A especificação `&printerMark=`pelo URL resulta na utilização de valores padrão para todos os parâmetros. Especificar `&printerMark=1` resultados em marcas de aparagem sendo definidas como 1 e valores padrão para outros parâmetros. Mas para definir o nth elemento como ON, todos os parâmetros (n-1) precisam ser especificados por meio do URL.
* Especificar apenas um valor para `&trimMargin`, `&bleedMargin`e `&mediaMargin` resulta na aplicação desse valor a todas as margens superior, inferior, esquerda e direita da arte-final original.
* Especificar somente os valores superior e esquerdo por meio `&trimMargin`, `&bleedMargin`e `&mediaMargin` resulta na atribuição do valor superior ao valor inferior e no valor esquerdo igual à direita.
* Não especificar o valor direito por meio `&trimMargin`, `&bleedMargin`e `&mediaMargin` resulta na atribuição do valor esquerdo à direita.
* Para um PDF de várias páginas, as marcas/margens da impressora são aplicadas a todas as páginas (no Acrobat, os usuários podem selecionar intervalos de páginas para marcas/margens da impressora).
* A saída de um PDF com marcas/margens de impressora ativadas corresponde exatamente ao Acrobat X, a menos que especificado de outra forma.

Se quiser criar um arquivo PDF compatível com PDF/X-4 através do modificador de &amp;joboption no URL, você deve estar ciente das limitações relacionadas às marcas de impressora especificadas no PDF ISO_15930-7-2008.pdf:

* Cada objeto Página de um arquivo PDF inclui uma MediaBox. Cada objeto de página em um arquivo em conformidade com PDF/X-4 deve incluir uma TrimBox ou uma ArtBox, mas não ambos. A MediaBox pode ser incluída por herança.
* Se a BleedBox estiver presente, a ArtBox ou a TrimBox não deve ultrapassar os limites da BleedBox. Se a CropBox estiver presente, nenhuma das ArtBox, TrimBox ou BleedBox devem se estender para além dos limites da CropBox.
* Nenhuma das ArtBox, TrimBox, CropBox ou BleedBox deve se estender além dos limites da MediaBox.
* Algumas práticas do setor exigem o uso da BleedBox. Devem ser seguidas as práticas comerciais adequadas.
* Recomenda-se o uso da TrimBox sobre o uso da ArtBox.
* Todas as anotações, exceto as anotações TrapNet e PrinterMark, devem ter um valor para Rect totalmente fora da BleedBox (ou da TrimBox ou da ArtBox, se nenhuma BleedBox estiver presente). Todas as anotações PrinterMark devem ter um valor para Rect totalmente fora da TrimBox ou ArtBox. Um leitor em conformidade com PDF/X-4 pode ignorar completamente as anotações, exceto as anotações em PDF TrapNet.
* Considera-se que um Rect se encontra completamente fora de uma caixa delimitadora se todas as coordenadas do Rect estiverem situadas fora da caixa delimitadora ou no seu bordo e a interseção dos dois retângulos for zero.
* Se o dicionário ViewerPreferences contiver as teclas ViewArea, ViewClip, PrintArea ou PrintClip, cada uma dessas teclas deve ter o valor MediaBox ou (se uma BleedBox estiver presente em todos os objetos de página do arquivo) BleedBox.

