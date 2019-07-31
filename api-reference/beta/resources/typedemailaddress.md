---
title: typedEmailAddress リソースの種類
description: 連絡先の名前、電子メールアドレス、および対応する電子メールアドレスの種類を表します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: c5ece5d1ad1c5c38253d73353b05b94727855fd5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007572"
---
# <a name="typedemailaddress-resource-type"></a>typedEmailAddress リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[連絡先](contact.md)の名前、電子メールアドレス、および対応する電子メールアドレスの種類を表します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|address|String|連絡先の電子メールアドレス。|
|name|String|連絡先の表示名。|
|type |String |電子メールアドレスの種類。 可能な値は、`unknown`、`work`、`personal`、`main`、`other` です。 既定値はです`unknown`。これは、**アドレス**が特定の種類として設定されていないことを意味します。 |
|otherLabel |String  |ユーザー設定の電子メールアドレスの種類を指定**** し、 `other`型をに設定して、ユーザー設定文字列に**otherlabel**を割り当てることができます。 たとえば、ボランティア活動に特定の電子メールアドレスを使用することができます。 **型**をに`other`設定し、 **otherlabel**をなどのカスタム文字列に`Volunteer work`設定します。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.typedEmailAddress"
}-->

```json
{
  "address": "string",
  "name": "string",
  "type": "string",
  "otherLabel": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
