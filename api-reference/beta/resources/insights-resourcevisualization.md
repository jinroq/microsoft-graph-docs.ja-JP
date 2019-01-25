---
title: resourceVisualization リソースの種類
description: 複合型のプロパティ情報にはが含まれています。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 48ec1619d07d0f31bf8325c25b161084f505b3ee
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526761"
---
# <a name="resourcevisualization-resource-type"></a><span data-ttu-id="48e95-103">resourceVisualization リソースの種類</span><span class="sxs-lookup"><span data-stu-id="48e95-103">resourceVisualization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48e95-104">複合型のプロパティ[情報](insights.md)にはが含まれています。</span><span class="sxs-lookup"><span data-stu-id="48e95-104">Complex type containing properties of [Insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="48e95-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="48e95-105">JSON representation</span></span>

<span data-ttu-id="48e95-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="48e95-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="48e95-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="48e95-107">Properties</span></span>

| <span data-ttu-id="48e95-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="48e95-108">Property</span></span>              | <span data-ttu-id="48e95-109">型</span><span class="sxs-lookup"><span data-stu-id="48e95-109">Type</span></span>          | <span data-ttu-id="48e95-110">説明</span><span class="sxs-lookup"><span data-stu-id="48e95-110">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="48e95-111">タイトル</span><span class="sxs-lookup"><span data-stu-id="48e95-111">title</span></span>                 | <span data-ttu-id="48e95-112">String</span><span class="sxs-lookup"><span data-stu-id="48e95-112">String</span></span>        | <span data-ttu-id="48e95-113">アイテムのタイトルのテキストです。</span><span class="sxs-lookup"><span data-stu-id="48e95-113">The item's title text.</span></span>               |
| <span data-ttu-id="48e95-114">type</span><span class="sxs-lookup"><span data-stu-id="48e95-114">type</span></span>              | <span data-ttu-id="48e95-115">String</span><span class="sxs-lookup"><span data-stu-id="48e95-115">String</span></span>        | <span data-ttu-id="48e95-116">項目のメディア ・ タイプ。</span><span class="sxs-lookup"><span data-stu-id="48e95-116">The item's media type.</span></span> <span data-ttu-id="48e95-117">特定の種類に基づいて特定のファイルをフィルター処理するために使用できます。</span><span class="sxs-lookup"><span data-stu-id="48e95-117">Can be used for filtering for a specific file based on a specific type.</span></span> <span data-ttu-id="48e95-118">サポートされている型の下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="48e95-118">See below for supported types.</span></span> |
| <span data-ttu-id="48e95-119">MediaType</span><span class="sxs-lookup"><span data-stu-id="48e95-119">mediaType</span></span>             | <span data-ttu-id="48e95-120">String</span><span class="sxs-lookup"><span data-stu-id="48e95-120">String</span></span>        | <span data-ttu-id="48e95-121">項目のメディア ・ タイプ。</span><span class="sxs-lookup"><span data-stu-id="48e95-121">The item's media type.</span></span> <span data-ttu-id="48e95-122">IANA メディアのサポートされている Mime の種類に基づいて、ファイルの特定の種類のフィルター処理に使用できます。</span><span class="sxs-lookup"><span data-stu-id="48e95-122">Can be used for for filtering for a specific type of file based on supported IANA Media Mime Types.</span></span> <span data-ttu-id="48e95-123">すべてのメディアの Mime タイプがサポートされていることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="48e95-123">Note that not all Media Mime Types are supported.</span></span> |
| <span data-ttu-id="48e95-124">PreviewImageUrl</span><span class="sxs-lookup"><span data-stu-id="48e95-124">previewImageUrl</span></span>       | <span data-ttu-id="48e95-125">String</span><span class="sxs-lookup"><span data-stu-id="48e95-125">String</span></span>        | <span data-ttu-id="48e95-126">先頭のアイテムのプレビュー イメージの URL です。</span><span class="sxs-lookup"><span data-stu-id="48e95-126">A URL leading to the preview image for the item.</span></span> |
| <span data-ttu-id="48e95-127">previewText</span><span class="sxs-lookup"><span data-stu-id="48e95-127">previewText</span></span>           | <span data-ttu-id="48e95-128">String</span><span class="sxs-lookup"><span data-stu-id="48e95-128">String</span></span>        | <span data-ttu-id="48e95-129">アイテムのプレビュー テキストです。</span><span class="sxs-lookup"><span data-stu-id="48e95-129">A preview text for the item.</span></span> |
| <span data-ttu-id="48e95-130">containerWebUrl</span><span class="sxs-lookup"><span data-stu-id="48e95-130">containerWebUrl</span></span>       | <span data-ttu-id="48e95-131">String</span><span class="sxs-lookup"><span data-stu-id="48e95-131">String</span></span>        | <span data-ttu-id="48e95-132">アイテムが格納されるフォルダーへのパスです。</span><span class="sxs-lookup"><span data-stu-id="48e95-132">A path leading to the folder in which the item is stored.</span></span> |
| <span data-ttu-id="48e95-133">containerDisplayName</span><span class="sxs-lookup"><span data-stu-id="48e95-133">containerDisplayName</span></span>  | <span data-ttu-id="48e95-134">String</span><span class="sxs-lookup"><span data-stu-id="48e95-134">String</span></span>        | <span data-ttu-id="48e95-135">アイテムを保存する場所を説明する文字列。</span><span class="sxs-lookup"><span data-stu-id="48e95-135">A string describing where the item is stored.</span></span> <span data-ttu-id="48e95-136">たとえば、SharePoint サイト、または項目を格納する OneDrive の所有者を識別するユーザー名の名前です。</span><span class="sxs-lookup"><span data-stu-id="48e95-136">For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.</span></span>  |
| <span data-ttu-id="48e95-137">ContainerType</span><span class="sxs-lookup"><span data-stu-id="48e95-137">containerType</span></span>         | <span data-ttu-id="48e95-138">String</span><span class="sxs-lookup"><span data-stu-id="48e95-138">String</span></span> | <span data-ttu-id="48e95-139">ファイルを格納するコンテナーの種類によってフィルター処理するために使用できます。</span><span class="sxs-lookup"><span data-stu-id="48e95-139">Can be used for filtering by the type of container in which the file is stored.</span></span> <span data-ttu-id="48e95-140">サイトなど OneDriveBusiness。</span><span class="sxs-lookup"><span data-stu-id="48e95-140">Such as Site or OneDriveBusiness.</span></span>       |

