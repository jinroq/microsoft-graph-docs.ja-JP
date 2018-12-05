---
title: conditionalAccessPolicy リソースの種類
description: 対応する記号の活動によってトリガーされる条件付きのアクセス ポリシーまたはポリシーに関連する属性を示します。
ms.openlocfilehash: 56a06d6b5fcba96dc472eb63fe24ba3920b0dd09
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074208"
---
# <a name="conditionalaccesspolicy-resource-type"></a>conditionalAccessPolicy リソースの種類
対応する記号の活動によってトリガーされる条件付きのアクセス ポリシーまたはポリシーに関連する属性を示します。



## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|displayName|String|条件付きのアクセス ポリシーの名前 (例:「が必要な MFA の Salesforce」).|
|enforcedGrantControls|String コレクション|条件付きアクセス ポリシーによって適用される許可のコントロールを参照 (例:「多要素認証を必要とする])。|
|enforcedSessionControls|String コレクション|条件付きアクセス ポリシーによって適用されるセッションのコントロールを参照 (例:"適用アプリケーションのコントロールを必要とする])。|
|id|String|条件付きのアクセス ポリシーの一意の GUID|
|result|String| 起動された CA のポリシーの結果を示します。使用可能な値は次のとおりです。<br/> `success` <br/> `failure` <br/> `notApplied`・ ポリシーの条件が満たされなかったために、ポリシーが適用されていません。 <br/> `notEnabled`-これは、ポリシーが無効の状態のためです。|

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