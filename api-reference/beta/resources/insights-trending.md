---
title: 傾向のあるリソースの種類
description: ユーザーに関連するドキュメントへのユーザー接続の高度な関係 (ユーザーに関連しています)。 OneDrive ファイル、および SharePoint チームサイトに保存されたファイルは、ユーザーの周囲での傾向があります。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 7963a3c518fd4fc946da4f6714a3aa52aa4b87eb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006221"
---
# <a name="trending-resource-type"></a><span data-ttu-id="c6c0d-104">傾向のあるリソースの種類</span><span class="sxs-lookup"><span data-stu-id="c6c0d-104">trending resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6c0d-105">ユーザーに関連するドキュメントへのユーザー接続の高度な関係 (ユーザーに関連しています)。</span><span class="sxs-lookup"><span data-stu-id="c6c0d-105">Rich relationship connecting a user to documents that are trending around the user (are relevant to the user).</span></span> <span data-ttu-id="c6c0d-106">OneDrive ファイル、および SharePoint チームサイトに保存されたファイルは、ユーザーの周囲での傾向があります。</span><span class="sxs-lookup"><span data-stu-id="c6c0d-106">OneDrive files, and files stored on SharePoint team sites can trend around the user.</span></span>

## <a name="methods"></a><span data-ttu-id="c6c0d-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="c6c0d-107">Methods</span></span>

| <span data-ttu-id="c6c0d-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c6c0d-108">Method</span></span>       | <span data-ttu-id="c6c0d-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c6c0d-109">Return Type</span></span>  |<span data-ttu-id="c6c0d-110">説明</span><span class="sxs-lookup"><span data-stu-id="c6c0d-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c6c0d-111">人気上昇中を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="c6c0d-111">List trending</span></span>](../api/insights-list-trending.md) |<span data-ttu-id="c6c0d-112">[insights_trending](insights-trending.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c6c0d-112">[insights_trending](insights-trending.md) collection</span></span>| <span data-ttu-id="c6c0d-113">トレンドファイルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="c6c0d-113">Get a list of trending files.</span></span>|

## <a name="properties"></a><span data-ttu-id="c6c0d-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c6c0d-114">Properties</span></span>

| <span data-ttu-id="c6c0d-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c6c0d-115">Property</span></span>      | <span data-ttu-id="c6c0d-116">型</span><span class="sxs-lookup"><span data-stu-id="c6c0d-116">Type</span></span>                              | <span data-ttu-id="c6c0d-117">説明</span><span class="sxs-lookup"><span data-stu-id="c6c0d-117">Description</span></span>  |
| ------------- |---------------                    | -------------|
| <span data-ttu-id="c6c0d-118">id</span><span class="sxs-lookup"><span data-stu-id="c6c0d-118">id</span></span>                    | <span data-ttu-id="c6c0d-119">String</span><span class="sxs-lookup"><span data-stu-id="c6c0d-119">String</span></span>                    | <span data-ttu-id="c6c0d-120">リレーションシップの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="c6c0d-120">Unique identifier of the relationship.</span></span> <span data-ttu-id="c6c0d-121">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c6c0d-121">Read only.</span></span>        |
| <span data-ttu-id="c6c0d-122">weight</span><span class="sxs-lookup"><span data-stu-id="c6c0d-122">weight</span></span>                | <span data-ttu-id="c6c0d-123">2 行分</span><span class="sxs-lookup"><span data-stu-id="c6c0d-123">Double</span></span>                    | <span data-ttu-id="c6c0d-124">ドキュメントの現在の傾向を示す値。</span><span class="sxs-lookup"><span data-stu-id="c6c0d-124">Value indicating how much the document is currently trending.</span></span> <span data-ttu-id="c6c0d-125">数値が大きいほど、ドキュメントは現在ユーザーの傾向を示しています (より関連性が高い)。</span><span class="sxs-lookup"><span data-stu-id="c6c0d-125">The larger the number, the more the document is currently trending around the user (the more relevant it is).</span></span> <span data-ttu-id="c6c0d-126">返されたドキュメントは、この値で並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="c6c0d-126">Returned documents are sorted by this value.</span></span>  |
| <span data-ttu-id="c6c0d-127">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="c6c0d-127">resourceVisualization</span></span> | [<span data-ttu-id="c6c0d-128">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="c6c0d-128">resourceVisualization</span></span>](insights-resourcevisualization.md)    | <span data-ttu-id="c6c0d-129">ユーザーの作業でドキュメントをビジュアル化するために使用できるプロパティ。</span><span class="sxs-lookup"><span data-stu-id="c6c0d-129">Properties that you can use to visualize the document in your experience.</span></span> |
| <span data-ttu-id="c6c0d-130">resourceReference</span><span class="sxs-lookup"><span data-stu-id="c6c0d-130">resourceReference</span></span>     | [<span data-ttu-id="c6c0d-131">resourceReference</span><span class="sxs-lookup"><span data-stu-id="c6c0d-131">resourceReference</span></span>](insights-resourcereference.md)        | <span data-ttu-id="c6c0d-132">ドキュメントの url や種類など、傾向ドキュメントの参照プロパティ。</span><span class="sxs-lookup"><span data-stu-id="c6c0d-132">Reference properties of the trending document, such as the url and type of the document.</span></span> |
| <span data-ttu-id="c6c0d-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c6c0d-133">lastModifiedDateTime</span></span>  | <span data-ttu-id="c6c0d-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6c0d-134">DateTimeOffset</span></span>            | |
## <a name="relationships"></a><span data-ttu-id="c6c0d-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c6c0d-135">Relationships</span></span>

| <span data-ttu-id="c6c0d-136">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c6c0d-136">Property</span></span>      | <span data-ttu-id="c6c0d-137">型</span><span class="sxs-lookup"><span data-stu-id="c6c0d-137">Type</span></span>          | <span data-ttu-id="c6c0d-138">説明</span><span class="sxs-lookup"><span data-stu-id="c6c0d-138">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="c6c0d-139">リソース</span><span class="sxs-lookup"><span data-stu-id="c6c0d-139">resource</span></span>      | <span data-ttu-id="c6c0d-140">エンティティ</span><span class="sxs-lookup"><span data-stu-id="c6c0d-140">entity</span></span>        | <span data-ttu-id="c6c0d-141">トレンド分析ドキュメントに移動するために使用します。</span><span class="sxs-lookup"><span data-stu-id="c6c0d-141">Used for navigating to the trending document.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c6c0d-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c6c0d-142">JSON representation</span></span>

<span data-ttu-id="c6c0d-143">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="c6c0d-143">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [
    "resource"
  ],
  "@odata.type": "microsoft.graph.trending"
}-->

```json
{
  "id": "string",
  "weight": "double",
  "resourceVisualization": {"@odata.type": "microsoft.graph.resourceVisualization"},
  "resourceReference": {"@odata.type": "microsoft.graph.resourceReference"},
  "lastModifiedDateTime": "String (timestamp)"
}
```
