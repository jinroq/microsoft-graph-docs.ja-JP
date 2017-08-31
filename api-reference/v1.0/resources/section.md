# <a name="section-resource-type"></a><span data-ttu-id="037a9-101">section リソースの種類</span><span class="sxs-lookup"><span data-stu-id="037a9-101">section resource type</span></span>

<span data-ttu-id="037a9-p101">OneNote ノートブックのセクションです。セクションには、ページを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="037a9-p101">A section in a OneNote notebook. Sections can contain pages.</span></span>

## <a name="json-representation"></a><span data-ttu-id="037a9-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="037a9-104">JSON representation</span></span>

<span data-ttu-id="037a9-105">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="037a9-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
## <a name="properties"></a><span data-ttu-id="037a9-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="037a9-106">Properties</span></span>
| <span data-ttu-id="037a9-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="037a9-107">Property</span></span>     | <span data-ttu-id="037a9-108">型</span><span class="sxs-lookup"><span data-stu-id="037a9-108">Type</span></span>   |<span data-ttu-id="037a9-109">説明</span><span class="sxs-lookup"><span data-stu-id="037a9-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="037a9-110">createdBy</span><span class="sxs-lookup"><span data-stu-id="037a9-110">createdBy</span></span>|[<span data-ttu-id="037a9-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="037a9-111">identitySet</span></span>](identityset.md)|<span data-ttu-id="037a9-p102">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="037a9-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="037a9-114">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="037a9-114">createdDateTime</span></span>|<span data-ttu-id="037a9-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="037a9-115">DateTimeOffset</span></span>|<span data-ttu-id="037a9-p103">セクションが作成された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="037a9-p103">The date and time when the section was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="037a9-120">id</span><span class="sxs-lookup"><span data-stu-id="037a9-120">id</span></span>|<span data-ttu-id="037a9-121">String</span><span class="sxs-lookup"><span data-stu-id="037a9-121">String</span></span>|<span data-ttu-id="037a9-p104">セクションの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="037a9-p104">The unique identifier of the section.  Read-only.</span></span>|
|<span data-ttu-id="037a9-124">isDefault</span><span class="sxs-lookup"><span data-stu-id="037a9-124">isDefault</span></span>|<span data-ttu-id="037a9-125">ブール値</span><span class="sxs-lookup"><span data-stu-id="037a9-125">Boolean</span></span>|<span data-ttu-id="037a9-p105">これがユーザーの既定のセクションであるかどうかを示します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="037a9-p105">Indicates whether this is the user's default section. Read-only.</span></span>|
|<span data-ttu-id="037a9-128">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="037a9-128">lastModifiedBy</span></span>|[<span data-ttu-id="037a9-129">identitySet</span><span class="sxs-lookup"><span data-stu-id="037a9-129">identitySet</span></span>](identityset.md)|<span data-ttu-id="037a9-p106">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="037a9-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="037a9-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="037a9-132">lastModifiedDateTime</span></span>|<span data-ttu-id="037a9-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="037a9-133">DateTimeOffset</span></span>|<span data-ttu-id="037a9-p107">セクションが最後に変更された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="037a9-p107">The date and time when the section was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="037a9-138">links</span><span class="sxs-lookup"><span data-stu-id="037a9-138">links</span></span>|[<span data-ttu-id="037a9-139">SectionLinks</span><span class="sxs-lookup"><span data-stu-id="037a9-139">SectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="037a9-p108">セクションを開くためのリンク。`oneNoteClientURL` リンクが OneNote のネイティブ クライアントでセクションを開きます (インストールされている場合)。`oneNoteWebURL` リンクでは、OneNote Online でセクションを開きます。</span><span class="sxs-lookup"><span data-stu-id="037a9-p108">Links for opening the section. The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed. The `oneNoteWebURL` link opens the section in OneNote Online.</span></span>|
|<span data-ttu-id="037a9-143">displayName</span><span class="sxs-lookup"><span data-stu-id="037a9-143">displayName</span></span>|<span data-ttu-id="037a9-144">String</span><span class="sxs-lookup"><span data-stu-id="037a9-144">String</span></span>|<span data-ttu-id="037a9-145">セクションの名前。</span><span class="sxs-lookup"><span data-stu-id="037a9-145">The name of the section.</span></span> |
|<span data-ttu-id="037a9-146">pagesUrl</span><span class="sxs-lookup"><span data-stu-id="037a9-146">pagesUrl</span></span>|<span data-ttu-id="037a9-147">String</span><span class="sxs-lookup"><span data-stu-id="037a9-147">String</span></span>|<span data-ttu-id="037a9-p109">セクション内のすべてのページに関する詳細情報を入手できる `pages` エンドポイント。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="037a9-p109">The `pages` endpoint where you can get details for all the pages in the section. Read-only.</span></span>|
|<span data-ttu-id="037a9-150">self</span><span class="sxs-lookup"><span data-stu-id="037a9-150">self</span></span>|<span data-ttu-id="037a9-151">String</span><span class="sxs-lookup"><span data-stu-id="037a9-151">String</span></span>|<span data-ttu-id="037a9-p110">セクションに関する詳細情報を入手できるエンドポイント。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="037a9-p110">The endpoint where you can get details about the section. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="037a9-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="037a9-154">Relationships</span></span>
| <span data-ttu-id="037a9-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="037a9-155">Relationship</span></span> | <span data-ttu-id="037a9-156">型</span><span class="sxs-lookup"><span data-stu-id="037a9-156">Type</span></span>   |<span data-ttu-id="037a9-157">説明</span><span class="sxs-lookup"><span data-stu-id="037a9-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="037a9-158">pages</span><span class="sxs-lookup"><span data-stu-id="037a9-158">pages</span></span>|<span data-ttu-id="037a9-159">[Page](page.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="037a9-159">[Page](page.md) collection</span></span>|<span data-ttu-id="037a9-p111">セクション内のページのコレクションです。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="037a9-p111">The collection of pages in the section.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="037a9-163">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="037a9-163">parentNotebook</span></span>|[<span data-ttu-id="037a9-164">Notebook</span><span class="sxs-lookup"><span data-stu-id="037a9-164">Notebook</span></span>](notebook.md)|<span data-ttu-id="037a9-p112">セクションを含むノートブック。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="037a9-p112">The notebook that contains the section.  Read-only.</span></span>|
|<span data-ttu-id="037a9-167">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="037a9-167">parentSectionGroup</span></span>|[<span data-ttu-id="037a9-168">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="037a9-168">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="037a9-p113">セクションを含むセクション グループ。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="037a9-p113">The section group that contains the section.  Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="037a9-171">メソッド</span><span class="sxs-lookup"><span data-stu-id="037a9-171">Methods</span></span>

| <span data-ttu-id="037a9-172">メソッド</span><span class="sxs-lookup"><span data-stu-id="037a9-172">Method</span></span>           | <span data-ttu-id="037a9-173">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="037a9-173">Return Type</span></span>    |<span data-ttu-id="037a9-174">説明</span><span class="sxs-lookup"><span data-stu-id="037a9-174">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="037a9-175">Get section</span><span class="sxs-lookup"><span data-stu-id="037a9-175">Get section</span></span>](../api/section_get.md) | [<span data-ttu-id="037a9-176">Section</span><span class="sxs-lookup"><span data-stu-id="037a9-176">Section</span></span>](section.md) |<span data-ttu-id="037a9-177">セクションのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="037a9-177">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="037a9-178">Create page</span><span class="sxs-lookup"><span data-stu-id="037a9-178">Create page</span></span>](../api/section_post_pages.md) |[<span data-ttu-id="037a9-179">Page</span><span class="sxs-lookup"><span data-stu-id="037a9-179">Page</span></span>](page.md)| <span data-ttu-id="037a9-180">指定されたセクションでページのコレクションに投稿してページを作成します。</span><span class="sxs-lookup"><span data-stu-id="037a9-180">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="037a9-181">List pages</span><span class="sxs-lookup"><span data-stu-id="037a9-181">List pages</span></span>](../api/section_list_pages.md) |<span data-ttu-id="037a9-182">[Page](page.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="037a9-182">[Page](page.md) collection</span></span>| <span data-ttu-id="037a9-183">指定されたセクション内のページのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="037a9-183">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="037a9-184">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="037a9-184">copyToNotebook</span></span>](../api/section_copytonotebook.md)|<span data-ttu-id="037a9-185">なし</span><span class="sxs-lookup"><span data-stu-id="037a9-185">None</span></span>|<span data-ttu-id="037a9-186">特定のノートブックにセクションをコピーします。</span><span class="sxs-lookup"><span data-stu-id="037a9-186">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="037a9-187">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="037a9-187">copyToSectionGroup</span></span>](../api/section_copytosectiongroup.md)|<span data-ttu-id="037a9-188">なし</span><span class="sxs-lookup"><span data-stu-id="037a9-188">None</span></span>|<span data-ttu-id="037a9-189">特定のセクション グループにセクションをコピーします。</span><span class="sxs-lookup"><span data-stu-id="037a9-189">Copy the section to a specific section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
