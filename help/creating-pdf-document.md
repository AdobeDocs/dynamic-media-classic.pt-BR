---
title: Criação de um documento PDF
seo-title: Criação de um documento PDF
description: 'null'
seo-description: Saiba como criar um documento PDF usando o processo Web-to-Print no Dynamic Media Classic.
uuid: 274 fb 06 b -320 b -40 fa -8 b 61-c 224 d 8 aceaa 1
contentOwner: admin
content-type: reference
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorias/modelo-publishing
discoiquuid: 87 e 91 e 8 e -10 a 2-4 fba -87 c 7-aad 2 bd 798146
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Criação de um documento PDF {#creating-a-pdf-document}

A etapa final do processo de Web para imprimir está gerando o PDF personalizado. Depois que os usuários finais personalizam o modelo usando o aplicativo da Web criado, ele cria um documento PDF final. Esse PDF final é geralmente enviado para um provedor de serviços de impressão para impressão de nível profissional. Para certificar-se de que o PDF final seja impresso como esperado, os desenvolvedores usam o arquivo de joboptions correto e configuram fontes, marcas de impressora e cores corretamente.

## Configuração de predefinições de PDF {#setting-up-pdf-presets}

Especifique o nível de compatibilidade de PDF e as configurações da impressora criando e carregando um arquivo de joboptions de PDF para o servidor do Dynamic Media Classic. Por exemplo, você pode escolher a saída PDF em conformidade com PDF/X -4 (recomendado para fluxos de trabalho de publicação de impressão em PDF). Você pode criar o arquivo de joboptions no software de criação (como o Adobe Illustrator) ou no Acrobat. Sempre verifique com sua impressora, que pode aconselhá-lo nas configurações apropriadas da opção de trabalho para seu trabalho de impressão.

Para obter mais informações sobre como criar arquivos de joboptions e informações sobre como criar um arquivo de joboptions no Acrobat, consulte Ajuda do Adobe Acrobat.

Para criar um arquivo de joboptions no Illustrator:

1. Escolha Editar &gt; Predefinições de Adobe PDF.
1. Na caixa de diálogo, selecione a predefinição que deseja usar.

   As seguintes Configurações de opção de trabalho são suportadas pelo Dynamic Media Classic:

   | Opção de trabalho | Descrição |
   |--- |--- |
   | Geral | <ul><li>Compatibilidade </li><li>Compactação de nível de objeto</li><li>Incorporar miniaturas</li><li>Otimizar para visualização rápida na Web</li></ul> |
   | Imagens | <ul><li>Diminuição da resolução</li><li>Resolução</li><li>Limite</li><li>Compactação para cor, cinza e mono</li></ul> |
   | Fontes | <ul><li>Incorporar todas as fontes (as fontes são incorporadas por padrão)</li><li>Incorporar fontes opentype</li><li>Subconjunto de fontes incorporadas quando a porcentagem de caracteres usados é menor que:</li><li>Sempre incorporar lista</li><li>Nunca incorporar lista</li></ul> |
   | Cor | <ul><li>Estratégia de cores (somente imagens são tratadas como tags de tudo)</li><li>Propósito de renderização do documento</li><li>Somente os seguintes espaços de trabalho são compatíveis com 4.2.5. 4.3 permitirá que você use qualquer cliente que tenha sido carregado no IPS.</li><li>Como solução, você pode especificar o espaço de cor de destino para que a arte-final seja convertida para uso dos perfis de cores padrão da empresa.</li></ul> |
   | RGB | <ul><li>e-srgb </li><li>Scrgb com intervalo de codificação [-4.0, 4.0]</li><li>Lab D 50</li><li>PCS XYZ</li><li>XYZ simples</li><li>ROMM - RGB linear</li><li>ROMM-RGB</li><li>Sycc 8 bits</li><li>e-sycc 8 bits</li></ul> |
   | Cinza | <ul><li>Gama Cinza 1.8</li><li>Gama Cinza 2.2</li><li>Aumento de ponto 10%</li><li>Aumento de ponto 15%</li><li>Aumento de ponto 20%</li><li>Aumento de ponto 25%</li><li>Aumento de ponto 30%</li><li>Sgray</li></ul> |
   | Preservar valores CMYK para espaços de cores CMYK calibrados |  |
   | Avançado | Preservar comentários OPI sempre é ativado |
   | Padrões | Padrão de conformidade |

   >[!NOTE]
   >
   >O Dynamic Media Classic ignora as configurações de marcadores de impressora no arquivo joboptions. Em vez disso, as marcas de impressora são configuradas por meio de comandos de URL clássica do Dynamic Media.

1. Clique em Exportar, em seguida, especifique um nome e um local e clique em Salvar.
1. Carregue o arquivo de opções de trabalho como um ativo para o Sistema de publicação Scene 7.

   Use-o com o modelo publicado fazendo referência a ele no URL. Por exemplo:

   `https://yourpublishserver.scene7.com/is/agm/SiliconPublishing/PetNews?&fmt=pdf,cmyk&joboption=SPSfilenameid`

## Preparação do PDF para impressão {#preparing-the-pdf-for-print}

Antes de finalizar o PDF para impressão, siga as diretrizes nesta seção.

**Imagens**

Verifique se todas as imagens no trabalho de publicação foram carregadas no seu Servidor do Dynamic Media Classic e publicadas.

**Fontes**

Verifique se todas as fontes no trabalho de publicação foram carregadas no seu Servidor do Dynamic Media Classic e publicadas. Tenha em mente que você tem direitos legais para hospedar as fontes se planeja permitir que os usuários finais alterem os mesmos.

**Resolução da imagem (pixels por polegada)**

A resolução de imagens bitmap é preservada pelo servidor do Dynamic Media Classic em pdfs prontos para impressão. O Dynamic Media Classic atualiza a resolução da imagem, se necessário. Para obter melhores resultados, deixe a resolução no valor padrão (normalmente 72 dpi) ao visualizar na Web. A resolução padrão para todas as imagens na empresa é definida na janela Configurações de publicação/Servidor de imagens na seção Resolução de impressão padrão. As resoluções mais altas (como 300 dpi) podem resultar em tempo de processamento mais longo e devem ser aplicadas somente a um PDF pronto para impressão. Use o comando imageres = no URL para substituir manualmente a resolução padrão de trabalhos em PDF.

**Gerenciamento de cores**

Seu documento e imagens podem usar tons de cinza, CMYK, cores spot, RGB ou modelos de cores Lab. Cada um pode ser descalibrado ou calibrado por meio de um perfil de cor ICC. Para obter melhores resultados, incorpore o perfil no PDF pronto para impressão. O Dynamic Media Classic Server faz isso por padrão. Verifique se todos os perfis de cores necessários foram carregados na plataforma do Dynamic Media Classic. De preferência, certifique-se de que as opções de gerenciamento de cores definidas no aplicativo de design correspondam àquelas definidas no seu servidor do Dynamic Media Classic:

**Configurações do gerenciamento de cores do aplicativo de design:** Nas Configurações de cores do aplicativo de criação (como o Adobe Illustrator), especifique os perfis de cores RGB e CMYK na seção Espaços de trabalho.

**Configurações do gerenciamento de cores do Dynamic Media Classic:** Normalmente, as configurações de gerenciamento de cores no aplicativo de design devem corresponder aos perfis de cores padrão no servidor do Dynamic Media Classic. Essas configurações podem ser encontradas na janela Configurações de publicação/Servidor de imagens.

## Exibição de marcas de impressora {#displaying-printer-marks}

Você pode criar um PDF para um destes casos:

* Um documento concluído
* Um documento intermediário, como um filme ou chapa, que pode ser enviado para uma impressora para produção

Um documento intermediário pode conter conteúdo de produção adicional, como margens de sangria, marcas de impressora e assim por diante. Normalmente, esse conteúdo é mostrado fora dos limites da página finalizada.

Todas as marcas disponíveis na tela «Adicionar marcas de impressora» no Acrobat são compatíveis. As marcas de impressora são controladas com o `printerMark` parâmetro. A sintaxe `&printerMark=trim marks, bleed marks, registration marks, color bars, page information, style, line weight, layer embed`é.

* trim marks = 0|1
* sangria de sangria = 0|1
* marcas de registro = 0|1
* barras de cores = 0|1
* informações da página = 0|1
* style = Illustrator | Illustratorj | Quarkxpress
* espessura da linha = 0.125 | 0.25 | 0.50
* camada embed = 0|1

Ao preparar um documento para produção impressa, as marcas de impressora podem ser necessárias para ajudar o serviço de impressão a alinhar os filmes de separação para a produção de testes, medir o filme para corrigir a calibração e a densidade da tinta, recortar filme ao tamanho e assim por diante. As marcas de impressora indicam os limites das caixas de documento, como caixas de aparagem e caixas de sangria. O conteúdo relacionado à produção pode incluir:

**Caixa** de mídia Os limites da mídia física na qual a página será impressa. O conteúdo fora da caixa de mídia pode ser descartado sem problemas sem afetar o significado do arquivo.

**Caixa** de Sangema região para a qual o conteúdo da página é cortado quando se compacta em um ambiente de produção. A caixa de sangria pode incluir áreas necessárias para acomodar as limitações físicas de equipamento de cortar, dobrar e aparar. O valor padrão é a caixa de corte da página.

**Caixa** de Aparaas dimensões desejadas da página finalizada após o aparo. A caixa de aparagem pode ser menor que a caixa de mídia para permitir o conteúdo relacionado à produção, como instruções de impressão, marcas de corte e barras de cores. O valor padrão é a caixa de corte da página.

**Caixa** de arte A extensão do conteúdo significativo da página (incluindo o espaço em branco potencial) conforme pretendido pelo criador da página. O valor padrão é a caixa de corte da página.

Você pode usar os modificadores mostrados nesta tabela para replicar as marcas de impressora disponíveis no Adobe Illustrator, indesign e Acrobat:

| Modificador/Valores | Descrição |
|--- |--- |
| Bleedmargin = top, left, bottom, right | Especificado no Acrobat com a opção Definir caixas de página. Selecione bleedbox e especifique as margens com a opção Controles de margem.<br><br>Os valores representam a distância das bordas superior, esquerda, inferior e direita das bordas originais da arte-final (a caixa de mídia) que fica invertida. Os valores (0-1000) estão em pontos.<br><br>Nova altura = altura original - (superior + inferior)<br><br>Nova largura = largura original - (esquerda + direita) |
| Mediamargin = superior, esquerda, inferior, direita | Especificado no Acrobat com a opção Definir caixas de página. Modifique o Tamanho da página personalizada na opção Alterar tamanho da página.<br><br>Os valores representam a distância das bordas superior, esquerda, inferior e direita das bordas originais da arte-final (a caixa de mídia) que fica fora dos lugares. Os valores (0-1000) estão em pontos.<br><br>Nova altura = top + bottom + heightnew<br><br>largura = top + bottom + original widtha<br><br>nova altura e os novos valores de largura determinam o novo tamanho de página do PDF gerado.<br><br>Quando uma nova Caixa de mídia é definida, todos os cálculos da margem de aparagem e da margem de sangria precisam considerar a nova Caixa de mídia como a borda da arte-final. |
| Trimeway = top, left, bottom, right | Especificado no Acrobat com a opção Definir caixas de página. Selecione Caixa de aparagem e especifique as margens com a opção Controles de margem.<br><br>Os valores representam a distância das bordas superior, esquerda, inferior e direita das bordas originais da arte-final (a caixa de mídia) que fica invertida. Os valores (0-1000) estão em pontos.<br><br>Nova altura = altura original - (superior + inferior)<br><br>Nova largura = largura original - (esquerda + direita) |
| Printermark = marcas de aparagem, marcas de sangria, marcas de registro, barras de cores, informações de página, estilo, espessura da linha, incorporar camada | Os valores são:<br><br>Os sinais de aparagem = 0,1 (padrão is 0)<br><br>Anged marks = 0,1 (padrão is 0)<br><br>marcas de registro = 0,1 (padrão is 0)<br><br>as barras de cores = 0,1 (<br><br>padrão é 0)<br><br>style = Default, indesignj 1, indesignj 2, Illustrator, illustratorj, quarkxpress (padrão é Padrão) o peso<br><br>da linha = 0.125-0.2, ambos os valores inclusivos (padrão é 0.25)<br><br>embutidos = 0, 1, com 1 criação de uma nova camada contendo todas as marcas de impressora (padrão é 1)<br><br>Dependendo do estilo usado, as marcas e barras de cores aparecem diferentes e correspondem aos estilos correspondentes usados por Acrobat. |

Observe o seguinte sobre as marcas de impressora:

* Especifique margens de sangria, margens de aparagem e margens de mídia por meio de chamadas de URL ao especificar marcas de impressora. Especificar marcas de impressora sem especificar essas margens faz com que elas apareçam fora da região visível do PDF gerado. Além disso, as marcas de aparagem e as marcas de sangria se sobrepõem.
* A especificação dos mesmos valores de margem para a margem de aparagem e a margem de sangria resulta em marcas de aparagem e em marcas de sangria sobrepostas quando ambos os sinalizadores estão definidos como 1 em `&printerMark`.
* Especificar fmt = swf/formatos de imagem por meio de chamadas de URL resulta na saída sem nenhuma marca ou marca de impressora porque esse recurso é específico para a saída PDF.
* A especificação `&printerMark=`por meio do URL resulta em valores padrão usados para todos os parâmetros. Especificar `&printerMark=1` resultados em marcas de aparagem que estão sendo definidas como 1 e valores padrão para outros parâmetros. Mas para definir o enésimo elemento como Ativado, todos os parâmetros (n -1) precisam ser especificados por meio do URL.
* Especificar apenas um valor para `&trimMargin`, `&bleedMargin`e `&mediaMargin` resulta no valor aplicado a todas as margens superior, inferior, esquerda e direita da arte-final original.
* Especificar apenas os valores superior e esquerda por meio `&trimMargin`de, `&bleedMargin`e `&mediaMargin` resulta no valor superior sendo atribuído ao valor inferior e o valor à esquerda sendo igual à direita.
* Não especificar o valor certo por meio `&trimMargin`, `&bleedMargin`e `&mediaMargin` resulta no valor esquerdo sendo atribuído à direita.
* Para um PDF de várias páginas, as marcas/margens de impressora são aplicadas a todas as páginas (no Acrobat, os usuários podem selecionar intervalos de páginas para marcas/margens de impressora).
* A saída de um PDF com marcas/margens de impressora ativadas corresponde exatamente com o Acrobat X, salvo indicação em contrário.

Se você quiser criar um arquivo PDF em conformidade com o PDF/X -4 através do modificador de &amp; joboption no URL, você deve estar ciente das limitações relacionadas às marcas de impressora especificadas no PDF ISO_15930-7-2008.pdf:

* Cada objeto de Página de um arquivo PDF inclui uma mediabox. Cada objeto de Página em um arquivo de conformidade PDF/X -4 deve incluir uma trimbox ou uma Arte-final, mas não ambos. A mediabox pode ser incluída por herança.
* Se a bleedbox estiver presente, a artbox ou a trimbox não poderão ultrapassar os limites da bleedbox. Se a cropbox estiver presente, nenhum da arte-final, a trimbox ou a bleedbox serão estendidas além dos limites da cropbox.
* Nenhum da arte, a trimbox, a recorpbox ou a bleedbox devem se estender para além dos limites da mediabox.
* Algumas práticas do setor exigem o uso da bleedbox. As práticas comerciais apropriadas devem ser seguidas.
* O uso da trimbox é recomendado sobre o uso da arte-final.
* Todas as anotações diferentes das anotações trapnet e printermark devem ter um valor para Rect se distelar completamente fora da bleedbox (ou a trimbox ou a artbox caso nenhuma bleedbox esteja presente). Todas as anotações printermark devem ter um valor para Rect se distancia completamente fora da trimbox ou da artbox. Um leitor de conformidade PDF/X -4 pode ignorar completamente anotações, exceto as anotações PDF trapnet.
* Um Rect será considerado como completamente fora de uma caixa delimitadora se todas as coordenadas do Rect ficarem fora da caixa delimitadora ou na borda, e a interseção dos dois retângulos for zero.
* Se o dicionário viewerpreferences contiver as teclas viewarea, viewclip, printarea ou printclip, cada uma dessas chaves apresentará o valor mediabox ou (se uma bleedbox estiver presente em todos os objetos de página do arquivo) bleedbox.

