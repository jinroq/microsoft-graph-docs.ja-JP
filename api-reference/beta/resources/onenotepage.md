---
title: onenotePage リソースの種類
description: OneNote ノートブックのページ。
localization_priority: Normal
ms.openlocfilehash: 04e06fefd0b48a5d794f20733a4755e030cb7e0d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630798"
---
# <a name="onenotepage-resource-type"></a><span data-ttu-id="6eb22-103">onenotePage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6eb22-103">onenotePage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6eb22-104">OneNote ノートブックのページ。</span><span class="sxs-lookup"><span data-stu-id="6eb22-104">A page in a OneNote notebook.</span></span>

## <a name="properties"></a><span data-ttu-id="6eb22-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6eb22-105">Properties</span></span>
| <span data-ttu-id="6eb22-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6eb22-106">Property</span></span>     | <span data-ttu-id="6eb22-107">型</span><span class="sxs-lookup"><span data-stu-id="6eb22-107">Type</span></span>   |<span data-ttu-id="6eb22-108">説明</span><span class="sxs-lookup"><span data-stu-id="6eb22-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6eb22-109">content</span><span class="sxs-lookup"><span data-stu-id="6eb22-109">content</span></span>|<span data-ttu-id="6eb22-110">Stream</span><span class="sxs-lookup"><span data-stu-id="6eb22-110">Stream</span></span>|<span data-ttu-id="6eb22-111">ページの HTML コンテンツ。</span><span class="sxs-lookup"><span data-stu-id="6eb22-111">The page's HTML content.</span></span>|
|<span data-ttu-id="6eb22-112">contentUrl</span><span class="sxs-lookup"><span data-stu-id="6eb22-112">contentUrl</span></span>|<span data-ttu-id="6eb22-113">String</span><span class="sxs-lookup"><span data-stu-id="6eb22-113">String</span></span>|<span data-ttu-id="6eb22-114">ページの HTML コンテンツの URL。</span><span class="sxs-lookup"><span data-stu-id="6eb22-114">The URL for the page's HTML content.</span></span>  <span data-ttu-id="6eb22-115">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="6eb22-115">Read-only.</span></span>|
|<span data-ttu-id="6eb22-116">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="6eb22-116">createdByAppId</span></span>|<span data-ttu-id="6eb22-117">String</span><span class="sxs-lookup"><span data-stu-id="6eb22-117">String</span></span>|<span data-ttu-id="6eb22-118">ページを作成したアプリケーションの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="6eb22-118">The unique identifier of the application that created the page.</span></span> <span data-ttu-id="6eb22-119">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="6eb22-119">Read-only.</span></span>|
|<span data-ttu-id="6eb22-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6eb22-120">createdDateTime</span></span>|<span data-ttu-id="6eb22-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6eb22-121">DateTimeOffset</span></span>|<span data-ttu-id="6eb22-122">ページが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="6eb22-122">The date and time when the page was created.</span></span> <span data-ttu-id="6eb22-123">Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="6eb22-123">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6eb22-124">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="6eb22-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="6eb22-125">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6eb22-125">Read-only.</span></span>|
|<span data-ttu-id="6eb22-126">id</span><span class="sxs-lookup"><span data-stu-id="6eb22-126">id</span></span>|<span data-ttu-id="6eb22-127">文字列</span><span class="sxs-lookup"><span data-stu-id="6eb22-127">String</span></span>|<span data-ttu-id="6eb22-128">ページの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="6eb22-128">The unique identifier of the page.</span></span>  <span data-ttu-id="6eb22-129">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="6eb22-129">Read-only.</span></span>|
|<span data-ttu-id="6eb22-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6eb22-130">lastModifiedDateTime</span></span>|<span data-ttu-id="6eb22-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6eb22-131">DateTimeOffset</span></span>|<span data-ttu-id="6eb22-132">ページが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="6eb22-132">The date and time when the page was last modified.</span></span> <span data-ttu-id="6eb22-133">Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="6eb22-133">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6eb22-134">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="6eb22-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="6eb22-135">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6eb22-135">Read-only.</span></span>|
|<span data-ttu-id="6eb22-136">大まか</span><span class="sxs-lookup"><span data-stu-id="6eb22-136">level</span></span>|<span data-ttu-id="6eb22-137">Int32</span><span class="sxs-lookup"><span data-stu-id="6eb22-137">Int32</span></span>|<span data-ttu-id="6eb22-138">ページのインデントレベルを示します。</span><span class="sxs-lookup"><span data-stu-id="6eb22-138">The indentation level of the page.</span></span> <span data-ttu-id="6eb22-139">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6eb22-139">Read-only.</span></span>|
|<span data-ttu-id="6eb22-140">リンク</span><span class="sxs-lookup"><span data-stu-id="6eb22-140">links</span></span>|[<span data-ttu-id="6eb22-141">pageLinks</span><span class="sxs-lookup"><span data-stu-id="6eb22-141">pageLinks</span></span>](pagelinks.md)|<span data-ttu-id="6eb22-142">ページを開くためのリンク。</span><span class="sxs-lookup"><span data-stu-id="6eb22-142">Links for opening the page.</span></span> <span data-ttu-id="6eb22-143">この`oneNoteClientURL`リンクは、インストールされている場合は、OneNote native client でページを開きます。</span><span class="sxs-lookup"><span data-stu-id="6eb22-143">The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed.</span></span> <span data-ttu-id="6eb22-144">この`oneNoteWebUrl`リンクは、OneNote Online でページを開きます。</span><span class="sxs-lookup"><span data-stu-id="6eb22-144">The `oneNoteWebUrl` link opens the page in OneNote Online.</span></span> <span data-ttu-id="6eb22-145">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="6eb22-145">Read-only.</span></span>|
|<span data-ttu-id="6eb22-146">降順</span><span class="sxs-lookup"><span data-stu-id="6eb22-146">order</span></span>|<span data-ttu-id="6eb22-147">Int32</span><span class="sxs-lookup"><span data-stu-id="6eb22-147">Int32</span></span>|<span data-ttu-id="6eb22-148">親セクション内のページの順序。</span><span class="sxs-lookup"><span data-stu-id="6eb22-148">The order of the page within its parent section.</span></span> <span data-ttu-id="6eb22-149">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="6eb22-149">Read-only.</span></span>|
|<span data-ttu-id="6eb22-150">self</span><span class="sxs-lookup"><span data-stu-id="6eb22-150">self</span></span>|<span data-ttu-id="6eb22-151">String</span><span class="sxs-lookup"><span data-stu-id="6eb22-151">String</span></span>|<span data-ttu-id="6eb22-152">ページに関する詳細を取得できるエンドポイント。</span><span class="sxs-lookup"><span data-stu-id="6eb22-152">The endpoint where you can get details about the page.</span></span> <span data-ttu-id="6eb22-153">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="6eb22-153">Read-only.</span></span>|
|<span data-ttu-id="6eb22-154">title</span><span class="sxs-lookup"><span data-stu-id="6eb22-154">title</span></span>|<span data-ttu-id="6eb22-155">String</span><span class="sxs-lookup"><span data-stu-id="6eb22-155">String</span></span>|<span data-ttu-id="6eb22-156">ページのタイトル。</span><span class="sxs-lookup"><span data-stu-id="6eb22-156">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6eb22-157">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6eb22-157">Relationships</span></span>
| <span data-ttu-id="6eb22-158">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6eb22-158">Relationship</span></span> | <span data-ttu-id="6eb22-159">型</span><span class="sxs-lookup"><span data-stu-id="6eb22-159">Type</span></span>   |<span data-ttu-id="6eb22-160">説明</span><span class="sxs-lookup"><span data-stu-id="6eb22-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6eb22-161">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="6eb22-161">parentNotebook</span></span>|[<span data-ttu-id="6eb22-162">ノートブック</span><span class="sxs-lookup"><span data-stu-id="6eb22-162">notebook</span></span>](notebook.md)|<span data-ttu-id="6eb22-163">ページを含むノートブック。</span><span class="sxs-lookup"><span data-stu-id="6eb22-163">The notebook that contains the page.</span></span>  <span data-ttu-id="6eb22-164">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="6eb22-164">Read-only.</span></span>|
|<span data-ttu-id="6eb22-165">parentSection</span><span class="sxs-lookup"><span data-stu-id="6eb22-165">parentSection</span></span>|[<span data-ttu-id="6eb22-166">onenoteSection</span><span class="sxs-lookup"><span data-stu-id="6eb22-166">onenoteSection</span></span>](onenotesection.md)|<span data-ttu-id="6eb22-167">ページを含むセクション。</span><span class="sxs-lookup"><span data-stu-id="6eb22-167">The section that contains the page.</span></span> <span data-ttu-id="6eb22-168">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="6eb22-168">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="6eb22-169">メソッド</span><span class="sxs-lookup"><span data-stu-id="6eb22-169">Methods</span></span>

