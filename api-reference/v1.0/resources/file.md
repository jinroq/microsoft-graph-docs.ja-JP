---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: File
localization_priority: Normal
description: ファイル リソースは、ファイル関連のデータ項目を 1 つの構造にグループ化します。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 51ec91a635db2ca259ba84cea29304e4e6ac7cbb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030374"
---
# <a name="file-resource-type"></a>ファイル リソースの種類

**ファイル** リソースは、ファイル関連のデータ項目を 1 つの構造にグループ化します。

[**DriveItem**](driveitem.md) に null 以外の**ファイル** ファセットがある場合は、項目はファイルを表します。他のプロパティに加えて、ファイルにはファイルのバイト ストリームを含む**コンテンツ**関係があります。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.file"
}-->

```json
{
  "hashes": {"@odata.type": "microsoft.graph.hashes"},
  "mimeType": "string"
}
```

## <a name="properties"></a>プロパティ

| プロパティ | 型                    | 説明                                                                                                                                      |
|:---------|:------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| hashes   | [方向性](hashes.md) | ファイルのバイナリ コンテンツのハッシュ (利用可能な場合)。読み取り専用です。                                                                                    |
| mimeType | string                  | ファイルの MIME の種類。これはサーバーのロジックによって決定されます。またファイルのアップロード時に指定された値でない場合があります。読み取り専用です。 |

## <a name="remarks"></a>注釈 

DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。

<!-- {
  "type": "#page.annotation",
  "description": "The file facet describes properties of a file",
  "keywords": "file,item,facet",
  "section": "documentation",
  "tocPath": "Facets/File"
} -->
