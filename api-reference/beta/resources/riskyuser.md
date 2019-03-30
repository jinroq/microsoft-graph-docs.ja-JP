---
title: riskyUsers リソースの種類
description: 危険にさらされている Azure AD ユーザーを表します。 Azure AD は、さまざまなシグナルやマシン学習に基づいて、ユーザーのリスクを継続的に評価します。 この API は、プログラムによって Azure AD 内のすべてのリスクユーザーにアクセスを提供します。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3265ea40903ca2c5c10272f5df280bd3715af366
ms.sourcegitcommit: fd9f62fd9a6d311f98afe2e31afca8b818c402c2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/30/2019
ms.locfileid: "31003721"
---
# <a name="riskyusers-resource-type"></a>riskyUsers リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

危険にさらされている Azure AD ユーザーを表します。 Azure AD は、さまざまなシグナルやマシン学習に基づいて、ユーザーのリスクを継続的に評価します。 この API は、プログラムによって Azure AD 内のすべてのリスクユーザーにアクセスを提供します。

リスクイベントの詳細については、「 [Azure Active Directory id 保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)」を参照してください。

>**注:** riskyUsers API を使用するには、Azure AD Premium P2 ライセンスが必要です。

## <a name="methods"></a>メソッド

| メソッド   | 戻り値の型|説明|
|:---------------|:--------|:----------|
|[リスト riskyUsers](../api/riskyusers-list.md) | [riskyUsers](riskyUser.md) |リスクの高いユーザーとそのプロパティを一覧表示します。|
|[riskyUsers を取得する](../api/riskyusers-get.md) | [riskyUsers](riskyUser.md)|特定の危険なユーザーおよびそのプロパティを取得します。|
|[riskyUsers が侵害されたことを確認する](../api/riskyusers-confirmcompromised.md)|危険なユーザーが侵害されていることを確認します。|
|[riskyUsers を閉じる](../api/riskyusers-dismiss.md)|危険なユーザーのリスクを無視します。|

## <a name="properties"></a>プロパティ

| プロパティ   | 型|説明|
|:---------------|:--------|:----------|
|`id`|`string`|危険にさらされているユーザーの一意の id|
|`isDeleted`|`bool`|ユーザーが削除されるかどうかを示します。 可能な値は`true`、です。`false`|
|`isGuest`|`bool`|ユーザーがゲストユーザーであるかどうかを示します。 可能な値は、`true`、`false` です。 True の場合は、ユーザーの id がテナントの外部にある場合に考慮します。 このユーザーは、Azure AD、MSA、またはサードパーティの id プロバイダーで id を持つ B2B または B2C ユーザーの場合があります。 False 場合は、ユーザーの id がテナントの内側にある場合|
|`isProcessing`|`bool`|ユーザーの危険な状態がバックエンドによって処理されていることを示します。|
|`risk`|[さらさ](risk.md)|危険ユーザーの状態|
|`riskLastUpdatedDateTime`|`datetime`|危険性のあるユーザーが最後に更新された日時|
|`userDisplayName`|`string`|危険ユーザーの表示名|
|`userPrincipalName`|`string`|危険ユーザープリンシパル名|


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.riskyusers"
}-->

```json
{
 "id": "string",
"riskLastUpdatedDateTime": "dateTimeOffset",
"isGuest": "boolean",
"isProcessing": "boolean",
"isDeleted": "boolean",
"risk": {"@odata.type": "microsoft.graph.risk"},
"userDisplayName": "string",
"userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "riskyusers resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
