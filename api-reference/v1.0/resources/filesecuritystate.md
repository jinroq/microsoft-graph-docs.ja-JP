---
title: fileSecurityState リソースの種類
description: アラートに関連するファイル (プロセスではない) に関する情報が含まれています。
localization_priority: Normal
ms.openlocfilehash: 14ffa41b395bde04972f0af0436297aa4d038524
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894097"
---
# <a name="filesecuritystate-resource-type"></a>fileSecurityState リソースの種類

アラートに関連するファイル (プロセスではない) に関する情報が含まれています。

## <a name="properties"></a>プロパティ

| プロパティ   | 種類|説明|
|:---------------|:--------|:----------|
|fileHash|[fileHash](filehash.md)|複合型の暗号化などの場所に依存したファイルのハッシュが含まれています。|
|名前|String|ファイルの名前 (パス) です。|
|path|String|ファイルとイメージ ファイルのファイルの完全パスです。|
|riskScore|String|プロバイダー生成された計算されるリスクの警告ファイルのスコアです。 0 - 1 パーセントに相当する値の範囲をお勧めします。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileSecurityState"
}-->

```json
{
  "fileHash": {"@odata.type": "microsoft.graph.fileHash"},
  "name": "String",
  "path": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
