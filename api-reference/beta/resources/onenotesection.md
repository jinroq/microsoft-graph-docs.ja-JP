---
title: onenoteSection リソースの種類
description: OneNote ノートブックのセクション。 セクションには、ページを含めることができます。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ed90d29e0441544bffd2576a255acf17e6cb3996
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966404"
---
# <a name="onenotesection-resource-type"></a><span data-ttu-id="96b65-104">onenoteSection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="96b65-104">onenoteSection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96b65-105">OneNote ノートブックのセクション。</span><span class="sxs-lookup"><span data-stu-id="96b65-105">A section in a OneNote notebook.</span></span> <span data-ttu-id="96b65-106">セクションには、ページを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="96b65-106">Sections can contain pages.</span></span>

## <a name="properties"></a><span data-ttu-id="96b65-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96b65-107">Properties</span></span>
| <span data-ttu-id="96b65-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96b65-108">Property</span></span>     | <span data-ttu-id="96b65-109">型</span><span class="sxs-lookup"><span data-stu-id="96b65-109">Type</span></span>   |<span data-ttu-id="96b65-110">説明</span><span class="sxs-lookup"><span data-stu-id="96b65-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="96b65-111">createdBy</span><span class="sxs-lookup"><span data-stu-id="96b65-111">createdBy</span></span>|[<span data-ttu-id="96b65-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="96b65-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="96b65-p103">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="96b65-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="96b65-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="96b65-115">createdDateTime</span></span>|<span data-ttu-id="96b65-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96b65-116">DateTimeOffset</span></span>|<span data-ttu-id="96b65-117">セクションが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="96b65-117">The date and time when the section was created.</span></span> <span data-ttu-id="96b65-118">Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="96b65-118">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="96b65-119">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="96b65-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="96b65-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="96b65-120">Read-only.</span></span>|
|<span data-ttu-id="96b65-121">id</span><span class="sxs-lookup"><span data-stu-id="96b65-121">id</span></span>|<span data-ttu-id="96b65-122">文字列</span><span class="sxs-lookup"><span data-stu-id="96b65-122">String</span></span>|<span data-ttu-id="96b65-123">セクションの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="96b65-123">The unique identifier of the section.</span></span>  <span data-ttu-id="96b65-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="96b65-124">Read-only.</span></span>|
|<span data-ttu-id="96b65-125">isDefault</span><span class="sxs-lookup"><span data-stu-id="96b65-125">isDefault</span></span>|<span data-ttu-id="96b65-126">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="96b65-126">Boolean</span></span>|<span data-ttu-id="96b65-127">これがユーザーの既定のセクションであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="96b65-127">Indicates whether this is the user's default section.</span></span> <span data-ttu-id="96b65-128">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="96b65-128">Read-only.</span></span>|
|<span data-ttu-id="96b65-129">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="96b65-129">lastModifiedBy</span></span>|[<span data-ttu-id="96b65-130">identitySet</span><span class="sxs-lookup"><span data-stu-id="96b65-130">identitySet</span></span>](identityset.md)|<span data-ttu-id="96b65-p107">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="96b65-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="96b65-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="96b65-133">lastModifiedDateTime</span></span>|<span data-ttu-id="96b65-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96b65-134">DateTimeOffset</span></span>|<span data-ttu-id="96b65-135">セクションが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="96b65-135">The date and time when the section was last modified.</span></span> <span data-ttu-id="96b65-136">Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="96b65-136">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="96b65-137">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="96b65-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="96b65-138">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="96b65-138">Read-only.</span></span>|
|<span data-ttu-id="96b65-139">リンク</span><span class="sxs-lookup"><span data-stu-id="96b65-139">links</span></span>|[<span data-ttu-id="96b65-140">sectionLinks</span><span class="sxs-lookup"><span data-stu-id="96b65-140">sectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="96b65-141">セクションを開くためのリンク。</span><span class="sxs-lookup"><span data-stu-id="96b65-141">Links for opening the section.</span></span> <span data-ttu-id="96b65-142">リンク`oneNoteClientURL`によって、OneNote native client のセクションがインストールされている場合は、そのセクションが開きます。</span><span class="sxs-lookup"><span data-stu-id="96b65-142">The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed.</span></span> <span data-ttu-id="96b65-143">リンク`oneNoteWebURL`は、web 上の OneNote でセクションを開きます。</span><span class="sxs-lookup"><span data-stu-id="96b65-143">The `oneNoteWebURL` link opens the section in OneNote on the web.</span></span>|
|<span data-ttu-id="96b65-144">displayName</span><span class="sxs-lookup"><span data-stu-id="96b65-144">displayName</span></span>|<span data-ttu-id="96b65-145">String</span><span class="sxs-lookup"><span data-stu-id="96b65-145">String</span></span>|<span data-ttu-id="96b65-146">セクションの名前。</span><span class="sxs-lookup"><span data-stu-id="96b65-146">The name of the section.</span></span> |
|<span data-ttu-id="96b65-147">pagesUrl</span><span class="sxs-lookup"><span data-stu-id="96b65-147">pagesUrl</span></span>|<span data-ttu-id="96b65-148">String</span><span class="sxs-lookup"><span data-stu-id="96b65-148">String</span></span>|<span data-ttu-id="96b65-149">セクション`pages`内のすべてのページの詳細を取得できるエンドポイント。</span><span class="sxs-lookup"><span data-stu-id="96b65-149">The `pages` endpoint where you can get details for all the pages in the section.</span></span> <span data-ttu-id="96b65-150">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="96b65-150">Read-only.</span></span>|
|<span data-ttu-id="96b65-151">self</span><span class="sxs-lookup"><span data-stu-id="96b65-151">self</span></span>|<span data-ttu-id="96b65-152">String</span><span class="sxs-lookup"><span data-stu-id="96b65-152">String</span></span>|<span data-ttu-id="96b65-153">セクションに関する詳細を取得できるエンドポイント。</span><span class="sxs-lookup"><span data-stu-id="96b65-153">The endpoint where you can get details about the section.</span></span> <span data-ttu-id="96b65-154">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="96b65-154">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="96b65-155">関係</span><span class="sxs-lookup"><span data-stu-id="96b65-155">Relationships</span></span>
| <span data-ttu-id="96b65-156">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="96b65-156">Relationship</span></span> | <span data-ttu-id="96b65-157">型</span><span class="sxs-lookup"><span data-stu-id="96b65-157">Type</span></span>   |<span data-ttu-id="96b65-158">説明</span><span class="sxs-lookup"><span data-stu-id="96b65-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="96b65-159">ページ</span><span class="sxs-lookup"><span data-stu-id="96b65-159">pages</span></span>|<span data-ttu-id="96b65-160">[onenotePage](onenotepage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="96b65-160">[onenotePage](onenotepage.md) collection</span></span>|<span data-ttu-id="96b65-161">セクション内のページのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="96b65-161">The collection of pages in the section.</span></span>  <span data-ttu-id="96b65-162">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="96b65-162">Read-only.</span></span> <span data-ttu-id="96b65-163">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="96b65-163">Nullable.</span></span>|
|<span data-ttu-id="96b65-164">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="96b65-164">parentNotebook</span></span>|[<span data-ttu-id="96b65-165">ノートブック</span><span class="sxs-lookup"><span data-stu-id="96b65-165">notebook</span></span>](notebook.md)|<span data-ttu-id="96b65-166">セクションを含むノートブック。</span><span class="sxs-lookup"><span data-stu-id="96b65-166">The notebook that contains the section.</span></span>  <span data-ttu-id="96b65-167">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="96b65-167">Read-only.</span></span>|
|<span data-ttu-id="96b65-168">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="96b65-168">parentSectionGroup</span></span>|[<span data-ttu-id="96b65-169">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="96b65-169">sectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="96b65-170">セクションを含むセクショングループ。</span><span class="sxs-lookup"><span data-stu-id="96b65-170">The section group that contains the section.</span></span>  <span data-ttu-id="96b65-171">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="96b65-171">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="96b65-172">メソッド</span><span class="sxs-lookup"><span data-stu-id="96b65-172">Methods</span></span>

| <span data-ttu-id="96b65-173">メソッド</span><span class="sxs-lookup"><span data-stu-id="96b65-173">Method</span></span>           | <span data-ttu-id="96b65-174">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="96b65-174">Return Type</span></span>    |<span data-ttu-id="96b65-175">説明</span><span class="sxs-lookup"><span data-stu-id="96b65-175">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="96b65-176">セクションを取得する</span><span class="sxs-lookup"><span data-stu-id="96b65-176">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="96b65-177">onenoteSection</span><span class="sxs-lookup"><span data-stu-id="96b65-177">onenoteSection</span></span>](onenotesection.md) |<span data-ttu-id="96b65-178">セクションのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="96b65-178">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="96b65-179">Create page</span><span class="sxs-lookup"><span data-stu-id="96b65-179">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="96b65-180">onenotePage</span><span class="sxs-lookup"><span data-stu-id="96b65-180">onenotePage</span></span>](onenotepage.md)| <span data-ttu-id="96b65-181">指定したセクションの pages コレクションへの投稿によってページを作成します。</span><span class="sxs-lookup"><span data-stu-id="96b65-181">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="96b65-182">ページを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="96b65-182">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="96b65-183">[onenotePage](onenotepage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="96b65-183">[onenotePage](onenotepage.md) collection</span></span>| <span data-ttu-id="96b65-184">指定したセクション内のページのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="96b65-184">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="96b65-185">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="96b65-185">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="96b65-186">None</span><span class="sxs-lookup"><span data-stu-id="96b65-186">None</span></span>|<span data-ttu-id="96b65-187">セクションを特定のノートブックにコピーします。</span><span class="sxs-lookup"><span data-stu-id="96b65-187">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="96b65-188">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="96b65-188">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="96b65-189">None</span><span class="sxs-lookup"><span data-stu-id="96b65-189">None</span></span>|<span data-ttu-id="96b65-190">セクションを特定のセクショングループにコピーします。</span><span class="sxs-lookup"><span data-stu-id="96b65-190">Copy the section to a specific section group.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="96b65-191">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="96b65-191">JSON representation</span></span>

<span data-ttu-id="96b65-192">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="96b65-192">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "pages",
    "parentNotebook",
    "parentSectionGroup"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.onenoteSection"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isDefault": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.sectionLinks"},
  "displayName": "string",
  "pagesUrl": "string",
  "self": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
