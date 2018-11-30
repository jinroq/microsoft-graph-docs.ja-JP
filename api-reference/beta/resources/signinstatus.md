---
title: signInStatus リソースの種類
description: サインインの状態 (成功または失敗) の記号では、します。
ms.openlocfilehash: cafa0dffe1b1d798d87225ac82901cf041d5e4fa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073321"
---
# <a name="signinstatus-resource-type"></a>signInStatus リソースの種類
サインインの状態 (成功または失敗) の記号では、します。



## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|additionalDetails|String|サインインの活動の詳細を説明します。|
|errorCode|Int32|サインインに失敗した時に生成される 5 6digit のエラー コードを提供します。 [エラー コードとメッセージの一覧](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)を確認してください。|
|failureReason|String|対応する記号でアクティビティのエラー メッセージまたはエラーの原因を提供します。 [エラー コードとメッセージの一覧](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)を確認してください。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInStatus"
}-->

```json
{
  "additionalDetails": "String",
  "errorCode": 1024,
  "failureReason": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->