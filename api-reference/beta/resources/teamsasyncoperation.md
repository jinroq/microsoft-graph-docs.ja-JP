---
title: teamsAsyncOperation リソースの種類
description: 'Microsoft Teams の非同期操作は、1つの API 要求の有効期間を transcends する操作です。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c016b90ae6198204e9b99e3ae1e8d72b22919e8b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345771"
---
# <a name="teamsasyncoperation-resource-type"></a><span data-ttu-id="d6d63-103">teamsAsyncOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d6d63-103">teamsAsyncOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6d63-104">Microsoft Teams の非同期操作は、1つの API 要求の有効期間を transcends する操作です。</span><span class="sxs-lookup"><span data-stu-id="d6d63-104">A Microsoft Teams async operation is an operation that transcends the lifetime of a single API request.</span></span> <span data-ttu-id="d6d63-105">これらの操作は、送信元の要求の時間内に実行するのに時間がかかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="d6d63-105">These operations are long-running or too expensive to complete within the timeframe of their originating request.</span></span>

<span data-ttu-id="d6d63-106">async 操作が開始されると、メソッドは202の受け入れられた応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="d6d63-106">When an async operation is initiated, the method returns a 202 Accepted response code.</span></span> <span data-ttu-id="d6d63-107">また、応答には、teamsAsyncOperation の場所が含まれている場所のヘッダーも含まれます。</span><span class="sxs-lookup"><span data-stu-id="d6d63-107">The response will also contain a Location header, which contains the location of the teamsAsyncOperation.</span></span> <span data-ttu-id="d6d63-108">この場所に GET 要求を行うことによって、操作の状態を定期的にチェックします。チェックの間、>30 秒間待機します。</span><span class="sxs-lookup"><span data-stu-id="d6d63-108">Periodically check the status of the operation by making a GET request to this location; wait >30 seconds between checks.</span></span>
<span data-ttu-id="d6d63-109">要求が正常に完了すると、状態は "succeeded" になり、targetresourcelocation は作成/変更されたリソースを参照するようになります。</span><span class="sxs-lookup"><span data-stu-id="d6d63-109">When the request completes successfully, the status will be "succeeded" and the targetResourceLocation will point to the created/modified resource.</span></span>

## <a name="properties"></a><span data-ttu-id="d6d63-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d6d63-110">Properties</span></span>

| <span data-ttu-id="d6d63-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d6d63-111">Property</span></span> | <span data-ttu-id="d6d63-112">型</span><span class="sxs-lookup"><span data-stu-id="d6d63-112">Type</span></span>   | <span data-ttu-id="d6d63-113">説明</span><span class="sxs-lookup"><span data-stu-id="d6d63-113">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d6d63-114">id</span><span class="sxs-lookup"><span data-stu-id="d6d63-114">id</span></span>|<span data-ttu-id="d6d63-115">string</span><span class="sxs-lookup"><span data-stu-id="d6d63-115">string</span></span> |<span data-ttu-id="d6d63-116">一意の操作 id。</span><span class="sxs-lookup"><span data-stu-id="d6d63-116">Unique operation id.</span></span>|
|<span data-ttu-id="d6d63-117">operationType</span><span class="sxs-lookup"><span data-stu-id="d6d63-117">operationType</span></span>|[<span data-ttu-id="d6d63-118">teamsAsyncOperationType</span><span class="sxs-lookup"><span data-stu-id="d6d63-118">teamsAsyncOperationType</span></span>](teamsasyncoperationtype.md) |<span data-ttu-id="d6d63-119">説明されている操作の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="d6d63-119">Denotes which type of operation is being described.</span></span>|
|<span data-ttu-id="d6d63-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d6d63-120">createdDateTime</span></span>|<span data-ttu-id="d6d63-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6d63-121">DateTimeOffset</span></span> |<span data-ttu-id="d6d63-122">操作が作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="d6d63-122">Time when the operation was created.</span></span>|
|<span data-ttu-id="d6d63-123">status</span><span class="sxs-lookup"><span data-stu-id="d6d63-123">status</span></span>|[<span data-ttu-id="d6d63-124">teamsAsyncOperationStatus</span><span class="sxs-lookup"><span data-stu-id="d6d63-124">teamsAsyncOperationStatus</span></span>](teamsasyncoperationstatus.md)| <span data-ttu-id="d6d63-125">操作の状態。</span><span class="sxs-lookup"><span data-stu-id="d6d63-125">Operation status.</span></span>|
|<span data-ttu-id="d6d63-126">lastactiondatetime</span><span class="sxs-lookup"><span data-stu-id="d6d63-126">lastActionDateTime</span></span>|<span data-ttu-id="d6d63-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6d63-127">DateTimeOffset</span></span> |<span data-ttu-id="d6d63-128">async 操作が最後に更新された時刻。</span><span class="sxs-lookup"><span data-stu-id="d6d63-128">Time when the async operation was last updated.</span></span>|
|<span data-ttu-id="d6d63-129">attemptsCount</span><span class="sxs-lookup"><span data-stu-id="d6d63-129">attemptsCount</span></span>|<span data-ttu-id="d6d63-130">Int32</span><span class="sxs-lookup"><span data-stu-id="d6d63-130">Int32</span></span>|<span data-ttu-id="d6d63-131">操作が成功したか失敗したかがマークされるまでの、操作が試行された回数。</span><span class="sxs-lookup"><span data-stu-id="d6d63-131">Number of times the operation was attempted before being marked successful or failed.</span></span>|
|<span data-ttu-id="d6d63-132">targetresourceid</span><span class="sxs-lookup"><span data-stu-id="d6d63-132">targetResourceId</span></span>|<span data-ttu-id="d6d63-133">guid</span><span class="sxs-lookup"><span data-stu-id="d6d63-133">guid</span></span> |<span data-ttu-id="d6d63-134">この非同期操作の結果として作成または変更されるオブジェクトの ID (通常は[チーム](../resources/team.md))。</span><span class="sxs-lookup"><span data-stu-id="d6d63-134">The ID of the object that's created or modified as result of this async operation, typically a [team](../resources/team.md).</span></span>|
|<span data-ttu-id="d6d63-135">targetresourcelocation</span><span class="sxs-lookup"><span data-stu-id="d6d63-135">targetResourceLocation</span></span>|<span data-ttu-id="d6d63-136">string</span><span class="sxs-lookup"><span data-stu-id="d6d63-136">string</span></span>|<span data-ttu-id="d6d63-137">この非同期操作の結果として作成または変更されたオブジェクトの場所。</span><span class="sxs-lookup"><span data-stu-id="d6d63-137">The location of the object that's created or modified as result of this async operation.</span></span> <span data-ttu-id="d6d63-138">この URL は、不透明な値として扱われ、そのコンポーネントのパスに解析されることはありません。</span><span class="sxs-lookup"><span data-stu-id="d6d63-138">This URL should be treated as an opaque value and not parsed into its component paths.</span></span>|
|<span data-ttu-id="d6d63-139">error</span><span class="sxs-lookup"><span data-stu-id="d6d63-139">error</span></span>|[<span data-ttu-id="d6d63-140">operationerror</span><span class="sxs-lookup"><span data-stu-id="d6d63-140">operationError</span></span>](operationerror.md)|<span data-ttu-id="d6d63-141">非同期操作が失敗する原因となるエラー。</span><span class="sxs-lookup"><span data-stu-id="d6d63-141">Any error that causes the async operation to fail.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d6d63-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d6d63-142">JSON representation</span></span>

<span data-ttu-id="d6d63-143">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d6d63-143">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsAsyncOperation"
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
  "suppressions": []
}
-->
