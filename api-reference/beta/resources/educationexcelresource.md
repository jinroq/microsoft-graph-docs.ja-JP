---
title: educationExcelResource リソースの種類
description: 'EducationResource のサブクラスです。 この種類のリソースでは、Excel ドキュメントを表します。  '
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 7f772f7911667c76e64c31a856f3a9f8b6f3e6ff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858101"
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
