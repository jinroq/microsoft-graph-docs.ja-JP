---
title: educationWordResource リソースの種類
description: 'EducationResource のサブクラス。 これは Word ドキュメントリソースです。 Word ファイルは、に関連付けられた**fileResource**ディレクトリにアップロードする必要があります。 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 0bd326ea45130da7e7eadb7eb1d21ae3a6c31cce
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972286"
---
# <a name="educationwordresource-resource-type"></a>educationWordResource リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[EducationResource](educationresource.md)のサブクラス。 これは Word ドキュメントリソースです。 Word ファイルは、割り当てまたは送信に関連付けられている**fileResource**ディレクトリにアップロードする必要があります。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|fileUrl|String|ディスク上のファイルの場所。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationWordResource"
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
  "description": "educationWordResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
