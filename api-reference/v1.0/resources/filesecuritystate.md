---
title: fileSecurityState リソースの種類
description: 通知に関連するファイル (プロセスではない) に関する情報が含まれます。
localization_priority: Normal
ms.openlocfilehash: 14ffa41b395bde04972f0af0436297aa4d038524
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564793"
---
# <a name="filesecuritystate-resource-type"></a>fileSecurityState リソースの種類

通知に関連するファイル (プロセスではない) に関する情報が含まれます。

## <a name="properties"></a>プロパティ

| プロパティ   | 型|説明|
|:---------------|:--------|:----------|
|fileHash|[fileHash](filehash.md)|ファイルハッシュを含む複合型 (暗号化と場所に依存)。|
|name|String|ファイル名 (パスなし)。|
|path|String|ファイル/イメージファイルの完全なファイルパス。|
|riskScore|String|通知ファイルのプロバイダーが生成/計算したリスクスコア。 推奨値の範囲0-1。パーセンテージに相当します。|

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
