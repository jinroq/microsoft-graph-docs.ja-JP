---
title: teamsAsyncOperation リソースの種類
description: 'マイクロソフト チームの非同期操作は、操作を 1 つの API 要求の有効期間を超えてしまうことです。 '
ms.openlocfilehash: 66279b933202167f85ed7d1fc4709e8e61034537
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067854"
---
# <a name="teamsasyncoperation-resource-type"></a><span data-ttu-id="6cc21-103">teamsAsyncOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6cc21-103">teamsAsyncOperation resource type</span></span>

> <span data-ttu-id="6cc21-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6cc21-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6cc21-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6cc21-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6cc21-106">マイクロソフト チームの非同期操作は、操作を 1 つの API 要求の有効期間を超えてしまうことです。</span><span class="sxs-lookup"><span data-stu-id="6cc21-106">A Microsoft Teams async operation is an operation that transcends the lifetime of a single API request.</span></span> <span data-ttu-id="6cc21-107">これらの操作は、実行時間の長い、または、最初の要求の時間枠で完了するのにはコストが高すぎます。</span><span class="sxs-lookup"><span data-stu-id="6cc21-107">These operations are long-running or too expensive to complete within the timeframe of their originating request.</span></span>

<span data-ttu-id="6cc21-108">非同期操作が開始されると、メソッドは、202 の承諾済みの応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="6cc21-108">When an async operation is initiated, the method returns a 202 Accepted response code.</span></span> <span data-ttu-id="6cc21-109">応答は、teamsAsyncOperation の場所を含む場所のヘッダーも格納されます。</span><span class="sxs-lookup"><span data-stu-id="6cc21-109">The response will also contain a Location header, which contains the location of the teamsAsyncOperation.</span></span> <span data-ttu-id="6cc21-110">この場所に GET 要求を行うことによって、オペレーションのステータスを定期的にチェックします。待機 > 30 秒間隔でチェックします。</span><span class="sxs-lookup"><span data-stu-id="6cc21-110">Periodically check the status of the operation by making a GET request to this location; wait >30 seconds between checks.</span></span>
<span data-ttu-id="6cc21-111">要求が正常に完了したら、状態は、"成功し、targetResourceLocation が作成/変更したリソースを指します。</span><span class="sxs-lookup"><span data-stu-id="6cc21-111">When the request completes successfully, the status will be "succeeded" and the targetResourceLocation will point to the created/modified resource.</span></span>

## <a name="properties"></a><span data-ttu-id="6cc21-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6cc21-112">Properties</span></span>

