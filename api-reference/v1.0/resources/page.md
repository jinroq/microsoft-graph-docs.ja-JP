---
title: page リソースの種類
description: OneNote ノートブックのページ。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 4a8ff5f6d0d9ed435d51d005df21a73bcb25a930
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035638"
---
# <a name="page-resource-type"></a><span data-ttu-id="96c43-103">page リソースの種類</span><span class="sxs-lookup"><span data-stu-id="96c43-103">page resource type</span></span>

<span data-ttu-id="96c43-104">OneNote ノートブックのページ。</span><span class="sxs-lookup"><span data-stu-id="96c43-104">A page in a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="96c43-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="96c43-105">JSON representation</span></span>

<span data-ttu-id="96c43-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="96c43-106">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntitySchemaObjectModel",
  "optionalProperties": [
    "parentNotebook",
    "parentSection"
  ],
  "isMediaEntity": true,
  "@odata.type": "microsoft.graph.onenotePage"
}-->

```json
{
  "content": "stream",
  "contentUrl": "string",
  "createdByAppId": "string",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "level": 1024,
  "links": {"@odata.type": "microsoft.graph.pageLinks"},
  "order": 1024,
  "self": "string",
  "title": "string"
}

```
## <a name="properties"></a><span data-ttu-id="96c43-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96c43-107">Properties</span></span>
| <span data-ttu-id="96c43-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96c43-108">Property</span></span>     | <span data-ttu-id="96c43-109">型</span><span class="sxs-lookup"><span data-stu-id="96c43-109">Type</span></span>   |<span data-ttu-id="96c43-110">説明</span><span class="sxs-lookup"><span data-stu-id="96c43-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="96c43-111">content</span><span class="sxs-lookup"><span data-stu-id="96c43-111">content</span></span>|<span data-ttu-id="96c43-112">Stream</span><span class="sxs-lookup"><span data-stu-id="96c43-112">Stream</span></span>|<span data-ttu-id="96c43-113">ページの HTML コンテンツ。</span><span class="sxs-lookup"><span data-stu-id="96c43-113">The page's HTML content.</span></span>|
|<span data-ttu-id="96c43-114">contentUrl</span><span class="sxs-lookup"><span data-stu-id="96c43-114">contentUrl</span></span>|<span data-ttu-id="96c43-115">String</span><span class="sxs-lookup"><span data-stu-id="96c43-115">String</span></span>|<span data-ttu-id="96c43-116">ページの HTML コンテンツの URL。</span><span class="sxs-lookup"><span data-stu-id="96c43-116">The URL for the page's HTML content.</span></span>  <span data-ttu-id="96c43-117">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="96c43-117">Read-only.</span></span>|
|<span data-ttu-id="96c43-118">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="96c43-118">createdByAppId</span></span>|<span data-ttu-id="96c43-119">String</span><span class="sxs-lookup"><span data-stu-id="96c43-119">String</span></span>|<span data-ttu-id="96c43-120">ページを作成したアプリケーションの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="96c43-120">The unique identifier of the application that created the page.</span></span> <span data-ttu-id="96c43-121">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="96c43-121">Read-only.</span></span>|
|<span data-ttu-id="96c43-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="96c43-122">createdDateTime</span></span>|<span data-ttu-id="96c43-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96c43-123">DateTimeOffset</span></span>|<span data-ttu-id="96c43-124">ページが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="96c43-124">The date and time when the page was created.</span></span> <span data-ttu-id="96c43-125">Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="96c43-125">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="96c43-126">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="96c43-126">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="96c43-127">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="96c43-127">Read-only.</span></span>|
|<span data-ttu-id="96c43-128">id</span><span class="sxs-lookup"><span data-stu-id="96c43-128">id</span></span>|<span data-ttu-id="96c43-129">文字列</span><span class="sxs-lookup"><span data-stu-id="96c43-129">String</span></span>|<span data-ttu-id="96c43-130">ページの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="96c43-130">The unique identifier of the page.</span></span>  <span data-ttu-id="96c43-131">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="96c43-131">Read-only.</span></span>|
|<span data-ttu-id="96c43-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="96c43-132">lastModifiedDateTime</span></span>|<span data-ttu-id="96c43-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96c43-133">DateTimeOffset</span></span>|<span data-ttu-id="96c43-134">ページが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="96c43-134">The date and time when the page was last modified.</span></span> <span data-ttu-id="96c43-135">Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="96c43-135">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="96c43-136">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="96c43-136">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="96c43-137">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="96c43-137">Read-only.</span></span>|
|<span data-ttu-id="96c43-138">level</span><span class="sxs-lookup"><span data-stu-id="96c43-138">level</span></span>|<span data-ttu-id="96c43-139">Int32</span><span class="sxs-lookup"><span data-stu-id="96c43-139">Int32</span></span>|<span data-ttu-id="96c43-140">ページのインデントレベルを示します。</span><span class="sxs-lookup"><span data-stu-id="96c43-140">The indentation level of the page.</span></span> <span data-ttu-id="96c43-141">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="96c43-141">Read-only.</span></span>|
|<span data-ttu-id="96c43-142">リンク</span><span class="sxs-lookup"><span data-stu-id="96c43-142">links</span></span>|[<span data-ttu-id="96c43-143">PageLinks</span><span class="sxs-lookup"><span data-stu-id="96c43-143">PageLinks</span></span>](pagelinks.md)|<span data-ttu-id="96c43-144">ページを開くためのリンク。</span><span class="sxs-lookup"><span data-stu-id="96c43-144">Links for opening the page.</span></span> <span data-ttu-id="96c43-145">この`oneNoteClientURL`リンクは、インストールされている場合は、OneNote native client でページを開きます。</span><span class="sxs-lookup"><span data-stu-id="96c43-145">The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed.</span></span> <span data-ttu-id="96c43-146">リンク`oneNoteWebUrl`は、web 上の OneNote でページを開きます。</span><span class="sxs-lookup"><span data-stu-id="96c43-146">The `oneNoteWebUrl` link opens the page in OneNote on the web.</span></span> <span data-ttu-id="96c43-147">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="96c43-147">Read-only.</span></span>|
|<span data-ttu-id="96c43-148">降順</span><span class="sxs-lookup"><span data-stu-id="96c43-148">order</span></span>|<span data-ttu-id="96c43-149">Int32</span><span class="sxs-lookup"><span data-stu-id="96c43-149">Int32</span></span>|<span data-ttu-id="96c43-150">親セクション内のページの順序。</span><span class="sxs-lookup"><span data-stu-id="96c43-150">The order of the page within its parent section.</span></span> <span data-ttu-id="96c43-151">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="96c43-151">Read-only.</span></span>|
|<span data-ttu-id="96c43-152">self</span><span class="sxs-lookup"><span data-stu-id="96c43-152">self</span></span>|<span data-ttu-id="96c43-153">String</span><span class="sxs-lookup"><span data-stu-id="96c43-153">String</span></span>|<span data-ttu-id="96c43-154">ページに関する詳細を取得できるエンドポイント。</span><span class="sxs-lookup"><span data-stu-id="96c43-154">The endpoint where you can get details about the page.</span></span> <span data-ttu-id="96c43-155">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="96c43-155">Read-only.</span></span>|
|<span data-ttu-id="96c43-156">title</span><span class="sxs-lookup"><span data-stu-id="96c43-156">title</span></span>|<span data-ttu-id="96c43-157">String</span><span class="sxs-lookup"><span data-stu-id="96c43-157">String</span></span>|<span data-ttu-id="96c43-158">ページのタイトル。</span><span class="sxs-lookup"><span data-stu-id="96c43-158">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="96c43-159">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="96c43-159">Relationships</span></span>
| <span data-ttu-id="96c43-160">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="96c43-160">Relationship</span></span> | <span data-ttu-id="96c43-161">型</span><span class="sxs-lookup"><span data-stu-id="96c43-161">Type</span></span>   |<span data-ttu-id="96c43-162">説明</span><span class="sxs-lookup"><span data-stu-id="96c43-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="96c43-163">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="96c43-163">parentNotebook</span></span>|[<span data-ttu-id="96c43-164">Notebook</span><span class="sxs-lookup"><span data-stu-id="96c43-164">Notebook</span></span>](notebook.md)|<span data-ttu-id="96c43-165">ページを含むノートブック。</span><span class="sxs-lookup"><span data-stu-id="96c43-165">The notebook that contains the page.</span></span>  <span data-ttu-id="96c43-166">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="96c43-166">Read-only.</span></span>|
|<span data-ttu-id="96c43-167">parentSection</span><span class="sxs-lookup"><span data-stu-id="96c43-167">parentSection</span></span>|[<span data-ttu-id="96c43-168">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="96c43-168">OnenoteSection</span></span>](section.md)|<span data-ttu-id="96c43-169">ページを含むセクション。</span><span class="sxs-lookup"><span data-stu-id="96c43-169">The section that contains the page.</span></span> <span data-ttu-id="96c43-170">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="96c43-170">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="96c43-171">メソッド</span><span class="sxs-lookup"><span data-stu-id="96c43-171">Methods</span></span>

