---
title: トレンド ・ リソースの種類
description: ユーザー (は、ユーザーに関連する) 傾向を示しているドキュメントへのユーザーの接続の豊富な関係です。 OneDrive ファイルでは、チームの SharePoint サイトにファイルを保存できるユーザー傾向があるとします。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 07fe0f50d6961f0fce6c426c7fb2431f17127bf7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507496"
---
# <a name="trending-resource-type"></a><span data-ttu-id="ecb1c-104">トレンド ・ リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ecb1c-104">trending resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ecb1c-105">ユーザー (は、ユーザーに関連する) 傾向を示しているドキュメントへのユーザーの接続の豊富な関係です。</span><span class="sxs-lookup"><span data-stu-id="ecb1c-105">Rich relationship connecting a user to documents that are trending around the user (are relevant to the user).</span></span> <span data-ttu-id="ecb1c-106">OneDrive ファイルでは、チームの SharePoint サイトにファイルを保存できるユーザー傾向があるとします。</span><span class="sxs-lookup"><span data-stu-id="ecb1c-106">OneDrive files, and files stored on SharePoint team sites can trend around the user.</span></span>

## <a name="methods"></a><span data-ttu-id="ecb1c-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="ecb1c-107">Methods</span></span>

| <span data-ttu-id="ecb1c-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="ecb1c-108">Method</span></span>       | <span data-ttu-id="ecb1c-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ecb1c-109">Return Type</span></span>  |<span data-ttu-id="ecb1c-110">説明</span><span class="sxs-lookup"><span data-stu-id="ecb1c-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ecb1c-111">リストのトレンド分析</span><span class="sxs-lookup"><span data-stu-id="ecb1c-111">List trending</span></span>](../api/insights-list-trending.md) |<span data-ttu-id="ecb1c-112">[insights_trending](insights-trending.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ecb1c-112">[insights_trending](insights-trending.md) collection</span></span>| <span data-ttu-id="ecb1c-113">トレンド ・ ファイルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="ecb1c-113">Get a list of trending files.</span></span>|

## <a name="properties"></a><span data-ttu-id="ecb1c-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ecb1c-114">Properties</span></span>

| <span data-ttu-id="ecb1c-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ecb1c-115">Property</span></span>      | <span data-ttu-id="ecb1c-116">型</span><span class="sxs-lookup"><span data-stu-id="ecb1c-116">Type</span></span>                              | <span data-ttu-id="ecb1c-117">説明</span><span class="sxs-lookup"><span data-stu-id="ecb1c-117">Description</span></span>  |
| ------------- |---------------                    | -------------|
| <span data-ttu-id="ecb1c-118">id</span><span class="sxs-lookup"><span data-stu-id="ecb1c-118">id</span></span>                    | <span data-ttu-id="ecb1c-119">String</span><span class="sxs-lookup"><span data-stu-id="ecb1c-119">String</span></span>                    | <span data-ttu-id="ecb1c-120">リレーションシップの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="ecb1c-120">Unique identifier of the relationship.</span></span> <span data-ttu-id="ecb1c-121">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ecb1c-121">Read only.</span></span>        |
| <span data-ttu-id="ecb1c-122">weight</span><span class="sxs-lookup"><span data-stu-id="ecb1c-122">weight</span></span>                | <span data-ttu-id="ecb1c-123">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="ecb1c-123">Double</span></span>                    | <span data-ttu-id="ecb1c-124">どれだけドキュメントが現在のトレンド分析を示す値です。</span><span class="sxs-lookup"><span data-stu-id="ecb1c-124">Value indicating how much the document is currently trending.</span></span> <span data-ttu-id="ecb1c-125">大きい番号より文書が現在のトレンド分析ユーザー (関連するほどである)。</span><span class="sxs-lookup"><span data-stu-id="ecb1c-125">The larger the number, the more the document is currently trending around the user (the more relevant it is).</span></span> <span data-ttu-id="ecb1c-126">返されたドキュメントは、この値で並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="ecb1c-126">Returned documents are sorted by this value.</span></span>  |
| <span data-ttu-id="ecb1c-127">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="ecb1c-127">resourceVisualization</span></span> | [<span data-ttu-id="ecb1c-128">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="ecb1c-128">resourceVisualization</span></span>](insights-resourcevisualization.md)    | <span data-ttu-id="ecb1c-129">プロパティは、時にドキュメントをビジュアル化を使用することができます。</span><span class="sxs-lookup"><span data-stu-id="ecb1c-129">Properties that you can use to visualize the document in your experience.</span></span> |
| <span data-ttu-id="ecb1c-130">resourceReference</span><span class="sxs-lookup"><span data-stu-id="ecb1c-130">resourceReference</span></span>     | [<span data-ttu-id="ecb1c-131">resourceReference</span><span class="sxs-lookup"><span data-stu-id="ecb1c-131">resourceReference</span></span>](insights-resourcereference.md)        | <span data-ttu-id="ecb1c-132">トレンド ・ ドキュメント、url、ドキュメントの種類などのプロパティを参照します。</span><span class="sxs-lookup"><span data-stu-id="ecb1c-132">Reference properties of the trending document, such as the url and type of the document.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ecb1c-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ecb1c-133">Relationships</span></span>

| <span data-ttu-id="ecb1c-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ecb1c-134">Property</span></span>      | <span data-ttu-id="ecb1c-135">型</span><span class="sxs-lookup"><span data-stu-id="ecb1c-135">Type</span></span>          | <span data-ttu-id="ecb1c-136">説明</span><span class="sxs-lookup"><span data-stu-id="ecb1c-136">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="ecb1c-137">リソース</span><span class="sxs-lookup"><span data-stu-id="ecb1c-137">resource</span></span>      | <span data-ttu-id="ecb1c-138">Entity</span><span class="sxs-lookup"><span data-stu-id="ecb1c-138">Entity</span></span>        | <span data-ttu-id="ecb1c-139">トレンドのドキュメントに移動するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="ecb1c-139">Used for navigating to the trending document.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ecb1c-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ecb1c-140">JSON representation</span></span>

<span data-ttu-id="ecb1c-141">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="ecb1c-141">Here is a JSON representation of the resource</span></span>

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
