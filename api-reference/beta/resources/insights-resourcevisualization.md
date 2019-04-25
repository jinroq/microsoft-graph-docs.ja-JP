---
title: resourcevisualization リソースの種類
description: Insights のプロパティを含む複合型。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 48ec1619d07d0f31bf8325c25b161084f505b3ee
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550738"
---
# <a name="resourcevisualization-resource-type"></a><span data-ttu-id="70d43-103">resourcevisualization リソースの種類</span><span class="sxs-lookup"><span data-stu-id="70d43-103">resourceVisualization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70d43-104">[Insights](insights.md)のプロパティを含む複合型。</span><span class="sxs-lookup"><span data-stu-id="70d43-104">Complex type containing properties of [Insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="70d43-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="70d43-105">JSON representation</span></span>

<span data-ttu-id="70d43-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="70d43-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="70d43-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="70d43-107">Properties</span></span>

| <span data-ttu-id="70d43-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="70d43-108">Property</span></span>              | <span data-ttu-id="70d43-109">型</span><span class="sxs-lookup"><span data-stu-id="70d43-109">Type</span></span>          | <span data-ttu-id="70d43-110">説明</span><span class="sxs-lookup"><span data-stu-id="70d43-110">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="70d43-111">title</span><span class="sxs-lookup"><span data-stu-id="70d43-111">title</span></span>                 | <span data-ttu-id="70d43-112">String</span><span class="sxs-lookup"><span data-stu-id="70d43-112">String</span></span>        | <span data-ttu-id="70d43-113">アイテムのタイトルテキスト。</span><span class="sxs-lookup"><span data-stu-id="70d43-113">The item's title text.</span></span>               |
| <span data-ttu-id="70d43-114">type</span><span class="sxs-lookup"><span data-stu-id="70d43-114">type</span></span>              | <span data-ttu-id="70d43-115">String</span><span class="sxs-lookup"><span data-stu-id="70d43-115">String</span></span>        | <span data-ttu-id="70d43-116">アイテムのメディアの種類。</span><span class="sxs-lookup"><span data-stu-id="70d43-116">The item's media type.</span></span> <span data-ttu-id="70d43-117">特定の種類に基づいて特定のファイルをフィルター処理するために使用できます。</span><span class="sxs-lookup"><span data-stu-id="70d43-117">Can be used for filtering for a specific file based on a specific type.</span></span> <span data-ttu-id="70d43-118">サポートされる種類については、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="70d43-118">See below for supported types.</span></span> |
| <span data-ttu-id="70d43-119">mediaType</span><span class="sxs-lookup"><span data-stu-id="70d43-119">mediaType</span></span>             | <span data-ttu-id="70d43-120">String</span><span class="sxs-lookup"><span data-stu-id="70d43-120">String</span></span>        | <span data-ttu-id="70d43-121">アイテムのメディアの種類。</span><span class="sxs-lookup"><span data-stu-id="70d43-121">The item's media type.</span></span> <span data-ttu-id="70d43-122">は、サポートされている IANA メディア Mime タイプに基づいて、特定の種類のファイルをフィルター処理するために使用できます。</span><span class="sxs-lookup"><span data-stu-id="70d43-122">Can be used for for filtering for a specific type of file based on supported IANA Media Mime Types.</span></span> <span data-ttu-id="70d43-123">すべてのメディア Mime タイプがサポートされるわけではないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="70d43-123">Note that not all Media Mime Types are supported.</span></span> |
| <span data-ttu-id="70d43-124">previewImageUrl</span><span class="sxs-lookup"><span data-stu-id="70d43-124">previewImageUrl</span></span>       | <span data-ttu-id="70d43-125">String</span><span class="sxs-lookup"><span data-stu-id="70d43-125">String</span></span>        | <span data-ttu-id="70d43-126">アイテムのプレビューイメージの先頭になる URL。</span><span class="sxs-lookup"><span data-stu-id="70d43-126">A URL leading to the preview image for the item.</span></span> |
| <span data-ttu-id="70d43-127">previewText</span><span class="sxs-lookup"><span data-stu-id="70d43-127">previewText</span></span>           | <span data-ttu-id="70d43-128">String</span><span class="sxs-lookup"><span data-stu-id="70d43-128">String</span></span>        | <span data-ttu-id="70d43-129">アイテムのプレビューテキスト。</span><span class="sxs-lookup"><span data-stu-id="70d43-129">A preview text for the item.</span></span> |
| <span data-ttu-id="70d43-130">containerWebUrl</span><span class="sxs-lookup"><span data-stu-id="70d43-130">containerWebUrl</span></span>       | <span data-ttu-id="70d43-131">String</span><span class="sxs-lookup"><span data-stu-id="70d43-131">String</span></span>        | <span data-ttu-id="70d43-132">アイテムが格納されるフォルダーへのパス。</span><span class="sxs-lookup"><span data-stu-id="70d43-132">A path leading to the folder in which the item is stored.</span></span> |
| <span data-ttu-id="70d43-133">containerDisplayName</span><span class="sxs-lookup"><span data-stu-id="70d43-133">containerDisplayName</span></span>  | <span data-ttu-id="70d43-134">String</span><span class="sxs-lookup"><span data-stu-id="70d43-134">String</span></span>        | <span data-ttu-id="70d43-135">アイテムが格納されている場所を示す文字列。</span><span class="sxs-lookup"><span data-stu-id="70d43-135">A string describing where the item is stored.</span></span> <span data-ttu-id="70d43-136">たとえば、SharePoint サイトの名前、またはアイテムを格納している OneDrive の所有者を識別するユーザー名。</span><span class="sxs-lookup"><span data-stu-id="70d43-136">For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.</span></span>  |
| <span data-ttu-id="70d43-137">containerType</span><span class="sxs-lookup"><span data-stu-id="70d43-137">containerType</span></span>         | <span data-ttu-id="70d43-138">String</span><span class="sxs-lookup"><span data-stu-id="70d43-138">String</span></span> | <span data-ttu-id="70d43-139">ファイルが格納されているコンテナーの種類によるフィルター処理に使用できます。</span><span class="sxs-lookup"><span data-stu-id="70d43-139">Can be used for filtering by the type of container in which the file is stored.</span></span> <span data-ttu-id="70d43-140">サイト、onedrive business など。</span><span class="sxs-lookup"><span data-stu-id="70d43-140">Such as Site or OneDriveBusiness.</span></span>       |

