---
title: teamsAsyncOperation リソースの種類
description: 'マイクロソフト チームの非同期操作は、操作を 1 つの API 要求の有効期間を超えてしまうことです。 '
author: nkramer
ms.openlocfilehash: f88f5eba32fbd0629bf66a61dca963a7815988fd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305559"
---
# <a name="teamsasyncoperation-resource-type"></a><span data-ttu-id="64f5c-103">teamsAsyncOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="64f5c-103">teamsAsyncOperation resource type</span></span>

> <span data-ttu-id="64f5c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="64f5c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="64f5c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="64f5c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="64f5c-106">マイクロソフト チームの非同期操作は、操作を 1 つの API 要求の有効期間を超えてしまうことです。</span><span class="sxs-lookup"><span data-stu-id="64f5c-106">A Microsoft Teams async operation is an operation that transcends the lifetime of a single API request.</span></span> <span data-ttu-id="64f5c-107">これらの操作は、実行時間の長い、または、最初の要求の時間枠で完了するのにはコストが高すぎます。</span><span class="sxs-lookup"><span data-stu-id="64f5c-107">These operations are long-running or too expensive to complete within the timeframe of their originating request.</span></span>

<span data-ttu-id="64f5c-108">非同期操作が開始されると、メソッドは、202 の承諾済みの応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="64f5c-108">When an async operation is initiated, the method returns a 202 Accepted response code.</span></span> <span data-ttu-id="64f5c-109">応答は、teamsAsyncOperation の場所を含む場所のヘッダーも格納されます。</span><span class="sxs-lookup"><span data-stu-id="64f5c-109">The response will also contain a Location header, which contains the location of the teamsAsyncOperation.</span></span> <span data-ttu-id="64f5c-110">この場所に GET 要求を行うことによって、オペレーションのステータスを定期的にチェックします。待機 > 30 秒間隔でチェックします。</span><span class="sxs-lookup"><span data-stu-id="64f5c-110">Periodically check the status of the operation by making a GET request to this location; wait >30 seconds between checks.</span></span>
<span data-ttu-id="64f5c-111">要求が正常に完了したら、状態は、"成功し、targetResourceLocation が作成/変更したリソースを指します。</span><span class="sxs-lookup"><span data-stu-id="64f5c-111">When the request completes successfully, the status will be "succeeded" and the targetResourceLocation will point to the created/modified resource.</span></span>

## <a name="properties"></a><span data-ttu-id="64f5c-112">Properties</span><span class="sxs-lookup"><span data-stu-id="64f5c-112">Properties</span></span>

