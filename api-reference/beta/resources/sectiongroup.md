---
title: sectionGroup リソースの種類
description: OneNote ノートブックのセクション グループ。セクション グループには、セクションとセクション グループを含めることができます。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 8ecd8633b3311459368a16477be391778087882c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976759"
---
# <a name="sectiongroup-resource-type"></a><span data-ttu-id="c96e0-104">sectionGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c96e0-104">sectionGroup resource type</span></span>

> <span data-ttu-id="c96e0-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c96e0-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c96e0-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c96e0-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c96e0-p103">OneNote ノートブックのセクション グループ。セクション グループには、セクションとセクション グループを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="c96e0-p103">A section group in a OneNote notebook. Section groups can contain sections and section groups.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c96e0-109">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c96e0-109">JSON representation</span></span>

<span data-ttu-id="c96e0-110">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c96e0-110">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "parentNotebook",
    "parentSectionGroup",
    "sectionGroups",
    "sections"
  ],
  "@odata.type": "microsoft.graph.sectiongroup"
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
## <a name="properties"></a><span data-ttu-id="c96e0-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c96e0-111">Properties</span></span>
| <span data-ttu-id="c96e0-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c96e0-112">Property</span></span>     | <span data-ttu-id="c96e0-113">型</span><span class="sxs-lookup"><span data-stu-id="c96e0-113">Type</span></span>   |<span data-ttu-id="c96e0-114">説明</span><span class="sxs-lookup"><span data-stu-id="c96e0-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c96e0-115">createdBy</span><span class="sxs-lookup"><span data-stu-id="c96e0-115">createdBy</span></span>|[<span data-ttu-id="c96e0-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="c96e0-116">identitySet</span></span>](identityset.md)|<span data-ttu-id="c96e0-p104">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c96e0-p104">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="c96e0-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c96e0-119">createdDateTime</span></span>|<span data-ttu-id="c96e0-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c96e0-120">DateTimeOffset</span></span>|<span data-ttu-id="c96e0-p105">セクション グループが作成された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c96e0-p105">The date and time when the section group was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="c96e0-125">id</span><span class="sxs-lookup"><span data-stu-id="c96e0-125">id</span></span>|<span data-ttu-id="c96e0-126">String</span><span class="sxs-lookup"><span data-stu-id="c96e0-126">String</span></span>|<span data-ttu-id="c96e0-p106">セクション グループの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c96e0-p106">The unique identifier of the section group. Read-only.</span></span>|
|<span data-ttu-id="c96e0-129">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="c96e0-129">lastModifiedBy</span></span>|[<span data-ttu-id="c96e0-130">identitySet</span><span class="sxs-lookup"><span data-stu-id="c96e0-130">identitySet</span></span>](identityset.md)|<span data-ttu-id="c96e0-p107">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c96e0-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="c96e0-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c96e0-133">lastModifiedDateTime</span></span>|<span data-ttu-id="c96e0-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c96e0-134">DateTimeOffset</span></span>|<span data-ttu-id="c96e0-p108">セクション グループが最後に変更された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c96e0-p108">The date and time when the section group was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="c96e0-139">displayName</span><span class="sxs-lookup"><span data-stu-id="c96e0-139">displayName</span></span>|<span data-ttu-id="c96e0-140">String</span><span class="sxs-lookup"><span data-stu-id="c96e0-140">String</span></span>|<span data-ttu-id="c96e0-141">セクション グループの名前。</span><span class="sxs-lookup"><span data-stu-id="c96e0-141">The name of the section group.</span></span>|
|<span data-ttu-id="c96e0-142">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="c96e0-142">sectionGroupsUrl</span></span>|<span data-ttu-id="c96e0-143">String</span><span class="sxs-lookup"><span data-stu-id="c96e0-143">String</span></span>|<span data-ttu-id="c96e0-p109">セクション グループ内のすべてのセクション グループを返す `sectionGroups` ナビゲーション プロパティの URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c96e0-p109">The URL for the `sectionGroups` navigation property, which returns all the section groups in the section group. Read-only.</span></span>|
|<span data-ttu-id="c96e0-146">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="c96e0-146">sectionsUrl</span></span>|<span data-ttu-id="c96e0-147">String</span><span class="sxs-lookup"><span data-stu-id="c96e0-147">String</span></span>|<span data-ttu-id="c96e0-p110">セクション グループ内のすべてのセクションを返す `sections` ナビゲーション プロパティの URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c96e0-p110">The URL for the `sections` navigation property, which returns all the sections in the section group. Read-only.</span></span>|
|<span data-ttu-id="c96e0-150">self</span><span class="sxs-lookup"><span data-stu-id="c96e0-150">self</span></span>|<span data-ttu-id="c96e0-151">String</span><span class="sxs-lookup"><span data-stu-id="c96e0-151">String</span></span>|<span data-ttu-id="c96e0-p111">セクション グループに関する詳細情報を入手できるエンドポイント。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c96e0-p111">The endpoint where you can get details about the section group. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c96e0-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c96e0-154">Relationships</span></span>
| <span data-ttu-id="c96e0-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c96e0-155">Relationship</span></span> | <span data-ttu-id="c96e0-156">型</span><span class="sxs-lookup"><span data-stu-id="c96e0-156">Type</span></span>   |<span data-ttu-id="c96e0-157">説明</span><span class="sxs-lookup"><span data-stu-id="c96e0-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c96e0-158">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="c96e0-158">parentNotebook</span></span>|[<span data-ttu-id="c96e0-159">Notebook</span><span class="sxs-lookup"><span data-stu-id="c96e0-159">Notebook</span></span>](notebook.md)|<span data-ttu-id="c96e0-p112">セクション グループを含むノートブック。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c96e0-p112">The notebook that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="c96e0-162">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="c96e0-162">parentSectionGroup</span></span>|[<span data-ttu-id="c96e0-163">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="c96e0-163">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="c96e0-p113">セクション グループを含むセクション グループ。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c96e0-p113">The section group that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="c96e0-166">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="c96e0-166">sectionGroups</span></span>|<span data-ttu-id="c96e0-167">[SectionGroup](sectiongroup.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c96e0-167">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="c96e0-p114">セクション内のセクション グループ。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="c96e0-p114">The section groups in the section. Read-only. Nullable.</span></span>|
|<span data-ttu-id="c96e0-171">sections</span><span class="sxs-lookup"><span data-stu-id="c96e0-171">sections</span></span>|<span data-ttu-id="c96e0-172">[Section](section.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c96e0-172">[Section](section.md) collection</span></span>|<span data-ttu-id="c96e0-p115">セクション グループ内のセクション。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="c96e0-p115">The sections in the section group. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="c96e0-176">メソッド</span><span class="sxs-lookup"><span data-stu-id="c96e0-176">Methods</span></span>

| <span data-ttu-id="c96e0-177">メソッド</span><span class="sxs-lookup"><span data-stu-id="c96e0-177">Method</span></span>           | <span data-ttu-id="c96e0-178">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c96e0-178">Return Type</span></span>    |<span data-ttu-id="c96e0-179">説明</span><span class="sxs-lookup"><span data-stu-id="c96e0-179">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c96e0-180">Get section group</span><span class="sxs-lookup"><span data-stu-id="c96e0-180">Get section group</span></span>](../api/sectiongroup-get.md) | [<span data-ttu-id="c96e0-181">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="c96e0-181">SectionGroup</span></span>](sectiongroup.md) |<span data-ttu-id="c96e0-182">セクション グループのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c96e0-182">Read the properties and relationships of the section group.</span></span>|
|[<span data-ttu-id="c96e0-183">Create section group</span><span class="sxs-lookup"><span data-stu-id="c96e0-183">Create section group</span></span>](../api/sectiongroup-post-sectiongroups.md) |[<span data-ttu-id="c96e0-184">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="c96e0-184">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="c96e0-185">指定したセクション グループで sectionGroup コレクションに投稿してセクション グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="c96e0-185">Create a section group by posting to the sectionGroups collection in the specified section group.</span></span>|
|[<span data-ttu-id="c96e0-186">List section groups</span><span class="sxs-lookup"><span data-stu-id="c96e0-186">List section groups</span></span>](../api/sectiongroup-list-sectiongroups.md) |<span data-ttu-id="c96e0-187">[SectionGroup](sectiongroup.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c96e0-187">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="c96e0-188">指定されたセクション グループ内のセクション グループのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="c96e0-188">Get collection of section groups in the specified section group.</span></span>|
|[<span data-ttu-id="c96e0-189">Create section</span><span class="sxs-lookup"><span data-stu-id="c96e0-189">Create section</span></span>](../api/sectiongroup-post-sections.md) |[<span data-ttu-id="c96e0-190">Section</span><span class="sxs-lookup"><span data-stu-id="c96e0-190">Section</span></span>](section.md)| <span data-ttu-id="c96e0-191">指定されたセクション グループでセクションのコレクションを投稿してセクションを作成します。</span><span class="sxs-lookup"><span data-stu-id="c96e0-191">Create a section by posting to the sections collection in the specified section group.</span></span>|
|[<span data-ttu-id="c96e0-192">List sections</span><span class="sxs-lookup"><span data-stu-id="c96e0-192">List sections</span></span>](../api/sectiongroup-list-sections.md) |<span data-ttu-id="c96e0-193">[Section](section.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c96e0-193">[Section](section.md) collection</span></span>| <span data-ttu-id="c96e0-194">指定されたセクション グループ内のセクションのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="c96e0-194">Get a collection of sections in the specified section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