## <a name="type-property-values"></a><span data-ttu-id="70d43-141">Type プロパティの値</span><span class="sxs-lookup"><span data-stu-id="70d43-141">Type property values</span></span>
-   <span data-ttu-id="70d43-142">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="70d43-142">PowerPoint</span></span>
-   <span data-ttu-id="70d43-143">Word</span><span class="sxs-lookup"><span data-stu-id="70d43-143">Word</span></span>
-   <span data-ttu-id="70d43-144">Excel</span><span class="sxs-lookup"><span data-stu-id="70d43-144">Excel</span></span>
-   <span data-ttu-id="70d43-145">文書</span><span class="sxs-lookup"><span data-stu-id="70d43-145">Pdf</span></span>
-   <span data-ttu-id="70d43-146">OneNote</span><span class="sxs-lookup"><span data-stu-id="70d43-146">OneNote</span></span>
-   <span data-ttu-id="70d43-147">OneNotePage</span><span class="sxs-lookup"><span data-stu-id="70d43-147">OneNotePage</span></span>
-   <span data-ttu-id="70d43-148">InfoPath</span><span class="sxs-lookup"><span data-stu-id="70d43-148">InfoPath</span></span>
-   <span data-ttu-id="70d43-149">Visio</span><span class="sxs-lookup"><span data-stu-id="70d43-149">Visio</span></span>
-   <span data-ttu-id="70d43-150">Publisher</span><span class="sxs-lookup"><span data-stu-id="70d43-150">Publisher</span></span>
-   <span data-ttu-id="70d43-151">プロジェクト</span><span class="sxs-lookup"><span data-stu-id="70d43-151">Project</span></span>
-   <span data-ttu-id="70d43-152">Access</span><span class="sxs-lookup"><span data-stu-id="70d43-152">Access</span></span>
-   <span data-ttu-id="70d43-153">メール</span><span class="sxs-lookup"><span data-stu-id="70d43-153">Mail</span></span>
-   <span data-ttu-id="70d43-154">.csv</span><span class="sxs-lookup"><span data-stu-id="70d43-154">Csv</span></span>
-   <span data-ttu-id="70d43-155">アーカイブ</span><span class="sxs-lookup"><span data-stu-id="70d43-155">Archive</span></span>
-   <span data-ttu-id="70d43-156">Xps</span><span class="sxs-lookup"><span data-stu-id="70d43-156">Xps</span></span>
-   <span data-ttu-id="70d43-157">オーディオ</span><span class="sxs-lookup"><span data-stu-id="70d43-157">Audio</span></span>
-   <span data-ttu-id="70d43-158">ビデオ</span><span class="sxs-lookup"><span data-stu-id="70d43-158">Video</span></span>
-   <span data-ttu-id="70d43-159">イメージ</span><span class="sxs-lookup"><span data-stu-id="70d43-159">Image</span></span>
-   <span data-ttu-id="70d43-160">Web</span><span class="sxs-lookup"><span data-stu-id="70d43-160">Web</span></span>
-   <span data-ttu-id="70d43-161">テキスト</span><span class="sxs-lookup"><span data-stu-id="70d43-161">Text</span></span>
-   <span data-ttu-id="70d43-162">Xml</span><span class="sxs-lookup"><span data-stu-id="70d43-162">Xml</span></span>
-   <span data-ttu-id="70d43-163">Story</span><span class="sxs-lookup"><span data-stu-id="70d43-163">Story</span></span>
-   <span data-ttu-id="70d43-164">externalcontent</span><span class="sxs-lookup"><span data-stu-id="70d43-164">ExternalContent</span></span>
-   <span data-ttu-id="70d43-165">フォルダー</span><span class="sxs-lookup"><span data-stu-id="70d43-165">Folder</span></span>
-   <span data-ttu-id="70d43-166">その他</span><span class="sxs-lookup"><span data-stu-id="70d43-166">Other</span></span>