| <span data-ttu-id="6eb22-170">メソッド</span><span class="sxs-lookup"><span data-stu-id="6eb22-170">Method</span></span>           | <span data-ttu-id="6eb22-171">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6eb22-171">Return Type</span></span>    |<span data-ttu-id="6eb22-172">説明</span><span class="sxs-lookup"><span data-stu-id="6eb22-172">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6eb22-173">ページを取得する</span><span class="sxs-lookup"><span data-stu-id="6eb22-173">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="6eb22-174">onenotePage</span><span class="sxs-lookup"><span data-stu-id="6eb22-174">onenotePage</span></span>](onenotepage.md) |<span data-ttu-id="6eb22-175">ページのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6eb22-175">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="6eb22-176">ページ コンテンツを更新する</span><span class="sxs-lookup"><span data-stu-id="6eb22-176">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="6eb22-177">なし</span><span class="sxs-lookup"><span data-stu-id="6eb22-177">None</span></span> |<span data-ttu-id="6eb22-178">ページの HTML コンテンツを更新します。</span><span class="sxs-lookup"><span data-stu-id="6eb22-178">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="6eb22-179">ページの削除</span><span class="sxs-lookup"><span data-stu-id="6eb22-179">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="6eb22-180">なし</span><span class="sxs-lookup"><span data-stu-id="6eb22-180">None</span></span> |<span data-ttu-id="6eb22-181">ページを削除します。</span><span class="sxs-lookup"><span data-stu-id="6eb22-181">Delete the page.</span></span> |
|[<span data-ttu-id="6eb22-182">copyToSection</span><span class="sxs-lookup"><span data-stu-id="6eb22-182">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="6eb22-183">なし</span><span class="sxs-lookup"><span data-stu-id="6eb22-183">None</span></span> |<span data-ttu-id="6eb22-184">ページを特定のセクションにコピーします。</span><span class="sxs-lookup"><span data-stu-id="6eb22-184">Copies the page to a specific section.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6eb22-185">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6eb22-185">JSON representation</span></span>

<span data-ttu-id="6eb22-186">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6eb22-186">Here is a JSON representation of the resource.</span></span>

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
