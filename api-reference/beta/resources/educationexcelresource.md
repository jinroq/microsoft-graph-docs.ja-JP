---
title: educationExcelResource リソースの種類
description: 'EducationResource のサブクラスです。 この種類のリソースでは、Excel ドキュメントを表します。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 11f28da1f2acaecbdd4f57abe8c6c8a03fbac0f9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982373"
---
# <a name="educationexcelresource-resource-type"></a>educationExcelResource リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[EducationResource](educationresource.md)のサブクラスです。 この種類のリソースでは、Excel ドキュメントを表します。  
 
>**注:** Excel ファイルは、このリソースが所属する割り当てまたは提出書類のオブジェクトに関連付けられているリソースのフォルダーにする必要があります。


## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|fileUrl|String|Excel ファイルのオブジェクトへのポインター。|

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
<!-- {
  "type": "#page.annotation",
  "description": "educationExcelResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