| <span data-ttu-id="64f5c-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="64f5c-113">Property</span></span> | <span data-ttu-id="64f5c-114">種類</span><span class="sxs-lookup"><span data-stu-id="64f5c-114">Type</span></span>   | <span data-ttu-id="64f5c-115">説明</span><span class="sxs-lookup"><span data-stu-id="64f5c-115">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="64f5c-116">ID</span><span class="sxs-lookup"><span data-stu-id="64f5c-116">id</span></span>|<span data-ttu-id="64f5c-117">string</span><span class="sxs-lookup"><span data-stu-id="64f5c-117">string</span></span> |<span data-ttu-id="64f5c-118">操作の一意の id です。</span><span class="sxs-lookup"><span data-stu-id="64f5c-118">Unique operation id.</span></span>|
|<span data-ttu-id="64f5c-119">入力</span><span class="sxs-lookup"><span data-stu-id="64f5c-119">operationType</span></span>|[<span data-ttu-id="64f5c-120">teamsAsyncOperationType</span><span class="sxs-lookup"><span data-stu-id="64f5c-120">teamsAsyncOperationType</span></span>](teamsasyncoperationtype.md) |<span data-ttu-id="64f5c-121">説明している操作の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="64f5c-121">Denotes which type of operation is being described.</span></span>|
|<span data-ttu-id="64f5c-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="64f5c-122">createdDateTime</span></span>|<span data-ttu-id="64f5c-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64f5c-123">DateTimeOffset</span></span> |<span data-ttu-id="64f5c-124">操作が作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="64f5c-124">Time when the operation was created.</span></span>|
|<span data-ttu-id="64f5c-125">status</span><span class="sxs-lookup"><span data-stu-id="64f5c-125">status</span></span>|[<span data-ttu-id="64f5c-126">teamsAsyncOperationStatus</span><span class="sxs-lookup"><span data-stu-id="64f5c-126">teamsAsyncOperationStatus</span></span>](teamsasyncoperationstatus.md)| <span data-ttu-id="64f5c-127">操作の状態です。</span><span class="sxs-lookup"><span data-stu-id="64f5c-127">Operation status.</span></span>|
|<span data-ttu-id="64f5c-128">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="64f5c-128">lastActionDateTime</span></span>|<span data-ttu-id="64f5c-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64f5c-129">DateTimeOffset</span></span> |<span data-ttu-id="64f5c-130">非同期操作が最後に更新された時間です。</span><span class="sxs-lookup"><span data-stu-id="64f5c-130">Time when the async operation was last updated.</span></span>|
|<span data-ttu-id="64f5c-131">attemptsCount</span><span class="sxs-lookup"><span data-stu-id="64f5c-131">attemptsCount</span></span>|<span data-ttu-id="64f5c-132">Int32</span><span class="sxs-lookup"><span data-stu-id="64f5c-132">Int32</span></span>|<span data-ttu-id="64f5c-133">成功または失敗にマークされる前に操作が試行された回数です。</span><span class="sxs-lookup"><span data-stu-id="64f5c-133">Number of times the operation was attempted before being marked successful or failed.</span></span>|
|<span data-ttu-id="64f5c-134">targetResourceId</span><span class="sxs-lookup"><span data-stu-id="64f5c-134">targetResourceId</span></span>|<span data-ttu-id="64f5c-135">guid</span><span class="sxs-lookup"><span data-stu-id="64f5c-135">guid</span></span> |<span data-ttu-id="64f5c-136">作成または[チーム](../resources/team.md)では通常、この非同期操作を受けて変更されたオブジェクトの ID です。</span><span class="sxs-lookup"><span data-stu-id="64f5c-136">The ID of the object that's created or modified as result of this async operation, typically a [team](../resources/team.md).</span></span>|
|<span data-ttu-id="64f5c-137">targetResourceLocation</span><span class="sxs-lookup"><span data-stu-id="64f5c-137">targetResourceLocation</span></span>|<span data-ttu-id="64f5c-138">string</span><span class="sxs-lookup"><span data-stu-id="64f5c-138">string</span></span>|<span data-ttu-id="64f5c-139">作成または、この非同期操作を受けて変更されたオブジェクトの位置。</span><span class="sxs-lookup"><span data-stu-id="64f5c-139">The location of the object that's created or modified as result of this async operation.</span></span> <span data-ttu-id="64f5c-140">この URL は非透過値として扱われます、そのコンポーネントのパスには解析されませんする必要があります。</span><span class="sxs-lookup"><span data-stu-id="64f5c-140">This URL should be treated as an opaque value and not parsed into its component paths.</span></span>|
|<span data-ttu-id="64f5c-141">エラー</span><span class="sxs-lookup"><span data-stu-id="64f5c-141">error</span></span>|[<span data-ttu-id="64f5c-142">operationError</span><span class="sxs-lookup"><span data-stu-id="64f5c-142">operationError</span></span>](operationerror.md)|<span data-ttu-id="64f5c-143">非同期操作が失敗の原因となるすべてのエラーです。</span><span class="sxs-lookup"><span data-stu-id="64f5c-143">Any error that causes the async operation to fail.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="64f5c-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="64f5c-144">JSON representation</span></span>

<span data-ttu-id="64f5c-145">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="64f5c-145">The following is a JSON representation of the resource.</span></span>

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