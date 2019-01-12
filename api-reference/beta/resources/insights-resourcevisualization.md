---
title: resourceVisualization リソースの種類
description: 複合型のプロパティ情報にはが含まれています。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: f8426d13968e5bea929c8e26f71346fa554a5242
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990657"
---
# <a name="resourcevisualization-resource-type"></a><span data-ttu-id="a4b68-103">resourceVisualization リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a4b68-103">resourceVisualization resource type</span></span>

> <span data-ttu-id="a4b68-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a4b68-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a4b68-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4b68-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a4b68-106">複合型のプロパティ[情報](insights.md)にはが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a4b68-106">Complex type containing properties of [Insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4b68-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a4b68-107">JSON representation</span></span>

<span data-ttu-id="a4b68-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="a4b68-108">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="a4b68-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4b68-109">Properties</span></span>

| <span data-ttu-id="a4b68-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4b68-110">Property</span></span>              | <span data-ttu-id="a4b68-111">型</span><span class="sxs-lookup"><span data-stu-id="a4b68-111">Type</span></span>          | <span data-ttu-id="a4b68-112">説明</span><span class="sxs-lookup"><span data-stu-id="a4b68-112">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="a4b68-113">タイトル</span><span class="sxs-lookup"><span data-stu-id="a4b68-113">title</span></span>                 | <span data-ttu-id="a4b68-114">String</span><span class="sxs-lookup"><span data-stu-id="a4b68-114">String</span></span>        | <span data-ttu-id="a4b68-115">アイテムのタイトルのテキストです。</span><span class="sxs-lookup"><span data-stu-id="a4b68-115">The item's title text.</span></span>               |
| <span data-ttu-id="a4b68-116">type</span><span class="sxs-lookup"><span data-stu-id="a4b68-116">type</span></span>              | <span data-ttu-id="a4b68-117">String</span><span class="sxs-lookup"><span data-stu-id="a4b68-117">String</span></span>        | <span data-ttu-id="a4b68-118">項目のメディア ・ タイプ。</span><span class="sxs-lookup"><span data-stu-id="a4b68-118">The item's media type.</span></span> <span data-ttu-id="a4b68-119">特定の種類に基づいて特定のファイルをフィルター処理するために使用できます。</span><span class="sxs-lookup"><span data-stu-id="a4b68-119">Can be used for filtering for a specific file based on a specific type.</span></span> <span data-ttu-id="a4b68-120">サポートされている型の下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a4b68-120">See below for supported types.</span></span> |
| <span data-ttu-id="a4b68-121">メディアの種類</span><span class="sxs-lookup"><span data-stu-id="a4b68-121">mediaType</span></span>             | <span data-ttu-id="a4b68-122">String</span><span class="sxs-lookup"><span data-stu-id="a4b68-122">String</span></span>        | <span data-ttu-id="a4b68-123">項目のメディア ・ タイプ。</span><span class="sxs-lookup"><span data-stu-id="a4b68-123">The item's media type.</span></span> <span data-ttu-id="a4b68-124">IANA メディアのサポートされている Mime の種類に基づいて、ファイルの特定の種類のフィルター処理に使用できます。</span><span class="sxs-lookup"><span data-stu-id="a4b68-124">Can be used for for filtering for a specific type of file based on supported IANA Media Mime Types.</span></span> <span data-ttu-id="a4b68-125">すべてのメディアの Mime タイプがサポートされていることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="a4b68-125">Note that not all Media Mime Types are supported.</span></span> |
| <span data-ttu-id="a4b68-126">previewImageUrl</span><span class="sxs-lookup"><span data-stu-id="a4b68-126">previewImageUrl</span></span>       | <span data-ttu-id="a4b68-127">String</span><span class="sxs-lookup"><span data-stu-id="a4b68-127">String</span></span>        | <span data-ttu-id="a4b68-128">先頭のアイテムのプレビュー イメージの URL です。</span><span class="sxs-lookup"><span data-stu-id="a4b68-128">A URL leading to the preview image for the item.</span></span> |
| <span data-ttu-id="a4b68-129">previewText</span><span class="sxs-lookup"><span data-stu-id="a4b68-129">previewText</span></span>           | <span data-ttu-id="a4b68-130">String</span><span class="sxs-lookup"><span data-stu-id="a4b68-130">String</span></span>        | <span data-ttu-id="a4b68-131">アイテムのプレビュー テキストです。</span><span class="sxs-lookup"><span data-stu-id="a4b68-131">A preview text for the item.</span></span> |
| <span data-ttu-id="a4b68-132">containerWebUrl</span><span class="sxs-lookup"><span data-stu-id="a4b68-132">containerWebUrl</span></span>       | <span data-ttu-id="a4b68-133">String</span><span class="sxs-lookup"><span data-stu-id="a4b68-133">String</span></span>        | <span data-ttu-id="a4b68-134">アイテムが格納されるフォルダーへのパスです。</span><span class="sxs-lookup"><span data-stu-id="a4b68-134">A path leading to the folder in which the item is stored.</span></span> |
| <span data-ttu-id="a4b68-135">containerDisplayName</span><span class="sxs-lookup"><span data-stu-id="a4b68-135">containerDisplayName</span></span>  | <span data-ttu-id="a4b68-136">String</span><span class="sxs-lookup"><span data-stu-id="a4b68-136">String</span></span>        | <span data-ttu-id="a4b68-137">アイテムを保存する場所を説明する文字列。</span><span class="sxs-lookup"><span data-stu-id="a4b68-137">A string describing where the item is stored.</span></span> <span data-ttu-id="a4b68-138">たとえば、SharePoint サイト、または項目を格納する OneDrive の所有者を識別するユーザー名の名前です。</span><span class="sxs-lookup"><span data-stu-id="a4b68-138">For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.</span></span>  |
| <span data-ttu-id="a4b68-139">コンテナー</span><span class="sxs-lookup"><span data-stu-id="a4b68-139">containerType</span></span>         | <span data-ttu-id="a4b68-140">String</span><span class="sxs-lookup"><span data-stu-id="a4b68-140">String</span></span> | <span data-ttu-id="a4b68-141">ファイルを格納するコンテナーの種類によってフィルター処理するために使用できます。</span><span class="sxs-lookup"><span data-stu-id="a4b68-141">Can be used for filtering by the type of container in which the file is stored.</span></span> <span data-ttu-id="a4b68-142">サイトなど OneDriveBusiness。</span><span class="sxs-lookup"><span data-stu-id="a4b68-142">Such as Site or OneDriveBusiness.</span></span>       |