| <span data-ttu-id="6cc21-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6cc21-113">Property</span></span> | <span data-ttu-id="6cc21-114">型</span><span class="sxs-lookup"><span data-stu-id="6cc21-114">Type</span></span>   | <span data-ttu-id="6cc21-115">説明</span><span class="sxs-lookup"><span data-stu-id="6cc21-115">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="6cc21-116">ID</span><span class="sxs-lookup"><span data-stu-id="6cc21-116">id</span></span>|<span data-ttu-id="6cc21-117">文字列</span><span class="sxs-lookup"><span data-stu-id="6cc21-117">string</span></span> |<span data-ttu-id="6cc21-118">操作の一意の id です。</span><span class="sxs-lookup"><span data-stu-id="6cc21-118">Unique operation id.</span></span>|
|<span data-ttu-id="6cc21-119">入力</span><span class="sxs-lookup"><span data-stu-id="6cc21-119">operationType</span></span>|[<span data-ttu-id="6cc21-120">teamsAsyncOperationType</span><span class="sxs-lookup"><span data-stu-id="6cc21-120">teamsAsyncOperationType</span></span>](teamsasyncoperationtype.md) |<span data-ttu-id="6cc21-121">説明している操作の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="6cc21-121">Denotes which type of operation is being described.</span></span>|
|<span data-ttu-id="6cc21-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6cc21-122">createdDateTime</span></span>|<span data-ttu-id="6cc21-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6cc21-123">DateTimeOffset</span></span> |<span data-ttu-id="6cc21-124">操作が作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="6cc21-124">Time when the operation was created.</span></span>|
|<span data-ttu-id="6cc21-125">status</span><span class="sxs-lookup"><span data-stu-id="6cc21-125">status</span></span>|[<span data-ttu-id="6cc21-126">teamsAsyncOperationStatus</span><span class="sxs-lookup"><span data-stu-id="6cc21-126">teamsAsyncOperationStatus</span></span>](teamsasyncoperationstatus.md)| <span data-ttu-id="6cc21-127">操作の状態です。</span><span class="sxs-lookup"><span data-stu-id="6cc21-127">Operation status.</span></span>|
|<span data-ttu-id="6cc21-128">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="6cc21-128">lastActionDateTime</span></span>|<span data-ttu-id="6cc21-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6cc21-129">DateTimeOffset</span></span> |<span data-ttu-id="6cc21-130">非同期操作が最後に更新された時間です。</span><span class="sxs-lookup"><span data-stu-id="6cc21-130">Time when the async operation was last updated.</span></span>|
|<span data-ttu-id="6cc21-131">attemptsCount</span><span class="sxs-lookup"><span data-stu-id="6cc21-131">attemptsCount</span></span>|<span data-ttu-id="6cc21-132">Int32</span><span class="sxs-lookup"><span data-stu-id="6cc21-132">Int32</span></span>|<span data-ttu-id="6cc21-133">成功または失敗にマークされる前に操作が試行された回数です。</span><span class="sxs-lookup"><span data-stu-id="6cc21-133">Number of times the operation was attempted before being marked successful or failed.</span></span>|
|<span data-ttu-id="6cc21-134">targetResourceId</span><span class="sxs-lookup"><span data-stu-id="6cc21-134">targetResourceId</span></span>|<span data-ttu-id="6cc21-135">guid</span><span class="sxs-lookup"><span data-stu-id="6cc21-135">guid</span></span> |<span data-ttu-id="6cc21-136">作成または[チーム](../resources/team.md)では通常、この非同期操作を受けて変更されたオブジェクトの ID です。</span><span class="sxs-lookup"><span data-stu-id="6cc21-136">The ID of the object that's created or modified as result of this async operation, typically a [team](../resources/team.md).</span></span>|
|<span data-ttu-id="6cc21-137">targetResourceLocation</span><span class="sxs-lookup"><span data-stu-id="6cc21-137">targetResourceLocation</span></span>|<span data-ttu-id="6cc21-138">文字列</span><span class="sxs-lookup"><span data-stu-id="6cc21-138">string</span></span>|<span data-ttu-id="6cc21-139">作成または、この非同期操作を受けて変更されたオブジェクトの位置。</span><span class="sxs-lookup"><span data-stu-id="6cc21-139">The location of the object that's created or modified as result of this async operation.</span></span> <span data-ttu-id="6cc21-140">この URL は非透過値として扱われます、そのコンポーネントのパスには解析されませんする必要があります。</span><span class="sxs-lookup"><span data-stu-id="6cc21-140">This URL should be treated as an opaque value and not parsed into its component paths.</span></span>|
|<span data-ttu-id="6cc21-141">エラー</span><span class="sxs-lookup"><span data-stu-id="6cc21-141">error</span></span>|[<span data-ttu-id="6cc21-142">operationError</span><span class="sxs-lookup"><span data-stu-id="6cc21-142">operationError</span></span>](operationerror.md)|<span data-ttu-id="6cc21-143">非同期操作が失敗の原因となるすべてのエラーです。</span><span class="sxs-lookup"><span data-stu-id="6cc21-143">Any error that causes the async operation to fail.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6cc21-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6cc21-144">JSON representation</span></span>

<span data-ttu-id="6cc21-145">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6cc21-145">The following is a JSON representation of the resource.</span></span>

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
