---
title: used リソースの種類
description: 特定のユーザーが使用するドキュメントを表す洞察。 insights は、ユーザーが表示またはアクセスした最も関連性のあるドキュメントを返します。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 407822dc4ff3f0536b0cbff3bf2894ad96d5d878
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333555"
---
# <a name="usedinsight-resource-type"></a><span data-ttu-id="018c7-104">used リソースの種類</span><span class="sxs-lookup"><span data-stu-id="018c7-104">usedInsight resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="018c7-105">特定のユーザーが使用するドキュメントを表す洞察。</span><span class="sxs-lookup"><span data-stu-id="018c7-105">An insight representing documents used by a specific user.</span></span> <span data-ttu-id="018c7-106">insights は、ユーザーが表示またはアクセスした最も関連性のあるドキュメントを返します。</span><span class="sxs-lookup"><span data-stu-id="018c7-106">The insights returns the most relevant documents that a user viewed or accessed.</span></span> <span data-ttu-id="018c7-107">これには次のドキュメントが含まれます。</span><span class="sxs-lookup"><span data-stu-id="018c7-107">This includes documents in:</span></span>

- <span data-ttu-id="018c7-108">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="018c7-108">OneDrive for Business</span></span>
- <span data-ttu-id="018c7-109">SharePoint</span><span class="sxs-lookup"><span data-stu-id="018c7-109">SharePoint</span></span>

## <a name="methods"></a><span data-ttu-id="018c7-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="018c7-110">Methods</span></span>

| <span data-ttu-id="018c7-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="018c7-111">Method</span></span>       | <span data-ttu-id="018c7-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="018c7-112">Return Type</span></span>  |<span data-ttu-id="018c7-113">説明</span><span class="sxs-lookup"><span data-stu-id="018c7-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="018c7-114">使用するリスト</span><span class="sxs-lookup"><span data-stu-id="018c7-114">List used</span></span>](../api/insights-list-used.md) |<span data-ttu-id="018c7-115">使われる[洞察](insights-used.md)のコレクション</span><span class="sxs-lookup"><span data-stu-id="018c7-115">[usedInsight](insights-used.md) collection</span></span>| <span data-ttu-id="018c7-116">使用されているファイルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="018c7-116">Get a list of used files.</span></span>|

## <a name="properties"></a><span data-ttu-id="018c7-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="018c7-117">Properties</span></span>

| <span data-ttu-id="018c7-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="018c7-118">Property</span></span>              | <span data-ttu-id="018c7-119">型</span><span class="sxs-lookup"><span data-stu-id="018c7-119">Type</span></span>                      | <span data-ttu-id="018c7-120">説明</span><span class="sxs-lookup"><span data-stu-id="018c7-120">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="018c7-121">id</span><span class="sxs-lookup"><span data-stu-id="018c7-121">id</span></span>                    | <span data-ttu-id="018c7-122">String</span><span class="sxs-lookup"><span data-stu-id="018c7-122">String</span></span>                    | <span data-ttu-id="018c7-123">リレーションシップの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="018c7-123">Unique identifier of the relationship.</span></span> <span data-ttu-id="018c7-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="018c7-124">Read only.</span></span>        |
| <span data-ttu-id="018c7-125">lastused</span><span class="sxs-lookup"><span data-stu-id="018c7-125">lastUsed</span></span>              | [<span data-ttu-id="018c7-126">usageDetails</span><span class="sxs-lookup"><span data-stu-id="018c7-126">usageDetails</span></span>](insights-usagedetails.md)              | <span data-ttu-id="018c7-127">ユーザーが最後にアイテムを表示および変更した日時に関する情報。</span><span class="sxs-lookup"><span data-stu-id="018c7-127">Information about when the item was last viewed and modified by the user.</span></span> <span data-ttu-id="018c7-128">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="018c7-128">Read only.</span></span>     |
| <span data-ttu-id="018c7-129">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="018c7-129">resourceVisualization</span></span> | [<span data-ttu-id="018c7-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="018c7-130">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="018c7-131">ユーザーの作業でドキュメントをビジュアル化するために使用できるプロパティ。</span><span class="sxs-lookup"><span data-stu-id="018c7-131">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="018c7-132">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="018c7-132">Read-only</span></span>      |
| <span data-ttu-id="018c7-133">resourceReference</span><span class="sxs-lookup"><span data-stu-id="018c7-133">resourceReference</span></span>     | [<span data-ttu-id="018c7-134">resourceReference</span><span class="sxs-lookup"><span data-stu-id="018c7-134">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="018c7-135">ドキュメントの url や種類など、使用されているドキュメントの参照プロパティ。</span><span class="sxs-lookup"><span data-stu-id="018c7-135">Reference properties of the used document, such as the url and type of the document.</span></span> <span data-ttu-id="018c7-136">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="018c7-136">Read-only</span></span>     |

## <a name="relationships"></a><span data-ttu-id="018c7-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="018c7-137">Relationships</span></span>

| <span data-ttu-id="018c7-138">プロパティ</span><span class="sxs-lookup"><span data-stu-id="018c7-138">Property</span></span>      | <span data-ttu-id="018c7-139">型</span><span class="sxs-lookup"><span data-stu-id="018c7-139">Type</span></span>          | <span data-ttu-id="018c7-140">説明</span><span class="sxs-lookup"><span data-stu-id="018c7-140">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="018c7-141">リソース</span><span class="sxs-lookup"><span data-stu-id="018c7-141">resource</span></span>      | <span data-ttu-id="018c7-142">[entity](entity.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="018c7-142">[entity](entity.md) collection</span></span>    | <span data-ttu-id="018c7-143">使用されたアイテムに移動するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="018c7-143">Used for navigating to the item that was used.</span></span> <span data-ttu-id="018c7-144">添付ファイルの場合、type は*fileattachment*になります。</span><span class="sxs-lookup"><span data-stu-id="018c7-144">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="018c7-145">リンクされた添付ファイルの場合、種類は [*ドライブ] 項目*です。</span><span class="sxs-lookup"><span data-stu-id="018c7-145">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="018c7-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="018c7-146">JSON representation</span></span>
<span data-ttu-id="018c7-147">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="018c7-147">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [
    "resource"
  ],
  "@odata.type": "microsoft.graph.usedInsight"
}-->

```json
{
  "id": "string",
  "lastUsed": "usageDetails",
  "resourceVisualization": { "@odata.type": "microsoft.graph.resourceVisualization" },
  "resourceReference": { "@odata.type": "microsoft.graph.resourceReference" }
}
```
