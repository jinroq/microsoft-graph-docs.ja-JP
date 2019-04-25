---
title: educationFormResource リソースの種類
description: educationResource のサブクラス。 このリソースはフォームです。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5e0b03eeea8c0e9d22a9f7279c821f6d90211470
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542847"
---
# <a name="educationformresource-resource-type"></a>educationFormResource リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[educationResource](educationresource.md)のサブクラス。 このリソースはフォームです。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|originalFormId|String|フォームの元の id。|
|formId|String|フォームの Id。|
|isgroupform|ブール値|フォームがクラスグループに属しているかどうか。|
|viewurl|String|フォームの学生の URL。|
|viewurl|String|フォームの学生の URL。|
|editurl|String|フォームの教師 URL。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFormResource"
}-->

```json
{
  "originalFormId": "String"
  "formId": "String"
  "isGroupForm": "Boolean"
  "viewUrl": "String"
  "editUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationFormResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationformresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
