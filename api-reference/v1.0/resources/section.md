---
title: セクションリソースの種類
description: OneNote ノートブックのセクション。 セクションには、ページを含めることができます。
localization_priority: Normal
ms.openlocfilehash: 8cb7869c914d53e92cc62546ef0936ecb70e8735
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/26/2019
ms.locfileid: "35236644"
---
# <a name="section-resource-type"></a><span data-ttu-id="12f89-104">セクションリソースの種類</span><span class="sxs-lookup"><span data-stu-id="12f89-104">section resource type</span></span>

<span data-ttu-id="12f89-105">OneNote ノートブックのセクション。</span><span class="sxs-lookup"><span data-stu-id="12f89-105">A section in a OneNote notebook.</span></span> <span data-ttu-id="12f89-106">セクションには、ページを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="12f89-106">Sections can contain pages.</span></span>

## <a name="json-representation"></a><span data-ttu-id="12f89-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="12f89-107">JSON representation</span></span>

<span data-ttu-id="12f89-108">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="12f89-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityHierarchyModel",
  "optionalProperties": [
    "pages",
    "parentNotebook",
    "parentSectionGroup"
  ],
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
## <a name="properties"></a><span data-ttu-id="12f89-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="12f89-109">Properties</span></span>
| <span data-ttu-id="12f89-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="12f89-110">Property</span></span>     | <span data-ttu-id="12f89-111">型</span><span class="sxs-lookup"><span data-stu-id="12f89-111">Type</span></span>   |<span data-ttu-id="12f89-112">説明</span><span class="sxs-lookup"><span data-stu-id="12f89-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12f89-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="12f89-113">createdBy</span></span>|[<span data-ttu-id="12f89-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="12f89-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="12f89-p103">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="12f89-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="12f89-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="12f89-117">createdDateTime</span></span>|<span data-ttu-id="12f89-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12f89-118">DateTimeOffset</span></span>|<span data-ttu-id="12f89-119">セクションが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="12f89-119">The date and time when the section was created.</span></span> <span data-ttu-id="12f89-120">Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="12f89-120">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="12f89-121">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="12f89-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="12f89-122">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="12f89-122">Read-only.</span></span>|
|<span data-ttu-id="12f89-123">id</span><span class="sxs-lookup"><span data-stu-id="12f89-123">id</span></span>|<span data-ttu-id="12f89-124">文字列</span><span class="sxs-lookup"><span data-stu-id="12f89-124">String</span></span>|<span data-ttu-id="12f89-125">セクションの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="12f89-125">The unique identifier of the section.</span></span>  <span data-ttu-id="12f89-126">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="12f89-126">Read-only.</span></span>|
|<span data-ttu-id="12f89-127">isDefault</span><span class="sxs-lookup"><span data-stu-id="12f89-127">isDefault</span></span>|<span data-ttu-id="12f89-128">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="12f89-128">Boolean</span></span>|<span data-ttu-id="12f89-129">これがユーザーの既定のセクションであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="12f89-129">Indicates whether this is the user's default section.</span></span> <span data-ttu-id="12f89-130">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="12f89-130">Read-only.</span></span>|
|<span data-ttu-id="12f89-131">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="12f89-131">lastModifiedBy</span></span>|[<span data-ttu-id="12f89-132">identitySet</span><span class="sxs-lookup"><span data-stu-id="12f89-132">identitySet</span></span>](identityset.md)|<span data-ttu-id="12f89-p107">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="12f89-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="12f89-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="12f89-135">lastModifiedDateTime</span></span>|<span data-ttu-id="12f89-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12f89-136">DateTimeOffset</span></span>|<span data-ttu-id="12f89-137">セクションが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="12f89-137">The date and time when the section was last modified.</span></span> <span data-ttu-id="12f89-138">Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="12f89-138">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="12f89-139">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="12f89-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="12f89-140">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="12f89-140">Read-only.</span></span>|
|<span data-ttu-id="12f89-141">リンク</span><span class="sxs-lookup"><span data-stu-id="12f89-141">links</span></span>|[<span data-ttu-id="12f89-142">SectionLinks</span><span class="sxs-lookup"><span data-stu-id="12f89-142">SectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="12f89-143">セクションを開くためのリンク。</span><span class="sxs-lookup"><span data-stu-id="12f89-143">Links for opening the section.</span></span> <span data-ttu-id="12f89-144">リンク`oneNoteClientURL`によって、OneNote native client のセクションがインストールされている場合は、そのセクションが開きます。</span><span class="sxs-lookup"><span data-stu-id="12f89-144">The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed.</span></span> <span data-ttu-id="12f89-145">リンク`oneNoteWebURL`は、web 上の OneNote でセクションを開きます。</span><span class="sxs-lookup"><span data-stu-id="12f89-145">The `oneNoteWebURL` link opens the section in OneNote on the web.</span></span>|
|<span data-ttu-id="12f89-146">displayName</span><span class="sxs-lookup"><span data-stu-id="12f89-146">displayName</span></span>|<span data-ttu-id="12f89-147">String</span><span class="sxs-lookup"><span data-stu-id="12f89-147">String</span></span>|<span data-ttu-id="12f89-148">セクションの名前。</span><span class="sxs-lookup"><span data-stu-id="12f89-148">The name of the section.</span></span> |
|<span data-ttu-id="12f89-149">pagesUrl</span><span class="sxs-lookup"><span data-stu-id="12f89-149">pagesUrl</span></span>|<span data-ttu-id="12f89-150">String</span><span class="sxs-lookup"><span data-stu-id="12f89-150">String</span></span>|<span data-ttu-id="12f89-151">セクション`pages`内のすべてのページの詳細を取得できるエンドポイント。</span><span class="sxs-lookup"><span data-stu-id="12f89-151">The `pages` endpoint where you can get details for all the pages in the section.</span></span> <span data-ttu-id="12f89-152">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="12f89-152">Read-only.</span></span>|
|<span data-ttu-id="12f89-153">self</span><span class="sxs-lookup"><span data-stu-id="12f89-153">self</span></span>|<span data-ttu-id="12f89-154">String</span><span class="sxs-lookup"><span data-stu-id="12f89-154">String</span></span>|<span data-ttu-id="12f89-155">セクションに関する詳細を取得できるエンドポイント。</span><span class="sxs-lookup"><span data-stu-id="12f89-155">The endpoint where you can get details about the section.</span></span> <span data-ttu-id="12f89-156">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="12f89-156">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="12f89-157">関係</span><span class="sxs-lookup"><span data-stu-id="12f89-157">Relationships</span></span>
| <span data-ttu-id="12f89-158">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="12f89-158">Relationship</span></span> | <span data-ttu-id="12f89-159">型</span><span class="sxs-lookup"><span data-stu-id="12f89-159">Type</span></span>   |<span data-ttu-id="12f89-160">説明</span><span class="sxs-lookup"><span data-stu-id="12f89-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12f89-161">ページ</span><span class="sxs-lookup"><span data-stu-id="12f89-161">pages</span></span>|<span data-ttu-id="12f89-162">[OnenotePage](page.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="12f89-162">[OnenotePage](page.md) collection</span></span>|<span data-ttu-id="12f89-163">セクション内のページのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="12f89-163">The collection of pages in the section.</span></span>  <span data-ttu-id="12f89-164">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="12f89-164">Read-only.</span></span> <span data-ttu-id="12f89-165">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="12f89-165">Nullable.</span></span>|
|<span data-ttu-id="12f89-166">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="12f89-166">parentNotebook</span></span>|[<span data-ttu-id="12f89-167">Notebook</span><span class="sxs-lookup"><span data-stu-id="12f89-167">Notebook</span></span>](notebook.md)|<span data-ttu-id="12f89-168">セクションを含むノートブック。</span><span class="sxs-lookup"><span data-stu-id="12f89-168">The notebook that contains the section.</span></span>  <span data-ttu-id="12f89-169">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="12f89-169">Read-only.</span></span>|
|<span data-ttu-id="12f89-170">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="12f89-170">parentSectionGroup</span></span>|[<span data-ttu-id="12f89-171">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="12f89-171">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="12f89-172">セクションを含むセクショングループ。</span><span class="sxs-lookup"><span data-stu-id="12f89-172">The section group that contains the section.</span></span>  <span data-ttu-id="12f89-173">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="12f89-173">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="12f89-174">メソッド</span><span class="sxs-lookup"><span data-stu-id="12f89-174">Methods</span></span>

| <span data-ttu-id="12f89-175">メソッド</span><span class="sxs-lookup"><span data-stu-id="12f89-175">Method</span></span>           | <span data-ttu-id="12f89-176">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="12f89-176">Return Type</span></span>    |<span data-ttu-id="12f89-177">説明</span><span class="sxs-lookup"><span data-stu-id="12f89-177">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="12f89-178">セクションを取得する</span><span class="sxs-lookup"><span data-stu-id="12f89-178">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="12f89-179">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="12f89-179">OnenoteSection</span></span>](section.md) |<span data-ttu-id="12f89-180">セクションのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="12f89-180">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="12f89-181">Create page</span><span class="sxs-lookup"><span data-stu-id="12f89-181">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="12f89-182">Page</span><span class="sxs-lookup"><span data-stu-id="12f89-182">Page</span></span>](page.md)| <span data-ttu-id="12f89-183">指定したセクションの pages コレクションへの投稿によってページを作成します。</span><span class="sxs-lookup"><span data-stu-id="12f89-183">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="12f89-184">List pages</span><span class="sxs-lookup"><span data-stu-id="12f89-184">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="12f89-185">[Page](page.md) collection</span><span class="sxs-lookup"><span data-stu-id="12f89-185">[Page](page.md) collection</span></span>| <span data-ttu-id="12f89-186">指定したセクション内のページのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="12f89-186">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="12f89-187">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="12f89-187">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="12f89-188">None</span><span class="sxs-lookup"><span data-stu-id="12f89-188">None</span></span>|<span data-ttu-id="12f89-189">セクションを特定のノートブックにコピーします。</span><span class="sxs-lookup"><span data-stu-id="12f89-189">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="12f89-190">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="12f89-190">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="12f89-191">None</span><span class="sxs-lookup"><span data-stu-id="12f89-191">None</span></span>|<span data-ttu-id="12f89-192">セクションを特定のセクショングループにコピーします。</span><span class="sxs-lookup"><span data-stu-id="12f89-192">Copy the section to a specific section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
