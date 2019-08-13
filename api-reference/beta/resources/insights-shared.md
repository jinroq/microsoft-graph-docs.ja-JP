---
title: /リソースの種類 (Sharepoint)
description: または特定のユーザーによって共有されているファイルを表す洞察。 次の共有ファイルがサポートされています。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: e95a7a54d2cdce7e23bcc4792368cfa250241963
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366351"
---
# <a name="sharedinsight-resource-type"></a><span data-ttu-id="5c6f4-104">/リソースの種類 (Sharepoint)</span><span class="sxs-lookup"><span data-stu-id="5c6f4-104">sharedInsight resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c6f4-105">または特定のユーザーによって共有されているファイルを表す洞察。</span><span class="sxs-lookup"><span data-stu-id="5c6f4-105">An insight representing files shared with or by a specific user.</span></span> <span data-ttu-id="5c6f4-106">次の共有ファイルがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="5c6f4-106">The following shared files are supported:</span></span>

- <span data-ttu-id="5c6f4-107">電子メールまたは会議の招待に直接添付されたファイル。</span><span class="sxs-lookup"><span data-stu-id="5c6f4-107">Files attached directly in an email or a meeting invite.</span></span>
- <span data-ttu-id="5c6f4-108">OneDrive for Business および SharePoint のモダン添付ファイル-ユーザーが電子メールのリンクとして共有する、OneDrive for business および SharePoint に格納されているファイル。</span><span class="sxs-lookup"><span data-stu-id="5c6f4-108">OneDrive for Business and SharePoint modern attachments - files stored in OneDrive for Business and SharePoint that users share as a links in an email.</span></span>

<span data-ttu-id="5c6f4-109">**注**: 現在、データを使用して共有 API の結果を設定する作業を行っています。</span><span class="sxs-lookup"><span data-stu-id="5c6f4-109">**Note**: We are currently working on populating the results of the Shared API with data.</span></span> <span data-ttu-id="5c6f4-110">リリース後の最初の週に、一部のデータが欠落している場合があります。</span><span class="sxs-lookup"><span data-stu-id="5c6f4-110">There may be some data missing in the first weeks after release.</span></span>

## <a name="methods"></a><span data-ttu-id="5c6f4-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="5c6f4-111">Methods</span></span>

| <span data-ttu-id="5c6f4-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="5c6f4-112">Method</span></span>       | <span data-ttu-id="5c6f4-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5c6f4-113">Return Type</span></span>  |<span data-ttu-id="5c6f4-114">説明</span><span class="sxs-lookup"><span data-stu-id="5c6f4-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5c6f4-115">共有リスト</span><span class="sxs-lookup"><span data-stu-id="5c6f4-115">List shared</span></span>](../api/insights-list-shared.md) |<span data-ttu-id="5c6f4-116">[insights_shared](insights-shared.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="5c6f4-116">[insights_shared](insights-shared.md) collection</span></span>| <span data-ttu-id="5c6f4-117">共有ファイルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="5c6f4-117">Get a list of shared files.</span></span>|

## <a name="properties"></a><span data-ttu-id="5c6f4-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5c6f4-118">Properties</span></span>

| <span data-ttu-id="5c6f4-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5c6f4-119">Property</span></span>              | <span data-ttu-id="5c6f4-120">型</span><span class="sxs-lookup"><span data-stu-id="5c6f4-120">Type</span></span>                      | <span data-ttu-id="5c6f4-121">説明</span><span class="sxs-lookup"><span data-stu-id="5c6f4-121">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="5c6f4-122">id</span><span class="sxs-lookup"><span data-stu-id="5c6f4-122">id</span></span>                    | <span data-ttu-id="5c6f4-123">String</span><span class="sxs-lookup"><span data-stu-id="5c6f4-123">String</span></span>                    | <span data-ttu-id="5c6f4-124">リレーションシップの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="5c6f4-124">Unique identifier of the relationship.</span></span> <span data-ttu-id="5c6f4-125">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5c6f4-125">Read only.</span></span>        |
| <span data-ttu-id="5c6f4-126">lastShared</span><span class="sxs-lookup"><span data-stu-id="5c6f4-126">lastShared</span></span>            | [<span data-ttu-id="5c6f4-127">sharingDetail</span><span class="sxs-lookup"><span data-stu-id="5c6f4-127">sharingDetail</span></span>](insights-sharingdetail.md)                | <span data-ttu-id="5c6f4-128">共有アイテムの詳細。</span><span class="sxs-lookup"><span data-stu-id="5c6f4-128">Details about the shared item.</span></span> <span data-ttu-id="5c6f4-129">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5c6f4-129">Read only.</span></span>        |
| <span data-ttu-id="5c6f4-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="5c6f4-130">resourceVisualization</span></span> | [<span data-ttu-id="5c6f4-131">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="5c6f4-131">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="5c6f4-132">ユーザーの作業でドキュメントをビジュアル化するために使用できるプロパティ。</span><span class="sxs-lookup"><span data-stu-id="5c6f4-132">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="5c6f4-133">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="5c6f4-133">Read-only</span></span>      |
| <span data-ttu-id="5c6f4-134">resourceReference</span><span class="sxs-lookup"><span data-stu-id="5c6f4-134">resourceReference</span></span>     | [<span data-ttu-id="5c6f4-135">resourceReference</span><span class="sxs-lookup"><span data-stu-id="5c6f4-135">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="5c6f4-136">ドキュメントの url や種類など、共有ドキュメントの参照プロパティ。</span><span class="sxs-lookup"><span data-stu-id="5c6f4-136">Reference properties of the shared document, such as the url and type of the document.</span></span> <span data-ttu-id="5c6f4-137">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="5c6f4-137">Read-only</span></span>       |

## <a name="relationships"></a><span data-ttu-id="5c6f4-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5c6f4-138">Relationships</span></span>

| <span data-ttu-id="5c6f4-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5c6f4-139">Property</span></span>      | <span data-ttu-id="5c6f4-140">型</span><span class="sxs-lookup"><span data-stu-id="5c6f4-140">Type</span></span>          | <span data-ttu-id="5c6f4-141">説明</span><span class="sxs-lookup"><span data-stu-id="5c6f4-141">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="5c6f4-142">リソース</span><span class="sxs-lookup"><span data-stu-id="5c6f4-142">resource</span></span>      | <span data-ttu-id="5c6f4-143">entity コレクション</span><span class="sxs-lookup"><span data-stu-id="5c6f4-143">entity collection</span></span> | <span data-ttu-id="5c6f4-144">共有されているアイテムに移動するために使用します。</span><span class="sxs-lookup"><span data-stu-id="5c6f4-144">Used for navigating to the item that was shared.</span></span> <span data-ttu-id="5c6f4-145">添付ファイルの場合、type は*Fileattachment*になります。</span><span class="sxs-lookup"><span data-stu-id="5c6f4-145">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="5c6f4-146">リンクされた添付ファイルの場合、種類は [*ドライブ] 項目*です。</span><span class="sxs-lookup"><span data-stu-id="5c6f4-146">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5c6f4-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5c6f4-147">JSON representation</span></span>
<span data-ttu-id="5c6f4-148">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="5c6f4-148">Here is a JSON representation of the resource</span></span>
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
