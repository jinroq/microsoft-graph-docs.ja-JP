# <a name="sectiongroup-resource-type"></a><span data-ttu-id="0c328-101">sectionGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0c328-101">sectionGroup resource type</span></span>

<span data-ttu-id="0c328-p101">OneNote ノートブックのセクション グループ。セクション グループには、セクションとセクション グループを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="0c328-p101">A section group in a OneNote notebook. Section groups can contain sections and section groups.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c328-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0c328-104">JSON representation</span></span>

<span data-ttu-id="0c328-105">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0c328-105">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="0c328-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c328-106">Properties</span></span>
| <span data-ttu-id="0c328-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c328-107">Property</span></span>     | <span data-ttu-id="0c328-108">型</span><span class="sxs-lookup"><span data-stu-id="0c328-108">Type</span></span>   |<span data-ttu-id="0c328-109">説明</span><span class="sxs-lookup"><span data-stu-id="0c328-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c328-110">createdBy</span><span class="sxs-lookup"><span data-stu-id="0c328-110">createdBy</span></span>|[<span data-ttu-id="0c328-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="0c328-111">identitySet</span></span>](identityset.md)|<span data-ttu-id="0c328-p102">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="0c328-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="0c328-114">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0c328-114">createdDateTime</span></span>|<span data-ttu-id="0c328-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c328-115">DateTimeOffset</span></span>|<span data-ttu-id="0c328-p103">セクション グループが作成された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0c328-p103">The date and time when the section group was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="0c328-120">id</span><span class="sxs-lookup"><span data-stu-id="0c328-120">id</span></span>|<span data-ttu-id="0c328-121">String</span><span class="sxs-lookup"><span data-stu-id="0c328-121">String</span></span>|<span data-ttu-id="0c328-p104">セクション グループの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0c328-p104">The unique identifier of the section group. Read-only.</span></span>|
|<span data-ttu-id="0c328-124">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="0c328-124">lastModifiedBy</span></span>|[<span data-ttu-id="0c328-125">identitySet</span><span class="sxs-lookup"><span data-stu-id="0c328-125">identitySet</span></span>](identityset.md)|<span data-ttu-id="0c328-p105">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0c328-p105">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="0c328-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0c328-128">lastModifiedDateTime</span></span>|<span data-ttu-id="0c328-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c328-129">DateTimeOffset</span></span>|<span data-ttu-id="0c328-p106">セクション グループが最後に変更された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0c328-p106">The date and time when the section group was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="0c328-134">displayName</span><span class="sxs-lookup"><span data-stu-id="0c328-134">displayName</span></span>|<span data-ttu-id="0c328-135">String</span><span class="sxs-lookup"><span data-stu-id="0c328-135">String</span></span>|<span data-ttu-id="0c328-136">セクション グループの名前。</span><span class="sxs-lookup"><span data-stu-id="0c328-136">The name of the section group.</span></span>|
|<span data-ttu-id="0c328-137">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="0c328-137">sectionGroupsUrl</span></span>|<span data-ttu-id="0c328-138">String</span><span class="sxs-lookup"><span data-stu-id="0c328-138">String</span></span>|<span data-ttu-id="0c328-p107">セクション グループ内のすべてのセクション グループを返す `sectionGroups` ナビゲーション プロパティの URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0c328-p107">The URL for the `sectionGroups` navigation property, which returns all the section groups in the section group. Read-only.</span></span>|
|<span data-ttu-id="0c328-141">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="0c328-141">sectionsUrl</span></span>|<span data-ttu-id="0c328-142">String</span><span class="sxs-lookup"><span data-stu-id="0c328-142">String</span></span>|<span data-ttu-id="0c328-p108">セクション グループ内のすべてのセクションを返す `sections` ナビゲーション プロパティの URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0c328-p108">The URL for the `sections` navigation property, which returns all the sections in the section group. Read-only.</span></span>|
|<span data-ttu-id="0c328-145">self</span><span class="sxs-lookup"><span data-stu-id="0c328-145">self</span></span>|<span data-ttu-id="0c328-146">String</span><span class="sxs-lookup"><span data-stu-id="0c328-146">String</span></span>|<span data-ttu-id="0c328-p109">セクション グループに関する詳細情報を入手できるエンドポイント。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0c328-p109">The endpoint where you can get details about the section group. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c328-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0c328-149">Relationships</span></span>
| <span data-ttu-id="0c328-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0c328-150">Relationship</span></span> | <span data-ttu-id="0c328-151">型</span><span class="sxs-lookup"><span data-stu-id="0c328-151">Type</span></span>   |<span data-ttu-id="0c328-152">説明</span><span class="sxs-lookup"><span data-stu-id="0c328-152">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c328-153">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="0c328-153">parentNotebook</span></span>|[<span data-ttu-id="0c328-154">Notebook</span><span class="sxs-lookup"><span data-stu-id="0c328-154">Notebook</span></span>](notebook.md)|<span data-ttu-id="0c328-p110">セクション グループを含むノートブック。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0c328-p110">The notebook that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="0c328-157">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="0c328-157">parentSectionGroup</span></span>|[<span data-ttu-id="0c328-158">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="0c328-158">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="0c328-p111">セクション グループを含むセクション グループ。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0c328-p111">The section group that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="0c328-161">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="0c328-161">sectionGroups</span></span>|<span data-ttu-id="0c328-162">[SectionGroup](sectiongroup.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0c328-162">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="0c328-p112">セクション内のセクション グループ。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="0c328-p112">The section groups in the section. Read-only. Nullable.</span></span>|
|<span data-ttu-id="0c328-166">sections</span><span class="sxs-lookup"><span data-stu-id="0c328-166">sections</span></span>|<span data-ttu-id="0c328-167">[Section](section.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0c328-167">[Section](section.md) collection</span></span>|<span data-ttu-id="0c328-p113">セクション グループ内のセクション。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="0c328-p113">The sections in the section group. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="0c328-171">メソッド</span><span class="sxs-lookup"><span data-stu-id="0c328-171">Methods</span></span>

| <span data-ttu-id="0c328-172">メソッド</span><span class="sxs-lookup"><span data-stu-id="0c328-172">Method</span></span>           | <span data-ttu-id="0c328-173">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0c328-173">Return Type</span></span>    |<span data-ttu-id="0c328-174">説明</span><span class="sxs-lookup"><span data-stu-id="0c328-174">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0c328-175">Get section group</span><span class="sxs-lookup"><span data-stu-id="0c328-175">Get section group</span></span>](../api/sectiongroup_get.md) | [<span data-ttu-id="0c328-176">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="0c328-176">SectionGroup</span></span>](sectiongroup.md) |<span data-ttu-id="0c328-177">セクション グループのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0c328-177">Read the properties and relationships of the section group.</span></span>|
|[<span data-ttu-id="0c328-178">Create section group</span><span class="sxs-lookup"><span data-stu-id="0c328-178">Create section group</span></span>](../api/sectiongroup_post_sectiongroups.md) |[<span data-ttu-id="0c328-179">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="0c328-179">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="0c328-180">指定したセクション グループで sectionGroup コレクションに投稿してセクション グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="0c328-180">Create a section group by posting to the sectionGroups collection in the specified section group.</span></span>|
|[<span data-ttu-id="0c328-181">List section groups</span><span class="sxs-lookup"><span data-stu-id="0c328-181">List section groups</span></span>](../api/sectiongroup_list_sectiongroups.md) |<span data-ttu-id="0c328-182">[SectionGroup](sectiongroup.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0c328-182">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="0c328-183">指定されたセクション グループ内のセクション グループのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="0c328-183">Get collection of section groups in the specified section group.</span></span>|
|[<span data-ttu-id="0c328-184">Create section</span><span class="sxs-lookup"><span data-stu-id="0c328-184">Create section</span></span>](../api/sectiongroup_post_sections.md) |[<span data-ttu-id="0c328-185">Section</span><span class="sxs-lookup"><span data-stu-id="0c328-185">Section</span></span>](section.md)| <span data-ttu-id="0c328-186">指定されたセクション グループでセクションのコレクションを投稿してセクションを作成します。</span><span class="sxs-lookup"><span data-stu-id="0c328-186">Create a section by posting to the sections collection in the specified section group.</span></span>|
|[<span data-ttu-id="0c328-187">List sections</span><span class="sxs-lookup"><span data-stu-id="0c328-187">List sections</span></span>](../api/sectiongroup_list_sections.md) |<span data-ttu-id="0c328-188">[Section](section.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0c328-188">[Section](section.md) collection</span></span>| <span data-ttu-id="0c328-189">指定されたセクション グループ内のセクションのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="0c328-189">Get a collection of sections in the specified section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
