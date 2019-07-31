---
title: resourceVisualization リソースの種類
description: Insights のプロパティを含む複合型。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: ce18edcdd4fc1b28288736767d38926d41612b67
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005731"
---
# <a name="resourcevisualization-resource-type"></a><span data-ttu-id="3e03f-103">resourceVisualization リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3e03f-103">resourceVisualization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e03f-104">[Insights](officegraphinsights.md)のプロパティを含む複合型。</span><span class="sxs-lookup"><span data-stu-id="3e03f-104">Complex type containing properties of [insights](officegraphinsights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e03f-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3e03f-105">JSON representation</span></span>

<span data-ttu-id="3e03f-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="3e03f-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],  
  "@odata.type": "microsoft.graph.resourceVisualization"
}-->
```json
{
  "title": "string",
  "type"  : "string",
  "mediaType": "string",
  "previewImageUrl": "string",
  "previewText": "string",
  "containerWebUrl": "string",
  "containerDisplayName": "string",
  "containerType": "string"
}
```

## <a name="properties"></a><span data-ttu-id="3e03f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3e03f-107">Properties</span></span>

| <span data-ttu-id="3e03f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3e03f-108">Property</span></span>              | <span data-ttu-id="3e03f-109">型</span><span class="sxs-lookup"><span data-stu-id="3e03f-109">Type</span></span>          | <span data-ttu-id="3e03f-110">説明</span><span class="sxs-lookup"><span data-stu-id="3e03f-110">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="3e03f-111">title</span><span class="sxs-lookup"><span data-stu-id="3e03f-111">title</span></span>                 | <span data-ttu-id="3e03f-112">String</span><span class="sxs-lookup"><span data-stu-id="3e03f-112">String</span></span>        | <span data-ttu-id="3e03f-113">アイテムのタイトルテキスト。</span><span class="sxs-lookup"><span data-stu-id="3e03f-113">The item's title text.</span></span>               |
| <span data-ttu-id="3e03f-114">type</span><span class="sxs-lookup"><span data-stu-id="3e03f-114">type</span></span>              | <span data-ttu-id="3e03f-115">String</span><span class="sxs-lookup"><span data-stu-id="3e03f-115">String</span></span>        | <span data-ttu-id="3e03f-116">アイテムのメディアの種類。</span><span class="sxs-lookup"><span data-stu-id="3e03f-116">The item's media type.</span></span> <span data-ttu-id="3e03f-117">特定の種類に基づいて特定のファイルをフィルター処理するために使用できます。</span><span class="sxs-lookup"><span data-stu-id="3e03f-117">Can be used for filtering for a specific file based on a specific type.</span></span> <span data-ttu-id="3e03f-118">サポートされる種類については、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3e03f-118">See below for supported types.</span></span> |
| <span data-ttu-id="3e03f-119">mediaType</span><span class="sxs-lookup"><span data-stu-id="3e03f-119">mediaType</span></span>             | <span data-ttu-id="3e03f-120">String</span><span class="sxs-lookup"><span data-stu-id="3e03f-120">String</span></span>        | <span data-ttu-id="3e03f-121">アイテムのメディアの種類。</span><span class="sxs-lookup"><span data-stu-id="3e03f-121">The item's media type.</span></span> <span data-ttu-id="3e03f-122">サポートされている IANA メディア Mime タイプに基づいて、特定の種類のファイルのフィルター処理に使用できます。</span><span class="sxs-lookup"><span data-stu-id="3e03f-122">Can be used for filtering for a specific type of file based on supported IANA Media Mime Types.</span></span> <span data-ttu-id="3e03f-123">すべてのメディア Mime タイプがサポートされるわけではないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="3e03f-123">Note that not all Media Mime Types are supported.</span></span> |
| <span data-ttu-id="3e03f-124">previewImageUrl</span><span class="sxs-lookup"><span data-stu-id="3e03f-124">previewImageUrl</span></span>       | <span data-ttu-id="3e03f-125">String</span><span class="sxs-lookup"><span data-stu-id="3e03f-125">String</span></span>        | <span data-ttu-id="3e03f-126">アイテムのプレビューイメージの先頭になる URL。</span><span class="sxs-lookup"><span data-stu-id="3e03f-126">A URL leading to the preview image for the item.</span></span> |
| <span data-ttu-id="3e03f-127">previewText</span><span class="sxs-lookup"><span data-stu-id="3e03f-127">previewText</span></span>           | <span data-ttu-id="3e03f-128">String</span><span class="sxs-lookup"><span data-stu-id="3e03f-128">String</span></span>        | <span data-ttu-id="3e03f-129">アイテムのプレビューテキスト。</span><span class="sxs-lookup"><span data-stu-id="3e03f-129">A preview text for the item.</span></span> |
| <span data-ttu-id="3e03f-130">containerWebUrl</span><span class="sxs-lookup"><span data-stu-id="3e03f-130">containerWebUrl</span></span>       | <span data-ttu-id="3e03f-131">String</span><span class="sxs-lookup"><span data-stu-id="3e03f-131">String</span></span>        | <span data-ttu-id="3e03f-132">アイテムが格納されるフォルダーへのパス。</span><span class="sxs-lookup"><span data-stu-id="3e03f-132">A path leading to the folder in which the item is stored.</span></span> |
| <span data-ttu-id="3e03f-133">containerDisplayName</span><span class="sxs-lookup"><span data-stu-id="3e03f-133">containerDisplayName</span></span>  | <span data-ttu-id="3e03f-134">String</span><span class="sxs-lookup"><span data-stu-id="3e03f-134">String</span></span>        | <span data-ttu-id="3e03f-135">アイテムが格納されている場所を示す文字列。</span><span class="sxs-lookup"><span data-stu-id="3e03f-135">A string describing where the item is stored.</span></span> <span data-ttu-id="3e03f-136">たとえば、SharePoint サイトの名前、またはアイテムを格納している OneDrive の所有者を識別するユーザー名。</span><span class="sxs-lookup"><span data-stu-id="3e03f-136">For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.</span></span>  |
| <span data-ttu-id="3e03f-137">containerType</span><span class="sxs-lookup"><span data-stu-id="3e03f-137">containerType</span></span>         | <span data-ttu-id="3e03f-138">String</span><span class="sxs-lookup"><span data-stu-id="3e03f-138">String</span></span> | <span data-ttu-id="3e03f-139">ファイルが格納されているコンテナーの種類によるフィルター処理に使用できます。</span><span class="sxs-lookup"><span data-stu-id="3e03f-139">Can be used for filtering by the type of container in which the file is stored.</span></span> <span data-ttu-id="3e03f-140">サイト、Onedrive Business など。</span><span class="sxs-lookup"><span data-stu-id="3e03f-140">Such as Site or OneDriveBusiness.</span></span>       |

