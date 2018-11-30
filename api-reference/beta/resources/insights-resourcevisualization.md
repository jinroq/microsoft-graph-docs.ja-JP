---
title: resourceVisualization リソースの種類
description: 複合型のプロパティ情報にはが含まれています。
ms.openlocfilehash: 3ed61a8547e072938fc073d90f2592baf4c08fba
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071539"
---
# <a name="resourcevisualization-resource-type"></a><span data-ttu-id="bf7b1-103">resourceVisualization リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bf7b1-103">resourceVisualization resource type</span></span>

> <span data-ttu-id="bf7b1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bf7b1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf7b1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bf7b1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bf7b1-106">複合型のプロパティ[情報](insights.md)にはが含まれています。</span><span class="sxs-lookup"><span data-stu-id="bf7b1-106">Complex type containing properties of [Insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf7b1-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bf7b1-107">JSON representation</span></span>

<span data-ttu-id="bf7b1-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="bf7b1-108">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="bf7b1-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf7b1-109">Properties</span></span>

| <span data-ttu-id="bf7b1-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf7b1-110">Property</span></span>              | <span data-ttu-id="bf7b1-111">型</span><span class="sxs-lookup"><span data-stu-id="bf7b1-111">Type</span></span>          | <span data-ttu-id="bf7b1-112">説明</span><span class="sxs-lookup"><span data-stu-id="bf7b1-112">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="bf7b1-113">タイトル</span><span class="sxs-lookup"><span data-stu-id="bf7b1-113">title</span></span>                 | <span data-ttu-id="bf7b1-114">String</span><span class="sxs-lookup"><span data-stu-id="bf7b1-114">String</span></span>        | <span data-ttu-id="bf7b1-115">アイテムのタイトルのテキストです。</span><span class="sxs-lookup"><span data-stu-id="bf7b1-115">The item's title text.</span></span>               |
| <span data-ttu-id="bf7b1-116">type</span><span class="sxs-lookup"><span data-stu-id="bf7b1-116">type</span></span>              | <span data-ttu-id="bf7b1-117">String</span><span class="sxs-lookup"><span data-stu-id="bf7b1-117">String</span></span>        | <span data-ttu-id="bf7b1-118">項目のメディア ・ タイプ。</span><span class="sxs-lookup"><span data-stu-id="bf7b1-118">The item's media type.</span></span> <span data-ttu-id="bf7b1-119">特定の種類に基づいて特定のファイルをフィルター処理するために使用できます。</span><span class="sxs-lookup"><span data-stu-id="bf7b1-119">Can be used for filtering for a specific file based on a specific type.</span></span> <span data-ttu-id="bf7b1-120">サポートされている型の下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bf7b1-120">See below for supported types.</span></span> |
| <span data-ttu-id="bf7b1-121">メディアの種類</span><span class="sxs-lookup"><span data-stu-id="bf7b1-121">mediaType</span></span>             | <span data-ttu-id="bf7b1-122">String</span><span class="sxs-lookup"><span data-stu-id="bf7b1-122">String</span></span>        | <span data-ttu-id="bf7b1-123">項目のメディア ・ タイプ。</span><span class="sxs-lookup"><span data-stu-id="bf7b1-123">The item's media type.</span></span> <span data-ttu-id="bf7b1-124">IANA メディアのサポートされている Mime の種類に基づいて、ファイルの特定の種類のフィルター処理に使用できます。</span><span class="sxs-lookup"><span data-stu-id="bf7b1-124">Can be used for for filtering for a specific type of file based on supported IANA Media Mime Types.</span></span> <span data-ttu-id="bf7b1-125">すべてのメディアの Mime タイプがサポートされていることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="bf7b1-125">Note that not all Media Mime Types are supported.</span></span> |
| <span data-ttu-id="bf7b1-126">previewImageUrl</span><span class="sxs-lookup"><span data-stu-id="bf7b1-126">previewImageUrl</span></span>       | <span data-ttu-id="bf7b1-127">String</span><span class="sxs-lookup"><span data-stu-id="bf7b1-127">String</span></span>        | <span data-ttu-id="bf7b1-128">先頭のアイテムのプレビュー イメージの URL です。</span><span class="sxs-lookup"><span data-stu-id="bf7b1-128">A URL leading to the preview image for the item.</span></span> |
| <span data-ttu-id="bf7b1-129">previewText</span><span class="sxs-lookup"><span data-stu-id="bf7b1-129">previewText</span></span>           | <span data-ttu-id="bf7b1-130">String</span><span class="sxs-lookup"><span data-stu-id="bf7b1-130">String</span></span>        | <span data-ttu-id="bf7b1-131">アイテムのプレビュー テキストです。</span><span class="sxs-lookup"><span data-stu-id="bf7b1-131">A preview text for the item.</span></span> |
| <span data-ttu-id="bf7b1-132">containerWebUrl</span><span class="sxs-lookup"><span data-stu-id="bf7b1-132">containerWebUrl</span></span>       | <span data-ttu-id="bf7b1-133">String</span><span class="sxs-lookup"><span data-stu-id="bf7b1-133">String</span></span>        | <span data-ttu-id="bf7b1-134">アイテムが格納されるフォルダーへのパスです。</span><span class="sxs-lookup"><span data-stu-id="bf7b1-134">A path leading to the folder in which the item is stored.</span></span> |
| <span data-ttu-id="bf7b1-135">containerDisplayName</span><span class="sxs-lookup"><span data-stu-id="bf7b1-135">containerDisplayName</span></span>  | <span data-ttu-id="bf7b1-136">String</span><span class="sxs-lookup"><span data-stu-id="bf7b1-136">String</span></span>        | <span data-ttu-id="bf7b1-137">アイテムを保存する場所を説明する文字列。</span><span class="sxs-lookup"><span data-stu-id="bf7b1-137">A string describing where the item is stored.</span></span> <span data-ttu-id="bf7b1-138">たとえば、SharePoint サイト、または項目を格納する OneDrive の所有者を識別するユーザー名の名前です。</span><span class="sxs-lookup"><span data-stu-id="bf7b1-138">For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.</span></span>  |
| <span data-ttu-id="bf7b1-139">コンテナー</span><span class="sxs-lookup"><span data-stu-id="bf7b1-139">containerType</span></span>         | <span data-ttu-id="bf7b1-140">String</span><span class="sxs-lookup"><span data-stu-id="bf7b1-140">String</span></span> | <span data-ttu-id="bf7b1-141">ファイルを格納するコンテナーの種類によってフィルター処理するために使用できます。</span><span class="sxs-lookup"><span data-stu-id="bf7b1-141">Can be used for filtering by the type of container in which the file is stored.</span></span> <span data-ttu-id="bf7b1-142">サイトなど OneDriveBusiness。</span><span class="sxs-lookup"><span data-stu-id="bf7b1-142">Such as Site or OneDriveBusiness.</span></span>       |

## <a name="type-property-values"></a><span data-ttu-id="bf7b1-143">プロパティ値の型</span><span class="sxs-lookup"><span data-stu-id="bf7b1-143">Type property values</span></span>
-   <span data-ttu-id="bf7b1-144">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="bf7b1-144">PowerPoint</span></span>
-   <span data-ttu-id="bf7b1-145">Word</span><span class="sxs-lookup"><span data-stu-id="bf7b1-145">Word</span></span>
-   <span data-ttu-id="bf7b1-146">Excel</span><span class="sxs-lookup"><span data-stu-id="bf7b1-146">Excel</span></span>
-   <span data-ttu-id="bf7b1-147">Pdf</span><span class="sxs-lookup"><span data-stu-id="bf7b1-147">Pdf</span></span>
-   <span data-ttu-id="bf7b1-148">OneNote</span><span class="sxs-lookup"><span data-stu-id="bf7b1-148">OneNote</span></span>
-   <span data-ttu-id="bf7b1-149">OneNotePage</span><span class="sxs-lookup"><span data-stu-id="bf7b1-149">OneNotePage</span></span>
-   <span data-ttu-id="bf7b1-150">InfoPath</span><span class="sxs-lookup"><span data-stu-id="bf7b1-150">InfoPath</span></span>
-   <span data-ttu-id="bf7b1-151">Visio</span><span class="sxs-lookup"><span data-stu-id="bf7b1-151">Visio</span></span>
-   <span data-ttu-id="bf7b1-152">Publisher</span><span class="sxs-lookup"><span data-stu-id="bf7b1-152">Publisher</span></span>
-   <span data-ttu-id="bf7b1-153">プロジェクト</span><span class="sxs-lookup"><span data-stu-id="bf7b1-153">Project</span></span>
-   <span data-ttu-id="bf7b1-154">Access</span><span class="sxs-lookup"><span data-stu-id="bf7b1-154">Access</span></span>
-   <span data-ttu-id="bf7b1-155">メール</span><span class="sxs-lookup"><span data-stu-id="bf7b1-155">Mail</span></span>
-   <span data-ttu-id="bf7b1-156">Csv</span><span class="sxs-lookup"><span data-stu-id="bf7b1-156">Csv</span></span>
-   <span data-ttu-id="bf7b1-157">アーカイブ</span><span class="sxs-lookup"><span data-stu-id="bf7b1-157">Archive</span></span>
-   <span data-ttu-id="bf7b1-158">Xps</span><span class="sxs-lookup"><span data-stu-id="bf7b1-158">Xps</span></span>
-   <span data-ttu-id="bf7b1-159">オーディオ</span><span class="sxs-lookup"><span data-stu-id="bf7b1-159">Audio</span></span>
-   <span data-ttu-id="bf7b1-160">ビデオ</span><span class="sxs-lookup"><span data-stu-id="bf7b1-160">Video</span></span>
-   <span data-ttu-id="bf7b1-161">画像</span><span class="sxs-lookup"><span data-stu-id="bf7b1-161">Image</span></span>
-   <span data-ttu-id="bf7b1-162">Web</span><span class="sxs-lookup"><span data-stu-id="bf7b1-162">Web</span></span>
-   <span data-ttu-id="bf7b1-163">テキスト</span><span class="sxs-lookup"><span data-stu-id="bf7b1-163">Text</span></span>
-   <span data-ttu-id="bf7b1-164">Xml</span><span class="sxs-lookup"><span data-stu-id="bf7b1-164">Xml</span></span>
-   <span data-ttu-id="bf7b1-165">Story</span><span class="sxs-lookup"><span data-stu-id="bf7b1-165">Story</span></span>
-   <span data-ttu-id="bf7b1-166">ExternalContent</span><span class="sxs-lookup"><span data-stu-id="bf7b1-166">ExternalContent</span></span>
-   <span data-ttu-id="bf7b1-167">フォルダー</span><span class="sxs-lookup"><span data-stu-id="bf7b1-167">Folder</span></span>
-   <span data-ttu-id="bf7b1-168">その他</span><span class="sxs-lookup"><span data-stu-id="bf7b1-168">Other</span></span>

<span data-ttu-id="bf7b1-169">クエリの例:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span><span class="sxs-lookup"><span data-stu-id="bf7b1-169">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span></span>

## <a name="containertype-property-values"></a><span data-ttu-id="bf7b1-170">コンテナーのプロパティの値</span><span class="sxs-lookup"><span data-stu-id="bf7b1-170">containerType property values</span></span>
<span data-ttu-id="bf7b1-171">サポートされている型が異なりますコンテナーの元となる[情報](insights.md)がファイルを返します。</span><span class="sxs-lookup"><span data-stu-id="bf7b1-171">The supported types can differ based on containers from which the [Insight](insights.md) returns files.</span></span> <span data-ttu-id="bf7b1-172">たとえば、のみ[共有](insights-shared.md)情報を得ることは、'ドロップ ボックス'、'ボックス'、および 'ください' からファイルを返します。</span><span class="sxs-lookup"><span data-stu-id="bf7b1-172">For example, only the [Shared](insights-shared.md) insight returns files from 'DropBox', 'Box', and 'GDrive'.</span></span>

-   <span data-ttu-id="bf7b1-173">OneDriveBusiness</span><span class="sxs-lookup"><span data-stu-id="bf7b1-173">OneDriveBusiness</span></span>
-   <span data-ttu-id="bf7b1-174">サイト</span><span class="sxs-lookup"><span data-stu-id="bf7b1-174">Site</span></span>
-   <span data-ttu-id="bf7b1-175">メール</span><span class="sxs-lookup"><span data-stu-id="bf7b1-175">Mail</span></span>
-   <span data-ttu-id="bf7b1-176">ドロップ ボックス</span><span class="sxs-lookup"><span data-stu-id="bf7b1-176">DropBox</span></span>
-   <span data-ttu-id="bf7b1-177">ボックス</span><span class="sxs-lookup"><span data-stu-id="bf7b1-177">Box</span></span>
-   <span data-ttu-id="bf7b1-178">ください</span><span class="sxs-lookup"><span data-stu-id="bf7b1-178">GDrive</span></span>

<span data-ttu-id="bf7b1-179">クエリの例:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span><span class="sxs-lookup"><span data-stu-id="bf7b1-179">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span></span>