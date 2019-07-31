---
title: educationExcelResource リソースの種類
description: 'EducationResource のサブクラス。 このリソースの種類は、Excel ドキュメントを表します。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ef85a92b2629e8a652ce59210018725d6afecb9a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972748"
---
# <a name="educationexcelresource-resource-type"></a>educationExcelResource リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[EducationResource](educationresource.md)のサブクラス。 このリソースの種類は、Excel ドキュメントを表します。  
 
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
  "suppressions": []
}
-->
