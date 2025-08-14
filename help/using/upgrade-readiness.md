---
title: Prontidão para atualização
description: Uma lista de verificação de preparação de atualização quando você deseja avançar de [!DNL Adobe Dynamic Media Classic] para [!DNL Dynamic Media] em [!DNL Adobe Experience Manager].
feature: Dynamic Media Classic
role: Admin,User
exl-id: 86537998-b7e9-449c-83eb-6fd04533a00f
topic: Administration, Migration
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 0%

---

# Lista de verificação de preparação para atualização

Use a lista de verificação a seguir para ajudá-lo a entender e se preparar para uma atualização do [!DNL Dynamic Media Classic] para o [!DNL Dynamic Media].

|  | Tarefa | Descrição |
| :--- | :--- | --- |
| **Fase 1: Licenciamento** | Executar contrato | Com base no tráfego e no armazenamento, a equipe de conta da Adobe trabalha com você na transição da licença do [!DNL Dynamic Media Classic] para a renovação na licença do [!DNL Dynamic Media]. |
| **Fase 2: Preparação** | Validar uso do recurso | Confirme se os recursos que estão sendo usados no [!DNL Dynamic Media Classic] estão disponíveis no [!DNL Dynamic Media]. Consulte a página [Comparação de recursos](/help/using/upgrade-feature-comparison.md). Os principais recursos ainda não disponíveis em [!DNL Dynamic Media] incluem:<br>· Configurador Visual (Autor da Imagem, Renderização da Imagem).<br>· Modelos de Imagem (1:1 Modelo).<br>· eCatalogs.<br>Se os recursos acima estiverem sendo usados, a atualização ainda poderá ocorrer com a suposição de que esses recursos estarão acessíveis por meio do [!DNL Dynamic Media Classic]. |
|   | Identificar ativos | Localizar e preparar ativos e predefinições a serem usados para atualização. |
| **Fase 3: Ambiente** | Atualizar [!DNL Adobe Experience Manager] | Todas as instâncias de [!DNL Adobe Experience Manager] devem ser atualizadas para a versão mais recente. |
|   | Instalação [!DNL Dynamic Media] | A Adobe Consulting ou o Parceiro configura o [!DNL Dynamic Media] com suas credenciais. |
| **Fase 4: atualização** | Replicar ativos | Durante o processo de atualização, os ativos designados do [!DNL Dynamic Media Classic] são replicados para o Dynamic Media. |
| **Fase 5: Instalação Administrativa** | Configurar usuários e permissões | Crie usuários e conceda as permissões apropriadas. |
|   | Configurar perfis de codificação de vídeo | Criar perfis de codificação de vídeo. |
|   | Configurar predefinições do visualizador | Criar predefinições do visualizador. |
|   | Definir predefinições da imagem | Configurar predefinições da imagem. |
| **Fase 6: Validação** | Validação | Verificar casos de uso, ativos, links e APIs. |
