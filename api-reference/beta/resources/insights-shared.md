---
title: /リソースの種類 (sharepoint)
description: または特定のユーザーによって共有されているファイルを表す洞察。 次の共有ファイルがサポートされています。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 128a85bb9aa2e9f51d2393029cce3c27f8c4e6f8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339992"
---
# <a name="sharedinsight-resource-type"></a><span data-ttu-id="aabd3-104">/リソースの種類 (sharepoint)</span><span class="sxs-lookup"><span data-stu-id="aabd3-104">sharedInsight resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aabd3-105">または特定のユーザーによって共有されているファイルを表す洞察。</span><span class="sxs-lookup"><span data-stu-id="aabd3-105">An insight representing files shared with or by a specific user.</span></span> <span data-ttu-id="aabd3-106">次の共有ファイルがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="aabd3-106">The following shared files are supported:</span></span>

- <span data-ttu-id="aabd3-107">電子メールまたは会議の招待に直接添付されたファイル。</span><span class="sxs-lookup"><span data-stu-id="aabd3-107">Files attached directly in an email or a meeting invite.</span></span>
- <span data-ttu-id="aabd3-108">onedrive for Bussiness および sharepoint モダン添付ファイル-ユーザーが電子メールのリンクとして共有する、onedrive for business および sharepoint に格納されているファイル。</span><span class="sxs-lookup"><span data-stu-id="aabd3-108">OneDrive for Bussiness and SharePoint modern attachments - files stored in OneDrive for Business and SharePoint that users share as a links in an email.</span></span>

<span data-ttu-id="aabd3-109">**注**: 現在、データを使用して共有 API の結果を設定する作業を行っています。</span><span class="sxs-lookup"><span data-stu-id="aabd3-109">**Note**: We are currently working on populating the results of the Shared API with data.</span></span> <span data-ttu-id="aabd3-110">リリース後の最初の週に、一部のデータが欠落している場合があります。</span><span class="sxs-lookup"><span data-stu-id="aabd3-110">There may be some data missing in the first weeks after release.</span></span>

## <a name="methods"></a><span data-ttu-id="aabd3-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="aabd3-111">Methods</span></span>

| <span data-ttu-id="aabd3-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="aabd3-112">Method</span></span>       | <span data-ttu-id="aabd3-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="aabd3-113">Return Type</span></span>  |<span data-ttu-id="aabd3-114">説明</span><span class="sxs-lookup"><span data-stu-id="aabd3-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="aabd3-115">共有リスト</span><span class="sxs-lookup"><span data-stu-id="aabd3-115">List shared</span></span>](../api/insights-list-shared.md) |<span data-ttu-id="aabd3-116">[insights_shared](insights-shared.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="aabd3-116">[insights_shared](insights-shared.md) collection</span></span>| <span data-ttu-id="aabd3-117">共有ファイルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="aabd3-117">Get a list of shared files.</span></span>|

## <a name="properties"></a><span data-ttu-id="aabd3-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aabd3-118">Properties</span></span>

| <span data-ttu-id="aabd3-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aabd3-119">Property</span></span>              | <span data-ttu-id="aabd3-120">型</span><span class="sxs-lookup"><span data-stu-id="aabd3-120">Type</span></span>                      | <span data-ttu-id="aabd3-121">説明</span><span class="sxs-lookup"><span data-stu-id="aabd3-121">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="aabd3-122">id</span><span class="sxs-lookup"><span data-stu-id="aabd3-122">id</span></span>                    | <span data-ttu-id="aabd3-123">String</span><span class="sxs-lookup"><span data-stu-id="aabd3-123">String</span></span>                    | <span data-ttu-id="aabd3-124">リレーションシップの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="aabd3-124">Unique identifier of the relationship.</span></span> <span data-ttu-id="aabd3-125">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="aabd3-125">Read only.</span></span>        |
| <span data-ttu-id="aabd3-126">lastshared</span><span class="sxs-lookup"><span data-stu-id="aabd3-126">lastShared</span></span>            | [<span data-ttu-id="aabd3-127">sharingDetail</span><span class="sxs-lookup"><span data-stu-id="aabd3-127">sharingDetail</span></span>](insights-sharingdetail.md)                | <span data-ttu-id="aabd3-128">共有アイテムの詳細。</span><span class="sxs-lookup"><span data-stu-id="aabd3-128">Details about the shared item.</span></span> <span data-ttu-id="aabd3-129">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="aabd3-129">Read only.</span></span>        |
| <span data-ttu-id="aabd3-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="aabd3-130">resourceVisualization</span></span> | [<span data-ttu-id="aabd3-131">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="aabd3-131">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="aabd3-132">ユーザーの作業でドキュメントをビジュアル化するために使用できるプロパティ。</span><span class="sxs-lookup"><span data-stu-id="aabd3-132">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="aabd3-133">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="aabd3-133">Read-only</span></span>      |
| <span data-ttu-id="aabd3-134">resourceReference</span><span class="sxs-lookup"><span data-stu-id="aabd3-134">resourceReference</span></span>     | [<span data-ttu-id="aabd3-135">resourceReference</span><span class="sxs-lookup"><span data-stu-id="aabd3-135">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="aabd3-136">ドキュメントの url や種類など、共有ドキュメントの参照プロパティ。</span><span class="sxs-lookup"><span data-stu-id="aabd3-136">Reference properties of the shared document, such as the url and type of the document.</span></span> <span data-ttu-id="aabd3-137">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="aabd3-137">Read-only</span></span>       |

## <a name="relationships"></a><span data-ttu-id="aabd3-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="aabd3-138">Relationships</span></span>

| <span data-ttu-id="aabd3-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aabd3-139">Property</span></span>      | <span data-ttu-id="aabd3-140">型</span><span class="sxs-lookup"><span data-stu-id="aabd3-140">Type</span></span>          | <span data-ttu-id="aabd3-141">説明</span><span class="sxs-lookup"><span data-stu-id="aabd3-141">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="aabd3-142">リソース</span><span class="sxs-lookup"><span data-stu-id="aabd3-142">resource</span></span>      | <span data-ttu-id="aabd3-143">entity コレクション</span><span class="sxs-lookup"><span data-stu-id="aabd3-143">entity collection</span></span> | <span data-ttu-id="aabd3-144">共有されているアイテムに移動するために使用します。</span><span class="sxs-lookup"><span data-stu-id="aabd3-144">Used for navigating to the item that was shared.</span></span> <span data-ttu-id="aabd3-145">添付ファイルの場合、type は*fileattachment*になります。</span><span class="sxs-lookup"><span data-stu-id="aabd3-145">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="aabd3-146">リンクされた添付ファイルの場合、種類は [*ドライブ] 項目*です。</span><span class="sxs-lookup"><span data-stu-id="aabd3-146">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="aabd3-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aabd3-147">JSON representation</span></span>
<span data-ttu-id="aabd3-148">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="aabd3-148">Here is a JSON representation of the resource</span></span>
<!--{
  "blockType":"resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sharedInsight"
}-->
```json
{
  "id": "string",
  "lastShared": "sharingDetail",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
