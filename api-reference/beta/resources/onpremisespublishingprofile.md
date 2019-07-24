---
title: onPremisesPublishingProfile リソースの種類
description: onPremisesPublishingProfile リソースの種類。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1eb442b6f3317ac7c0e2f130442e4a62c7f9c152
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841326"
---
# <a name="onpremisespublishingprofile-resource-type"></a>onPremisesPublishingProfile リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

さまざまな Azure サービス (たとえば、Azue Active Directory Connect パススルー認証、Workday to Azure AD ユーザープロビジョニング) は、企業ネットワークの外部からさまざまな社内リソースへの条件付きアクセスを許可します。 テナント管理者によってインストールされた[社内エージェント](onpremisesagent.md)は、発行された特定の[リソース](publishedresource.md)への要求にアクセスしたり、処理したりするように構成できます。
[エージェントグループ](onpremisesagentgroup.md)を使用すると、テナント管理者は特定のエージェントを割り当てて、発行された特定の社内リソースを提供できます。 テナント管理者は、複数のエージェントをまとめてグループ化し、発行された各リソースをグループに割り当てることができます。 同じオンプレミスの発行タイプのエンティティセット全体が**onPremisesPublishingProfile**によって表されます。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
| [OnPremisesPublishingProfile を取得する](../api/onpremisespublishingprofile-get.md) | [onPremisesPublishingProfile](onpremisespublishingprofile.md) | **OnPremisesPublishingProfile**オブジェクトのプロパティとリレーションシップを読み取ります。 |
| [OnPremisesPublishingProfile の更新](../api/onpremisespublishingprofile-update.md) | None | [OnPremisesPublishingProfile](onpremisespublishingprofile.md)オブジェクトを更新します。

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|hybridAgentUpdaterConfiguration|[hybridAgentUpdaterConfiguration](hybridagentupdaterconfiguration.md)| **HybridAgentUpdaterConfiguration**オブジェクトを表します。|
|id|String| 発行の種類を表します。 可能な値は、`appProxy`、`exchangeOnline`、`authentication`、`provisioning`、`adAdministration` です。 読み取り専用です。|

## <a name="relationships"></a>関係

| リレーションシップ | 型        | 説明 |
|:-------------|:------------|:------------|
|agentGroups|[onPremisesAgentGroup](onpremisesagentgroup.md)コレクション| 既存の**onPremisesAgentGroup**オブジェクトのリスト。 読み取り専用です。 Null 許容型。|
|エージェント|[onPremisesAgent](onpremisesagent.md)コレクション| 存在していた**onPremisesAgent**オブジェクトのリスト。 読み取り専用です。 Null 許容型。|
|publishedResources|[Publishedresource](publishedresource.md)コレクション| 既存の**Publishedresource**オブジェクトのリスト。 読み取り専用です。 Null 許容型。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "hybridAgentUpdaterConfiguration": {"@odata.type": "microsoft.graph.hybridAgentUpdaterConfiguration"},
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesPublishingProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
