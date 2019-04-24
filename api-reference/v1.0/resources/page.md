---
title: page リソースの種類
description: OneNote ノートブックのページ。
localization_priority: Normal
ms.openlocfilehash: b7c92aaae401e022a79f7c3b72cb15b3093d0b7d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462551"
---
# <a name="page-resource-type"></a><span data-ttu-id="a42dd-103">page リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a42dd-103">page resource type</span></span>

<span data-ttu-id="a42dd-104">OneNote ノートブックのページ。</span><span class="sxs-lookup"><span data-stu-id="a42dd-104">A page in a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a42dd-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a42dd-105">JSON representation</span></span>

<span data-ttu-id="a42dd-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a42dd-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="a42dd-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a42dd-107">Properties</span></span>
| <span data-ttu-id="a42dd-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a42dd-108">Property</span></span>     | <span data-ttu-id="a42dd-109">型</span><span class="sxs-lookup"><span data-stu-id="a42dd-109">Type</span></span>   |<span data-ttu-id="a42dd-110">説明</span><span class="sxs-lookup"><span data-stu-id="a42dd-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a42dd-111">content</span><span class="sxs-lookup"><span data-stu-id="a42dd-111">content</span></span>|<span data-ttu-id="a42dd-112">Stream</span><span class="sxs-lookup"><span data-stu-id="a42dd-112">Stream</span></span>|<span data-ttu-id="a42dd-113">ページの HTML コンテンツ。</span><span class="sxs-lookup"><span data-stu-id="a42dd-113">The page's HTML content.</span></span>|
|<span data-ttu-id="a42dd-114">contentUrl</span><span class="sxs-lookup"><span data-stu-id="a42dd-114">contentUrl</span></span>|<span data-ttu-id="a42dd-115">String</span><span class="sxs-lookup"><span data-stu-id="a42dd-115">String</span></span>|<span data-ttu-id="a42dd-116">ページの HTML コンテンツの URL。</span><span class="sxs-lookup"><span data-stu-id="a42dd-116">The URL for the page's HTML content.</span></span>  <span data-ttu-id="a42dd-117">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a42dd-117">Read-only.</span></span>|
|<span data-ttu-id="a42dd-118">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="a42dd-118">createdByAppId</span></span>|<span data-ttu-id="a42dd-119">String</span><span class="sxs-lookup"><span data-stu-id="a42dd-119">String</span></span>|<span data-ttu-id="a42dd-120">ページを作成したアプリケーションの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="a42dd-120">The unique identifier of the application that created the page.</span></span> <span data-ttu-id="a42dd-121">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a42dd-121">Read-only.</span></span>|
|<span data-ttu-id="a42dd-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a42dd-122">createdDateTime</span></span>|<span data-ttu-id="a42dd-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a42dd-123">DateTimeOffset</span></span>|<span data-ttu-id="a42dd-124">ページが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="a42dd-124">The date and time when the page was created.</span></span> <span data-ttu-id="a42dd-125">Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="a42dd-125">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a42dd-126">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a42dd-126">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="a42dd-127">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a42dd-127">Read-only.</span></span>|
|<span data-ttu-id="a42dd-128">id</span><span class="sxs-lookup"><span data-stu-id="a42dd-128">id</span></span>|<span data-ttu-id="a42dd-129">String</span><span class="sxs-lookup"><span data-stu-id="a42dd-129">String</span></span>|<span data-ttu-id="a42dd-130">ページの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="a42dd-130">The unique identifier of the page.</span></span>  <span data-ttu-id="a42dd-131">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a42dd-131">Read-only.</span></span>|
|<span data-ttu-id="a42dd-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a42dd-132">lastModifiedDateTime</span></span>|<span data-ttu-id="a42dd-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a42dd-133">DateTimeOffset</span></span>|<span data-ttu-id="a42dd-134">ページが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="a42dd-134">The date and time when the page was last modified.</span></span> <span data-ttu-id="a42dd-135">Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="a42dd-135">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a42dd-136">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a42dd-136">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="a42dd-137">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a42dd-137">Read-only.</span></span>|
|<span data-ttu-id="a42dd-138">level</span><span class="sxs-lookup"><span data-stu-id="a42dd-138">level</span></span>|<span data-ttu-id="a42dd-139">Int32</span><span class="sxs-lookup"><span data-stu-id="a42dd-139">Int32</span></span>|<span data-ttu-id="a42dd-140">ページのインデントレベルを示します。</span><span class="sxs-lookup"><span data-stu-id="a42dd-140">The indentation level of the page.</span></span> <span data-ttu-id="a42dd-141">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a42dd-141">Read-only.</span></span>|
|<span data-ttu-id="a42dd-142">リンク</span><span class="sxs-lookup"><span data-stu-id="a42dd-142">links</span></span>|[<span data-ttu-id="a42dd-143">PageLinks</span><span class="sxs-lookup"><span data-stu-id="a42dd-143">PageLinks</span></span>](pagelinks.md)|<span data-ttu-id="a42dd-144">ページを開くためのリンク。</span><span class="sxs-lookup"><span data-stu-id="a42dd-144">Links for opening the page.</span></span> <span data-ttu-id="a42dd-145">この`oneNoteClientURL`リンクは、インストールされている場合は、OneNote native client でページを開きます。</span><span class="sxs-lookup"><span data-stu-id="a42dd-145">The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed.</span></span> <span data-ttu-id="a42dd-146">この`oneNoteWebUrl`リンクは、OneNote Online でページを開きます。</span><span class="sxs-lookup"><span data-stu-id="a42dd-146">The `oneNoteWebUrl` link opens the page in OneNote Online.</span></span> <span data-ttu-id="a42dd-147">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a42dd-147">Read-only.</span></span>|
|<span data-ttu-id="a42dd-148">降順</span><span class="sxs-lookup"><span data-stu-id="a42dd-148">order</span></span>|<span data-ttu-id="a42dd-149">Int32</span><span class="sxs-lookup"><span data-stu-id="a42dd-149">Int32</span></span>|<span data-ttu-id="a42dd-150">親セクション内のページの順序。</span><span class="sxs-lookup"><span data-stu-id="a42dd-150">The order of the page within its parent section.</span></span> <span data-ttu-id="a42dd-151">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a42dd-151">Read-only.</span></span>|
|<span data-ttu-id="a42dd-152">self</span><span class="sxs-lookup"><span data-stu-id="a42dd-152">self</span></span>|<span data-ttu-id="a42dd-153">String</span><span class="sxs-lookup"><span data-stu-id="a42dd-153">String</span></span>|<span data-ttu-id="a42dd-154">ページに関する詳細を取得できるエンドポイント。</span><span class="sxs-lookup"><span data-stu-id="a42dd-154">The endpoint where you can get details about the page.</span></span> <span data-ttu-id="a42dd-155">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a42dd-155">Read-only.</span></span>|
|<span data-ttu-id="a42dd-156">title</span><span class="sxs-lookup"><span data-stu-id="a42dd-156">title</span></span>|<span data-ttu-id="a42dd-157">String</span><span class="sxs-lookup"><span data-stu-id="a42dd-157">String</span></span>|<span data-ttu-id="a42dd-158">ページのタイトル。</span><span class="sxs-lookup"><span data-stu-id="a42dd-158">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a42dd-159">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a42dd-159">Relationships</span></span>
| <span data-ttu-id="a42dd-160">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a42dd-160">Relationship</span></span> | <span data-ttu-id="a42dd-161">型</span><span class="sxs-lookup"><span data-stu-id="a42dd-161">Type</span></span>   |<span data-ttu-id="a42dd-162">説明</span><span class="sxs-lookup"><span data-stu-id="a42dd-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a42dd-163">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="a42dd-163">parentNotebook</span></span>|[<span data-ttu-id="a42dd-164">Notebook</span><span class="sxs-lookup"><span data-stu-id="a42dd-164">Notebook</span></span>](notebook.md)|<span data-ttu-id="a42dd-165">ページを含むノートブック。</span><span class="sxs-lookup"><span data-stu-id="a42dd-165">The notebook that contains the page.</span></span>  <span data-ttu-id="a42dd-166">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a42dd-166">Read-only.</span></span>|
|<span data-ttu-id="a42dd-167">parentSection</span><span class="sxs-lookup"><span data-stu-id="a42dd-167">parentSection</span></span>|[<span data-ttu-id="a42dd-168">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="a42dd-168">OnenoteSection</span></span>](section.md)|<span data-ttu-id="a42dd-169">ページを含むセクション。</span><span class="sxs-lookup"><span data-stu-id="a42dd-169">The section that contains the page.</span></span> <span data-ttu-id="a42dd-170">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="a42dd-170">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="a42dd-171">メソッド</span><span class="sxs-lookup"><span data-stu-id="a42dd-171">Methods</span></span>

