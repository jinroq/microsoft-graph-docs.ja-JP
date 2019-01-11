---
title: logonUser のリソースの種類
description: このホスト上のログオン中のユーザーに関するステートフルな情報が含まれています
localization_priority: Normal
ms.openlocfilehash: 3b7862555c62eb16aaceaa53d4df58541426e08a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855595"
---
# <a name="logonuser-resource-type"></a>logonUser のリソースの種類

このホスト上のログオン中のユーザーに関するステートフルな情報が含まれています

## <a name="properties"></a>プロパティ

| プロパティ   | 種類 |説明|
|:---------------|:--------|:----------|
|accountDomain|String|使用するユーザー アカウントのドメインにログオンします。|
|accountName|String|使用するユーザー アカウントのアカウント名をログオンします。|
|accountType|String|ユーザー アカウントの種類、Windows の定義ごと。 可能な値は、`unknown`、`standard`、`power`、`administrator` です。|
|firstSeenDateTime|DateTimeOffset|このユーザー アカウントで最初のログオンが発生した日時 (プロバイダーが指定した期間)。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|lastSeenDateTime|DateTimeOffset|このユーザー アカウントで最新のログオンが発生した日時。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|logonId|String|ユーザー ログオン ID|
|logonTypes|String コレクション|最初に最後に表示されたときからログオンしたユーザーを確認するログオンの種類のコレクションです。 使用可能な値: `unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service`。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.logonUser"
}-->

```json
{
  "accountDomain": "String",
  "accountName": "String",
  "accountType": "String",
  "firstSeenDateTime": "String (timestamp)",
  "lastSeenDateTime": "String (timestamp)",
  "logonId": "String",
  "logonTypes": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "logonUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
