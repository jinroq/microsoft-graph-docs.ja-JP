---
title: プロセス リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
ms.openlocfilehash: 13de9a2485aeeaa06fdad3c7cce3eb1f81374193
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521209"
---
# <a name="process-resource-type"></a>プロセス リソースの種類

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ステートフルなアラートに関連するプロセスについてを説明します。

## <a name="properties"></a>プロパティ

| プロパティ   | 型|説明|
|:---------------|:--------|:----------|
|accountName|String|ユーザーは、例、アカウント名、SID、およびように識別子 (ユーザー アカウントのコンテキストでプロセスが実行された) を考慮します。|
|commandLine|String|完全な処理の呼び出しは、すべてのパラメーターを含むを使用できます。|
|createdDateTime|DateTimeOffset|プロセスが開始された時刻です。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。|
|fileHash|[fileHash](filehash.md)|複合型の暗号化などの場所に依存したファイルのハッシュが含まれています。|
|integrityLevel|processIntegrityLevel|プロセスの整合性レベルです。 使用可能な値: `unknown`、`untrusted`、`low`、`medium`、`high`、`system`。|
|isElevated|ブール値|プロセスが昇格した場合は true。|
|name|String|プロセスのイメージ ファイルの名前です。|
|parentProcessCreatedDateTime|DateTimeOffset|親プロセスの開始日時。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。|
|parentProcessId|Int32|プロセス ID (PID) の親プロセスです。|
|parentProcessName|String|親プロセスのイメージ ファイルの名前です。|
|path|String|ファイル名を含む完全パスです。|
|ProcessID|Int32|プロセス ID (PID) のプロセスです。|

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
<!--
{
  "type": "#page.annotation",
  "description": "process resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/process.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
