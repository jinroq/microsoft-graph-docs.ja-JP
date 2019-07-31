---
title: riskyUserHistoryItem リソースの種類
description: Azure AD ユーザーのリスク履歴を表します。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 586fdb046adc8977550cc386a27284752cf487c3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965335"
---
# <a name="riskyuserhistoryitem-resource-type"></a>riskyUserHistoryItem リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Azure ad Id 保護によって決定された Azure AD ユーザーのリスク履歴を表します。 

## <a name="methods"></a>メソッド

| メソッド   | 戻り値の型|説明|
|:---------------|:--------|:----------|
|[リストの履歴](../api/riskyuser-list-history.md) | [riskyUserHistoryItem](riskyuserhistoryitem.md)コレクション|Azure AD ユーザーのリスク履歴を取得します。|


## <a name="properties"></a>プロパティ

| プロパティ       | 型    | 説明 |
|:---------------|:--------|:------------|
| userId         | string  | ユーザーの id。 |
| initiatedBy    | bool    | 操作を実行するアクターの id。 |
| activity       | [riskUserActivity](riskuseractivity.md)| ユーザーのリスクレベルの変更に関連するアクティビティ。 | 

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.riskyUserHistoryItem",
  "baseType": "microsoft.graph.riskyUser"
}-->

```json
{
    "userId": "string",
    "initiatedBy": "string",
    "activity": {"@odata.type": "microsoft.graph.riskUserActivity"}
}
```


<!--
{
  "type": "#page.annotation",
  "description": "riskyUserHistoryItem resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
   
  ]
}
-->
