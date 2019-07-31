---
title: targetResource resource 複合型-Microsoft Graph API
description: 監査ログ報告組織 (テナント) アクティビティをサポートする Microsoft Graph API の targetResource entity resource 複合型を定義します。
author: davidmu1
localization_priority: Normal
doc_type: resourcePageType
ms.prod: azure-ad
ms.openlocfilehash: a67cfbccf9d05872ec0d9207ac54c51cda222053
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964579"
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