## <a name="type-property-values"></a><span data-ttu-id="3e03f-141">Type プロパティの値</span><span class="sxs-lookup"><span data-stu-id="3e03f-141">Type property values</span></span>
-   <span data-ttu-id="3e03f-142">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="3e03f-142">PowerPoint</span></span>
-   <span data-ttu-id="3e03f-143">Word</span><span class="sxs-lookup"><span data-stu-id="3e03f-143">Word</span></span>
-   <span data-ttu-id="3e03f-144">Excel</span><span class="sxs-lookup"><span data-stu-id="3e03f-144">Excel</span></span>
-   <span data-ttu-id="3e03f-145">文書</span><span class="sxs-lookup"><span data-stu-id="3e03f-145">Pdf</span></span>
-   <span data-ttu-id="3e03f-146">OneNote</span><span class="sxs-lookup"><span data-stu-id="3e03f-146">OneNote</span></span>
-   <span data-ttu-id="3e03f-147">OneNotePage</span><span class="sxs-lookup"><span data-stu-id="3e03f-147">OneNotePage</span></span>
-   <span data-ttu-id="3e03f-148">InfoPath</span><span class="sxs-lookup"><span data-stu-id="3e03f-148">InfoPath</span></span>
-   <span data-ttu-id="3e03f-149">Visio</span><span class="sxs-lookup"><span data-stu-id="3e03f-149">Visio</span></span>
-   <span data-ttu-id="3e03f-150">Publisher</span><span class="sxs-lookup"><span data-stu-id="3e03f-150">Publisher</span></span>
-   <span data-ttu-id="3e03f-151">Project</span><span class="sxs-lookup"><span data-stu-id="3e03f-151">Project</span></span>
-   <span data-ttu-id="3e03f-152">Access</span><span class="sxs-lookup"><span data-stu-id="3e03f-152">Access</span></span>
-   <span data-ttu-id="3e03f-153">メール</span><span class="sxs-lookup"><span data-stu-id="3e03f-153">Mail</span></span>
-   <span data-ttu-id="3e03f-154">.Csv</span><span class="sxs-lookup"><span data-stu-id="3e03f-154">Csv</span></span>
-   <span data-ttu-id="3e03f-155">アーカイブ</span><span class="sxs-lookup"><span data-stu-id="3e03f-155">Archive</span></span>
-   <span data-ttu-id="3e03f-156">Xps</span><span class="sxs-lookup"><span data-stu-id="3e03f-156">Xps</span></span>
-   <span data-ttu-id="3e03f-157">オーディオ</span><span class="sxs-lookup"><span data-stu-id="3e03f-157">Audio</span></span>
-   <span data-ttu-id="3e03f-158">ビデオ</span><span class="sxs-lookup"><span data-stu-id="3e03f-158">Video</span></span>
-   <span data-ttu-id="3e03f-159">イメージ</span><span class="sxs-lookup"><span data-stu-id="3e03f-159">Image</span></span>
-   <span data-ttu-id="3e03f-160">Web</span><span class="sxs-lookup"><span data-stu-id="3e03f-160">Web</span></span>
-   <span data-ttu-id="3e03f-161">テキスト</span><span class="sxs-lookup"><span data-stu-id="3e03f-161">Text</span></span>
-   <span data-ttu-id="3e03f-162">Xml</span><span class="sxs-lookup"><span data-stu-id="3e03f-162">Xml</span></span>
-   <span data-ttu-id="3e03f-163">Story</span><span class="sxs-lookup"><span data-stu-id="3e03f-163">Story</span></span>
-   <span data-ttu-id="3e03f-164">ExternalContent</span><span class="sxs-lookup"><span data-stu-id="3e03f-164">ExternalContent</span></span>
-   <span data-ttu-id="3e03f-165">フォルダー</span><span class="sxs-lookup"><span data-stu-id="3e03f-165">Folder</span></span>
-   <span data-ttu-id="3e03f-166">Other</span><span class="sxs-lookup"><span data-stu-id="3e03f-166">Other</span></span>

