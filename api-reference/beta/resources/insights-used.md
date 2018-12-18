---
title: リソースの種類を使用
description: 特定のユーザーによって使用されるドキュメントを表すの把握。 詳細情報は、ユーザーが表示またはアクセスする最も適切なドキュメントを返します。
author: simonhult
ms.openlocfilehash: 89eac33ad954905c77a26df669bb15a2cf471edd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323486"
---
# <a name="used-resource-type"></a><span data-ttu-id="10cb3-104">リソースの種類を使用</span><span class="sxs-lookup"><span data-stu-id="10cb3-104">used resource type</span></span>

> <span data-ttu-id="10cb3-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="10cb3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="10cb3-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="10cb3-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="10cb3-107">特定のユーザーによって使用されるドキュメントを表すの把握。</span><span class="sxs-lookup"><span data-stu-id="10cb3-107">An insight representing documents used by a specific user.</span></span> <span data-ttu-id="10cb3-108">詳細情報は、ユーザーが表示またはアクセスする最も適切なドキュメントを返します。</span><span class="sxs-lookup"><span data-stu-id="10cb3-108">The insights returns the most relevant documents that a user viewed or accessed.</span></span> <span data-ttu-id="10cb3-109">内のドキュメントが含まれます。</span><span class="sxs-lookup"><span data-stu-id="10cb3-109">This includes documents in:</span></span>

- <span data-ttu-id="10cb3-110">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="10cb3-110">OneDrive for Business</span></span>
- <span data-ttu-id="10cb3-111">SharePoint</span><span class="sxs-lookup"><span data-stu-id="10cb3-111">SharePoint</span></span>

## <a name="methods"></a><span data-ttu-id="10cb3-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="10cb3-112">Methods</span></span>

| <span data-ttu-id="10cb3-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="10cb3-113">Method</span></span>       | <span data-ttu-id="10cb3-114">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="10cb3-114">Return Type</span></span>  |<span data-ttu-id="10cb3-115">説明</span><span class="sxs-lookup"><span data-stu-id="10cb3-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="10cb3-116">リストの使用</span><span class="sxs-lookup"><span data-stu-id="10cb3-116">List used</span></span>](../api/insights-list-used.md) |<span data-ttu-id="10cb3-117">[insights_used](insights-used.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="10cb3-117">[insights_used](insights-used.md) collection</span></span>| <span data-ttu-id="10cb3-118">使用したファイルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="10cb3-118">Get a list of used files.</span></span>|

## <a name="properties"></a><span data-ttu-id="10cb3-119">Properties</span><span class="sxs-lookup"><span data-stu-id="10cb3-119">Properties</span></span>

| <span data-ttu-id="10cb3-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="10cb3-120">Property</span></span>              | <span data-ttu-id="10cb3-121">種類</span><span class="sxs-lookup"><span data-stu-id="10cb3-121">Type</span></span>                      | <span data-ttu-id="10cb3-122">説明</span><span class="sxs-lookup"><span data-stu-id="10cb3-122">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="10cb3-123">ID</span><span class="sxs-lookup"><span data-stu-id="10cb3-123">id</span></span>                    | <span data-ttu-id="10cb3-124">String</span><span class="sxs-lookup"><span data-stu-id="10cb3-124">String</span></span>                    | <span data-ttu-id="10cb3-125">リレーションシップの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="10cb3-125">Unique identifier of the relationship.</span></span> <span data-ttu-id="10cb3-126">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="10cb3-126">Read only.</span></span>        |
| <span data-ttu-id="10cb3-127">lastUsed</span><span class="sxs-lookup"><span data-stu-id="10cb3-127">lastUsed</span></span>              | [<span data-ttu-id="10cb3-128">usageDetails</span><span class="sxs-lookup"><span data-stu-id="10cb3-128">usageDetails</span></span>](insights-usagedetails.md)              | <span data-ttu-id="10cb3-129">アイテムが最後表示し、ユーザーによって変更された場合について説明します。</span><span class="sxs-lookup"><span data-stu-id="10cb3-129">Information about when the item was last viewed and modified by the user.</span></span> <span data-ttu-id="10cb3-130">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="10cb3-130">Read only.</span></span>     |
| <span data-ttu-id="10cb3-131">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="10cb3-131">resourceVisualization</span></span> | [<span data-ttu-id="10cb3-132">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="10cb3-132">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="10cb3-133">プロパティは、時にドキュメントをビジュアル化を使用することができます。</span><span class="sxs-lookup"><span data-stu-id="10cb3-133">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="10cb3-134">取得のみ可能な値です</span><span class="sxs-lookup"><span data-stu-id="10cb3-134">Read-only</span></span>      |
| <span data-ttu-id="10cb3-135">resourceReference</span><span class="sxs-lookup"><span data-stu-id="10cb3-135">resourceReference</span></span>     | [<span data-ttu-id="10cb3-136">resourceReference</span><span class="sxs-lookup"><span data-stu-id="10cb3-136">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="10cb3-137">Url およびドキュメントの種類など、使用されているドキュメントのプロパティを参照。</span><span class="sxs-lookup"><span data-stu-id="10cb3-137">Reference properties of the used document, such as the url and type of the document.</span></span> <span data-ttu-id="10cb3-138">取得のみ可能な値です</span><span class="sxs-lookup"><span data-stu-id="10cb3-138">Read-only</span></span>     |

## <a name="relationships"></a><span data-ttu-id="10cb3-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="10cb3-139">Relationships</span></span>

| <span data-ttu-id="10cb3-140">プロパティ</span><span class="sxs-lookup"><span data-stu-id="10cb3-140">Property</span></span>      | <span data-ttu-id="10cb3-141">種類</span><span class="sxs-lookup"><span data-stu-id="10cb3-141">Type</span></span>          | <span data-ttu-id="10cb3-142">説明</span><span class="sxs-lookup"><span data-stu-id="10cb3-142">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="10cb3-143">リソース</span><span class="sxs-lookup"><span data-stu-id="10cb3-143">resource</span></span>      | <span data-ttu-id="10cb3-144">Entity</span><span class="sxs-lookup"><span data-stu-id="10cb3-144">Entity</span></span>        | <span data-ttu-id="10cb3-145">使用された項目に移動するために使用します。</span><span class="sxs-lookup"><span data-stu-id="10cb3-145">Used for navigating to the item that was used.</span></span> <span data-ttu-id="10cb3-146">ファイルの添付ファイルの種類は、 *fileAttachment*です。</span><span class="sxs-lookup"><span data-stu-id="10cb3-146">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="10cb3-147">リンクされた添付ファイルの場合は、型は、 *driveItem*です。</span><span class="sxs-lookup"><span data-stu-id="10cb3-147">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="10cb3-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="10cb3-148">JSON representation</span></span>
<span data-ttu-id="10cb3-149">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="10cb3-149">Here is a JSON representation of the resource</span></span>

```json
{
  "id": "string",
  "lastUsed": "usageDetails",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```