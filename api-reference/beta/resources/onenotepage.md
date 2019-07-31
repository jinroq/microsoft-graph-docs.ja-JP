---
title: onenotePage リソースの種類
description: OneNote ノートブックのページ。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3d43f517ec028534e9b443c6e6c6e3e667a09e43
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966420"
---
# <a name="onenotepage-resource-type"></a><span data-ttu-id="25255-103">onenotePage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="25255-103">onenotePage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25255-104">OneNote ノートブックのページ。</span><span class="sxs-lookup"><span data-stu-id="25255-104">A page in a OneNote notebook.</span></span>

## <a name="properties"></a><span data-ttu-id="25255-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="25255-105">Properties</span></span>
| <span data-ttu-id="25255-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="25255-106">Property</span></span>     | <span data-ttu-id="25255-107">型</span><span class="sxs-lookup"><span data-stu-id="25255-107">Type</span></span>   |<span data-ttu-id="25255-108">説明</span><span class="sxs-lookup"><span data-stu-id="25255-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="25255-109">content</span><span class="sxs-lookup"><span data-stu-id="25255-109">content</span></span>|<span data-ttu-id="25255-110">Stream</span><span class="sxs-lookup"><span data-stu-id="25255-110">Stream</span></span>|<span data-ttu-id="25255-111">ページの HTML コンテンツ。</span><span class="sxs-lookup"><span data-stu-id="25255-111">The page's HTML content.</span></span>|
|<span data-ttu-id="25255-112">contentUrl</span><span class="sxs-lookup"><span data-stu-id="25255-112">contentUrl</span></span>|<span data-ttu-id="25255-113">String</span><span class="sxs-lookup"><span data-stu-id="25255-113">String</span></span>|<span data-ttu-id="25255-114">ページの HTML コンテンツの URL。</span><span class="sxs-lookup"><span data-stu-id="25255-114">The URL for the page's HTML content.</span></span>  <span data-ttu-id="25255-115">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="25255-115">Read-only.</span></span>|
|<span data-ttu-id="25255-116">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="25255-116">createdByAppId</span></span>|<span data-ttu-id="25255-117">String</span><span class="sxs-lookup"><span data-stu-id="25255-117">String</span></span>|<span data-ttu-id="25255-118">ページを作成したアプリケーションの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="25255-118">The unique identifier of the application that created the page.</span></span> <span data-ttu-id="25255-119">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="25255-119">Read-only.</span></span>|
|<span data-ttu-id="25255-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="25255-120">createdDateTime</span></span>|<span data-ttu-id="25255-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25255-121">DateTimeOffset</span></span>|<span data-ttu-id="25255-122">ページが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="25255-122">The date and time when the page was created.</span></span> <span data-ttu-id="25255-123">Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="25255-123">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="25255-124">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="25255-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="25255-125">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="25255-125">Read-only.</span></span>|
|<span data-ttu-id="25255-126">id</span><span class="sxs-lookup"><span data-stu-id="25255-126">id</span></span>|<span data-ttu-id="25255-127">文字列</span><span class="sxs-lookup"><span data-stu-id="25255-127">String</span></span>|<span data-ttu-id="25255-128">ページの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="25255-128">The unique identifier of the page.</span></span>  <span data-ttu-id="25255-129">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="25255-129">Read-only.</span></span>|
|<span data-ttu-id="25255-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="25255-130">lastModifiedDateTime</span></span>|<span data-ttu-id="25255-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25255-131">DateTimeOffset</span></span>|<span data-ttu-id="25255-132">ページが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="25255-132">The date and time when the page was last modified.</span></span> <span data-ttu-id="25255-133">Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="25255-133">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="25255-134">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="25255-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="25255-135">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="25255-135">Read-only.</span></span>|
|<span data-ttu-id="25255-136">level</span><span class="sxs-lookup"><span data-stu-id="25255-136">level</span></span>|<span data-ttu-id="25255-137">Int32</span><span class="sxs-lookup"><span data-stu-id="25255-137">Int32</span></span>|<span data-ttu-id="25255-138">ページのインデントレベルを示します。</span><span class="sxs-lookup"><span data-stu-id="25255-138">The indentation level of the page.</span></span> <span data-ttu-id="25255-139">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="25255-139">Read-only.</span></span>|
|<span data-ttu-id="25255-140">リンク</span><span class="sxs-lookup"><span data-stu-id="25255-140">links</span></span>|[<span data-ttu-id="25255-141">pageLinks</span><span class="sxs-lookup"><span data-stu-id="25255-141">pageLinks</span></span>](pagelinks.md)|<span data-ttu-id="25255-142">ページを開くためのリンク。</span><span class="sxs-lookup"><span data-stu-id="25255-142">Links for opening the page.</span></span> <span data-ttu-id="25255-143">この`oneNoteClientURL`リンクは、インストールされている場合は、OneNote native client でページを開きます。</span><span class="sxs-lookup"><span data-stu-id="25255-143">The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed.</span></span> <span data-ttu-id="25255-144">リンク`oneNoteWebUrl`は、web 上の OneNote でページを開きます。</span><span class="sxs-lookup"><span data-stu-id="25255-144">The `oneNoteWebUrl` link opens the page in OneNote on the web.</span></span> <span data-ttu-id="25255-145">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="25255-145">Read-only.</span></span>|
|<span data-ttu-id="25255-146">降順</span><span class="sxs-lookup"><span data-stu-id="25255-146">order</span></span>|<span data-ttu-id="25255-147">Int32</span><span class="sxs-lookup"><span data-stu-id="25255-147">Int32</span></span>|<span data-ttu-id="25255-148">親セクション内のページの順序。</span><span class="sxs-lookup"><span data-stu-id="25255-148">The order of the page within its parent section.</span></span> <span data-ttu-id="25255-149">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="25255-149">Read-only.</span></span>|
|<span data-ttu-id="25255-150">self</span><span class="sxs-lookup"><span data-stu-id="25255-150">self</span></span>|<span data-ttu-id="25255-151">String</span><span class="sxs-lookup"><span data-stu-id="25255-151">String</span></span>|<span data-ttu-id="25255-152">ページに関する詳細を取得できるエンドポイント。</span><span class="sxs-lookup"><span data-stu-id="25255-152">The endpoint where you can get details about the page.</span></span> <span data-ttu-id="25255-153">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="25255-153">Read-only.</span></span>|
|<span data-ttu-id="25255-154">title</span><span class="sxs-lookup"><span data-stu-id="25255-154">title</span></span>|<span data-ttu-id="25255-155">String</span><span class="sxs-lookup"><span data-stu-id="25255-155">String</span></span>|<span data-ttu-id="25255-156">ページのタイトル。</span><span class="sxs-lookup"><span data-stu-id="25255-156">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="25255-157">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="25255-157">Relationships</span></span>
| <span data-ttu-id="25255-158">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="25255-158">Relationship</span></span> | <span data-ttu-id="25255-159">型</span><span class="sxs-lookup"><span data-stu-id="25255-159">Type</span></span>   |<span data-ttu-id="25255-160">説明</span><span class="sxs-lookup"><span data-stu-id="25255-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="25255-161">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="25255-161">parentNotebook</span></span>|[<span data-ttu-id="25255-162">ノートブック</span><span class="sxs-lookup"><span data-stu-id="25255-162">notebook</span></span>](notebook.md)|<span data-ttu-id="25255-163">ページを含むノートブック。</span><span class="sxs-lookup"><span data-stu-id="25255-163">The notebook that contains the page.</span></span>  <span data-ttu-id="25255-164">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="25255-164">Read-only.</span></span>|
|<span data-ttu-id="25255-165">parentSection</span><span class="sxs-lookup"><span data-stu-id="25255-165">parentSection</span></span>|[<span data-ttu-id="25255-166">onenoteSection</span><span class="sxs-lookup"><span data-stu-id="25255-166">onenoteSection</span></span>](onenotesection.md)|<span data-ttu-id="25255-167">ページを含むセクション。</span><span class="sxs-lookup"><span data-stu-id="25255-167">The section that contains the page.</span></span> <span data-ttu-id="25255-168">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="25255-168">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="25255-169">メソッド</span><span class="sxs-lookup"><span data-stu-id="25255-169">Methods</span></span>

