---
title: teamsAsyncOperation リソースの種類
description: 'マイクロソフト チームの非同期操作は、操作を 1 つの API 要求の有効期間を超えてしまうことです。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 61c26b0d594ccdbad8020557f60c6f6b23a83254
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513460"
---
# <a name="teamsasyncoperation-resource-type"></a>teamsAsyncOperation リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

マイクロソフト チームの非同期操作は、操作を 1 つの API 要求の有効期間を超えてしまうことです。 これらの操作は、実行時間の長い、または、最初の要求の時間枠で完了するのにはコストが高すぎます。

非同期操作が開始されると、メソッドは、202 の承諾済みの応答コードを返します。 応答は、teamsAsyncOperation の場所を含む場所のヘッダーも格納されます。 この場所に GET 要求を行うことによって、オペレーションのステータスを定期的にチェックします。チェックの間の >30 秒間を待ちます。
要求が正常に完了したら、状態は、"成功し、targetResourceLocation が作成/変更したリソースを指します。

## <a name="properties"></a>プロパティ

| プロパティ | 型   | 説明 |
|:---------------|:--------|:----------|
|id|string |操作の一意の id です。|
|入力|[teamsAsyncOperationType](teamsasyncoperationtype.md) |説明している操作の種類を表します。|
|createdDateTime|DateTimeOffset |操作が作成された時刻。|
|status|[teamsAsyncOperationStatus](teamsasyncoperationstatus.md)| 操作の状態です。|
|lastActionDateTime|DateTimeOffset |非同期操作が最後に更新された時間です。|
|attemptsCount|Int32|成功または失敗にマークされる前に操作が試行された回数です。|
|targetResourceId|guid |作成または[チーム](../resources/team.md)では通常、この非同期操作を受けて変更されたオブジェクトの ID です。|
|targetResourceLocation|string|作成または、この非同期操作を受けて変更されたオブジェクトの位置。 この URL は非透過値として扱われます、そのコンポーネントのパスには解析されませんする必要があります。|
|エラー|[operationError](operationerror.md)|非同期操作が失敗の原因となるすべてのエラーです。|

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
<!--
{
  "type": "#page.annotation",
  "description": "teams async operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsasyncoperation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
