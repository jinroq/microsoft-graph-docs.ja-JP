---
title: filehash リソースの種類
description: ファイルハッシュ (暗号化と場所に依存) に関するステートフルな情報を含みます。
localization_priority: Normal
ms.openlocfilehash: f5d865a7ded230ca611b8628c3648ec1e331c67d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547607"
---
# <a name="filehash-resource-type"></a>filehash リソースの種類

ファイルハッシュ (暗号化と場所に依存) に関するステートフルな情報を含みます。

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|hashtype|[filehashtype](filehashtypeenumtype.md)列挙型|ファイルハッシュの種類。 可能な値は、`unknown`、`sha1`、`sha256`、`md5`、`authenticodeHash256`、`lsHash`、`ctph`、`peSha1`、`peSha256` です。|
|hashvalue|String|ファイルハッシュの値。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileHash"
}-->

```json
{
  "hashType": "@odata.type: microsoft.graph.fileHashType",
  "hashValue": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileHash resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
