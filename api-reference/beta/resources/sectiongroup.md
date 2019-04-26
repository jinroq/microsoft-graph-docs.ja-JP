---
title: sectionGroup リソースの種類
description: OneNote ノートブックのセクショングループ。 セクショングループには、セクションとセクショングループを含めることができます。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: f1cd9757b0a58afb4183bd917a7a090b14502a36
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343400"
---
# <a name="sectiongroup-resource-type"></a><span data-ttu-id="831d2-104">sectionGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="831d2-104">sectionGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="831d2-105">OneNote ノートブックのセクショングループ。</span><span class="sxs-lookup"><span data-stu-id="831d2-105">A section group in a OneNote notebook.</span></span> <span data-ttu-id="831d2-106">セクショングループには、セクションとセクショングループを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="831d2-106">Section groups can contain sections and section groups.</span></span>

## <a name="json-representation"></a><span data-ttu-id="831d2-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="831d2-107">JSON representation</span></span>

<span data-ttu-id="831d2-108">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="831d2-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "parentNotebook",
    "parentSectionGroup",
    "sectionGroups",
    "sections"
  ],
  "keyProperty": "id",
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
## <a name="properties"></a><span data-ttu-id="831d2-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="831d2-109">Properties</span></span>
| <span data-ttu-id="831d2-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="831d2-110">Property</span></span>     | <span data-ttu-id="831d2-111">型</span><span class="sxs-lookup"><span data-stu-id="831d2-111">Type</span></span>   |<span data-ttu-id="831d2-112">説明</span><span class="sxs-lookup"><span data-stu-id="831d2-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="831d2-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="831d2-113">createdBy</span></span>|[<span data-ttu-id="831d2-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="831d2-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="831d2-p103">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="831d2-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="831d2-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="831d2-117">createdDateTime</span></span>|<span data-ttu-id="831d2-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="831d2-118">DateTimeOffset</span></span>|<span data-ttu-id="831d2-119">セクション グループが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="831d2-119">The date and time when the section group was created.</span></span> <span data-ttu-id="831d2-120">Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="831d2-120">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="831d2-121">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="831d2-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="831d2-122">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="831d2-122">Read-only.</span></span>|
|<span data-ttu-id="831d2-123">id</span><span class="sxs-lookup"><span data-stu-id="831d2-123">id</span></span>|<span data-ttu-id="831d2-124">String</span><span class="sxs-lookup"><span data-stu-id="831d2-124">String</span></span>|<span data-ttu-id="831d2-125">セクション グループの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="831d2-125">The unique identifier of the section group.</span></span> <span data-ttu-id="831d2-126">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="831d2-126">Read-only.</span></span>|
|<span data-ttu-id="831d2-127">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="831d2-127">lastModifiedBy</span></span>|[<span data-ttu-id="831d2-128">identitySet</span><span class="sxs-lookup"><span data-stu-id="831d2-128">identitySet</span></span>](identityset.md)|<span data-ttu-id="831d2-p106">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="831d2-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="831d2-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="831d2-131">lastModifiedDateTime</span></span>|<span data-ttu-id="831d2-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="831d2-132">DateTimeOffset</span></span>|<span data-ttu-id="831d2-133">セクション グループが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="831d2-133">The date and time when the section group was last modified.</span></span> <span data-ttu-id="831d2-134">Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="831d2-134">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="831d2-135">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="831d2-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="831d2-136">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="831d2-136">Read-only.</span></span>|
|<span data-ttu-id="831d2-137">displayName</span><span class="sxs-lookup"><span data-stu-id="831d2-137">displayName</span></span>|<span data-ttu-id="831d2-138">String</span><span class="sxs-lookup"><span data-stu-id="831d2-138">String</span></span>|<span data-ttu-id="831d2-139">セクション グループの名前。</span><span class="sxs-lookup"><span data-stu-id="831d2-139">The name of the section group.</span></span>|
|<span data-ttu-id="831d2-140">sectionグループ url</span><span class="sxs-lookup"><span data-stu-id="831d2-140">sectionGroupsUrl</span></span>|<span data-ttu-id="831d2-141">String</span><span class="sxs-lookup"><span data-stu-id="831d2-141">String</span></span>|<span data-ttu-id="831d2-142">`sectionGroups`ナビゲーションプロパティの URL。セクショングループ内のすべてのセクショングループを返します。</span><span class="sxs-lookup"><span data-stu-id="831d2-142">The URL for the `sectionGroups` navigation property, which returns all the section groups in the section group.</span></span> <span data-ttu-id="831d2-143">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="831d2-143">Read-only.</span></span>|
|<span data-ttu-id="831d2-144">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="831d2-144">sectionsUrl</span></span>|<span data-ttu-id="831d2-145">String</span><span class="sxs-lookup"><span data-stu-id="831d2-145">String</span></span>|<span data-ttu-id="831d2-146">`sections`ナビゲーションプロパティの URL。セクショングループ内のすべてのセクションを返します。</span><span class="sxs-lookup"><span data-stu-id="831d2-146">The URL for the `sections` navigation property, which returns all the sections in the section group.</span></span> <span data-ttu-id="831d2-147">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="831d2-147">Read-only.</span></span>|
|<span data-ttu-id="831d2-148">self</span><span class="sxs-lookup"><span data-stu-id="831d2-148">self</span></span>|<span data-ttu-id="831d2-149">String</span><span class="sxs-lookup"><span data-stu-id="831d2-149">String</span></span>|<span data-ttu-id="831d2-150">セクション グループに関する詳細を取得できるエンドポイント。</span><span class="sxs-lookup"><span data-stu-id="831d2-150">The endpoint where you can get details about the section group.</span></span> <span data-ttu-id="831d2-151">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="831d2-151">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="831d2-152">関係</span><span class="sxs-lookup"><span data-stu-id="831d2-152">Relationships</span></span>
| <span data-ttu-id="831d2-153">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="831d2-153">Relationship</span></span> | <span data-ttu-id="831d2-154">型</span><span class="sxs-lookup"><span data-stu-id="831d2-154">Type</span></span>   |<span data-ttu-id="831d2-155">説明</span><span class="sxs-lookup"><span data-stu-id="831d2-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="831d2-156">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="831d2-156">parentNotebook</span></span>|[<span data-ttu-id="831d2-157">ノートブック</span><span class="sxs-lookup"><span data-stu-id="831d2-157">notebook</span></span>](notebook.md)|<span data-ttu-id="831d2-158">セクショングループを含むノートブック。</span><span class="sxs-lookup"><span data-stu-id="831d2-158">The notebook that contains the section group.</span></span> <span data-ttu-id="831d2-159">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="831d2-159">Read-only.</span></span>|
|<span data-ttu-id="831d2-160">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="831d2-160">parentSectionGroup</span></span>|[<span data-ttu-id="831d2-161">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="831d2-161">sectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="831d2-162">セクショングループを含むセクショングループ。</span><span class="sxs-lookup"><span data-stu-id="831d2-162">The section group that contains the section group.</span></span> <span data-ttu-id="831d2-163">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="831d2-163">Read-only.</span></span>|
|<span data-ttu-id="831d2-164">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="831d2-164">sectionGroups</span></span>|<span data-ttu-id="831d2-165">[sectionGroup](sectiongroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="831d2-165">[sectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="831d2-166">セクション内のセクショングループ。</span><span class="sxs-lookup"><span data-stu-id="831d2-166">The section groups in the section.</span></span> <span data-ttu-id="831d2-167">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="831d2-167">Read-only.</span></span> <span data-ttu-id="831d2-168">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="831d2-168">Nullable.</span></span>|
|<span data-ttu-id="831d2-169">セクション</span><span class="sxs-lookup"><span data-stu-id="831d2-169">sections</span></span>|<span data-ttu-id="831d2-170">[onenoteSection](onenotesection.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="831d2-170">[onenoteSection](onenotesection.md) collection</span></span>|<span data-ttu-id="831d2-171">セクショングループ内のセクション。</span><span class="sxs-lookup"><span data-stu-id="831d2-171">The sections in the section group.</span></span> <span data-ttu-id="831d2-172">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="831d2-172">Read-only.</span></span> <span data-ttu-id="831d2-173">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="831d2-173">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="831d2-174">メソッド</span><span class="sxs-lookup"><span data-stu-id="831d2-174">Methods</span></span>

| <span data-ttu-id="831d2-175">メソッド</span><span class="sxs-lookup"><span data-stu-id="831d2-175">Method</span></span>           | <span data-ttu-id="831d2-176">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="831d2-176">Return Type</span></span>    |<span data-ttu-id="831d2-177">説明</span><span class="sxs-lookup"><span data-stu-id="831d2-177">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="831d2-178">セクション グループを取得する</span><span class="sxs-lookup"><span data-stu-id="831d2-178">Get section group</span></span>](../api/sectiongroup-get.md) | [<span data-ttu-id="831d2-179">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="831d2-179">sectionGroup</span></span>](sectiongroup.md) |<span data-ttu-id="831d2-180">セクショングループのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="831d2-180">Read the properties and relationships of the section group.</span></span>|
|[<span data-ttu-id="831d2-181">セクション グループを作成する</span><span class="sxs-lookup"><span data-stu-id="831d2-181">Create section group</span></span>](../api/sectiongroup-post-sectiongroups.md) |[<span data-ttu-id="831d2-182">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="831d2-182">sectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="831d2-183">指定したセクショングループの sectiongroups コレクションに投稿して、セクショングループを作成します。</span><span class="sxs-lookup"><span data-stu-id="831d2-183">Create a section group by posting to the sectionGroups collection in the specified section group.</span></span>|
|[<span data-ttu-id="831d2-184">List section groups</span><span class="sxs-lookup"><span data-stu-id="831d2-184">List section groups</span></span>](../api/sectiongroup-list-sectiongroups.md) |<span data-ttu-id="831d2-185">[sectionGroup](sectiongroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="831d2-185">[sectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="831d2-186">指定したセクショングループ内のセクショングループのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="831d2-186">Get collection of section groups in the specified section group.</span></span>|
|[<span data-ttu-id="831d2-187">セクションを作成する</span><span class="sxs-lookup"><span data-stu-id="831d2-187">Create section</span></span>](../api/sectiongroup-post-sections.md) |[<span data-ttu-id="831d2-188">onenoteSection</span><span class="sxs-lookup"><span data-stu-id="831d2-188">onenoteSection</span></span>](onenotesection.md)| <span data-ttu-id="831d2-189">指定したセクショングループ内の sections コレクションに投稿してセクションを作成します。</span><span class="sxs-lookup"><span data-stu-id="831d2-189">Create a section by posting to the sections collection in the specified section group.</span></span>|
|[<span data-ttu-id="831d2-190">List sections</span><span class="sxs-lookup"><span data-stu-id="831d2-190">List sections</span></span>](../api/sectiongroup-list-sections.md) |<span data-ttu-id="831d2-191">[onenoteSection](onenotesection.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="831d2-191">[onenoteSection](onenotesection.md) collection</span></span>| <span data-ttu-id="831d2-192">指定したセクショングループ内のセクションのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="831d2-192">Get a collection of sections in the specified section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
