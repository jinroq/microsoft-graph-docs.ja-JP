---
title: プロセス リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
ms.openlocfilehash: 36acd6ed0f6e2cee5095d445de3ba4ff024a024a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869469"
---
# <a name="process-resource-type"></a>プロセス リソースの種類

 > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

ステートフルなアラートに関連するプロセスについてを説明します。

## <a name="properties"></a>プロパティ

| プロパティ   | 種類|説明|
|:---------------|:--------|:----------|
|accountName|String|ユーザーは、例、アカウント名、SID、およびように識別子 (ユーザー アカウントのコンテキストでプロセスが実行された) を考慮します。|
|commandLine|String|完全な処理の呼び出しは、すべてのパラメーターを含むを使用できます。|
|createdDateTime|DateTimeOffset|プロセスが開始された時刻です。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|fileHash|[fileHash](filehash.md)|複合型の暗号化などの場所に依存したファイルのハッシュが含まれています。|
|integrityLevel|processIntegrityLevel|プロセスの整合性レベルです。 使用可能な値: `unknown`、`untrusted`、`low`、`medium`、`high`、`system`。|
|isElevated|ブール型|プロセスが昇格した場合は true。|
|名前|String|プロセスのイメージ ファイルの名前です。|
|parentProcessCreatedDateTime|DateTimeOffset|親プロセスの開始日時。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|parentProcessId|Int32|プロセス ID (PID) の親プロセスです。|
|parentProcessName|String|親プロセスのイメージ ファイルの名前です。|
|path|String|ファイル名を含む完全パスです。|
|プロセス Id|Int32|プロセス ID (PID) のプロセスです。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.process"
}-->

```json
{
  "accountName": "String",
  "commandLine": "String",
  "createdDateTime": "String (timestamp)",
  "fileHash": {"@odata.type": "microsoft.graph.fileHash"},
  "integrityLevel": "@odata.type: microsoft.graph.processIntegrityLevel",
  "isElevated": true,
  "name": "String",
  "parentProcessCreatedDateTime": "String (timestamp)",
  "parentProcessId": 1024,
  "parentProcessName": "String",
  "path": "String",
  "processId": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "process resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
