---
title: educationFileResource リソースの種類
description: educationResource のサブクラスで、割り当てまたは送信に関連付けられているファイルオブジェクトを表します。  この例では、ファイルは特別なファイル (Word、Excel など) の1つではなく、システム内で特別な処理を行わないファイルです。 ファイルリソースは、このリソースが添付されている割り当てまたは送信に関連付けられている**resourcefolder**に格納されている必要があります。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9a851c66e137da1941df9b0268657c9e1b7392b3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334248"
---
# <a name="educationfileresource-resource-type"></a>educationFileResource リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[educationResource](educationresource.md)のサブクラスで、割り当てまたは送信に関連付けられているファイルオブジェクトを表します。  この例では、ファイルは特別なファイル (Word、Excel など) の1つではなく、システム内で特別な処理を行わないファイルです。 ファイルリソースは、このリソースが添付されている割り当てまたは送信に関連付けられている**resourcefolder**に格納されている必要があります。

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
