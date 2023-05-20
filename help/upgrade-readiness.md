---
title: Prontidão para atualização
description: Uma lista de verificação de prontidão de atualização quando você deseja avançar de [!DNL Adobe Dynamic Media Classic] para [!DNL Dynamic Media] em [!DNL Adobe Experience Manager].
feature: Dynamic Media Classic
role: Admin,User
exl-id: 86537998-b7e9-449c-83eb-6fd04533a00f
source-git-commit: efe51280ac33579a8e690eb6483488eea9069159
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# Lista de verificação de preparação para atualização

Use a lista de verificação a seguir para ajudá-lo a entender e se preparar para uma atualização do [!DNL Dynamic Media Classic] para [!DNL Dynamic Media].

|  | Tarefa | Descrição |
| :--- | :--- | --- |
| **Fase 1: licenciamento** | Executar contrato | Com base no tráfego e no armazenamento, a equipe da conta do Adobe trabalha com você para fazer a transição do [!DNL Dynamic Media Classic] licença a ser renovada no [!DNL Dynamic Media] licença. |
| **Fase 2: Preparação** | Validar uso do recurso | Confirme os recursos que estão sendo usados no [!DNL Dynamic Media Classic] estão disponíveis em [!DNL Dynamic Media]. Consulte a [Comparação de recursos](/help/upgrade-feature-comparison.md) página. Principais recursos ainda não disponíveis no [!DNL Dynamic Media] incluem:<br>· Visual Configurator (Autor de imagem, Renderização de imagem).<br>· Modelos de imagem (modelo 1:1).<br>· eCatalogs.<br>Se os recursos acima estiverem sendo usados, a atualização ainda poderá ocorrer com o pressuposto de que esses recursos estarão acessíveis por meio de [!DNL Dynamic Media Classic]. |
|  | Identificar ativos | Localizar e preparar ativos e predefinições a serem usados para atualização. |
| **Fase 3: Ambiente** | Atualizar [!DNL Adobe Experience Manager] | Todas as instâncias de [!DNL Adobe Experience Manager] deve ser atualizado para a versão mais recente. |
|  | Configuração [!DNL Dynamic Media] | A Adobe Consulting ou o Partner configura [!DNL Dynamic Media] com suas credenciais. |
| **Fase 4: atualização** | Replicar ativos | Durante o processo de atualização, [!DNL Dynamic Media Classic] os ativos são replicados para o Dynamic Media. |
| **Fase 5: Configuração administrativa** | Configurar usuários e permissões | Crie usuários e conceda as permissões apropriadas. |
|  | Configurar perfis de codificação de vídeo | Criar perfis de codificação de vídeo. |
|  | Configurar predefinições do visualizador | Criar predefinições do visualizador. |
|  | Definir predefinições de imagem | Configurar predefinições de imagem. |
| **Fase 6: validação** | Validação | Verificar casos de uso, ativos, links e APIs. |