## <a name="type-property-values"></a><span data-ttu-id="a4b68-143">プロパティ値の型</span><span class="sxs-lookup"><span data-stu-id="a4b68-143">Type property values</span></span>
-   <span data-ttu-id="a4b68-144">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="a4b68-144">PowerPoint</span></span>
-   <span data-ttu-id="a4b68-145">Word</span><span class="sxs-lookup"><span data-stu-id="a4b68-145">Word</span></span>
-   <span data-ttu-id="a4b68-146">Excel</span><span class="sxs-lookup"><span data-stu-id="a4b68-146">Excel</span></span>
-   <span data-ttu-id="a4b68-147">Pdf</span><span class="sxs-lookup"><span data-stu-id="a4b68-147">Pdf</span></span>
-   <span data-ttu-id="a4b68-148">OneNote</span><span class="sxs-lookup"><span data-stu-id="a4b68-148">OneNote</span></span>
-   <span data-ttu-id="a4b68-149">OneNotePage</span><span class="sxs-lookup"><span data-stu-id="a4b68-149">OneNotePage</span></span>
-   <span data-ttu-id="a4b68-150">InfoPath</span><span class="sxs-lookup"><span data-stu-id="a4b68-150">InfoPath</span></span>
-   <span data-ttu-id="a4b68-151">Visio</span><span class="sxs-lookup"><span data-stu-id="a4b68-151">Visio</span></span>
-   <span data-ttu-id="a4b68-152">Publisher</span><span class="sxs-lookup"><span data-stu-id="a4b68-152">Publisher</span></span>
-   <span data-ttu-id="a4b68-153">Project</span><span class="sxs-lookup"><span data-stu-id="a4b68-153">Project</span></span>
-   <span data-ttu-id="a4b68-154">Access</span><span class="sxs-lookup"><span data-stu-id="a4b68-154">Access</span></span>
-   <span data-ttu-id="a4b68-155">メール</span><span class="sxs-lookup"><span data-stu-id="a4b68-155">Mail</span></span>
-   <span data-ttu-id="a4b68-156">Csv</span><span class="sxs-lookup"><span data-stu-id="a4b68-156">Csv</span></span>
-   <span data-ttu-id="a4b68-157">アーカイブ</span><span class="sxs-lookup"><span data-stu-id="a4b68-157">Archive</span></span>
-   <span data-ttu-id="a4b68-158">Xps</span><span class="sxs-lookup"><span data-stu-id="a4b68-158">Xps</span></span>
-   <span data-ttu-id="a4b68-159">オーディオ</span><span class="sxs-lookup"><span data-stu-id="a4b68-159">Audio</span></span>
-   <span data-ttu-id="a4b68-160">ビデオ</span><span class="sxs-lookup"><span data-stu-id="a4b68-160">Video</span></span>
-   <span data-ttu-id="a4b68-161">イメージ</span><span class="sxs-lookup"><span data-stu-id="a4b68-161">Image</span></span>
-   <span data-ttu-id="a4b68-162">Web</span><span class="sxs-lookup"><span data-stu-id="a4b68-162">Web</span></span>
-   <span data-ttu-id="a4b68-163">テキスト</span><span class="sxs-lookup"><span data-stu-id="a4b68-163">Text</span></span>
-   <span data-ttu-id="a4b68-164">Xml</span><span class="sxs-lookup"><span data-stu-id="a4b68-164">Xml</span></span>
-   <span data-ttu-id="a4b68-165">Story</span><span class="sxs-lookup"><span data-stu-id="a4b68-165">Story</span></span>
-   <span data-ttu-id="a4b68-166">ExternalContent</span><span class="sxs-lookup"><span data-stu-id="a4b68-166">ExternalContent</span></span>
-   <span data-ttu-id="a4b68-167">フォルダー</span><span class="sxs-lookup"><span data-stu-id="a4b68-167">Folder</span></span>
-   <span data-ttu-id="a4b68-168">その他</span><span class="sxs-lookup"><span data-stu-id="a4b68-168">Other</span></span>

