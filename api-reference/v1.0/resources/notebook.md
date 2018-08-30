# <a name="notebook-resource-type"></a><span data-ttu-id="a2184-101">notebook リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a2184-101">notebook resource type</span></span>

<span data-ttu-id="a2184-102">OneNote ノートブックです。</span><span class="sxs-lookup"><span data-stu-id="a2184-102">A OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a2184-103">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a2184-103">JSON representation</span></span>

<span data-ttu-id="a2184-104">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="a2184-104">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityHierarchyModel",
  "optionalProperties": [
    "sectionGroups",
    "sections"
  ],
  "@odata.type": "microsoft.graph.notebook"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isDefault": true,
  "isShared": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.notebookLinks"},
  "displayName": "string",
  "sectionGroupsUrl": "string",
  "sectionsUrl": "string",
  "self": "string",
  "userRole": "String"
}

```
## <a name="properties"></a><span data-ttu-id="a2184-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2184-105">Properties</span></span>
| <span data-ttu-id="a2184-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2184-106">Property</span></span>     | <span data-ttu-id="a2184-107">タイプ</span><span class="sxs-lookup"><span data-stu-id="a2184-107">Type</span></span>   |<span data-ttu-id="a2184-108">説明</span><span class="sxs-lookup"><span data-stu-id="a2184-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2184-109">createdBy</span><span class="sxs-lookup"><span data-stu-id="a2184-109">createdBy</span></span>|[<span data-ttu-id="a2184-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="a2184-110">identitySet</span></span>](identityset.md)|<span data-ttu-id="a2184-p101">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a2184-p101">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="a2184-113">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a2184-113">createdDateTime</span></span>|<span data-ttu-id="a2184-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2184-114">DateTimeOffset</span></span>|<span data-ttu-id="a2184-p102">ノートブックが作成された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a2184-p102">The date and time when the notebook was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="a2184-119">id</span><span class="sxs-lookup"><span data-stu-id="a2184-119">id</span></span>|<span data-ttu-id="a2184-120">String</span><span class="sxs-lookup"><span data-stu-id="a2184-120">String</span></span>|<span data-ttu-id="a2184-p103">ノートブックの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a2184-p103">The unique identifier of the notebook. Read-only.</span></span>|
|<span data-ttu-id="a2184-123">isDefault</span><span class="sxs-lookup"><span data-stu-id="a2184-123">isDefault</span></span>|<span data-ttu-id="a2184-124">ブール型</span><span class="sxs-lookup"><span data-stu-id="a2184-124">Boolean</span></span>|<span data-ttu-id="a2184-p104">これがユーザーの既定のノートブックであるかどうかを示します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a2184-p104">Indicates whether this is the user's default notebook. Read-only.</span></span>|
|<span data-ttu-id="a2184-127">IsShared</span><span class="sxs-lookup"><span data-stu-id="a2184-127">isShared</span></span>|<span data-ttu-id="a2184-128">ブール型</span><span class="sxs-lookup"><span data-stu-id="a2184-128">Boolean</span></span>|<span data-ttu-id="a2184-p105">ノートブックを共有するかどうかを示します。True の場合、所有者以外のユーザーにノートブックのコンテンツが表示されます。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a2184-p105">Indicates whether the notebook is shared. If true, the contents of the notebook can be seen by people other than the owner. Read-only.</span></span>|
|<span data-ttu-id="a2184-132">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="a2184-132">lastModifiedBy</span></span>|[<span data-ttu-id="a2184-133">identitySet</span><span class="sxs-lookup"><span data-stu-id="a2184-133">identitySet</span></span>](identityset.md)|<span data-ttu-id="a2184-p106">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a2184-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="a2184-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a2184-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a2184-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2184-137">DateTimeOffset</span></span>|<span data-ttu-id="a2184-p107">ノートブックが最後に変更された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a2184-p107">The date and time when the notebook was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="a2184-142">links</span><span class="sxs-lookup"><span data-stu-id="a2184-142">links</span></span>|[<span data-ttu-id="a2184-143">NotebookLinks</span><span class="sxs-lookup"><span data-stu-id="a2184-143">NotebookLinks</span></span>](notebooklinks.md)|<span data-ttu-id="a2184-p108">ノートブックを開くためのリンク。`oneNoteClientURL` リンクが OneNote のネイティブ クライアントでノートブックを開きます (インストールされている場合)。`oneNoteWebURL` リンクでは、OneNote Online でノートブックを開きます。</span><span class="sxs-lookup"><span data-stu-id="a2184-p108">Links for opening the notebook. The `oneNoteClientURL` link opens the notebook in the OneNote native client if it's installed. The `oneNoteWebURL` link opens the notebook in OneNote Online.</span></span>|
|<span data-ttu-id="a2184-147">displayName</span><span class="sxs-lookup"><span data-stu-id="a2184-147">displayName</span></span>|<span data-ttu-id="a2184-148">String</span><span class="sxs-lookup"><span data-stu-id="a2184-148">String</span></span>|<span data-ttu-id="a2184-149">ノートブックの名前。</span><span class="sxs-lookup"><span data-stu-id="a2184-149">The name of the notebook.</span></span>|
|<span data-ttu-id="a2184-150">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="a2184-150">sectionGroupsUrl</span></span>|<span data-ttu-id="a2184-151">String</span><span class="sxs-lookup"><span data-stu-id="a2184-151">String</span></span>|<span data-ttu-id="a2184-p109">ノートブック内のすべてのセクション グループを返す `sectionGroups` ナビゲーション プロパティの URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a2184-p109">The URL for the `sectionGroups` navigation property, which returns all the section groups in the notebook. Read-only.</span></span>|
|<span data-ttu-id="a2184-154">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="a2184-154">sectionsUrl</span></span>|<span data-ttu-id="a2184-155">String</span><span class="sxs-lookup"><span data-stu-id="a2184-155">String</span></span>|<span data-ttu-id="a2184-p110">ノートブック内のすべてのセクションを返す `sections` ナビゲーション プロパティの URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a2184-p110">The URL for the `sections` navigation property, which returns all the sections in the notebook. Read-only.</span></span>|
|<span data-ttu-id="a2184-158">self</span><span class="sxs-lookup"><span data-stu-id="a2184-158">self</span></span>|<span data-ttu-id="a2184-159">String</span><span class="sxs-lookup"><span data-stu-id="a2184-159">String</span></span>|<span data-ttu-id="a2184-p111">ノートブックに関する詳細情報を入手できるエンドポイント。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a2184-p111">The endpoint where you can get details about the notebook. Read-only.</span></span>|
|<span data-ttu-id="a2184-162">userRole</span><span class="sxs-lookup"><span data-stu-id="a2184-162">userRole</span></span>|<span data-ttu-id="a2184-163">onenoteUserRole</span><span class="sxs-lookup"><span data-stu-id="a2184-163">onenoteUserRole values</span></span>|<span data-ttu-id="a2184-p112">使用可能な値: `Owner`、`Contributor`、`Reader`、`None`。Owner は、ノートブックへの所有者レベルのアクセス権を表します。Contributor は、ノートブックへの読み取り/書き込みアクセス権を表します。Reader は、ノートブックへの読み取り専用アクセス権を表します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a2184-p112">Possible values are: `Owner`, `Contributor`, `Reader`, `None`. Owner represents owner-level access to the notebook. Contributor represents read/write access to the notebook. Reader represents read-only access to the notebook. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2184-169">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a2184-169">Relationships</span></span>
| <span data-ttu-id="a2184-170">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a2184-170">Relationship</span></span> | <span data-ttu-id="a2184-171">型</span><span class="sxs-lookup"><span data-stu-id="a2184-171">Type</span></span>   |<span data-ttu-id="a2184-172">説明</span><span class="sxs-lookup"><span data-stu-id="a2184-172">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2184-173">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="a2184-173">sectionGroups</span></span>|<span data-ttu-id="a2184-174">[SectionGroup](sectiongroup.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a2184-174">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="a2184-p113">ノートブック内のセクション グループ。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="a2184-p113">The section groups in the notebook. Read-only. Nullable.</span></span>|
|<span data-ttu-id="a2184-178">sections</span><span class="sxs-lookup"><span data-stu-id="a2184-178">sections</span></span>|<span data-ttu-id="a2184-179">[OnenoteSection](section.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a2184-179">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="a2184-p114">ノートブック内のセクション。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="a2184-p114">The sections in the notebook. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="a2184-183">メソッド</span><span class="sxs-lookup"><span data-stu-id="a2184-183">Methods</span></span>

| <span data-ttu-id="a2184-184">メソッド</span><span class="sxs-lookup"><span data-stu-id="a2184-184">Method</span></span>           | <span data-ttu-id="a2184-185">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a2184-185">Return Type</span></span>    |<span data-ttu-id="a2184-186">説明</span><span class="sxs-lookup"><span data-stu-id="a2184-186">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a2184-187">Get notebook</span><span class="sxs-lookup"><span data-stu-id="a2184-187">Get notebook</span></span>](../api/notebook_get.md) | [<span data-ttu-id="a2184-188">Notebook</span><span class="sxs-lookup"><span data-stu-id="a2184-188">Notebook</span></span>](notebook.md) |<span data-ttu-id="a2184-189">ノートブックのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a2184-189">Read the properties and relationships of the notebook.</span></span>|
|[<span data-ttu-id="a2184-190">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="a2184-190">getRecentNotebooks</span></span>](../api/notebook_getrecentnotebooks.md) | <span data-ttu-id="a2184-191">[recentNotebook](recentnotebook.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a2184-191">[recentNotebook](recentnotebook.md) collection</span></span> | <span data-ttu-id="a2184-192">ユーザーの最近アクセスしたノートブックのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="a2184-192">Get a collection of the most recently accessed notebooks for the user.</span></span> |
|[<span data-ttu-id="a2184-193">Create section group</span><span class="sxs-lookup"><span data-stu-id="a2184-193">Create section group</span></span>](../api/notebook_post_sectiongroups.md) |[<span data-ttu-id="a2184-194">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="a2184-194">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="a2184-195">指定したノートブックで sectionGroup コレクションに投稿してセクション グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="a2184-195">Create a section group by posting to the sectionGroups collection in the specified notebook.</span></span>|
|[<span data-ttu-id="a2184-196">List section groups</span><span class="sxs-lookup"><span data-stu-id="a2184-196">List section groups</span></span>](../api/notebook_list_sectiongroups.md) |<span data-ttu-id="a2184-197">[SectionGroup](sectiongroup.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a2184-197">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="a2184-198">指定されたノートブック内のセクション グループのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="a2184-198">Get a collection of section groups in the specified notebook.</span></span>|
|[<span data-ttu-id="a2184-199">Create section</span><span class="sxs-lookup"><span data-stu-id="a2184-199">Create section</span></span>](../api/notebook_post_sections.md) |[<span data-ttu-id="a2184-200">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="a2184-200">OnenoteSection</span></span>](section.md)| <span data-ttu-id="a2184-201">指定されたノートブックでセクションのコレクションに投稿してセクションを作成します。</span><span class="sxs-lookup"><span data-stu-id="a2184-201">Create a section by posting to the sections collection in the specified notebook.</span></span>|
|[<span data-ttu-id="a2184-202">List sections</span><span class="sxs-lookup"><span data-stu-id="a2184-202">List sections</span></span>](../api/notebook_list_sections.md) |<span data-ttu-id="a2184-203">[OnenoteSection](section.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a2184-203">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="a2184-204">指定されたノートブック内のセクションのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="a2184-204">Get a collection of sections in the specified notebook.</span></span>|
|[<span data-ttu-id="a2184-205">copyNotebook</span><span class="sxs-lookup"><span data-stu-id="a2184-205">copyNotebook</span></span>](../api/notebook_copynotebook.md)| <span data-ttu-id="a2184-206">なし</span><span class="sxs-lookup"><span data-stu-id="a2184-206">None</span></span> | <span data-ttu-id="a2184-207">ノートブックをコピーします。</span><span class="sxs-lookup"><span data-stu-id="a2184-207">Copies a notebook.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
