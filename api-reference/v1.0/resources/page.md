# <a name="page-resource-type"></a><span data-ttu-id="31dd3-101">page リソースの種類</span><span class="sxs-lookup"><span data-stu-id="31dd3-101">page resource type</span></span>

<span data-ttu-id="31dd3-102">OneNote ノートブックのページです。</span><span class="sxs-lookup"><span data-stu-id="31dd3-102">A page in a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="31dd3-103">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="31dd3-103">JSON representation</span></span>

<span data-ttu-id="31dd3-104">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="31dd3-104">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntitySchemaObjectModel",
  "optionalProperties": [
    "parentNotebook",
    "parentSection"
  ],
  "isMediaEntity": true,
  "@odata.type": "microsoft.graph.onenotePage"
}-->

```json
{
  "content": "stream",
  "contentUrl": "string",
  "createdByAppId": "string",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "level": 1024,
  "links": {"@odata.type": "microsoft.graph.pageLinks"},
  "order": 1024,
  "self": "string",
  "title": "string"
}

```
## <a name="properties"></a><span data-ttu-id="31dd3-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31dd3-105">Properties</span></span>
| <span data-ttu-id="31dd3-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31dd3-106">Property</span></span>     | <span data-ttu-id="31dd3-107">タイプ</span><span class="sxs-lookup"><span data-stu-id="31dd3-107">Type</span></span>   |<span data-ttu-id="31dd3-108">説明</span><span class="sxs-lookup"><span data-stu-id="31dd3-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31dd3-109">content</span><span class="sxs-lookup"><span data-stu-id="31dd3-109">content</span></span>|<span data-ttu-id="31dd3-110">ストリーム</span><span class="sxs-lookup"><span data-stu-id="31dd3-110">Stream</span></span>|<span data-ttu-id="31dd3-111">ページの HTML コンテンツ。</span><span class="sxs-lookup"><span data-stu-id="31dd3-111">The page's HTML content.</span></span>|
|<span data-ttu-id="31dd3-112">contentUrl</span><span class="sxs-lookup"><span data-stu-id="31dd3-112">contentUrl</span></span>|<span data-ttu-id="31dd3-113">文字列</span><span class="sxs-lookup"><span data-stu-id="31dd3-113">String</span></span>|<span data-ttu-id="31dd3-p101">ページの HTML コンテンツの URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="31dd3-p101">The URL for the page's HTML content.  Read-only.</span></span>|
|<span data-ttu-id="31dd3-116">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="31dd3-116">createdByAppId</span></span>|<span data-ttu-id="31dd3-117">文字列</span><span class="sxs-lookup"><span data-stu-id="31dd3-117">String</span></span>|<span data-ttu-id="31dd3-p102">ページを作成したアプリケーションの一意の識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="31dd3-p102">The unique identifier of the application that created the page. Read-only.</span></span>|
|<span data-ttu-id="31dd3-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="31dd3-120">createdDateTime</span></span>|<span data-ttu-id="31dd3-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31dd3-121">DateTimeOffset</span></span>|<span data-ttu-id="31dd3-p103">ページが作成された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="31dd3-p103">The date and time when the page was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="31dd3-126">ID</span><span class="sxs-lookup"><span data-stu-id="31dd3-126">id</span></span>|<span data-ttu-id="31dd3-127">文字列</span><span class="sxs-lookup"><span data-stu-id="31dd3-127">String</span></span>|<span data-ttu-id="31dd3-p104">ページの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="31dd3-p104">The unique identifier of the page.  Read-only.</span></span>|
|<span data-ttu-id="31dd3-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="31dd3-130">lastModifiedDateTime</span></span>|<span data-ttu-id="31dd3-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31dd3-131">DateTimeOffset</span></span>|<span data-ttu-id="31dd3-p105">ページが最後に変更された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="31dd3-p105">The date and time when the page was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="31dd3-136">level</span><span class="sxs-lookup"><span data-stu-id="31dd3-136">level</span></span>|<span data-ttu-id="31dd3-137">Int32</span><span class="sxs-lookup"><span data-stu-id="31dd3-137">Int32</span></span>|<span data-ttu-id="31dd3-p106">ページのインデント レベル。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="31dd3-p106">The indentation level of the page. Read-only.</span></span>|
|<span data-ttu-id="31dd3-140">links</span><span class="sxs-lookup"><span data-stu-id="31dd3-140">links</span></span>|[<span data-ttu-id="31dd3-141">PageLinks</span><span class="sxs-lookup"><span data-stu-id="31dd3-141">PageLinks</span></span>](pagelinks.md)|<span data-ttu-id="31dd3-p107">ページを開くためのリンク。`oneNoteClientURL`リンクが OneNote のネイティブ クライアントでページを開きます (インストールされている場合)。`oneNoteWebUrl` リンクでは、OneNote オンラインでページを開きます。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="31dd3-p107">Links for opening the page. The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed. The `oneNoteWebUrl` link opens the page in OneNote Online. Read-only.</span></span>|
|<span data-ttu-id="31dd3-146">order</span><span class="sxs-lookup"><span data-stu-id="31dd3-146">order</span></span>|<span data-ttu-id="31dd3-147">Int32</span><span class="sxs-lookup"><span data-stu-id="31dd3-147">Int32</span></span>|<span data-ttu-id="31dd3-p108">親セクション内でのページの順序。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="31dd3-p108">The order of the page within its parent section. Read-only.</span></span>|
|<span data-ttu-id="31dd3-150">self</span><span class="sxs-lookup"><span data-stu-id="31dd3-150">self</span></span>|<span data-ttu-id="31dd3-151">文字列</span><span class="sxs-lookup"><span data-stu-id="31dd3-151">String</span></span>|<span data-ttu-id="31dd3-p109">ページに関する詳細情報を入手できるエンドポイント。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="31dd3-p109">The endpoint where you can get details about the page. Read-only.</span></span>|
|<span data-ttu-id="31dd3-154">タイトル</span><span class="sxs-lookup"><span data-stu-id="31dd3-154">title</span></span>|<span data-ttu-id="31dd3-155">文字列</span><span class="sxs-lookup"><span data-stu-id="31dd3-155">String</span></span>|<span data-ttu-id="31dd3-156">ページのタイトル。</span><span class="sxs-lookup"><span data-stu-id="31dd3-156">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="31dd3-157">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="31dd3-157">Relationships</span></span>
| <span data-ttu-id="31dd3-158">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="31dd3-158">Relationship</span></span> | <span data-ttu-id="31dd3-159">型</span><span class="sxs-lookup"><span data-stu-id="31dd3-159">Type</span></span>   |<span data-ttu-id="31dd3-160">説明</span><span class="sxs-lookup"><span data-stu-id="31dd3-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31dd3-161">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="31dd3-161">parentNotebook</span></span>|[<span data-ttu-id="31dd3-162">ノートブック</span><span class="sxs-lookup"><span data-stu-id="31dd3-162">Notebook</span></span>](notebook.md)|<span data-ttu-id="31dd3-p110">ページを含むノートブック。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="31dd3-p110">The notebook that contains the page.  Read-only.</span></span>|
|<span data-ttu-id="31dd3-165">parentSection</span><span class="sxs-lookup"><span data-stu-id="31dd3-165">parentSection</span></span>|[<span data-ttu-id="31dd3-166">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="31dd3-166">OnenoteSection</span></span>](section.md)|<span data-ttu-id="31dd3-p111">ページを含むセクション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="31dd3-p111">The section that contains the page. Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="31dd3-169">メソッド</span><span class="sxs-lookup"><span data-stu-id="31dd3-169">Methods</span></span>