<span data-ttu-id="3e03f-167">クエリの例:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span><span class="sxs-lookup"><span data-stu-id="3e03f-167">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span></span>

## <a name="containertype-property-values"></a><span data-ttu-id="3e03f-168">containerType プロパティの値</span><span class="sxs-lookup"><span data-stu-id="3e03f-168">containerType property values</span></span>
<span data-ttu-id="3e03f-169">サポートされている種類は、 [Officegraphinsights](officegraphinsights.md)がファイルを返すコンテナーによって異なる場合があります。</span><span class="sxs-lookup"><span data-stu-id="3e03f-169">The supported types can differ based on containers from which [officeGraphInsights](officegraphinsights.md) returns files.</span></span> <span data-ttu-id="3e03f-170">たとえば、"DropBox"、"Box"、および "GDrive" からファイルを取得するのは、 [sharepoint](insights-shared.md)のファイルです。</span><span class="sxs-lookup"><span data-stu-id="3e03f-170">For example, only the [sharedInsight](insights-shared.md) insight returns files from 'DropBox', 'Box', and 'GDrive'.</span></span>

-   <span data-ttu-id="3e03f-171">Onedrive Business</span><span class="sxs-lookup"><span data-stu-id="3e03f-171">OneDriveBusiness</span></span>
-   <span data-ttu-id="3e03f-172">Site</span><span class="sxs-lookup"><span data-stu-id="3e03f-172">Site</span></span>
-   <span data-ttu-id="3e03f-173">メール</span><span class="sxs-lookup"><span data-stu-id="3e03f-173">Mail</span></span>
-   <span data-ttu-id="3e03f-174">DropBox</span><span class="sxs-lookup"><span data-stu-id="3e03f-174">DropBox</span></span>
-   <span data-ttu-id="3e03f-175">検索ボックス</span><span class="sxs-lookup"><span data-stu-id="3e03f-175">Box</span></span>
-   <span data-ttu-id="3e03f-176">GDrive</span><span class="sxs-lookup"><span data-stu-id="3e03f-176">GDrive</span></span>

<span data-ttu-id="3e03f-177">クエリの例:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span><span class="sxs-lookup"><span data-stu-id="3e03f-177">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span></span>
