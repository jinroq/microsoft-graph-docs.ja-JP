---
title: 傾向のあるリソースの種類
description: ユーザーに関連するドキュメントへのユーザー接続の高度な関係 (ユーザーに関連しています)。 OneDrive ファイル、および SharePoint チームサイトに保存されたファイルは、ユーザーの周囲での傾向があります。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 07fe0f50d6961f0fce6c426c7fb2431f17127bf7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551310"
---
# <a name="trending-resource-type"></a><span data-ttu-id="1c3b5-104">傾向のあるリソースの種類</span><span class="sxs-lookup"><span data-stu-id="1c3b5-104">trending resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c3b5-105">ユーザーに関連するドキュメントへのユーザー接続の高度な関係 (ユーザーに関連しています)。</span><span class="sxs-lookup"><span data-stu-id="1c3b5-105">Rich relationship connecting a user to documents that are trending around the user (are relevant to the user).</span></span> <span data-ttu-id="1c3b5-106">OneDrive ファイル、および SharePoint チームサイトに保存されたファイルは、ユーザーの周囲での傾向があります。</span><span class="sxs-lookup"><span data-stu-id="1c3b5-106">OneDrive files, and files stored on SharePoint team sites can trend around the user.</span></span>

## <a name="methods"></a><span data-ttu-id="1c3b5-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="1c3b5-107">Methods</span></span>

| <span data-ttu-id="1c3b5-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="1c3b5-108">Method</span></span>       | <span data-ttu-id="1c3b5-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1c3b5-109">Return Type</span></span>  |<span data-ttu-id="1c3b5-110">説明</span><span class="sxs-lookup"><span data-stu-id="1c3b5-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1c3b5-111">人気上昇中を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1c3b5-111">List trending</span></span>](../api/insights-list-trending.md) |<span data-ttu-id="1c3b5-112">[insights_trending](insights-trending.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1c3b5-112">[insights_trending](insights-trending.md) collection</span></span>| <span data-ttu-id="1c3b5-113">トレンドファイルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="1c3b5-113">Get a list of trending files.</span></span>|

## <a name="properties"></a><span data-ttu-id="1c3b5-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1c3b5-114">Properties</span></span>

| <span data-ttu-id="1c3b5-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1c3b5-115">Property</span></span>      | <span data-ttu-id="1c3b5-116">型</span><span class="sxs-lookup"><span data-stu-id="1c3b5-116">Type</span></span>                              | <span data-ttu-id="1c3b5-117">説明</span><span class="sxs-lookup"><span data-stu-id="1c3b5-117">Description</span></span>  |
| ------------- |---------------                    | -------------|
| <span data-ttu-id="1c3b5-118">id</span><span class="sxs-lookup"><span data-stu-id="1c3b5-118">id</span></span>                    | <span data-ttu-id="1c3b5-119">String</span><span class="sxs-lookup"><span data-stu-id="1c3b5-119">String</span></span>                    | <span data-ttu-id="1c3b5-120">リレーションシップの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="1c3b5-120">Unique identifier of the relationship.</span></span> <span data-ttu-id="1c3b5-121">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1c3b5-121">Read only.</span></span>        |
| <span data-ttu-id="1c3b5-122">weight</span><span class="sxs-lookup"><span data-stu-id="1c3b5-122">weight</span></span>                | <span data-ttu-id="1c3b5-123">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="1c3b5-123">Double</span></span>                    | <span data-ttu-id="1c3b5-124">ドキュメントの現在の傾向を示す値。</span><span class="sxs-lookup"><span data-stu-id="1c3b5-124">Value indicating how much the document is currently trending.</span></span> <span data-ttu-id="1c3b5-125">数値が大きいほど、ドキュメントは現在ユーザーの傾向を示しています (より関連性が高い)。</span><span class="sxs-lookup"><span data-stu-id="1c3b5-125">The larger the number, the more the document is currently trending around the user (the more relevant it is).</span></span> <span data-ttu-id="1c3b5-126">返されたドキュメントは、この値で並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="1c3b5-126">Returned documents are sorted by this value.</span></span>  |
| <span data-ttu-id="1c3b5-127">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="1c3b5-127">resourceVisualization</span></span> | [<span data-ttu-id="1c3b5-128">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="1c3b5-128">resourceVisualization</span></span>](insights-resourcevisualization.md)    | <span data-ttu-id="1c3b5-129">ユーザーの作業でドキュメントをビジュアル化するために使用できるプロパティ。</span><span class="sxs-lookup"><span data-stu-id="1c3b5-129">Properties that you can use to visualize the document in your experience.</span></span> |
| <span data-ttu-id="1c3b5-130">resourceReference</span><span class="sxs-lookup"><span data-stu-id="1c3b5-130">resourceReference</span></span>     | [<span data-ttu-id="1c3b5-131">resourceReference</span><span class="sxs-lookup"><span data-stu-id="1c3b5-131">resourceReference</span></span>](insights-resourcereference.md)        | <span data-ttu-id="1c3b5-132">ドキュメントの url や種類など、傾向ドキュメントの参照プロパティ。</span><span class="sxs-lookup"><span data-stu-id="1c3b5-132">Reference properties of the trending document, such as the url and type of the document.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1c3b5-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1c3b5-133">Relationships</span></span>

| <span data-ttu-id="1c3b5-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1c3b5-134">Property</span></span>      | <span data-ttu-id="1c3b5-135">型</span><span class="sxs-lookup"><span data-stu-id="1c3b5-135">Type</span></span>          | <span data-ttu-id="1c3b5-136">説明</span><span class="sxs-lookup"><span data-stu-id="1c3b5-136">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="1c3b5-137">リソース</span><span class="sxs-lookup"><span data-stu-id="1c3b5-137">resource</span></span>      | <span data-ttu-id="1c3b5-138">エンティティ</span><span class="sxs-lookup"><span data-stu-id="1c3b5-138">Entity</span></span>        | <span data-ttu-id="1c3b5-139">トレンド分析ドキュメントに移動するために使用します。</span><span class="sxs-lookup"><span data-stu-id="1c3b5-139">Used for navigating to the trending document.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1c3b5-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1c3b5-140">JSON representation</span></span>

<span data-ttu-id="1c3b5-141">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="1c3b5-141">Here is a JSON representation of the resource</span></span>

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