## <a name="type-property-values"></a><span data-ttu-id="48e95-141">プロパティ値の型</span><span class="sxs-lookup"><span data-stu-id="48e95-141">Type property values</span></span>
-   <span data-ttu-id="48e95-142">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="48e95-142">PowerPoint</span></span>
-   <span data-ttu-id="48e95-143">Word</span><span class="sxs-lookup"><span data-stu-id="48e95-143">Word</span></span>
-   <span data-ttu-id="48e95-144">Excel</span><span class="sxs-lookup"><span data-stu-id="48e95-144">Excel</span></span>
-   <span data-ttu-id="48e95-145">PDF</span><span class="sxs-lookup"><span data-stu-id="48e95-145">Pdf</span></span>
-   <span data-ttu-id="48e95-146">OneNote</span><span class="sxs-lookup"><span data-stu-id="48e95-146">OneNote</span></span>
-   <span data-ttu-id="48e95-147">OneNotePage</span><span class="sxs-lookup"><span data-stu-id="48e95-147">OneNotePage</span></span>
-   <span data-ttu-id="48e95-148">InfoPath</span><span class="sxs-lookup"><span data-stu-id="48e95-148">InfoPath</span></span>
-   <span data-ttu-id="48e95-149">Visio</span><span class="sxs-lookup"><span data-stu-id="48e95-149">Visio</span></span>
-   <span data-ttu-id="48e95-150">Publisher</span><span class="sxs-lookup"><span data-stu-id="48e95-150">Publisher</span></span>
-   <span data-ttu-id="48e95-151">Project</span><span class="sxs-lookup"><span data-stu-id="48e95-151">Project</span></span>
-   <span data-ttu-id="48e95-152">Access</span><span class="sxs-lookup"><span data-stu-id="48e95-152">Access</span></span>
-   <span data-ttu-id="48e95-153">メール</span><span class="sxs-lookup"><span data-stu-id="48e95-153">Mail</span></span>
-   <span data-ttu-id="48e95-154">\*.csv</span><span class="sxs-lookup"><span data-stu-id="48e95-154">Csv</span></span>
-   <span data-ttu-id="48e95-155">アーカイブ</span><span class="sxs-lookup"><span data-stu-id="48e95-155">Archive</span></span>
-   <span data-ttu-id="48e95-156">Xps</span><span class="sxs-lookup"><span data-stu-id="48e95-156">Xps</span></span>
-   <span data-ttu-id="48e95-157">オーディオ</span><span class="sxs-lookup"><span data-stu-id="48e95-157">Audio</span></span>
-   <span data-ttu-id="48e95-158">ビデオ</span><span class="sxs-lookup"><span data-stu-id="48e95-158">Video</span></span>
-   <span data-ttu-id="48e95-159">画像</span><span class="sxs-lookup"><span data-stu-id="48e95-159">Image</span></span>
-   <span data-ttu-id="48e95-160">Web</span><span class="sxs-lookup"><span data-stu-id="48e95-160">Web</span></span>
-   <span data-ttu-id="48e95-161">テキスト</span><span class="sxs-lookup"><span data-stu-id="48e95-161">Text</span></span>
-   <span data-ttu-id="48e95-162">Xml</span><span class="sxs-lookup"><span data-stu-id="48e95-162">Xml</span></span>
-   <span data-ttu-id="48e95-163">Story</span><span class="sxs-lookup"><span data-stu-id="48e95-163">Story</span></span>
-   <span data-ttu-id="48e95-164">ExternalContent</span><span class="sxs-lookup"><span data-stu-id="48e95-164">ExternalContent</span></span>
-   <span data-ttu-id="48e95-165">フォルダー</span><span class="sxs-lookup"><span data-stu-id="48e95-165">Folder</span></span>
-   <span data-ttu-id="48e95-166">Other</span><span class="sxs-lookup"><span data-stu-id="48e95-166">Other</span></span>

