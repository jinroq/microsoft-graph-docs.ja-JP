---
title: conditionalAccessPolicy リソースの種類
description: 対応するサインインアクティビティによってトリガーされた条件付きアクセスポリシーまたはポリシーに関連する属性を示します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2c45be8ee32c26187ccf42154ba6c06b60f5efc1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973217"
---
# <a name="conditionalaccesspolicy-resource-type"></a>conditionalAccessPolicy リソースの種類
対応するサインインアクティビティによってトリガーされた条件付きアクセスポリシーまたはポリシーに関連する属性を示します。



## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|displayName|String|条件付きアクセスポリシーの名前を参照します (例: "Salesforce の MFA が必要")。|
|enforcedGrantControls|文字列コレクション|条件付きアクセスポリシーによって適用される grant コントロールを参照します (例: "多要素認証を必要とする")。|
|enforcedSessionControls|文字列コレクション|条件付きアクセスポリシーによって適用されるセッションコントロールを参照します (例: "アプリ強制コントロールが必要です")。|
|id|文字列|条件付きアクセスポリシーの一意の GUID|
|result|String| トリガーされた CA ポリシーの結果を示します。可能な値は次のとおりです。<br/> `success` <br/> `failure` <br/> `notApplied`-ポリシー条件が満たされていないため、ポリシーは適用されません。 <br/> `notEnabled`-これは、ポリシーが無効な状態になっているためです。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.conditionalAccessPolicy"
}-->

```json
{
  "displayName": "String",
  "enforcedGrantControls": ["String"],
  "enforcedSessionControls": ["String"],
  "id": "String",
  "result": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