| <span data-ttu-id="25255-170">メソッド</span><span class="sxs-lookup"><span data-stu-id="25255-170">Method</span></span>           | <span data-ttu-id="25255-171">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="25255-171">Return Type</span></span>    |<span data-ttu-id="25255-172">説明</span><span class="sxs-lookup"><span data-stu-id="25255-172">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="25255-173">ページを取得する</span><span class="sxs-lookup"><span data-stu-id="25255-173">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="25255-174">onenotePage</span><span class="sxs-lookup"><span data-stu-id="25255-174">onenotePage</span></span>](onenotepage.md) |<span data-ttu-id="25255-175">ページのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="25255-175">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="25255-176">ページ コンテンツを更新する</span><span class="sxs-lookup"><span data-stu-id="25255-176">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="25255-177">None</span><span class="sxs-lookup"><span data-stu-id="25255-177">None</span></span> |<span data-ttu-id="25255-178">ページの HTML コンテンツを更新します。</span><span class="sxs-lookup"><span data-stu-id="25255-178">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="25255-179">ページの削除</span><span class="sxs-lookup"><span data-stu-id="25255-179">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="25255-180">None</span><span class="sxs-lookup"><span data-stu-id="25255-180">None</span></span> |<span data-ttu-id="25255-181">ページを削除します。</span><span class="sxs-lookup"><span data-stu-id="25255-181">Delete the page.</span></span> |
|[<span data-ttu-id="25255-182">copyToSection</span><span class="sxs-lookup"><span data-stu-id="25255-182">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="25255-183">None</span><span class="sxs-lookup"><span data-stu-id="25255-183">None</span></span> |<span data-ttu-id="25255-184">ページを特定のセクションにコピーします。</span><span class="sxs-lookup"><span data-stu-id="25255-184">Copies the page to a specific section.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="25255-185">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="25255-185">JSON representation</span></span>

<span data-ttu-id="25255-186">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="25255-186">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "parentNotebook",
    "parentSection"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
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
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