<span data-ttu-id="48e95-167">クエリの例:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span><span class="sxs-lookup"><span data-stu-id="48e95-167">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span></span>

## <a name="containertype-property-values"></a><span data-ttu-id="48e95-168">コンテナーのプロパティの値</span><span class="sxs-lookup"><span data-stu-id="48e95-168">containerType property values</span></span>
<span data-ttu-id="48e95-169">サポートされている型が異なりますコンテナーの元となる[情報](insights.md)がファイルを返します。</span><span class="sxs-lookup"><span data-stu-id="48e95-169">The supported types can differ based on containers from which the [Insight](insights.md) returns files.</span></span> <span data-ttu-id="48e95-170">たとえば、のみ[共有](insights-shared.md)情報を得ることは、'ドロップ ボックス'、'ボックス'、および 'ください' からファイルを返します。</span><span class="sxs-lookup"><span data-stu-id="48e95-170">For example, only the [Shared](insights-shared.md) insight returns files from 'DropBox', 'Box', and 'GDrive'.</span></span>

-   <span data-ttu-id="48e95-171">OneDriveBusiness</span><span class="sxs-lookup"><span data-stu-id="48e95-171">OneDriveBusiness</span></span>
-   <span data-ttu-id="48e95-172">Site</span><span class="sxs-lookup"><span data-stu-id="48e95-172">Site</span></span>
-   <span data-ttu-id="48e95-173">メール</span><span class="sxs-lookup"><span data-stu-id="48e95-173">Mail</span></span>
-   <span data-ttu-id="48e95-174">Dropbox</span><span class="sxs-lookup"><span data-stu-id="48e95-174">DropBox</span></span>
-   <span data-ttu-id="48e95-175">ボックス</span><span class="sxs-lookup"><span data-stu-id="48e95-175">Box</span></span>
-   <span data-ttu-id="48e95-176">ください</span><span class="sxs-lookup"><span data-stu-id="48e95-176">GDrive</span></span>

<span data-ttu-id="48e95-177">クエリの例:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span><span class="sxs-lookup"><span data-stu-id="48e95-177">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-resourcevisualization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
