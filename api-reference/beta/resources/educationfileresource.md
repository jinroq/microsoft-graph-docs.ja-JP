---
title: educationFileResource リソースの種類
description: EducationResource のサブクラスで、割り当てまたは送信に関連付けられているファイルオブジェクトを表します。  この例では、ファイルは特別なファイル (Word、Excel など) の1つではなく、システム内で特別な処理を行わないファイルです。 ファイルリソースは、このリソースが添付されている割り当てまたは送信に関連付けられている**Resourcefolder**に格納されている必要があります。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 678591d4c9662f1ab3fc68f7d35a0ec525c6e74f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972744"
---
# <a name="educationfileresource-resource-type"></a>educationFileResource リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[EducationResource](educationresource.md)のサブクラスで、割り当てまたは送信に関連付けられているファイルオブジェクトを表します。  この例では、ファイルは特別なファイル (Word、Excel など) の1つではなく、システム内で特別な処理を行わないファイルです。 ファイルリソースは、このリソースが添付されている割り当てまたは送信に関連付けられている**Resourcefolder**に格納されている必要があります。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|fileUrl|String|ファイルリソースのディスク上の場所です。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFileResource"
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
  "description": "educationFileResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
