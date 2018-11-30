---
title: リソースの種類を使用
description: 特定のユーザーによって使用されるドキュメントを表すの把握。 詳細情報は、ユーザーが表示またはアクセスする最も適切なドキュメントを返します。 内のドキュメントが含まれます。
ms.openlocfilehash: 3c82d268a67ef52d0ddfdad9193558080048ad6b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072327"
---
# <a name="used-resource-type"></a><span data-ttu-id="413fa-105">リソースの種類を使用</span><span class="sxs-lookup"><span data-stu-id="413fa-105">used resource type</span></span>

> <span data-ttu-id="413fa-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="413fa-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="413fa-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="413fa-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="413fa-108">特定のユーザーによって使用されるドキュメントを表すの把握。</span><span class="sxs-lookup"><span data-stu-id="413fa-108">An insight representing documents used by a specific user.</span></span> <span data-ttu-id="413fa-109">詳細情報は、ユーザーが表示またはアクセスする最も適切なドキュメントを返します。</span><span class="sxs-lookup"><span data-stu-id="413fa-109">The insights returns the most relevant documents that a user viewed or accessed.</span></span> <span data-ttu-id="413fa-110">内のドキュメントが含まれます。</span><span class="sxs-lookup"><span data-stu-id="413fa-110">This includes documents in:</span></span>

- <span data-ttu-id="413fa-111">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="413fa-111">OneDrive for Business</span></span>
- <span data-ttu-id="413fa-112">SharePoint</span><span class="sxs-lookup"><span data-stu-id="413fa-112">SharePoint</span></span>

## <a name="methods"></a><span data-ttu-id="413fa-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="413fa-113">Methods</span></span>

| <span data-ttu-id="413fa-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="413fa-114">Method</span></span>       | <span data-ttu-id="413fa-115">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="413fa-115">Return Type</span></span>  |<span data-ttu-id="413fa-116">説明</span><span class="sxs-lookup"><span data-stu-id="413fa-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="413fa-117">リストの使用</span><span class="sxs-lookup"><span data-stu-id="413fa-117">List used</span></span>](../api/insights-list-used.md) |<span data-ttu-id="413fa-118">[insights_used](insights-used.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="413fa-118">[insights_used](insights-used.md) collection</span></span>| <span data-ttu-id="413fa-119">使用したファイルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="413fa-119">Get a list of used files.</span></span>|

## <a name="properties"></a><span data-ttu-id="413fa-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="413fa-120">Properties</span></span>

| <span data-ttu-id="413fa-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="413fa-121">Property</span></span>              | <span data-ttu-id="413fa-122">型</span><span class="sxs-lookup"><span data-stu-id="413fa-122">Type</span></span>                      | <span data-ttu-id="413fa-123">説明</span><span class="sxs-lookup"><span data-stu-id="413fa-123">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="413fa-124">id</span><span class="sxs-lookup"><span data-stu-id="413fa-124">id</span></span>                    | <span data-ttu-id="413fa-125">String</span><span class="sxs-lookup"><span data-stu-id="413fa-125">String</span></span>                    | <span data-ttu-id="413fa-126">リレーションシップの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="413fa-126">Unique identifier of the relationship.</span></span> <span data-ttu-id="413fa-127">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="413fa-127">Read only.</span></span>        |
| <span data-ttu-id="413fa-128">lastUsed</span><span class="sxs-lookup"><span data-stu-id="413fa-128">lastUsed</span></span>              | [<span data-ttu-id="413fa-129">usageDetails</span><span class="sxs-lookup"><span data-stu-id="413fa-129">usageDetails</span></span>](insights-usagedetails.md)              | <span data-ttu-id="413fa-130">アイテムが最後表示し、ユーザーによって変更された場合について説明します。</span><span class="sxs-lookup"><span data-stu-id="413fa-130">Information about when the item was last viewed and modified by the user.</span></span> <span data-ttu-id="413fa-131">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="413fa-131">Read only.</span></span>     |
| <span data-ttu-id="413fa-132">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="413fa-132">resourceVisualization</span></span> | [<span data-ttu-id="413fa-133">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="413fa-133">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="413fa-134">プロパティは、時にドキュメントをビジュアル化を使用することができます。</span><span class="sxs-lookup"><span data-stu-id="413fa-134">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="413fa-135">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="413fa-135">Read-only</span></span>      |
| <span data-ttu-id="413fa-136">resourceReference</span><span class="sxs-lookup"><span data-stu-id="413fa-136">resourceReference</span></span>     | [<span data-ttu-id="413fa-137">resourceReference</span><span class="sxs-lookup"><span data-stu-id="413fa-137">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="413fa-138">Url およびドキュメントの種類など、使用されているドキュメントのプロパティを参照。</span><span class="sxs-lookup"><span data-stu-id="413fa-138">Reference properties of the used document, such as the url and type of the document.</span></span> <span data-ttu-id="413fa-139">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="413fa-139">Read-only</span></span>     |

## <a name="relationships"></a><span data-ttu-id="413fa-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="413fa-140">Relationships</span></span>

| <span data-ttu-id="413fa-141">プロパティ</span><span class="sxs-lookup"><span data-stu-id="413fa-141">Property</span></span>      | <span data-ttu-id="413fa-142">型</span><span class="sxs-lookup"><span data-stu-id="413fa-142">Type</span></span>          | <span data-ttu-id="413fa-143">説明</span><span class="sxs-lookup"><span data-stu-id="413fa-143">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="413fa-144">リソース</span><span class="sxs-lookup"><span data-stu-id="413fa-144">resource</span></span>      | <span data-ttu-id="413fa-145">エンティティ</span><span class="sxs-lookup"><span data-stu-id="413fa-145">Entity</span></span>        | <span data-ttu-id="413fa-146">使用された項目に移動するために使用します。</span><span class="sxs-lookup"><span data-stu-id="413fa-146">Used for navigating to the item that was used.</span></span> <span data-ttu-id="413fa-147">ファイルの添付ファイルの種類は、 *fileAttachment*です。</span><span class="sxs-lookup"><span data-stu-id="413fa-147">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="413fa-148">リンクされた添付ファイルの場合は、型は、 *driveItem*です。</span><span class="sxs-lookup"><span data-stu-id="413fa-148">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="413fa-149">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="413fa-149">JSON representation</span></span>
<span data-ttu-id="413fa-150">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="413fa-150">Here is a JSON representation of the resource</span></span>

```json
{
  "id": "string",
  "lastUsed": "usageDetails",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```