| <span data-ttu-id="31dd3-170">メソッド</span><span class="sxs-lookup"><span data-stu-id="31dd3-170">Method</span></span>           | <span data-ttu-id="31dd3-171">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="31dd3-171">Return Type</span></span>    |<span data-ttu-id="31dd3-172">説明</span><span class="sxs-lookup"><span data-stu-id="31dd3-172">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="31dd3-173">ページを取得</span><span class="sxs-lookup"><span data-stu-id="31dd3-173">Get page</span></span>](../api/page_get.md) | [<span data-ttu-id="31dd3-174">ページ</span><span class="sxs-lookup"><span data-stu-id="31dd3-174">Page</span></span>](page.md) |<span data-ttu-id="31dd3-175">ページのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="31dd3-175">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="31dd3-176">ページのコンテンツを更新</span><span class="sxs-lookup"><span data-stu-id="31dd3-176">Update page content</span></span>](../api/page_update.md) | <span data-ttu-id="31dd3-177">なし</span><span class="sxs-lookup"><span data-stu-id="31dd3-177">None</span></span> |<span data-ttu-id="31dd3-178">ページの HTML コンテンツを更新します。</span><span class="sxs-lookup"><span data-stu-id="31dd3-178">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="31dd3-179">ページを削除</span><span class="sxs-lookup"><span data-stu-id="31dd3-179">Delete page</span></span>](../api/page_delete.md) | <span data-ttu-id="31dd3-180">なし</span><span class="sxs-lookup"><span data-stu-id="31dd3-180">None</span></span> |<span data-ttu-id="31dd3-181">ページを削除します。</span><span class="sxs-lookup"><span data-stu-id="31dd3-181">Delete the page.</span></span> |
|[<span data-ttu-id="31dd3-182">copyToSection</span><span class="sxs-lookup"><span data-stu-id="31dd3-182">copyToSection</span></span>](../api/page_copytosection.md)| <span data-ttu-id="31dd3-183">なし</span><span class="sxs-lookup"><span data-stu-id="31dd3-183">None</span></span> |<span data-ttu-id="31dd3-184">特定のセクションにページをコピーします。</span><span class="sxs-lookup"><span data-stu-id="31dd3-184">Copies the page to a specific section.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->