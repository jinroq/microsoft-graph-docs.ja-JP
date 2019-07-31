---
title: fileSecurityState リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。"
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: f061ca71bcd16c16e0292673338e2cb8d915e845
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972013"
---
# <a name="filesecuritystate-resource-type"></a>fileSecurityState リソースの種類

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
<!--
{
  "type": "#page.annotation",
  "description": "fileSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
