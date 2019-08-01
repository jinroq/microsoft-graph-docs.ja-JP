---
title: teamsAsyncOperation リソースの種類
description: 'Microsoft Teams の非同期操作は、1つの API 要求の有効期間を transcends する操作です。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9c604d8823de4f48e4338b9637861e8a09505b78
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033755"
---
# <a name="teamsasyncoperation-resource-type"></a>teamsAsyncOperation リソースの種類



Microsoft Teams の非同期操作は、1つの API 要求の有効期間を transcends する操作です。 これらの操作は、送信元の要求の時間内に実行するのに時間がかかる場合があります。

Async 操作が開始されると、メソッドは202の受け入れられた応答コードを返します。 また、応答には、teamsAsyncOperation の場所が含まれている場所のヘッダーも含まれます。 この場所に GET 要求を行うことによって、操作の状態を定期的にチェックします。チェックが終わるまで30秒 >。
要求が正常に完了すると、状態は "succeeded" になり、targetResourceLocation は作成/変更されたリソースを参照するようになります。

## <a name="properties"></a>プロパティ

| プロパティ | 型   | 説明 |
|:---------------|:--------|:----------|
|id|string |一意の操作 id。|
|operationType|[teamsAsyncOperationType](teamsasyncoperationtype.md) |説明されている操作の種類を示します。|
|createdDateTime|DateTimeOffset |操作が作成された時刻。|
|status|[teamsAsyncOperationStatus](teamsasyncoperationstatus.md)| 操作の状態。|
|lastActionDateTime|DateTimeOffset |Async 操作が最後に更新された時刻。|
|attemptsCount|Int32|操作が成功したか失敗したかがマークされるまでの、操作が試行された回数。|
|targetResourceId|guid |この非同期操作の結果として作成または変更されるオブジェクトの ID (通常は[チーム](../resources/team.md))。|
|targetResourceLocation|string|この非同期操作の結果として作成または変更されたオブジェクトの場所。 この URL は、不透明な値として扱われ、そのコンポーネントのパスに解析されることはありません。|
|error|[operationError](operationerror.md)|非同期操作が失敗する原因となるエラー。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsasyncoperation"
}-->

```json
{
    "id": "string",
    "operationType": "archiveTeam",
    "createdDateTime": "2018-01-01T00:00:00.0000000Z",
    "status": "succeeded",
    "lastActionDateTime": "2018-01-01T00:00:00.0000000Z",
    "attemptsCount": 1,
    "targetResourceId": "fa4aa5a2-a75b-4769-86f4-9e2742a18fda",
    "targetResourceLocation": "/groups('fa4aa5a2-a75b-4769-86f4-9e2742a18fda')/team",
    "error": null
}
```

<!-- uuid: 20fd7863-9545-40d4-ae8f-fee2d115a690
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teams async operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
