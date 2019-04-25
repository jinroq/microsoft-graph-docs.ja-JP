---
title: typedEmailAddress リソースの種類
description: 連絡先の名前、電子メールアドレス、および対応する電子メールアドレスの種類を表します。
localization_priority: Normal
ms.openlocfilehash: 3b1230dabc1e49c6cb9220eea95f0c3b93053d96
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576459"
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
|otherlabel |String  |ユーザー設定の電子メールアドレスの種類を指定**** し、 `other`型をに設定して、ユーザー設定文字列に**otherlabel**を割り当てることができます。 たとえば、ボランティア活動に特定の電子メールアドレスを使用することができます。 **型**をに`other`設定し、 **otherlabel**をなどのカスタム文字列に`Volunteer work`設定します。 |

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
  "suppressions": [
    "Error: /api-reference/beta/resources/typedemailaddress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
