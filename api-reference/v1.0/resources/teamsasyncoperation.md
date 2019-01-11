---
title: teamsAsyncOperation リソースの種類
description: 'マイクロソフト チームの非同期操作は、操作を 1 つの API 要求の有効期間を超えてしまうことです。 '
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 607730ff48213b45177560046dc6f38afe1bcc75
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873620"
---
# <a name="teamsasyncoperation-resource-type"></a><span data-ttu-id="1477d-103">teamsAsyncOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1477d-103">teamsAsyncOperation resource type</span></span>



<span data-ttu-id="1477d-104">マイクロソフト チームの非同期操作は、操作を 1 つの API 要求の有効期間を超えてしまうことです。</span><span class="sxs-lookup"><span data-stu-id="1477d-104">A Microsoft Teams async operation is an operation that transcends the lifetime of a single API request.</span></span> <span data-ttu-id="1477d-105">これらの操作は、実行時間の長い、または、最初の要求の時間枠で完了するのにはコストが高すぎます。</span><span class="sxs-lookup"><span data-stu-id="1477d-105">These operations are long-running or too expensive to complete within the timeframe of their originating request.</span></span>

<span data-ttu-id="1477d-106">非同期操作が開始されると、メソッドは、202 の承諾済みの応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="1477d-106">When an async operation is initiated, the method returns a 202 Accepted response code.</span></span> <span data-ttu-id="1477d-107">応答は、teamsAsyncOperation の場所を含む場所のヘッダーも格納されます。</span><span class="sxs-lookup"><span data-stu-id="1477d-107">The response will also contain a Location header, which contains the location of the teamsAsyncOperation.</span></span> <span data-ttu-id="1477d-108">この場所に GET 要求を行うことによって、オペレーションのステータスを定期的にチェックします。待機 > 30 秒間隔でチェックします。</span><span class="sxs-lookup"><span data-stu-id="1477d-108">Periodically check the status of the operation by making a GET request to this location; wait >30 seconds between checks.</span></span>
<span data-ttu-id="1477d-109">要求が正常に完了したら、状態は、"成功し、targetResourceLocation が作成/変更したリソースを指します。</span><span class="sxs-lookup"><span data-stu-id="1477d-109">When the request completes successfully, the status will be "succeeded" and the targetResourceLocation will point to the created/modified resource.</span></span>

## <a name="properties"></a><span data-ttu-id="1477d-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1477d-110">Properties</span></span>

| <span data-ttu-id="1477d-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1477d-111">Property</span></span> | <span data-ttu-id="1477d-112">種類</span><span class="sxs-lookup"><span data-stu-id="1477d-112">Type</span></span>   | <span data-ttu-id="1477d-113">説明</span><span class="sxs-lookup"><span data-stu-id="1477d-113">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="1477d-114">ID</span><span class="sxs-lookup"><span data-stu-id="1477d-114">id</span></span>|<span data-ttu-id="1477d-115">文字列</span><span class="sxs-lookup"><span data-stu-id="1477d-115">string</span></span> |<span data-ttu-id="1477d-116">操作の一意の id です。</span><span class="sxs-lookup"><span data-stu-id="1477d-116">Unique operation id.</span></span>|
|<span data-ttu-id="1477d-117">入力</span><span class="sxs-lookup"><span data-stu-id="1477d-117">operationType</span></span>|[<span data-ttu-id="1477d-118">teamsAsyncOperationType</span><span class="sxs-lookup"><span data-stu-id="1477d-118">teamsAsyncOperationType</span></span>](teamsasyncoperationtype.md) |<span data-ttu-id="1477d-119">説明している操作の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="1477d-119">Denotes which type of operation is being described.</span></span>|
|<span data-ttu-id="1477d-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1477d-120">createdDateTime</span></span>|<span data-ttu-id="1477d-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1477d-121">DateTimeOffset</span></span> |<span data-ttu-id="1477d-122">操作が作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="1477d-122">Time when the operation was created.</span></span>|
|<span data-ttu-id="1477d-123">status</span><span class="sxs-lookup"><span data-stu-id="1477d-123">status</span></span>|[<span data-ttu-id="1477d-124">teamsAsyncOperationStatus</span><span class="sxs-lookup"><span data-stu-id="1477d-124">teamsAsyncOperationStatus</span></span>](teamsasyncoperationstatus.md)| <span data-ttu-id="1477d-125">操作の状態です。</span><span class="sxs-lookup"><span data-stu-id="1477d-125">Operation status.</span></span>|
|<span data-ttu-id="1477d-126">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="1477d-126">lastActionDateTime</span></span>|<span data-ttu-id="1477d-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1477d-127">DateTimeOffset</span></span> |<span data-ttu-id="1477d-128">非同期操作が最後に更新された時間です。</span><span class="sxs-lookup"><span data-stu-id="1477d-128">Time when the async operation was last updated.</span></span>|
|<span data-ttu-id="1477d-129">attemptsCount</span><span class="sxs-lookup"><span data-stu-id="1477d-129">attemptsCount</span></span>|<span data-ttu-id="1477d-130">Int32</span><span class="sxs-lookup"><span data-stu-id="1477d-130">Int32</span></span>|<span data-ttu-id="1477d-131">成功または失敗にマークされる前に操作が試行された回数です。</span><span class="sxs-lookup"><span data-stu-id="1477d-131">Number of times the operation was attempted before being marked successful or failed.</span></span>|
|<span data-ttu-id="1477d-132">targetResourceId</span><span class="sxs-lookup"><span data-stu-id="1477d-132">targetResourceId</span></span>|<span data-ttu-id="1477d-133">guid</span><span class="sxs-lookup"><span data-stu-id="1477d-133">guid</span></span> |<span data-ttu-id="1477d-134">作成または[チーム](../resources/team.md)では通常、この非同期操作を受けて変更されたオブジェクトの ID です。</span><span class="sxs-lookup"><span data-stu-id="1477d-134">The ID of the object that's created or modified as result of this async operation, typically a [team](../resources/team.md).</span></span>|
|<span data-ttu-id="1477d-135">targetResourceLocation</span><span class="sxs-lookup"><span data-stu-id="1477d-135">targetResourceLocation</span></span>|<span data-ttu-id="1477d-136">文字列</span><span class="sxs-lookup"><span data-stu-id="1477d-136">string</span></span>|<span data-ttu-id="1477d-137">作成または、この非同期操作を受けて変更されたオブジェクトの位置。</span><span class="sxs-lookup"><span data-stu-id="1477d-137">The location of the object that's created or modified as result of this async operation.</span></span> <span data-ttu-id="1477d-138">この URL は非透過値として扱われます、そのコンポーネントのパスには解析されませんする必要があります。</span><span class="sxs-lookup"><span data-stu-id="1477d-138">This URL should be treated as an opaque value and not parsed into its component paths.</span></span>|
|<span data-ttu-id="1477d-139">エラー</span><span class="sxs-lookup"><span data-stu-id="1477d-139">error</span></span>|[<span data-ttu-id="1477d-140">operationError</span><span class="sxs-lookup"><span data-stu-id="1477d-140">operationError</span></span>](operationerror.md)|<span data-ttu-id="1477d-141">非同期操作が失敗の原因となるすべてのエラーです。</span><span class="sxs-lookup"><span data-stu-id="1477d-141">Any error that causes the async operation to fail.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1477d-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1477d-142">JSON representation</span></span>

<span data-ttu-id="1477d-143">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1477d-143">The following is a JSON representation of the resource.</span></span>

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
