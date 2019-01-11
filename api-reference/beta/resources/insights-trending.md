---
title: トレンド ・ リソースの種類
description: ユーザー (は、ユーザーに関連する) 傾向を示しているドキュメントへのユーザーの接続の豊富な関係です。 OneDrive ファイルでは、チームの SharePoint サイトにファイルを保存できるユーザー傾向があるとします。
author: simonhult
localization_priority: Normal
ms.openlocfilehash: dc0154d3985e5f6e1e4770bb7d10bc727a0eb0ae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862385"
---
# <a name="trending-resource-type"></a><span data-ttu-id="462e8-104">トレンド ・ リソースの種類</span><span class="sxs-lookup"><span data-stu-id="462e8-104">trending resource type</span></span>

> <span data-ttu-id="462e8-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="462e8-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="462e8-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="462e8-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="462e8-107">ユーザー (は、ユーザーに関連する) 傾向を示しているドキュメントへのユーザーの接続の豊富な関係です。</span><span class="sxs-lookup"><span data-stu-id="462e8-107">Rich relationship connecting a user to documents that are trending around the user (are relevant to the user).</span></span> <span data-ttu-id="462e8-108">OneDrive ファイルでは、チームの SharePoint サイトにファイルを保存できるユーザー傾向があるとします。</span><span class="sxs-lookup"><span data-stu-id="462e8-108">OneDrive files, and files stored on SharePoint team sites can trend around the user.</span></span>

## <a name="methods"></a><span data-ttu-id="462e8-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="462e8-109">Methods</span></span>

| <span data-ttu-id="462e8-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="462e8-110">Method</span></span>       | <span data-ttu-id="462e8-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="462e8-111">Return Type</span></span>  |<span data-ttu-id="462e8-112">説明</span><span class="sxs-lookup"><span data-stu-id="462e8-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="462e8-113">リストのトレンド分析</span><span class="sxs-lookup"><span data-stu-id="462e8-113">List trending</span></span>](../api/insights-list-trending.md) |<span data-ttu-id="462e8-114">[insights_trending](insights-trending.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="462e8-114">[insights_trending](insights-trending.md) collection</span></span>| <span data-ttu-id="462e8-115">トレンド ・ ファイルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="462e8-115">Get a list of trending files.</span></span>|

## <a name="properties"></a><span data-ttu-id="462e8-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="462e8-116">Properties</span></span>

| <span data-ttu-id="462e8-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="462e8-117">Property</span></span>      | <span data-ttu-id="462e8-118">種類</span><span class="sxs-lookup"><span data-stu-id="462e8-118">Type</span></span>                              | <span data-ttu-id="462e8-119">説明</span><span class="sxs-lookup"><span data-stu-id="462e8-119">Description</span></span>  |
| ------------- |---------------                    | -------------|
| <span data-ttu-id="462e8-120">ID</span><span class="sxs-lookup"><span data-stu-id="462e8-120">id</span></span>                    | <span data-ttu-id="462e8-121">String</span><span class="sxs-lookup"><span data-stu-id="462e8-121">String</span></span>                    | <span data-ttu-id="462e8-122">リレーションシップの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="462e8-122">Unique identifier of the relationship.</span></span> <span data-ttu-id="462e8-123">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="462e8-123">Read only.</span></span>        |
| <span data-ttu-id="462e8-124">weight</span><span class="sxs-lookup"><span data-stu-id="462e8-124">weight</span></span>                | <span data-ttu-id="462e8-125">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="462e8-125">Double</span></span>                    | <span data-ttu-id="462e8-126">どれだけドキュメントが現在のトレンド分析を示す値です。</span><span class="sxs-lookup"><span data-stu-id="462e8-126">Value indicating how much the document is currently trending.</span></span> <span data-ttu-id="462e8-127">大きい番号より文書が現在のトレンド分析ユーザー (関連するほどである)。</span><span class="sxs-lookup"><span data-stu-id="462e8-127">The larger the number, the more the document is currently trending around the user (the more relevant it is).</span></span> <span data-ttu-id="462e8-128">返されたドキュメントは、この値で並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="462e8-128">Returned documents are sorted by this value.</span></span>  |
| <span data-ttu-id="462e8-129">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="462e8-129">resourceVisualization</span></span> | [<span data-ttu-id="462e8-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="462e8-130">resourceVisualization</span></span>](insights-resourcevisualization.md)    | <span data-ttu-id="462e8-131">プロパティは、時にドキュメントをビジュアル化を使用することができます。</span><span class="sxs-lookup"><span data-stu-id="462e8-131">Properties that you can use to visualize the document in your experience.</span></span> |
| <span data-ttu-id="462e8-132">resourceReference</span><span class="sxs-lookup"><span data-stu-id="462e8-132">resourceReference</span></span>     | [<span data-ttu-id="462e8-133">resourceReference</span><span class="sxs-lookup"><span data-stu-id="462e8-133">resourceReference</span></span>](insights-resourcereference.md)        | <span data-ttu-id="462e8-134">トレンド ・ ドキュメント、url、ドキュメントの種類などのプロパティを参照します。</span><span class="sxs-lookup"><span data-stu-id="462e8-134">Reference properties of the trending document, such as the url and type of the document.</span></span> |

## <a name="relationships"></a><span data-ttu-id="462e8-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="462e8-135">Relationships</span></span>

| <span data-ttu-id="462e8-136">プロパティ</span><span class="sxs-lookup"><span data-stu-id="462e8-136">Property</span></span>      | <span data-ttu-id="462e8-137">種類</span><span class="sxs-lookup"><span data-stu-id="462e8-137">Type</span></span>          | <span data-ttu-id="462e8-138">説明</span><span class="sxs-lookup"><span data-stu-id="462e8-138">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="462e8-139">リソース</span><span class="sxs-lookup"><span data-stu-id="462e8-139">resource</span></span>      | <span data-ttu-id="462e8-140">Entity</span><span class="sxs-lookup"><span data-stu-id="462e8-140">Entity</span></span>        | <span data-ttu-id="462e8-141">トレンドのドキュメントに移動するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="462e8-141">Used for navigating to the trending document.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="462e8-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="462e8-142">JSON representation</span></span>

<span data-ttu-id="462e8-143">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="462e8-143">Here is a JSON representation of the resource</span></span>

```json
{
  "id": "string",
  "weight": "double",
  "resourceVisualization": [{"@odata.type": "microsoft.graph.resourceVisualization"}],
  "resourceReference": [{"@odata.type": "microsoft.graph.resourceReference"}],
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