| <span data-ttu-id="a42dd-172">メソッド</span><span class="sxs-lookup"><span data-stu-id="a42dd-172">Method</span></span>           | <span data-ttu-id="a42dd-173">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a42dd-173">Return Type</span></span>    |<span data-ttu-id="a42dd-174">説明</span><span class="sxs-lookup"><span data-stu-id="a42dd-174">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a42dd-175">ページを取得する</span><span class="sxs-lookup"><span data-stu-id="a42dd-175">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="a42dd-176">Page</span><span class="sxs-lookup"><span data-stu-id="a42dd-176">Page</span></span>](page.md) |<span data-ttu-id="a42dd-177">ページのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a42dd-177">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="a42dd-178">ページ コンテンツを更新する</span><span class="sxs-lookup"><span data-stu-id="a42dd-178">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="a42dd-179">なし</span><span class="sxs-lookup"><span data-stu-id="a42dd-179">None</span></span> |<span data-ttu-id="a42dd-180">ページの HTML コンテンツを更新します。</span><span class="sxs-lookup"><span data-stu-id="a42dd-180">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="a42dd-181">ページの削除</span><span class="sxs-lookup"><span data-stu-id="a42dd-181">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="a42dd-182">なし</span><span class="sxs-lookup"><span data-stu-id="a42dd-182">None</span></span> |<span data-ttu-id="a42dd-183">ページを削除します。</span><span class="sxs-lookup"><span data-stu-id="a42dd-183">Delete the page.</span></span> |
|[<span data-ttu-id="a42dd-184">copyToSection</span><span class="sxs-lookup"><span data-stu-id="a42dd-184">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="a42dd-185">なし</span><span class="sxs-lookup"><span data-stu-id="a42dd-185">None</span></span> |<span data-ttu-id="a42dd-186">ページを特定のセクションにコピーします。</span><span class="sxs-lookup"><span data-stu-id="a42dd-186">Copies the page to a specific section.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