| <span data-ttu-id="96c43-172">メソッド</span><span class="sxs-lookup"><span data-stu-id="96c43-172">Method</span></span>           | <span data-ttu-id="96c43-173">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="96c43-173">Return Type</span></span>    |<span data-ttu-id="96c43-174">説明</span><span class="sxs-lookup"><span data-stu-id="96c43-174">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="96c43-175">ページを取得する</span><span class="sxs-lookup"><span data-stu-id="96c43-175">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="96c43-176">Page</span><span class="sxs-lookup"><span data-stu-id="96c43-176">Page</span></span>](page.md) |<span data-ttu-id="96c43-177">ページのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="96c43-177">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="96c43-178">ページ コンテンツを更新する</span><span class="sxs-lookup"><span data-stu-id="96c43-178">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="96c43-179">None</span><span class="sxs-lookup"><span data-stu-id="96c43-179">None</span></span> |<span data-ttu-id="96c43-180">ページの HTML コンテンツを更新します。</span><span class="sxs-lookup"><span data-stu-id="96c43-180">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="96c43-181">ページの削除</span><span class="sxs-lookup"><span data-stu-id="96c43-181">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="96c43-182">None</span><span class="sxs-lookup"><span data-stu-id="96c43-182">None</span></span> |<span data-ttu-id="96c43-183">ページを削除します。</span><span class="sxs-lookup"><span data-stu-id="96c43-183">Delete the page.</span></span> |
|[<span data-ttu-id="96c43-184">copyToSection</span><span class="sxs-lookup"><span data-stu-id="96c43-184">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="96c43-185">None</span><span class="sxs-lookup"><span data-stu-id="96c43-185">None</span></span> |<span data-ttu-id="96c43-186">ページを特定のセクションにコピーします。</span><span class="sxs-lookup"><span data-stu-id="96c43-186">Copies the page to a specific section.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