<span data-ttu-id="70d43-167">クエリの例:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span><span class="sxs-lookup"><span data-stu-id="70d43-167">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span></span>

## <a name="containertype-property-values"></a><span data-ttu-id="70d43-168">containerType プロパティの値</span><span class="sxs-lookup"><span data-stu-id="70d43-168">containerType property values</span></span>
<span data-ttu-id="70d43-169">サポートされている種類は、[洞察](insights.md)がファイルを返すコンテナーによって異なる場合があります。</span><span class="sxs-lookup"><span data-stu-id="70d43-169">The supported types can differ based on containers from which the [Insight](insights.md) returns files.</span></span> <span data-ttu-id="70d43-170">たとえば、[共有](insights-shared.md)された洞察のみが、' DropBox '、' Box '、' gdrive ' からファイルを返します。</span><span class="sxs-lookup"><span data-stu-id="70d43-170">For example, only the [Shared](insights-shared.md) insight returns files from 'DropBox', 'Box', and 'GDrive'.</span></span>

-   <span data-ttu-id="70d43-171">onedrive business</span><span class="sxs-lookup"><span data-stu-id="70d43-171">OneDriveBusiness</span></span>
-   <span data-ttu-id="70d43-172">サイト</span><span class="sxs-lookup"><span data-stu-id="70d43-172">Site</span></span>
-   <span data-ttu-id="70d43-173">メール</span><span class="sxs-lookup"><span data-stu-id="70d43-173">Mail</span></span>
-   <span data-ttu-id="70d43-174">DropBox</span><span class="sxs-lookup"><span data-stu-id="70d43-174">DropBox</span></span>
-   <span data-ttu-id="70d43-175">検索ボックス</span><span class="sxs-lookup"><span data-stu-id="70d43-175">Box</span></span>
-   <span data-ttu-id="70d43-176">gdrive</span><span class="sxs-lookup"><span data-stu-id="70d43-176">GDrive</span></span>

<span data-ttu-id="70d43-177">クエリの例:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span><span class="sxs-lookup"><span data-stu-id="70d43-177">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-resourcevisualization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
