---
title: targetResource リソースの種類
description: 監査アクティビティに関連付けられているターゲットリソースの種類を表します。
localization_priority: Normal
author: dhanyahk
ms.prod: azure-ad
ms.openlocfilehash: 33a381d6088245be235f37549184183443fe3237
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629216"
---
# <a name="targetresource-resource-type"></a>targetResource リソースの種類

監査アクティビティに関連付けられているターゲットリソースの種類を表します。 

## <a name="properties"></a>プロパティ

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|文字列|リソースの一意の ID を示します。|
|displayName|文字列型 (String)|リソースに対して定義されている表示名を示します。 通常、リソースの作成時に指定されます。|
|type|String|リソースの種類を表します。  値の例`Application`に`Group`は`ServicePrincipal`、、 `User`、、などがあります。|
|userPrincipalName|String|**型**がに`User`設定されている場合、これにはアクションを開始したユーザー名が含まれます。`null`その他の種類の場合。|
|groupType|String|**型**がに`Group`設定されている場合は、グループの種類を示します。|
|modifiedProperties|[modifiedProperty](modifiedproperty.md)コレクション|変更された各属性の名前、古い値、新しい値を示します。 プロパティの値は、操作の**種類**によって異なります。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResource"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "type": "String",
  "userPrincipalName": "String",
  "groupType": "String",
  "modifiedProperties": [{"@odata.type": "microsoft.graph.modifiedProperty"}]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
