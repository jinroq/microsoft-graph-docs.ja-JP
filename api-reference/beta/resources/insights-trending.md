---
title: トレンド ・ リソースの種類
description: ユーザー (は、ユーザーに関連する) 傾向を示しているドキュメントへのユーザーの接続の豊富な関係です。 OneDrive ファイルでは、チームの SharePoint サイトにファイルを保存できるユーザー傾向があるとします。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 07fe0f50d6961f0fce6c426c7fb2431f17127bf7
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640372"
---
# <a name="trending-resource-type"></a><span data-ttu-id="99968-104">トレンド ・ リソースの種類</span><span class="sxs-lookup"><span data-stu-id="99968-104">trending resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99968-105">ユーザー (は、ユーザーに関連する) 傾向を示しているドキュメントへのユーザーの接続の豊富な関係です。</span><span class="sxs-lookup"><span data-stu-id="99968-105">Rich relationship connecting a user to documents that are trending around the user (are relevant to the user).</span></span> <span data-ttu-id="99968-106">OneDrive ファイルでは、チームの SharePoint サイトにファイルを保存できるユーザー傾向があるとします。</span><span class="sxs-lookup"><span data-stu-id="99968-106">OneDrive files, and files stored on SharePoint team sites can trend around the user.</span></span>

## <a name="methods"></a><span data-ttu-id="99968-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="99968-107">Methods</span></span>

| <span data-ttu-id="99968-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="99968-108">Method</span></span>       | <span data-ttu-id="99968-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="99968-109">Return Type</span></span>  |<span data-ttu-id="99968-110">説明</span><span class="sxs-lookup"><span data-stu-id="99968-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="99968-111">リストのトレンド分析</span><span class="sxs-lookup"><span data-stu-id="99968-111">List trending</span></span>](../api/insights-list-trending.md) |<span data-ttu-id="99968-112">[insights_trending](insights-trending.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="99968-112">[insights_trending](insights-trending.md) collection</span></span>| <span data-ttu-id="99968-113">トレンド ・ ファイルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="99968-113">Get a list of trending files.</span></span>|

## <a name="properties"></a><span data-ttu-id="99968-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="99968-114">Properties</span></span>

| <span data-ttu-id="99968-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="99968-115">Property</span></span>      | <span data-ttu-id="99968-116">型</span><span class="sxs-lookup"><span data-stu-id="99968-116">Type</span></span>                              | <span data-ttu-id="99968-117">説明</span><span class="sxs-lookup"><span data-stu-id="99968-117">Description</span></span>  |
| ------------- |---------------                    | -------------|
| <span data-ttu-id="99968-118">id</span><span class="sxs-lookup"><span data-stu-id="99968-118">id</span></span>                    | <span data-ttu-id="99968-119">String</span><span class="sxs-lookup"><span data-stu-id="99968-119">String</span></span>                    | <span data-ttu-id="99968-120">リレーションシップの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="99968-120">Unique identifier of the relationship.</span></span> <span data-ttu-id="99968-121">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="99968-121">Read only.</span></span>        |
| <span data-ttu-id="99968-122">weight</span><span class="sxs-lookup"><span data-stu-id="99968-122">weight</span></span>                | <span data-ttu-id="99968-123">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="99968-123">Double</span></span>                    | <span data-ttu-id="99968-124">どれだけドキュメントが現在のトレンド分析を示す値です。</span><span class="sxs-lookup"><span data-stu-id="99968-124">Value indicating how much the document is currently trending.</span></span> <span data-ttu-id="99968-125">大きい番号より文書が現在のトレンド分析ユーザー (関連するほどである)。</span><span class="sxs-lookup"><span data-stu-id="99968-125">The larger the number, the more the document is currently trending around the user (the more relevant it is).</span></span> <span data-ttu-id="99968-126">返されたドキュメントは、この値で並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="99968-126">Returned documents are sorted by this value.</span></span>  |
| <span data-ttu-id="99968-127">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="99968-127">resourceVisualization</span></span> | [<span data-ttu-id="99968-128">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="99968-128">resourceVisualization</span></span>](insights-resourcevisualization.md)    | <span data-ttu-id="99968-129">プロパティは、時にドキュメントをビジュアル化を使用することができます。</span><span class="sxs-lookup"><span data-stu-id="99968-129">Properties that you can use to visualize the document in your experience.</span></span> |
| <span data-ttu-id="99968-130">resourceReference</span><span class="sxs-lookup"><span data-stu-id="99968-130">resourceReference</span></span>     | [<span data-ttu-id="99968-131">resourceReference</span><span class="sxs-lookup"><span data-stu-id="99968-131">resourceReference</span></span>](insights-resourcereference.md)        | <span data-ttu-id="99968-132">トレンド ・ ドキュメント、url、ドキュメントの種類などのプロパティを参照します。</span><span class="sxs-lookup"><span data-stu-id="99968-132">Reference properties of the trending document, such as the url and type of the document.</span></span> |

## <a name="relationships"></a><span data-ttu-id="99968-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="99968-133">Relationships</span></span>

| <span data-ttu-id="99968-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="99968-134">Property</span></span>      | <span data-ttu-id="99968-135">型</span><span class="sxs-lookup"><span data-stu-id="99968-135">Type</span></span>          | <span data-ttu-id="99968-136">説明</span><span class="sxs-lookup"><span data-stu-id="99968-136">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="99968-137">リソース</span><span class="sxs-lookup"><span data-stu-id="99968-137">resource</span></span>      | <span data-ttu-id="99968-138">Entity</span><span class="sxs-lookup"><span data-stu-id="99968-138">Entity</span></span>        | <span data-ttu-id="99968-139">トレンドのドキュメントに移動するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="99968-139">Used for navigating to the trending document.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="99968-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="99968-140">JSON representation</span></span>

<span data-ttu-id="99968-141">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="99968-141">Here is a JSON representation of the resource</span></span>

```json
{
  "id": "string",
  "weight": "double",
  "resourceVisualization": [{"@odata.type": "microsoft.graph.resourceVisualization"}],
  "resourceReference": [{"@odata.type": "microsoft.graph.resourceReference"}],
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-trending.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
