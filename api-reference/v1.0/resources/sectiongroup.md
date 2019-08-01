---
title: sectionGroup リソースの種類
description: OneNote ノートブックのセクショングループ。 セクショングループには、セクションとセクショングループを含めることができます。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 65511c11810a95dfaf7497b0cc2cb1b1ad89c8a2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034553"
---
# <a name="sectiongroup-resource-type"></a><span data-ttu-id="acf43-104">sectionGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="acf43-104">sectionGroup resource type</span></span>

<span data-ttu-id="acf43-105">OneNote ノートブックのセクショングループ。</span><span class="sxs-lookup"><span data-stu-id="acf43-105">A section group in a OneNote notebook.</span></span> <span data-ttu-id="acf43-106">セクショングループには、セクションとセクショングループを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="acf43-106">Section groups can contain sections and section groups.</span></span>

## <a name="json-representation"></a><span data-ttu-id="acf43-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="acf43-107">JSON representation</span></span>

<span data-ttu-id="acf43-108">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="acf43-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityHierarchyModel",
  "optionalProperties": [
    "parentNotebook",
    "parentSectionGroup",
    "sectionGroups",
    "sections"
  ],
  "@odata.type": "microsoft.graph.sectionGroup"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "string",
  "sectionGroupsUrl": "string",
  "sectionsUrl": "string",
  "self": "string"
}

