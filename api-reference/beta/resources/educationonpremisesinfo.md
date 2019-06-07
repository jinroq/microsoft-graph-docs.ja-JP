---
title: educationOnPremisesInfo リソースの種類
description: オンプレミスの Active Directory ユーザーアカウントを Azure AD ユーザーオブジェクトに関連付けるために使用される追加情報。
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c147755aea584674e17f2de913e039b7d3e0cf82
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764771"
---
# <a name="educationonpremisesinfo-resource-type"></a>educationOnPremisesInfo リソースの種類

オンプレミスの Active Directory ユーザーアカウントを Azure AD ユーザーオブジェクトに関連付けるために使用される追加情報。

## <a name="properties"></a>プロパティ

| プロパティ    | 型   | 説明                                               |
| :---------- | :----- | :-------------------------------------------------------- |
| immutableId | String | Active Directory 内のユーザーオブジェクトの一意識別子。 |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOnPremisesInfo"
}-->

```json
{
  "immutableId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOnPremisesInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
