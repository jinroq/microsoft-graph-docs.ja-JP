---
title: sectionGroup リソースの種類
description: OneNote ノートブックのセクション グループ。セクション グループには、セクションとセクション グループを含めることができます。
localization_priority: Normal
ms.openlocfilehash: f204c5422eb5f0f2580bfbed82ed28306dd0618f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806308"
---
# <a name="sectiongroup-resource-type"></a><span data-ttu-id="220ee-104">sectionGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="220ee-104">sectionGroup resource type</span></span>

<span data-ttu-id="220ee-p102">OneNote ノートブックのセクション グループ。セクション グループには、セクションとセクション グループを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="220ee-p102">A section group in a OneNote notebook. Section groups can contain sections and section groups.</span></span>

## <a name="json-representation"></a><span data-ttu-id="220ee-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="220ee-107">JSON representation</span></span>

<span data-ttu-id="220ee-108">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="220ee-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="220ee-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="220ee-109">Properties</span></span>
| <span data-ttu-id="220ee-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="220ee-110">Property</span></span>     | <span data-ttu-id="220ee-111">種類</span><span class="sxs-lookup"><span data-stu-id="220ee-111">Type</span></span>   |<span data-ttu-id="220ee-112">説明</span><span class="sxs-lookup"><span data-stu-id="220ee-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="220ee-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="220ee-113">createdBy</span></span>|[<span data-ttu-id="220ee-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="220ee-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="220ee-p103">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="220ee-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="220ee-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="220ee-117">createdDateTime</span></span>|<span data-ttu-id="220ee-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="220ee-118">DateTimeOffset</span></span>|<span data-ttu-id="220ee-p104">セクション グループが作成された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="220ee-p104">The date and time when the section group was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="220ee-123">id</span><span class="sxs-lookup"><span data-stu-id="220ee-123">id</span></span>|<span data-ttu-id="220ee-124">String</span><span class="sxs-lookup"><span data-stu-id="220ee-124">String</span></span>|<span data-ttu-id="220ee-p105">セクション グループの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="220ee-p105">The unique identifier of the section group. Read-only.</span></span>|
|<span data-ttu-id="220ee-127">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="220ee-127">lastModifiedBy</span></span>|[<span data-ttu-id="220ee-128">identitySet</span><span class="sxs-lookup"><span data-stu-id="220ee-128">identitySet</span></span>](identityset.md)|<span data-ttu-id="220ee-p106">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="220ee-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="220ee-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="220ee-131">lastModifiedDateTime</span></span>|<span data-ttu-id="220ee-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="220ee-132">DateTimeOffset</span></span>|<span data-ttu-id="220ee-p107">セクション グループが最後に変更された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="220ee-p107">The date and time when the section group was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="220ee-137">displayName</span><span class="sxs-lookup"><span data-stu-id="220ee-137">displayName</span></span>|<span data-ttu-id="220ee-138">String</span><span class="sxs-lookup"><span data-stu-id="220ee-138">String</span></span>|<span data-ttu-id="220ee-139">セクション グループの名前。</span><span class="sxs-lookup"><span data-stu-id="220ee-139">The name of the section group.</span></span>|
|<span data-ttu-id="220ee-140">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="220ee-140">sectionGroupsUrl</span></span>|<span data-ttu-id="220ee-141">String</span><span class="sxs-lookup"><span data-stu-id="220ee-141">String</span></span>|<span data-ttu-id="220ee-p108">セクション グループ内のすべてのセクション グループを返す `sectionGroups` ナビゲーション プロパティの URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="220ee-p108">The URL for the `sectionGroups` navigation property, which returns all the section groups in the section group. Read-only.</span></span>|
|<span data-ttu-id="220ee-144">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="220ee-144">sectionsUrl</span></span>|<span data-ttu-id="220ee-145">String</span><span class="sxs-lookup"><span data-stu-id="220ee-145">String</span></span>|<span data-ttu-id="220ee-p109">セクション グループ内のすべてのセクションを返す `sections` ナビゲーション プロパティの URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="220ee-p109">The URL for the `sections` navigation property, which returns all the sections in the section group. Read-only.</span></span>|
|<span data-ttu-id="220ee-148">self</span><span class="sxs-lookup"><span data-stu-id="220ee-148">self</span></span>|<span data-ttu-id="220ee-149">String</span><span class="sxs-lookup"><span data-stu-id="220ee-149">String</span></span>|<span data-ttu-id="220ee-p110">セクション グループに関する詳細情報を入手できるエンドポイント。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="220ee-p110">The endpoint where you can get details about the section group. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="220ee-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="220ee-152">Relationships</span></span>
| <span data-ttu-id="220ee-153">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="220ee-153">Relationship</span></span> | <span data-ttu-id="220ee-154">型</span><span class="sxs-lookup"><span data-stu-id="220ee-154">Type</span></span>   |<span data-ttu-id="220ee-155">説明</span><span class="sxs-lookup"><span data-stu-id="220ee-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="220ee-156">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="220ee-156">parentNotebook</span></span>|[<span data-ttu-id="220ee-157">Notebook</span><span class="sxs-lookup"><span data-stu-id="220ee-157">Notebook</span></span>](notebook.md)|<span data-ttu-id="220ee-p111">セクション グループを含むノートブック。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="220ee-p111">The notebook that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="220ee-160">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="220ee-160">parentSectionGroup</span></span>|[<span data-ttu-id="220ee-161">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="220ee-161">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="220ee-p112">セクション グループを含むセクション グループ。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="220ee-p112">The section group that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="220ee-164">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="220ee-164">sectionGroups</span></span>|<span data-ttu-id="220ee-165">[SectionGroup](sectiongroup.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="220ee-165">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="220ee-p113">セクション内のセクション グループ。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="220ee-p113">The section groups in the section. Read-only. Nullable.</span></span>|
|<span data-ttu-id="220ee-169">sections</span><span class="sxs-lookup"><span data-stu-id="220ee-169">sections</span></span>|<span data-ttu-id="220ee-170">[OnenoteSection](section.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="220ee-170">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="220ee-p114">セクション グループ内のセクション。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="220ee-p114">The sections in the section group. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="220ee-174">メソッド</span><span class="sxs-lookup"><span data-stu-id="220ee-174">Methods</span></span>

| <span data-ttu-id="220ee-175">メソッド</span><span class="sxs-lookup"><span data-stu-id="220ee-175">Method</span></span>           | <span data-ttu-id="220ee-176">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="220ee-176">Return Type</span></span>    |<span data-ttu-id="220ee-177">説明</span><span class="sxs-lookup"><span data-stu-id="220ee-177">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="220ee-178">Get section group</span><span class="sxs-lookup"><span data-stu-id="220ee-178">Get section group</span></span>](../api/sectiongroup-get.md) | [<span data-ttu-id="220ee-179">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="220ee-179">SectionGroup</span></span>](sectiongroup.md) |<span data-ttu-id="220ee-180">セクション グループのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="220ee-180">Read the properties and relationships of the section group.</span></span>|
|[<span data-ttu-id="220ee-181">Create section group</span><span class="sxs-lookup"><span data-stu-id="220ee-181">Create section group</span></span>](../api/sectiongroup-post-sectiongroups.md) |[<span data-ttu-id="220ee-182">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="220ee-182">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="220ee-183">指定したセクション グループで sectionGroup コレクションに投稿してセクション グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="220ee-183">Create a section group by posting to the sectionGroups collection in the specified section group.</span></span>|
|[<span data-ttu-id="220ee-184">List section groups</span><span class="sxs-lookup"><span data-stu-id="220ee-184">List section groups</span></span>](../api/sectiongroup-list-sectiongroups.md) |<span data-ttu-id="220ee-185">[SectionGroup](sectiongroup.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="220ee-185">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="220ee-186">指定されたセクション グループ内のセクション グループのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="220ee-186">Get collection of section groups in the specified section group.</span></span>|
|[<span data-ttu-id="220ee-187">Create section</span><span class="sxs-lookup"><span data-stu-id="220ee-187">Create section</span></span>](../api/sectiongroup-post-sections.md) |[<span data-ttu-id="220ee-188">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="220ee-188">OnenoteSection</span></span>](section.md)| <span data-ttu-id="220ee-189">指定されたセクション グループでセクションのコレクションを投稿してセクションを作成します。</span><span class="sxs-lookup"><span data-stu-id="220ee-189">Create a section by posting to the sections collection in the specified section group.</span></span>|
|[<span data-ttu-id="220ee-190">List sections</span><span class="sxs-lookup"><span data-stu-id="220ee-190">List sections</span></span>](../api/sectiongroup-list-sections.md) |<span data-ttu-id="220ee-191">[OnenoteSection](section.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="220ee-191">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="220ee-192">指定されたセクション グループ内のセクションのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="220ee-192">Get a collection of sections in the specified section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
