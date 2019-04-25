---
title: educationExcelResource リソースの種類
description: 'educationResource のサブクラス。 このリソースの種類は、Excel ドキュメントを表します。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 14d7823f166ca12d202a6561bc9fe7b158ab7476
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542824"
---
# <a name="educationexcelresource-resource-type"></a>educationExcelResource リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[educationResource](educationresource.md)のサブクラス。 このリソースの種類は、Excel ドキュメントを表します。  
 
>**注:** Excel ファイルは、このリソースが属する assignment または送信オブジェクトに関連付けられたリソースフォルダーにある必要があります。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|fileUrl|String|Excel ファイルオブジェクトへのポインター。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationExcelResource"
}-->

```json
{
  "fileUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationExcelResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationexcelresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
