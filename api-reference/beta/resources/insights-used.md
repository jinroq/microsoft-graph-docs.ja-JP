---
title: usedInsight リソースの種類
description: 特定のユーザーによって使用されるドキュメントを表すの把握。 詳細情報は、ユーザーが表示またはアクセスする最も適切なドキュメントを返します。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 056654a5e467e202b2bde5ac8ee98dccab93d7c9
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574230"
---
# <a name="used-resource-type"></a><span data-ttu-id="f94e8-104">リソースの種類を使用</span><span class="sxs-lookup"><span data-stu-id="f94e8-104">used resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f94e8-105">特定のユーザーによって使用されるドキュメントを表すの把握。</span><span class="sxs-lookup"><span data-stu-id="f94e8-105">An insight representing documents used by a specific user.</span></span> <span data-ttu-id="f94e8-106">詳細情報は、ユーザーが表示またはアクセスする最も適切なドキュメントを返します。</span><span class="sxs-lookup"><span data-stu-id="f94e8-106">The insights returns the most relevant documents that a user viewed or accessed.</span></span> <span data-ttu-id="f94e8-107">内のドキュメントが含まれます。</span><span class="sxs-lookup"><span data-stu-id="f94e8-107">This includes documents in:</span></span>

- <span data-ttu-id="f94e8-108">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="f94e8-108">OneDrive for Business</span></span>
- <span data-ttu-id="f94e8-109">SharePoint</span><span class="sxs-lookup"><span data-stu-id="f94e8-109">SharePoint</span></span>

## <a name="methods"></a><span data-ttu-id="f94e8-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="f94e8-110">Methods</span></span>

| <span data-ttu-id="f94e8-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="f94e8-111">Method</span></span>       | <span data-ttu-id="f94e8-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f94e8-112">Return Type</span></span>  |<span data-ttu-id="f94e8-113">説明</span><span class="sxs-lookup"><span data-stu-id="f94e8-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f94e8-114">リストの使用</span><span class="sxs-lookup"><span data-stu-id="f94e8-114">List used</span></span>](../api/insights-list-used.md) |<span data-ttu-id="f94e8-115">[insights_used](insights-used.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f94e8-115">[insights_used](insights-used.md) collection</span></span>| <span data-ttu-id="f94e8-116">使用したファイルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="f94e8-116">Get a list of used files.</span></span>|

## <a name="properties"></a><span data-ttu-id="f94e8-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f94e8-117">Properties</span></span>

| <span data-ttu-id="f94e8-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f94e8-118">Property</span></span>              | <span data-ttu-id="f94e8-119">型</span><span class="sxs-lookup"><span data-stu-id="f94e8-119">Type</span></span>                      | <span data-ttu-id="f94e8-120">説明</span><span class="sxs-lookup"><span data-stu-id="f94e8-120">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="f94e8-121">id</span><span class="sxs-lookup"><span data-stu-id="f94e8-121">id</span></span>                    | <span data-ttu-id="f94e8-122">String</span><span class="sxs-lookup"><span data-stu-id="f94e8-122">String</span></span>                    | <span data-ttu-id="f94e8-123">リレーションシップの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="f94e8-123">Unique identifier of the relationship.</span></span> <span data-ttu-id="f94e8-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f94e8-124">Read only.</span></span>        |
| <span data-ttu-id="f94e8-125">lastUsed</span><span class="sxs-lookup"><span data-stu-id="f94e8-125">lastUsed</span></span>              | [<span data-ttu-id="f94e8-126">usageDetails</span><span class="sxs-lookup"><span data-stu-id="f94e8-126">usageDetails</span></span>](insights-usagedetails.md)              | <span data-ttu-id="f94e8-127">アイテムが最後表示し、ユーザーによって変更された場合について説明します。</span><span class="sxs-lookup"><span data-stu-id="f94e8-127">Information about when the item was last viewed and modified by the user.</span></span> <span data-ttu-id="f94e8-128">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f94e8-128">Read only.</span></span>     |
| <span data-ttu-id="f94e8-129">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="f94e8-129">resourceVisualization</span></span> | [<span data-ttu-id="f94e8-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="f94e8-130">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="f94e8-131">プロパティは、時にドキュメントをビジュアル化を使用することができます。</span><span class="sxs-lookup"><span data-stu-id="f94e8-131">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="f94e8-132">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="f94e8-132">Read-only</span></span>      |
| <span data-ttu-id="f94e8-133">resourceReference</span><span class="sxs-lookup"><span data-stu-id="f94e8-133">resourceReference</span></span>     | [<span data-ttu-id="f94e8-134">resourceReference</span><span class="sxs-lookup"><span data-stu-id="f94e8-134">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="f94e8-135">Url およびドキュメントの種類など、使用されているドキュメントのプロパティを参照。</span><span class="sxs-lookup"><span data-stu-id="f94e8-135">Reference properties of the used document, such as the url and type of the document.</span></span> <span data-ttu-id="f94e8-136">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="f94e8-136">Read-only</span></span>     |

## <a name="relationships"></a><span data-ttu-id="f94e8-137">関係</span><span class="sxs-lookup"><span data-stu-id="f94e8-137">Relationships</span></span>

| <span data-ttu-id="f94e8-138">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f94e8-138">Property</span></span>      | <span data-ttu-id="f94e8-139">型</span><span class="sxs-lookup"><span data-stu-id="f94e8-139">Type</span></span>          | <span data-ttu-id="f94e8-140">説明</span><span class="sxs-lookup"><span data-stu-id="f94e8-140">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="f94e8-141">リソース</span><span class="sxs-lookup"><span data-stu-id="f94e8-141">resource</span></span>      | <span data-ttu-id="f94e8-142">エンティティのコレクション</span><span class="sxs-lookup"><span data-stu-id="f94e8-142">entity collection</span></span> | <span data-ttu-id="f94e8-143">使用された項目に移動するために使用します。</span><span class="sxs-lookup"><span data-stu-id="f94e8-143">Used for navigating to the item that was used.</span></span> <span data-ttu-id="f94e8-144">ファイルの添付ファイルの種類は、 *fileAttachment*です。</span><span class="sxs-lookup"><span data-stu-id="f94e8-144">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="f94e8-145">リンクされた添付ファイルの場合は、型は、 *driveItem*です。</span><span class="sxs-lookup"><span data-stu-id="f94e8-145">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f94e8-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f94e8-146">JSON representation</span></span>
<span data-ttu-id="f94e8-147">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="f94e8-147">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.usedInsight"
}-->
```json
{
  "id": "string",
  "lastUsed": "usageDetails",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-used.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