```
## <a name="properties"></a><span data-ttu-id="acf43-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="acf43-109">Properties</span></span>
| <span data-ttu-id="acf43-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="acf43-110">Property</span></span>     | <span data-ttu-id="acf43-111">型</span><span class="sxs-lookup"><span data-stu-id="acf43-111">Type</span></span>   |<span data-ttu-id="acf43-112">説明</span><span class="sxs-lookup"><span data-stu-id="acf43-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="acf43-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="acf43-113">createdBy</span></span>|[<span data-ttu-id="acf43-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="acf43-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="acf43-p103">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="acf43-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="acf43-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="acf43-117">createdDateTime</span></span>|<span data-ttu-id="acf43-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="acf43-118">DateTimeOffset</span></span>|<span data-ttu-id="acf43-119">セクション グループが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="acf43-119">The date and time when the section group was created.</span></span> <span data-ttu-id="acf43-120">Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="acf43-120">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="acf43-121">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="acf43-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="acf43-122">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="acf43-122">Read-only.</span></span>|
|<span data-ttu-id="acf43-123">id</span><span class="sxs-lookup"><span data-stu-id="acf43-123">id</span></span>|<span data-ttu-id="acf43-124">文字列</span><span class="sxs-lookup"><span data-stu-id="acf43-124">String</span></span>|<span data-ttu-id="acf43-125">セクション グループの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="acf43-125">The unique identifier of the section group.</span></span> <span data-ttu-id="acf43-126">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="acf43-126">Read-only.</span></span>|
|<span data-ttu-id="acf43-127">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="acf43-127">lastModifiedBy</span></span>|[<span data-ttu-id="acf43-128">identitySet</span><span class="sxs-lookup"><span data-stu-id="acf43-128">identitySet</span></span>](identityset.md)|<span data-ttu-id="acf43-p106">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="acf43-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="acf43-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="acf43-131">lastModifiedDateTime</span></span>|<span data-ttu-id="acf43-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="acf43-132">DateTimeOffset</span></span>|<span data-ttu-id="acf43-133">セクション グループが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="acf43-133">The date and time when the section group was last modified.</span></span> <span data-ttu-id="acf43-134">Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="acf43-134">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="acf43-135">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="acf43-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="acf43-136">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="acf43-136">Read-only.</span></span>|
|<span data-ttu-id="acf43-137">displayName</span><span class="sxs-lookup"><span data-stu-id="acf43-137">displayName</span></span>|<span data-ttu-id="acf43-138">String</span><span class="sxs-lookup"><span data-stu-id="acf43-138">String</span></span>|<span data-ttu-id="acf43-139">セクション グループの名前。</span><span class="sxs-lookup"><span data-stu-id="acf43-139">The name of the section group.</span></span>|
|<span data-ttu-id="acf43-140">Sectionグループ Url</span><span class="sxs-lookup"><span data-stu-id="acf43-140">sectionGroupsUrl</span></span>|<span data-ttu-id="acf43-141">String</span><span class="sxs-lookup"><span data-stu-id="acf43-141">String</span></span>|<span data-ttu-id="acf43-142">`sectionGroups`ナビゲーションプロパティの URL。セクショングループ内のすべてのセクショングループを返します。</span><span class="sxs-lookup"><span data-stu-id="acf43-142">The URL for the `sectionGroups` navigation property, which returns all the section groups in the section group.</span></span> <span data-ttu-id="acf43-143">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="acf43-143">Read-only.</span></span>|
|<span data-ttu-id="acf43-144">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="acf43-144">sectionsUrl</span></span>|<span data-ttu-id="acf43-145">String</span><span class="sxs-lookup"><span data-stu-id="acf43-145">String</span></span>|<span data-ttu-id="acf43-146">`sections`ナビゲーションプロパティの URL。セクショングループ内のすべてのセクションを返します。</span><span class="sxs-lookup"><span data-stu-id="acf43-146">The URL for the `sections` navigation property, which returns all the sections in the section group.</span></span> <span data-ttu-id="acf43-147">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="acf43-147">Read-only.</span></span>|
|<span data-ttu-id="acf43-148">self</span><span class="sxs-lookup"><span data-stu-id="acf43-148">self</span></span>|<span data-ttu-id="acf43-149">String</span><span class="sxs-lookup"><span data-stu-id="acf43-149">String</span></span>|<span data-ttu-id="acf43-150">セクション グループに関する詳細を取得できるエンドポイント。</span><span class="sxs-lookup"><span data-stu-id="acf43-150">The endpoint where you can get details about the section group.</span></span> <span data-ttu-id="acf43-151">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="acf43-151">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="acf43-152">関係</span><span class="sxs-lookup"><span data-stu-id="acf43-152">Relationships</span></span>
| <span data-ttu-id="acf43-153">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="acf43-153">Relationship</span></span> | <span data-ttu-id="acf43-154">型</span><span class="sxs-lookup"><span data-stu-id="acf43-154">Type</span></span>   |<span data-ttu-id="acf43-155">説明</span><span class="sxs-lookup"><span data-stu-id="acf43-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="acf43-156">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="acf43-156">parentNotebook</span></span>|[<span data-ttu-id="acf43-157">Notebook</span><span class="sxs-lookup"><span data-stu-id="acf43-157">Notebook</span></span>](notebook.md)|<span data-ttu-id="acf43-158">セクショングループを含むノートブック。</span><span class="sxs-lookup"><span data-stu-id="acf43-158">The notebook that contains the section group.</span></span> <span data-ttu-id="acf43-159">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="acf43-159">Read-only.</span></span>|
|<span data-ttu-id="acf43-160">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="acf43-160">parentSectionGroup</span></span>|[<span data-ttu-id="acf43-161">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="acf43-161">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="acf43-162">セクショングループを含むセクショングループ。</span><span class="sxs-lookup"><span data-stu-id="acf43-162">The section group that contains the section group.</span></span> <span data-ttu-id="acf43-163">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="acf43-163">Read-only.</span></span>|
|<span data-ttu-id="acf43-164">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="acf43-164">sectionGroups</span></span>|<span data-ttu-id="acf43-165">[SectionGroup](sectiongroup.md) collection</span><span class="sxs-lookup"><span data-stu-id="acf43-165">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="acf43-166">セクション内のセクショングループ。</span><span class="sxs-lookup"><span data-stu-id="acf43-166">The section groups in the section.</span></span> <span data-ttu-id="acf43-167">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="acf43-167">Read-only.</span></span> <span data-ttu-id="acf43-168">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="acf43-168">Nullable.</span></span>|
|<span data-ttu-id="acf43-169">セクション</span><span class="sxs-lookup"><span data-stu-id="acf43-169">sections</span></span>|<span data-ttu-id="acf43-170">[OnenoteSection](section.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="acf43-170">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="acf43-171">セクショングループ内のセクション。</span><span class="sxs-lookup"><span data-stu-id="acf43-171">The sections in the section group.</span></span> <span data-ttu-id="acf43-172">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="acf43-172">Read-only.</span></span> <span data-ttu-id="acf43-173">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="acf43-173">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="acf43-174">メソッド</span><span class="sxs-lookup"><span data-stu-id="acf43-174">Methods</span></span>

| <span data-ttu-id="acf43-175">メソッド</span><span class="sxs-lookup"><span data-stu-id="acf43-175">Method</span></span>           | <span data-ttu-id="acf43-176">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="acf43-176">Return Type</span></span>    |<span data-ttu-id="acf43-177">説明</span><span class="sxs-lookup"><span data-stu-id="acf43-177">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="acf43-178">セクション グループを取得する</span><span class="sxs-lookup"><span data-stu-id="acf43-178">Get section group</span></span>](../api/sectiongroup-get.md) | [<span data-ttu-id="acf43-179">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="acf43-179">SectionGroup</span></span>](sectiongroup.md) |<span data-ttu-id="acf43-180">セクショングループのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="acf43-180">Read the properties and relationships of the section group.</span></span>|
|[<span data-ttu-id="acf43-181">セクション グループを作成する</span><span class="sxs-lookup"><span data-stu-id="acf43-181">Create section group</span></span>](../api/sectiongroup-post-sectiongroups.md) |[<span data-ttu-id="acf43-182">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="acf43-182">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="acf43-183">指定したセクショングループの sectionGroups コレクションに投稿して、セクショングループを作成します。</span><span class="sxs-lookup"><span data-stu-id="acf43-183">Create a section group by posting to the sectionGroups collection in the specified section group.</span></span>|
|[<span data-ttu-id="acf43-184">List section groups</span><span class="sxs-lookup"><span data-stu-id="acf43-184">List section groups</span></span>](../api/sectiongroup-list-sectiongroups.md) |<span data-ttu-id="acf43-185">[SectionGroup](sectiongroup.md) collection</span><span class="sxs-lookup"><span data-stu-id="acf43-185">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="acf43-186">指定したセクショングループ内のセクショングループのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="acf43-186">Get collection of section groups in the specified section group.</span></span>|
|[<span data-ttu-id="acf43-187">セクションを作成する</span><span class="sxs-lookup"><span data-stu-id="acf43-187">Create section</span></span>](../api/sectiongroup-post-sections.md) |[<span data-ttu-id="acf43-188">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="acf43-188">OnenoteSection</span></span>](section.md)| <span data-ttu-id="acf43-189">指定したセクショングループ内の sections コレクションに投稿してセクションを作成します。</span><span class="sxs-lookup"><span data-stu-id="acf43-189">Create a section by posting to the sections collection in the specified section group.</span></span>|
|[<span data-ttu-id="acf43-190">List sections</span><span class="sxs-lookup"><span data-stu-id="acf43-190">List sections</span></span>](../api/sectiongroup-list-sections.md) |<span data-ttu-id="acf43-191">[OnenoteSection](section.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="acf43-191">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="acf43-192">指定したセクショングループ内のセクションのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="acf43-192">Get a collection of sections in the specified section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
