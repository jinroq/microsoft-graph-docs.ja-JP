---
title: プロセスリソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。"
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 6b67ec28dadb09442c5e3d66b6c03c54db821a85
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965692"
---
# <a name="process-resource-type"></a>プロセスリソースの種類

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通知に関連するプロセスに関するステートフルな情報を含みます。

## <a name="properties"></a>プロパティ

| プロパティ   | 型|説明|
|:---------------|:--------|:----------|
|accountName|String|ユーザーアカウント識別子 (アカウントの下で実行されたユーザーアカウントコンテキスト)。たとえば、AccountName、SID など。|
|commandLine|String|すべてのパラメーターを含む完全なプロセス呼び出しの commandline。|
|createdDateTime|DateTimeOffset|プロセスが開始された時刻。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|fileHash|[fileHash](filehash.md)|ファイルハッシュを含む複合型 (暗号化と場所に依存)。|
|integrityLevel|processIntegrityLevel|プロセスの整合性レベル。 使用可能な値: `unknown`、`untrusted`、`low`、`medium`、`high`、`system`。|
|isElevated|Boolean|プロセスが昇格された場合は True。|
|name|String|プロセスのイメージファイルの名前。|
|Parentprocess/Datetime|DateTimeOffset|親プロセスが開始された DateTime。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|parentProcessId|Int32|親プロセスのプロセス ID (PID)。|
|parentProcessName|String|親プロセスのイメージファイルの名前。|
|path|String|ファイル名を含む完全なパス。|
|processId|Int32|プロセスのプロセス ID (PID)。|

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
  "suppressions": []
}
-->
