---
title: 共有リソースの種類
description: または特定のユーザーが共有ファイルを表すの把握。 次の共有ファイルがサポートされています。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 49e18318c1e93d2393b957b404ff4617b334f237
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573180"
---
# <a name="shared-resource-type"></a><span data-ttu-id="4c673-104">共有リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4c673-104">shared resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c673-105">または特定のユーザーが共有ファイルを表すの把握。</span><span class="sxs-lookup"><span data-stu-id="4c673-105">An insight representing files shared with or by a specific user.</span></span> <span data-ttu-id="4c673-106">次の共有ファイルがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="4c673-106">The following shared files are supported:</span></span>

- <span data-ttu-id="4c673-107">電子メールや会議に直接接続されているファイルを招待します。</span><span class="sxs-lookup"><span data-stu-id="4c673-107">Files attached directly in an email or a meeting invite.</span></span>
- <span data-ttu-id="4c673-108">名刺と SharePoint 現代の添付ファイル、ビジネスおよびユーザーが、リンクとして電子メールで共有する SharePoint の OneDrive に格納されているファイルの OneDrive です。</span><span class="sxs-lookup"><span data-stu-id="4c673-108">OneDrive for Bussiness and SharePoint modern attachments - files stored in OneDrive for Business and SharePoint that users share as a links in an email.</span></span>

<span data-ttu-id="4c673-109">**注**: データの共有 API の結果を作成するのに現在進行中です。</span><span class="sxs-lookup"><span data-stu-id="4c673-109">**Note**: We are currently working on populating the results of the Shared API with data.</span></span> <span data-ttu-id="4c673-110">リリース後の最初の週で不足しているいくつかのデータがある可能性があります。</span><span class="sxs-lookup"><span data-stu-id="4c673-110">There may be some data missing in the first weeks after release.</span></span>

## <a name="methods"></a><span data-ttu-id="4c673-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="4c673-111">Methods</span></span>

| <span data-ttu-id="4c673-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="4c673-112">Method</span></span>       | <span data-ttu-id="4c673-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4c673-113">Return Type</span></span>  |<span data-ttu-id="4c673-114">説明</span><span class="sxs-lookup"><span data-stu-id="4c673-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4c673-115">共有リスト</span><span class="sxs-lookup"><span data-stu-id="4c673-115">List shared</span></span>](../api/insights-list-shared.md) |<span data-ttu-id="4c673-116">[insights_shared](insights-shared.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4c673-116">[insights_shared](insights-shared.md) collection</span></span>| <span data-ttu-id="4c673-117">共有ファイルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="4c673-117">Get a list of shared files.</span></span>|

## <a name="properties"></a><span data-ttu-id="4c673-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c673-118">Properties</span></span>

| <span data-ttu-id="4c673-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c673-119">Property</span></span>              | <span data-ttu-id="4c673-120">型</span><span class="sxs-lookup"><span data-stu-id="4c673-120">Type</span></span>                      | <span data-ttu-id="4c673-121">説明</span><span class="sxs-lookup"><span data-stu-id="4c673-121">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="4c673-122">id</span><span class="sxs-lookup"><span data-stu-id="4c673-122">id</span></span>                    | <span data-ttu-id="4c673-123">String</span><span class="sxs-lookup"><span data-stu-id="4c673-123">String</span></span>                    | <span data-ttu-id="4c673-124">リレーションシップの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="4c673-124">Unique identifier of the relationship.</span></span> <span data-ttu-id="4c673-125">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4c673-125">Read only.</span></span>        |
| <span data-ttu-id="4c673-126">lastShared</span><span class="sxs-lookup"><span data-stu-id="4c673-126">lastShared</span></span>            | [<span data-ttu-id="4c673-127">sharingDetail</span><span class="sxs-lookup"><span data-stu-id="4c673-127">sharingDetail</span></span>](insights-sharingdetail.md)                | <span data-ttu-id="4c673-128">共有アイテムに関する詳細情報です。</span><span class="sxs-lookup"><span data-stu-id="4c673-128">Details about the shared item.</span></span> <span data-ttu-id="4c673-129">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4c673-129">Read only.</span></span>        |
| <span data-ttu-id="4c673-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="4c673-130">resourceVisualization</span></span> | [<span data-ttu-id="4c673-131">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="4c673-131">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="4c673-132">プロパティは、時にドキュメントをビジュアル化を使用することができます。</span><span class="sxs-lookup"><span data-stu-id="4c673-132">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="4c673-133">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="4c673-133">Read-only</span></span>      |
| <span data-ttu-id="4c673-134">resourceReference</span><span class="sxs-lookup"><span data-stu-id="4c673-134">resourceReference</span></span>     | [<span data-ttu-id="4c673-135">resourceReference</span><span class="sxs-lookup"><span data-stu-id="4c673-135">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="4c673-136">Url およびドキュメントの種類など、共有ドキュメントのプロパティを参照します。</span><span class="sxs-lookup"><span data-stu-id="4c673-136">Reference properties of the shared document, such as the url and type of the document.</span></span> <span data-ttu-id="4c673-137">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="4c673-137">Read-only</span></span>       |

## <a name="relationships"></a><span data-ttu-id="4c673-138">関係</span><span class="sxs-lookup"><span data-stu-id="4c673-138">Relationships</span></span>

| <span data-ttu-id="4c673-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c673-139">Property</span></span>      | <span data-ttu-id="4c673-140">型</span><span class="sxs-lookup"><span data-stu-id="4c673-140">Type</span></span>          | <span data-ttu-id="4c673-141">説明</span><span class="sxs-lookup"><span data-stu-id="4c673-141">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="4c673-142">リソース</span><span class="sxs-lookup"><span data-stu-id="4c673-142">resource</span></span>      | <span data-ttu-id="4c673-143">エンティティのコレクション</span><span class="sxs-lookup"><span data-stu-id="4c673-143">entity collection</span></span> | <span data-ttu-id="4c673-144">共有されている項目に移動するために使用します。</span><span class="sxs-lookup"><span data-stu-id="4c673-144">Used for navigating to the item that was shared.</span></span> <span data-ttu-id="4c673-145">ファイルの添付ファイルの種類は、 *fileAttachment*です。</span><span class="sxs-lookup"><span data-stu-id="4c673-145">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="4c673-146">リンクされた添付ファイルの場合は、型は、 *driveItem*です。</span><span class="sxs-lookup"><span data-stu-id="4c673-146">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4c673-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4c673-147">JSON representation</span></span>
<span data-ttu-id="4c673-148">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="4c673-148">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.shared"
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-shared.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
