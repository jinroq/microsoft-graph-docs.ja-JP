---
title: 共有リソースの種類
description: または特定のユーザーが共有ファイルを表すの把握。 次の共有ファイルがサポートされています。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 11a6989e0130e7eedca7fff6f6cc9790d8109d84
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640127"
---
# <a name="shared-resource-type"></a><span data-ttu-id="32ae0-104">共有リソースの種類</span><span class="sxs-lookup"><span data-stu-id="32ae0-104">shared resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32ae0-105">または特定のユーザーが共有ファイルを表すの把握。</span><span class="sxs-lookup"><span data-stu-id="32ae0-105">An insight representing files shared with or by a specific user.</span></span> <span data-ttu-id="32ae0-106">次の共有ファイルがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="32ae0-106">The following shared files are supported:</span></span>

- <span data-ttu-id="32ae0-107">電子メールや会議に直接接続されているファイルを招待します。</span><span class="sxs-lookup"><span data-stu-id="32ae0-107">Files attached directly in an email or a meeting invite.</span></span>
- <span data-ttu-id="32ae0-108">名刺と SharePoint 現代の添付ファイル、ビジネスおよびユーザーが、リンクとして電子メールで共有する SharePoint の OneDrive に格納されているファイルの OneDrive です。</span><span class="sxs-lookup"><span data-stu-id="32ae0-108">OneDrive for Bussiness and SharePoint modern attachments - files stored in OneDrive for Business and SharePoint that users share as a links in an email.</span></span>

<span data-ttu-id="32ae0-109">**注**: データの共有 API の結果を作成するのに現在進行中です。</span><span class="sxs-lookup"><span data-stu-id="32ae0-109">**Note**: We are currently working on populating the results of the Shared API with data.</span></span> <span data-ttu-id="32ae0-110">リリース後の最初の週で不足しているいくつかのデータがある可能性があります。</span><span class="sxs-lookup"><span data-stu-id="32ae0-110">There may be some data missing in the first weeks after release.</span></span>

## <a name="methods"></a><span data-ttu-id="32ae0-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="32ae0-111">Methods</span></span>

| <span data-ttu-id="32ae0-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="32ae0-112">Method</span></span>       | <span data-ttu-id="32ae0-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="32ae0-113">Return Type</span></span>  |<span data-ttu-id="32ae0-114">説明</span><span class="sxs-lookup"><span data-stu-id="32ae0-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="32ae0-115">共有リスト</span><span class="sxs-lookup"><span data-stu-id="32ae0-115">List shared</span></span>](../api/insights-list-shared.md) |<span data-ttu-id="32ae0-116">[insights_shared](insights-shared.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="32ae0-116">[insights_shared](insights-shared.md) collection</span></span>| <span data-ttu-id="32ae0-117">共有ファイルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="32ae0-117">Get a list of shared files.</span></span>|

## <a name="properties"></a><span data-ttu-id="32ae0-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="32ae0-118">Properties</span></span>

| <span data-ttu-id="32ae0-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="32ae0-119">Property</span></span>              | <span data-ttu-id="32ae0-120">型</span><span class="sxs-lookup"><span data-stu-id="32ae0-120">Type</span></span>                      | <span data-ttu-id="32ae0-121">説明</span><span class="sxs-lookup"><span data-stu-id="32ae0-121">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="32ae0-122">id</span><span class="sxs-lookup"><span data-stu-id="32ae0-122">id</span></span>                    | <span data-ttu-id="32ae0-123">String</span><span class="sxs-lookup"><span data-stu-id="32ae0-123">String</span></span>                    | <span data-ttu-id="32ae0-124">リレーションシップの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="32ae0-124">Unique identifier of the relationship.</span></span> <span data-ttu-id="32ae0-125">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="32ae0-125">Read only.</span></span>        |
| <span data-ttu-id="32ae0-126">lastShared</span><span class="sxs-lookup"><span data-stu-id="32ae0-126">lastShared</span></span>            | [<span data-ttu-id="32ae0-127">sharingDetail</span><span class="sxs-lookup"><span data-stu-id="32ae0-127">sharingDetail</span></span>](insights-sharingdetail.md)                | <span data-ttu-id="32ae0-128">共有アイテムに関する詳細情報です。</span><span class="sxs-lookup"><span data-stu-id="32ae0-128">Details about the shared item.</span></span> <span data-ttu-id="32ae0-129">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="32ae0-129">Read only.</span></span>        |
| <span data-ttu-id="32ae0-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="32ae0-130">resourceVisualization</span></span> | [<span data-ttu-id="32ae0-131">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="32ae0-131">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="32ae0-132">プロパティは、時にドキュメントをビジュアル化を使用することができます。</span><span class="sxs-lookup"><span data-stu-id="32ae0-132">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="32ae0-133">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="32ae0-133">Read-only</span></span>      |
| <span data-ttu-id="32ae0-134">resourceReference</span><span class="sxs-lookup"><span data-stu-id="32ae0-134">resourceReference</span></span>     | [<span data-ttu-id="32ae0-135">resourceReference</span><span class="sxs-lookup"><span data-stu-id="32ae0-135">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="32ae0-136">Url およびドキュメントの種類など、共有ドキュメントのプロパティを参照します。</span><span class="sxs-lookup"><span data-stu-id="32ae0-136">Reference properties of the shared document, such as the url and type of the document.</span></span> <span data-ttu-id="32ae0-137">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="32ae0-137">Read-only</span></span>       |

## <a name="relationships"></a><span data-ttu-id="32ae0-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="32ae0-138">Relationships</span></span>

| <span data-ttu-id="32ae0-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="32ae0-139">Property</span></span>      | <span data-ttu-id="32ae0-140">型</span><span class="sxs-lookup"><span data-stu-id="32ae0-140">Type</span></span>          | <span data-ttu-id="32ae0-141">説明</span><span class="sxs-lookup"><span data-stu-id="32ae0-141">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="32ae0-142">リソース</span><span class="sxs-lookup"><span data-stu-id="32ae0-142">resource</span></span>      | <span data-ttu-id="32ae0-143">Entity</span><span class="sxs-lookup"><span data-stu-id="32ae0-143">Entity</span></span>        | <span data-ttu-id="32ae0-144">共有されている項目に移動するために使用します。</span><span class="sxs-lookup"><span data-stu-id="32ae0-144">Used for navigating to the item that was shared.</span></span> <span data-ttu-id="32ae0-145">ファイルの添付ファイルの種類は、 *fileAttachment*です。</span><span class="sxs-lookup"><span data-stu-id="32ae0-145">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="32ae0-146">リンクされた添付ファイルの場合は、型は、 *driveItem*です。</span><span class="sxs-lookup"><span data-stu-id="32ae0-146">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="32ae0-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="32ae0-147">JSON representation</span></span>
<span data-ttu-id="32ae0-148">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="32ae0-148">Here is a JSON representation of the resource</span></span>

```json
{
  "id": "string",
  "lastShared": "sharingDetail",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-shared.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
