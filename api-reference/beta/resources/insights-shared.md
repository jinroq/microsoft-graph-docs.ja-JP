---
title: 共有リソースの種類
description: または特定のユーザーが共有ファイルを表すの把握。 次の共有ファイルがサポートされています。
ms.openlocfilehash: 786e3cc94a3c108b30cca880491dab5725014570
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071447"
---
# <a name="shared-resource-type"></a><span data-ttu-id="73763-104">共有リソースの種類</span><span class="sxs-lookup"><span data-stu-id="73763-104">shared resource type</span></span>

> <span data-ttu-id="73763-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="73763-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73763-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="73763-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="73763-107">または特定のユーザーが共有ファイルを表すの把握。</span><span class="sxs-lookup"><span data-stu-id="73763-107">An insight representing files shared with or by a specific user.</span></span> <span data-ttu-id="73763-108">次の共有ファイルがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="73763-108">The following shared files are supported:</span></span>

- <span data-ttu-id="73763-109">電子メールや会議に直接接続されているファイルを招待します。</span><span class="sxs-lookup"><span data-stu-id="73763-109">Files attached directly in an email or a meeting invite.</span></span>
- <span data-ttu-id="73763-110">名刺と SharePoint 現代の添付ファイル、ビジネスおよびユーザーが、リンクとして電子メールで共有する SharePoint の OneDrive に格納されているファイルの OneDrive です。</span><span class="sxs-lookup"><span data-stu-id="73763-110">OneDrive for Bussiness and SharePoint modern attachments - files stored in OneDrive for Business and SharePoint that users share as a links in an email.</span></span>

<span data-ttu-id="73763-111">**注**: データの共有 API の結果を作成するのに現在進行中です。</span><span class="sxs-lookup"><span data-stu-id="73763-111">**Note**: We are currently working on populating the results of the Shared API with data.</span></span> <span data-ttu-id="73763-112">リリース後の最初の週で不足しているいくつかのデータがある可能性があります。</span><span class="sxs-lookup"><span data-stu-id="73763-112">There may be some data missing in the first weeks after release.</span></span>

## <a name="methods"></a><span data-ttu-id="73763-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="73763-113">Methods</span></span>

| <span data-ttu-id="73763-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="73763-114">Method</span></span>       | <span data-ttu-id="73763-115">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="73763-115">Return Type</span></span>  |<span data-ttu-id="73763-116">説明</span><span class="sxs-lookup"><span data-stu-id="73763-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="73763-117">共有リスト</span><span class="sxs-lookup"><span data-stu-id="73763-117">List shared</span></span>](../api/insights-list-shared.md) |<span data-ttu-id="73763-118">[insights_shared](insights-shared.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="73763-118">[insights_shared](insights-shared.md) collection</span></span>| <span data-ttu-id="73763-119">共有ファイルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="73763-119">Get a list of shared files.</span></span>|

## <a name="properties"></a><span data-ttu-id="73763-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="73763-120">Properties</span></span>

| <span data-ttu-id="73763-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="73763-121">Property</span></span>              | <span data-ttu-id="73763-122">型</span><span class="sxs-lookup"><span data-stu-id="73763-122">Type</span></span>                      | <span data-ttu-id="73763-123">説明</span><span class="sxs-lookup"><span data-stu-id="73763-123">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="73763-124">id</span><span class="sxs-lookup"><span data-stu-id="73763-124">id</span></span>                    | <span data-ttu-id="73763-125">String</span><span class="sxs-lookup"><span data-stu-id="73763-125">String</span></span>                    | <span data-ttu-id="73763-126">リレーションシップの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="73763-126">Unique identifier of the relationship.</span></span> <span data-ttu-id="73763-127">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="73763-127">Read only.</span></span>        |
| <span data-ttu-id="73763-128">lastShared</span><span class="sxs-lookup"><span data-stu-id="73763-128">lastShared</span></span>            | [<span data-ttu-id="73763-129">sharingDetail</span><span class="sxs-lookup"><span data-stu-id="73763-129">sharingDetail</span></span>](insights-sharingdetail.md)                | <span data-ttu-id="73763-130">共有アイテムに関する詳細情報です。</span><span class="sxs-lookup"><span data-stu-id="73763-130">Details about the shared item.</span></span> <span data-ttu-id="73763-131">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="73763-131">Read only.</span></span>        |
| <span data-ttu-id="73763-132">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="73763-132">resourceVisualization</span></span> | [<span data-ttu-id="73763-133">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="73763-133">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="73763-134">プロパティは、時にドキュメントをビジュアル化を使用することができます。</span><span class="sxs-lookup"><span data-stu-id="73763-134">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="73763-135">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="73763-135">Read-only</span></span>      |
| <span data-ttu-id="73763-136">resourceReference</span><span class="sxs-lookup"><span data-stu-id="73763-136">resourceReference</span></span>     | [<span data-ttu-id="73763-137">resourceReference</span><span class="sxs-lookup"><span data-stu-id="73763-137">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="73763-138">Url およびドキュメントの種類など、共有ドキュメントのプロパティを参照します。</span><span class="sxs-lookup"><span data-stu-id="73763-138">Reference properties of the shared document, such as the url and type of the document.</span></span> <span data-ttu-id="73763-139">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="73763-139">Read-only</span></span>       |

## <a name="relationships"></a><span data-ttu-id="73763-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="73763-140">Relationships</span></span>

| <span data-ttu-id="73763-141">プロパティ</span><span class="sxs-lookup"><span data-stu-id="73763-141">Property</span></span>      | <span data-ttu-id="73763-142">型</span><span class="sxs-lookup"><span data-stu-id="73763-142">Type</span></span>          | <span data-ttu-id="73763-143">説明</span><span class="sxs-lookup"><span data-stu-id="73763-143">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="73763-144">リソース</span><span class="sxs-lookup"><span data-stu-id="73763-144">resource</span></span>      | <span data-ttu-id="73763-145">エンティティ</span><span class="sxs-lookup"><span data-stu-id="73763-145">Entity</span></span>        | <span data-ttu-id="73763-146">共有されている項目に移動するために使用します。</span><span class="sxs-lookup"><span data-stu-id="73763-146">Used for navigating to the item that was shared.</span></span> <span data-ttu-id="73763-147">ファイルの添付ファイルの種類は、 *fileAttachment*です。</span><span class="sxs-lookup"><span data-stu-id="73763-147">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="73763-148">リンクされた添付ファイルの場合は、型は、 *driveItem*です。</span><span class="sxs-lookup"><span data-stu-id="73763-148">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="73763-149">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="73763-149">JSON representation</span></span>
<span data-ttu-id="73763-150">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="73763-150">Here is a JSON representation of the resource</span></span>

```json
{
  "id": "string",
  "lastShared": "sharingDetail",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```