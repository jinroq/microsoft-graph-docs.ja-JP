---
title: アプリケーション リソースの種類
description: ブックを管理する Excel アプリケーションを表します。
localization_priority: Normal
ms.openlocfilehash: a8e2124910301818e753b1f90a3168da3a072862
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804439"
---
# <a name="application-resource-type"></a>アプリケーション リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

ブックを管理する Excel アプリケーションを表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[アプリケーションを取得します。](../api/excelapplication-get.md) | [Application](application.md) |アプリケーション オブジェクトのプロパティと関係を参照してください。|
|[Calculate](../api/excelapplication-calculate.md)|なし|Excel で現在開いているすべてのブックを再計算します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|calculationMode|文字列|ブックで使用される計算モードを返します。 可能な値は、`Automatic`、`AutomaticExceptTables`、`Manual` です。 読み取り専用です。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.application"
}-->

```json
{
  "calculationMode": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Application resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
