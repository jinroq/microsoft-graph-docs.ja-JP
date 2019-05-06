---
title: riskyUserHistoryItem リソースの種類
description: Azure AD ユーザーのリスク履歴を表します。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 37f38a649aa3721e65b44e64571dafb797259cf6
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33620837"
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
