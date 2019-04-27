---
title: onenoteSection リソースの種類
description: OneNote ノートブックのセクション。 セクションには、ページを含めることができます。
localization_priority: Normal
ms.openlocfilehash: d262065f46052c1cae55b42babaa91a2e065d3ef
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348853"
---
# <a name="onenotesection-resource-type"></a><span data-ttu-id="cace3-104">onenoteSection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cace3-104">onenoteSection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cace3-105">OneNote ノートブックのセクション。</span><span class="sxs-lookup"><span data-stu-id="cace3-105">A section in a OneNote notebook.</span></span> <span data-ttu-id="cace3-106">セクションには、ページを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="cace3-106">Sections can contain pages.</span></span>

## <a name="properties"></a><span data-ttu-id="cace3-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cace3-107">Properties</span></span>
| <span data-ttu-id="cace3-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cace3-108">Property</span></span>     | <span data-ttu-id="cace3-109">種類</span><span class="sxs-lookup"><span data-stu-id="cace3-109">Type</span></span>   |<span data-ttu-id="cace3-110">説明</span><span class="sxs-lookup"><span data-stu-id="cace3-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cace3-111">createdBy</span><span class="sxs-lookup"><span data-stu-id="cace3-111">createdBy</span></span>|[<span data-ttu-id="cace3-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="cace3-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="cace3-p103">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cace3-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="cace3-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cace3-115">createdDateTime</span></span>|<span data-ttu-id="cace3-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cace3-116">DateTimeOffset</span></span>|<span data-ttu-id="cace3-117">セクションが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="cace3-117">The date and time when the section was created.</span></span> <span data-ttu-id="cace3-118">Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="cace3-118">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="cace3-119">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="cace3-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="cace3-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cace3-120">Read-only.</span></span>|
|<span data-ttu-id="cace3-121">id</span><span class="sxs-lookup"><span data-stu-id="cace3-121">id</span></span>|<span data-ttu-id="cace3-122">String</span><span class="sxs-lookup"><span data-stu-id="cace3-122">String</span></span>|<span data-ttu-id="cace3-123">セクションの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="cace3-123">The unique identifier of the section.</span></span>  <span data-ttu-id="cace3-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cace3-124">Read-only.</span></span>|
|<span data-ttu-id="cace3-125">isDefault</span><span class="sxs-lookup"><span data-stu-id="cace3-125">isDefault</span></span>|<span data-ttu-id="cace3-126">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="cace3-126">Boolean</span></span>|<span data-ttu-id="cace3-127">これがユーザーの既定のセクションであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cace3-127">Indicates whether this is the user's default section.</span></span> <span data-ttu-id="cace3-128">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cace3-128">Read-only.</span></span>|
|<span data-ttu-id="cace3-129">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="cace3-129">lastModifiedBy</span></span>|[<span data-ttu-id="cace3-130">identitySet</span><span class="sxs-lookup"><span data-stu-id="cace3-130">identitySet</span></span>](identityset.md)|<span data-ttu-id="cace3-p107">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cace3-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="cace3-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cace3-133">lastModifiedDateTime</span></span>|<span data-ttu-id="cace3-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cace3-134">DateTimeOffset</span></span>|<span data-ttu-id="cace3-135">セクションが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="cace3-135">The date and time when the section was last modified.</span></span> <span data-ttu-id="cace3-136">Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="cace3-136">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="cace3-137">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="cace3-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="cace3-138">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cace3-138">Read-only.</span></span>|
|<span data-ttu-id="cace3-139">リンク</span><span class="sxs-lookup"><span data-stu-id="cace3-139">links</span></span>|[<span data-ttu-id="cace3-140">sectionlinks</span><span class="sxs-lookup"><span data-stu-id="cace3-140">sectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="cace3-141">セクションを開くためのリンク。</span><span class="sxs-lookup"><span data-stu-id="cace3-141">Links for opening the section.</span></span> <span data-ttu-id="cace3-142">リンク`oneNoteClientURL`によって、OneNote native client のセクションがインストールされている場合は、そのセクションが開きます。</span><span class="sxs-lookup"><span data-stu-id="cace3-142">The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed.</span></span> <span data-ttu-id="cace3-143">リンク`oneNoteWebURL`によって、OneNote Online のセクションが開きます。</span><span class="sxs-lookup"><span data-stu-id="cace3-143">The `oneNoteWebURL` link opens the section in OneNote Online.</span></span>|
|<span data-ttu-id="cace3-144">displayName</span><span class="sxs-lookup"><span data-stu-id="cace3-144">displayName</span></span>|<span data-ttu-id="cace3-145">String</span><span class="sxs-lookup"><span data-stu-id="cace3-145">String</span></span>|<span data-ttu-id="cace3-146">セクションの名前。</span><span class="sxs-lookup"><span data-stu-id="cace3-146">The name of the section.</span></span> |
|<span data-ttu-id="cace3-147">pagesUrl</span><span class="sxs-lookup"><span data-stu-id="cace3-147">pagesUrl</span></span>|<span data-ttu-id="cace3-148">String</span><span class="sxs-lookup"><span data-stu-id="cace3-148">String</span></span>|<span data-ttu-id="cace3-149">セクション`pages`内のすべてのページの詳細を取得できるエンドポイント。</span><span class="sxs-lookup"><span data-stu-id="cace3-149">The `pages` endpoint where you can get details for all the pages in the section.</span></span> <span data-ttu-id="cace3-150">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cace3-150">Read-only.</span></span>|
|<span data-ttu-id="cace3-151">self</span><span class="sxs-lookup"><span data-stu-id="cace3-151">self</span></span>|<span data-ttu-id="cace3-152">String</span><span class="sxs-lookup"><span data-stu-id="cace3-152">String</span></span>|<span data-ttu-id="cace3-153">セクションに関する詳細を取得できるエンドポイント。</span><span class="sxs-lookup"><span data-stu-id="cace3-153">The endpoint where you can get details about the section.</span></span> <span data-ttu-id="cace3-154">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cace3-154">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cace3-155">関係</span><span class="sxs-lookup"><span data-stu-id="cace3-155">Relationships</span></span>
| <span data-ttu-id="cace3-156">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cace3-156">Relationship</span></span> | <span data-ttu-id="cace3-157">型</span><span class="sxs-lookup"><span data-stu-id="cace3-157">Type</span></span>   |<span data-ttu-id="cace3-158">説明</span><span class="sxs-lookup"><span data-stu-id="cace3-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cace3-159">ページ</span><span class="sxs-lookup"><span data-stu-id="cace3-159">pages</span></span>|<span data-ttu-id="cace3-160">[onenotePage](onenotepage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cace3-160">[onenotePage](onenotepage.md) collection</span></span>|<span data-ttu-id="cace3-161">セクション内のページのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="cace3-161">The collection of pages in the section.</span></span>  <span data-ttu-id="cace3-162">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cace3-162">Read-only.</span></span> <span data-ttu-id="cace3-163">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="cace3-163">Nullable.</span></span>|
|<span data-ttu-id="cace3-164">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="cace3-164">parentNotebook</span></span>|[<span data-ttu-id="cace3-165">ノートブック</span><span class="sxs-lookup"><span data-stu-id="cace3-165">notebook</span></span>](notebook.md)|<span data-ttu-id="cace3-166">セクションを含むノートブック。</span><span class="sxs-lookup"><span data-stu-id="cace3-166">The notebook that contains the section.</span></span>  <span data-ttu-id="cace3-167">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cace3-167">Read-only.</span></span>|
|<span data-ttu-id="cace3-168">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="cace3-168">parentSectionGroup</span></span>|[<span data-ttu-id="cace3-169">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="cace3-169">sectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="cace3-170">セクションを含むセクショングループ。</span><span class="sxs-lookup"><span data-stu-id="cace3-170">The section group that contains the section.</span></span>  <span data-ttu-id="cace3-171">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="cace3-171">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="cace3-172">メソッド</span><span class="sxs-lookup"><span data-stu-id="cace3-172">Methods</span></span>

| <span data-ttu-id="cace3-173">メソッド</span><span class="sxs-lookup"><span data-stu-id="cace3-173">Method</span></span>           | <span data-ttu-id="cace3-174">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cace3-174">Return Type</span></span>    |<span data-ttu-id="cace3-175">説明</span><span class="sxs-lookup"><span data-stu-id="cace3-175">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cace3-176">セクションを取得する</span><span class="sxs-lookup"><span data-stu-id="cace3-176">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="cace3-177">onenoteSection</span><span class="sxs-lookup"><span data-stu-id="cace3-177">onenoteSection</span></span>](onenotesection.md) |<span data-ttu-id="cace3-178">セクションのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="cace3-178">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="cace3-179">Create page</span><span class="sxs-lookup"><span data-stu-id="cace3-179">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="cace3-180">onenotePage</span><span class="sxs-lookup"><span data-stu-id="cace3-180">onenotePage</span></span>](onenotepage.md)| <span data-ttu-id="cace3-181">指定したセクションの pages コレクションへの投稿によってページを作成します。</span><span class="sxs-lookup"><span data-stu-id="cace3-181">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="cace3-182">ページを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="cace3-182">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="cace3-183">[onenotePage](onenotepage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cace3-183">[onenotePage](onenotepage.md) collection</span></span>| <span data-ttu-id="cace3-184">指定したセクション内のページのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="cace3-184">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="cace3-185">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="cace3-185">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="cace3-186">なし</span><span class="sxs-lookup"><span data-stu-id="cace3-186">None</span></span>|<span data-ttu-id="cace3-187">セクションを特定のノートブックにコピーします。</span><span class="sxs-lookup"><span data-stu-id="cace3-187">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="cace3-188">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="cace3-188">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="cace3-189">なし</span><span class="sxs-lookup"><span data-stu-id="cace3-189">None</span></span>|<span data-ttu-id="cace3-190">セクションを特定のセクショングループにコピーします。</span><span class="sxs-lookup"><span data-stu-id="cace3-190">Copy the section to a specific section group.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="cace3-191">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cace3-191">JSON representation</span></span>

<span data-ttu-id="cace3-192">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cace3-192">Here is a JSON representation of the resource.</span></span>

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
