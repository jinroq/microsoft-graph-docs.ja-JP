---
title: 使用されるリソースの種類
description: 特定のユーザーが使用するドキュメントを表す洞察。 insights は、ユーザーが表示またはアクセスした最も関連性のあるドキュメントを返します。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 35698741cd457f4e8d202b13dd9099bb2669b6e1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551292"
---
# <a name="used-resource-type"></a><span data-ttu-id="0b30c-104">使用されるリソースの種類</span><span class="sxs-lookup"><span data-stu-id="0b30c-104">used resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b30c-105">特定のユーザーが使用するドキュメントを表す洞察。</span><span class="sxs-lookup"><span data-stu-id="0b30c-105">An insight representing documents used by a specific user.</span></span> <span data-ttu-id="0b30c-106">insights は、ユーザーが表示またはアクセスした最も関連性のあるドキュメントを返します。</span><span class="sxs-lookup"><span data-stu-id="0b30c-106">The insights returns the most relevant documents that a user viewed or accessed.</span></span> <span data-ttu-id="0b30c-107">これには次のドキュメントが含まれます。</span><span class="sxs-lookup"><span data-stu-id="0b30c-107">This includes documents in:</span></span>

- <span data-ttu-id="0b30c-108">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="0b30c-108">OneDrive for Business</span></span>
- <span data-ttu-id="0b30c-109">SharePoint</span><span class="sxs-lookup"><span data-stu-id="0b30c-109">SharePoint</span></span>

## <a name="methods"></a><span data-ttu-id="0b30c-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="0b30c-110">Methods</span></span>

| <span data-ttu-id="0b30c-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="0b30c-111">Method</span></span>       | <span data-ttu-id="0b30c-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0b30c-112">Return Type</span></span>  |<span data-ttu-id="0b30c-113">説明</span><span class="sxs-lookup"><span data-stu-id="0b30c-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0b30c-114">使用するリスト</span><span class="sxs-lookup"><span data-stu-id="0b30c-114">List used</span></span>](../api/insights-list-used.md) |<span data-ttu-id="0b30c-115">[insights_used](insights-used.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0b30c-115">[insights_used](insights-used.md) collection</span></span>| <span data-ttu-id="0b30c-116">使用されているファイルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="0b30c-116">Get a list of used files.</span></span>|

## <a name="properties"></a><span data-ttu-id="0b30c-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0b30c-117">Properties</span></span>

| <span data-ttu-id="0b30c-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0b30c-118">Property</span></span>              | <span data-ttu-id="0b30c-119">型</span><span class="sxs-lookup"><span data-stu-id="0b30c-119">Type</span></span>                      | <span data-ttu-id="0b30c-120">説明</span><span class="sxs-lookup"><span data-stu-id="0b30c-120">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="0b30c-121">id</span><span class="sxs-lookup"><span data-stu-id="0b30c-121">id</span></span>                    | <span data-ttu-id="0b30c-122">String</span><span class="sxs-lookup"><span data-stu-id="0b30c-122">String</span></span>                    | <span data-ttu-id="0b30c-123">リレーションシップの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="0b30c-123">Unique identifier of the relationship.</span></span> <span data-ttu-id="0b30c-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0b30c-124">Read only.</span></span>        |
| <span data-ttu-id="0b30c-125">lastused</span><span class="sxs-lookup"><span data-stu-id="0b30c-125">lastUsed</span></span>              | [<span data-ttu-id="0b30c-126">usageDetails</span><span class="sxs-lookup"><span data-stu-id="0b30c-126">usageDetails</span></span>](insights-usagedetails.md)              | <span data-ttu-id="0b30c-127">ユーザーが最後にアイテムを表示および変更した日時に関する情報。</span><span class="sxs-lookup"><span data-stu-id="0b30c-127">Information about when the item was last viewed and modified by the user.</span></span> <span data-ttu-id="0b30c-128">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0b30c-128">Read only.</span></span>     |
| <span data-ttu-id="0b30c-129">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="0b30c-129">resourceVisualization</span></span> | [<span data-ttu-id="0b30c-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="0b30c-130">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="0b30c-131">ユーザーの作業でドキュメントをビジュアル化するために使用できるプロパティ。</span><span class="sxs-lookup"><span data-stu-id="0b30c-131">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="0b30c-132">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="0b30c-132">Read-only</span></span>      |
| <span data-ttu-id="0b30c-133">resourceReference</span><span class="sxs-lookup"><span data-stu-id="0b30c-133">resourceReference</span></span>     | [<span data-ttu-id="0b30c-134">resourceReference</span><span class="sxs-lookup"><span data-stu-id="0b30c-134">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="0b30c-135">ドキュメントの url や種類など、使用されているドキュメントの参照プロパティ。</span><span class="sxs-lookup"><span data-stu-id="0b30c-135">Reference properties of the used document, such as the url and type of the document.</span></span> <span data-ttu-id="0b30c-136">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="0b30c-136">Read-only</span></span>     |

## <a name="relationships"></a><span data-ttu-id="0b30c-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0b30c-137">Relationships</span></span>

| <span data-ttu-id="0b30c-138">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0b30c-138">Property</span></span>      | <span data-ttu-id="0b30c-139">型</span><span class="sxs-lookup"><span data-stu-id="0b30c-139">Type</span></span>          | <span data-ttu-id="0b30c-140">説明</span><span class="sxs-lookup"><span data-stu-id="0b30c-140">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="0b30c-141">リソース</span><span class="sxs-lookup"><span data-stu-id="0b30c-141">resource</span></span>      | <span data-ttu-id="0b30c-142">エンティティ</span><span class="sxs-lookup"><span data-stu-id="0b30c-142">Entity</span></span>        | <span data-ttu-id="0b30c-143">使用されたアイテムに移動するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="0b30c-143">Used for navigating to the item that was used.</span></span> <span data-ttu-id="0b30c-144">添付ファイルの場合、type は*fileattachment*になります。</span><span class="sxs-lookup"><span data-stu-id="0b30c-144">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="0b30c-145">リンクされた添付ファイルの場合、種類は [*ドライブ] 項目*です。</span><span class="sxs-lookup"><span data-stu-id="0b30c-145">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0b30c-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0b30c-146">JSON representation</span></span>
<span data-ttu-id="0b30c-147">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="0b30c-147">Here is a JSON representation of the resource</span></span>

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