<span data-ttu-id="a4b68-169">クエリの例:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span><span class="sxs-lookup"><span data-stu-id="a4b68-169">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span></span>

## <a name="containertype-property-values"></a><span data-ttu-id="a4b68-170">コンテナーのプロパティの値</span><span class="sxs-lookup"><span data-stu-id="a4b68-170">containerType property values</span></span>
<span data-ttu-id="a4b68-171">サポートされている型が異なりますコンテナーの元となる[情報](insights.md)がファイルを返します。</span><span class="sxs-lookup"><span data-stu-id="a4b68-171">The supported types can differ based on containers from which the [Insight](insights.md) returns files.</span></span> <span data-ttu-id="a4b68-172">たとえば、のみ[共有](insights-shared.md)情報を得ることは、'ドロップ ボックス'、'ボックス'、および 'ください' からファイルを返します。</span><span class="sxs-lookup"><span data-stu-id="a4b68-172">For example, only the [Shared](insights-shared.md) insight returns files from 'DropBox', 'Box', and 'GDrive'.</span></span>

-   <span data-ttu-id="a4b68-173">OneDriveBusiness</span><span class="sxs-lookup"><span data-stu-id="a4b68-173">OneDriveBusiness</span></span>
-   <span data-ttu-id="a4b68-174">Site</span><span class="sxs-lookup"><span data-stu-id="a4b68-174">Site</span></span>
-   <span data-ttu-id="a4b68-175">メール</span><span class="sxs-lookup"><span data-stu-id="a4b68-175">Mail</span></span>
-   <span data-ttu-id="a4b68-176">ドロップ ボックス</span><span class="sxs-lookup"><span data-stu-id="a4b68-176">DropBox</span></span>
-   <span data-ttu-id="a4b68-177">ボックス</span><span class="sxs-lookup"><span data-stu-id="a4b68-177">Box</span></span>
-   <span data-ttu-id="a4b68-178">ください</span><span class="sxs-lookup"><span data-stu-id="a4b68-178">GDrive</span></span>

<span data-ttu-id="a4b68-179">クエリの例:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span><span class="sxs-lookup"><span data-stu-id="a4b68-179">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span></span>
