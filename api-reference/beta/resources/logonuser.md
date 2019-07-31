---
title: logonUser リソースの種類
description: このホストにログオンしているユーザーに関するステートフルな情報を含みます。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 08053b2e3ba42c167edebb3678b41ccb3531e078
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009917"
---
# <a name="logonuser-resource-type"></a>logonUser リソースの種類

このホストにログオンしているユーザーに関するステートフルな情報を含みます。

## <a name="properties"></a>プロパティ

| プロパティ   | 型 |説明|
|:---------------|:--------|:----------|
|accountDomain|String|ログオンに使用されるユーザーアカウントのドメイン。|
|accountName|String|ログオンに使用されるユーザーアカウントのアカウント名。|
|accountType|String|ユーザーアカウントの種類 (Windows 定義あたり)。 使用可能な値は、`unknown`、`standard`、`power`、`administrator` です。|
|firstSeenDateTime|DateTimeOffset|このユーザーアカウントによる最も早いログオンが発生した日時 (プロバイダーが決定した期間)。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|lastSeenDateTime|DateTimeOffset|このユーザーアカウントによる最新のログオンが発生した DateTime。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|logonId|String|ユーザーログオン ID。|
|logonTypes|文字列コレクション|最初に表示された時点から、ログオンしているユーザーに対して観測されたログオンの種類のコレクション。 使用可能な値: `unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service`。|

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
