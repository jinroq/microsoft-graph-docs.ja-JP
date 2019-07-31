---
title: /リソースの種類 (Sharepoint)
description: または特定のユーザーによって共有されているファイルを表す洞察。 次の共有ファイルがサポートされています。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 47228e6597f24b9a6d662c7d87643322acaed40b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006235"
---
# <a name="sharedinsight-resource-type"></a><span data-ttu-id="63c7d-104">/リソースの種類 (Sharepoint)</span><span class="sxs-lookup"><span data-stu-id="63c7d-104">sharedInsight resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63c7d-105">または特定のユーザーによって共有されているファイルを表す洞察。</span><span class="sxs-lookup"><span data-stu-id="63c7d-105">An insight representing files shared with or by a specific user.</span></span> <span data-ttu-id="63c7d-106">次の共有ファイルがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="63c7d-106">The following shared files are supported:</span></span>

- <span data-ttu-id="63c7d-107">電子メールまたは会議の招待に直接添付されたファイル。</span><span class="sxs-lookup"><span data-stu-id="63c7d-107">Files attached directly in an email or a meeting invite.</span></span>
- <span data-ttu-id="63c7d-108">OneDrive for Bussiness および SharePoint モダン添付ファイル-ユーザーが電子メールのリンクとして共有する、OneDrive for Business および SharePoint に格納されているファイル。</span><span class="sxs-lookup"><span data-stu-id="63c7d-108">OneDrive for Bussiness and SharePoint modern attachments - files stored in OneDrive for Business and SharePoint that users share as a links in an email.</span></span>

<span data-ttu-id="63c7d-109">**注**: 現在、データを使用して共有 API の結果を設定する作業を行っています。</span><span class="sxs-lookup"><span data-stu-id="63c7d-109">**Note**: We are currently working on populating the results of the Shared API with data.</span></span> <span data-ttu-id="63c7d-110">リリース後の最初の週に、一部のデータが欠落している場合があります。</span><span class="sxs-lookup"><span data-stu-id="63c7d-110">There may be some data missing in the first weeks after release.</span></span>

## <a name="methods"></a><span data-ttu-id="63c7d-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="63c7d-111">Methods</span></span>

| <span data-ttu-id="63c7d-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="63c7d-112">Method</span></span>       | <span data-ttu-id="63c7d-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="63c7d-113">Return Type</span></span>  |<span data-ttu-id="63c7d-114">説明</span><span class="sxs-lookup"><span data-stu-id="63c7d-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="63c7d-115">共有リスト</span><span class="sxs-lookup"><span data-stu-id="63c7d-115">List shared</span></span>](../api/insights-list-shared.md) |<span data-ttu-id="63c7d-116">[insights_shared](insights-shared.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="63c7d-116">[insights_shared](insights-shared.md) collection</span></span>| <span data-ttu-id="63c7d-117">共有ファイルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="63c7d-117">Get a list of shared files.</span></span>|

## <a name="properties"></a><span data-ttu-id="63c7d-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="63c7d-118">Properties</span></span>

| <span data-ttu-id="63c7d-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="63c7d-119">Property</span></span>              | <span data-ttu-id="63c7d-120">型</span><span class="sxs-lookup"><span data-stu-id="63c7d-120">Type</span></span>                      | <span data-ttu-id="63c7d-121">説明</span><span class="sxs-lookup"><span data-stu-id="63c7d-121">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="63c7d-122">id</span><span class="sxs-lookup"><span data-stu-id="63c7d-122">id</span></span>                    | <span data-ttu-id="63c7d-123">String</span><span class="sxs-lookup"><span data-stu-id="63c7d-123">String</span></span>                    | <span data-ttu-id="63c7d-124">リレーションシップの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="63c7d-124">Unique identifier of the relationship.</span></span> <span data-ttu-id="63c7d-125">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="63c7d-125">Read only.</span></span>        |
| <span data-ttu-id="63c7d-126">lastShared</span><span class="sxs-lookup"><span data-stu-id="63c7d-126">lastShared</span></span>            | [<span data-ttu-id="63c7d-127">sharingDetail</span><span class="sxs-lookup"><span data-stu-id="63c7d-127">sharingDetail</span></span>](insights-sharingdetail.md)                | <span data-ttu-id="63c7d-128">共有アイテムの詳細。</span><span class="sxs-lookup"><span data-stu-id="63c7d-128">Details about the shared item.</span></span> <span data-ttu-id="63c7d-129">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="63c7d-129">Read only.</span></span>        |
| <span data-ttu-id="63c7d-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="63c7d-130">resourceVisualization</span></span> | [<span data-ttu-id="63c7d-131">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="63c7d-131">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="63c7d-132">ユーザーの作業でドキュメントをビジュアル化するために使用できるプロパティ。</span><span class="sxs-lookup"><span data-stu-id="63c7d-132">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="63c7d-133">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="63c7d-133">Read-only</span></span>      |
| <span data-ttu-id="63c7d-134">resourceReference</span><span class="sxs-lookup"><span data-stu-id="63c7d-134">resourceReference</span></span>     | [<span data-ttu-id="63c7d-135">resourceReference</span><span class="sxs-lookup"><span data-stu-id="63c7d-135">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="63c7d-136">ドキュメントの url や種類など、共有ドキュメントの参照プロパティ。</span><span class="sxs-lookup"><span data-stu-id="63c7d-136">Reference properties of the shared document, such as the url and type of the document.</span></span> <span data-ttu-id="63c7d-137">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="63c7d-137">Read-only</span></span>       |

## <a name="relationships"></a><span data-ttu-id="63c7d-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="63c7d-138">Relationships</span></span>

| <span data-ttu-id="63c7d-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="63c7d-139">Property</span></span>      | <span data-ttu-id="63c7d-140">型</span><span class="sxs-lookup"><span data-stu-id="63c7d-140">Type</span></span>          | <span data-ttu-id="63c7d-141">説明</span><span class="sxs-lookup"><span data-stu-id="63c7d-141">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="63c7d-142">リソース</span><span class="sxs-lookup"><span data-stu-id="63c7d-142">resource</span></span>      | <span data-ttu-id="63c7d-143">entity コレクション</span><span class="sxs-lookup"><span data-stu-id="63c7d-143">entity collection</span></span> | <span data-ttu-id="63c7d-144">共有されているアイテムに移動するために使用します。</span><span class="sxs-lookup"><span data-stu-id="63c7d-144">Used for navigating to the item that was shared.</span></span> <span data-ttu-id="63c7d-145">添付ファイルの場合、type は*Fileattachment*になります。</span><span class="sxs-lookup"><span data-stu-id="63c7d-145">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="63c7d-146">リンクされた添付ファイルの場合、種類は [*ドライブ] 項目*です。</span><span class="sxs-lookup"><span data-stu-id="63c7d-146">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="63c7d-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="63c7d-147">JSON representation</span></span>
<span data-ttu-id="63c7d-148">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="63c7d-148">Here is a JSON representation of the resource</span></span>
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
