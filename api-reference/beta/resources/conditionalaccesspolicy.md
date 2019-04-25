---
title: conditionalAccessPolicy リソースの種類
description: 対応するサインインアクティビティによってトリガーされた条件付きアクセスポリシーまたはポリシーに関連する属性を示します。
localization_priority: Normal
ms.openlocfilehash: 7b043e739f84715fb02fbdbd25599e5cfccc284a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543372"
---
# <a name="conditionalaccesspolicy-resource-type"></a>conditionalAccessPolicy リソースの種類
対応するサインインアクティビティによってトリガーされた条件付きアクセスポリシーまたはポリシーに関連する属性を示します。



## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|displayName|String|条件付きアクセスポリシーの名前を参照します (例: "Salesforce の MFA が必要")。|
|enforcedGrantControls|String collection|条件付きアクセスポリシーによって適用される grant コントロールを参照します (例: "多要素認証を必要とする")。|
|enforcedSessionControls|String collection|条件付きアクセスポリシーによって適用されるセッションコントロールを参照します (例: "アプリ強制コントロールが必要です")。|
|id|String|条件付きアクセスポリシーの一意の GUID|
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
