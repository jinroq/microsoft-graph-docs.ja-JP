---
title: fileHash リソースの種類
description: ステートフルな暗号化などの場所に依存したファイルのハッシュについてを説明します。
localization_priority: Normal
ms.openlocfilehash: 9d72812d1ad43999ea3ed5b28251d629b9380d47
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876770"
---
# <a name="filehash-resource-type"></a>fileHash リソースの種類

ステートフルな暗号化などの場所に依存したファイルのハッシュについてを説明します。

## <a name="properties"></a>プロパティ

| プロパティ     | 種類        | 説明 |
|:-------------|:------------|:------------|
|hashType|fileHashType|ファイル ハッシュ タイプを入力します。 可能な値は、`unknown`、`sha1`、`sha256`、`md5`、`authenticodeHash256`、`lsHash`、`ctph`、`peSha1`、`peSha256` です。|
|して|String|ファイル ハッシュの値です。|

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
