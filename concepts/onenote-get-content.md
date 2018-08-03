# <a name="get-onenote-content-and-structure-with-microsoft-graph"></a><span data-ttu-id="e3735-101">Microsoft Graph によって OneNote コンテンツと構造を取得する</span><span class="sxs-lookup"><span data-stu-id="e3735-101">Get OneNote content and structure with Microsoft Graph</span></span>

<span data-ttu-id="e3735-102">**適用対象**: OneDrive のコンシューマー ノートブック | Office 365 のエンタープライズ ノートブック</span><span class="sxs-lookup"><span data-stu-id="e3735-102">**Applies to:** Consumer notebooks on OneDrive | Enterprise notebooks on Office 365</span></span>

<span data-ttu-id="e3735-p101">OneNote のコンテンツと構造を取得するには、ターゲット エンドポイントに GET 要求を送信します。たとえば次のようにします。</span><span class="sxs-lookup"><span data-stu-id="e3735-p101">To get OneNote content and structure, you send a GET request to the target endpoint. For example:</span></span>

`GET ../onenote/pages/{id}`

<span data-ttu-id="e3735-105">要求が成功すると、Microsoft Graph は 200 HTTP 状態コードと、要求したエンティティまたはコンテンツを返します。</span><span class="sxs-lookup"><span data-stu-id="e3735-105">If the request is successful, Microsoft Graph returns a 200 HTTP status code and the entities or content that you requested.</span></span> <span data-ttu-id="e3735-106">OneNote のエンティティは、OData バージョン 4.0 仕様に準拠した JSON オブジェクトとして返されます。</span><span class="sxs-lookup"><span data-stu-id="e3735-106">OneNote entities are returned as JSON objects that conform to the OData version 4.0 specification.</span></span>

<span data-ttu-id="e3735-107">クエリ文字列オプションを使用すると、クエリをフィルターしてパフォーマンスを向上させることができます。</span><span class="sxs-lookup"><span data-stu-id="e3735-107">By using query string options, you can filter your queries and improve performance.</span></span>


<a name="request-uri"></a>

## <a name="construct-the-request-uri"></a><span data-ttu-id="e3735-108">要求 URI の構築</span><span class="sxs-lookup"><span data-stu-id="e3735-108">Construct the request URI</span></span>

<span data-ttu-id="e3735-109">要求 URI を構築するには、サービス ルート URL から開始します。</span><span class="sxs-lookup"><span data-stu-id="e3735-109">To construct the request URI, start with the service root URL:</span></span>

`https://graph.microsoft.com/v1.0/me/onenote`

<br/>

<span data-ttu-id="e3735-p103">次に、取得するリソースのエンドポイントを追加します ([リソース パス](#resource-paths-for-get-requests)については次のセクションを参照してください)。</span><span class="sxs-lookup"><span data-stu-id="e3735-p103">Then append the endpoint of the resource you want to retrieve. ([Resource paths](#resource-paths-for-get-requests) are shown in the next section.)</span></span>

<span data-ttu-id="e3735-112">完全な要求 URI は、次に示す例のいずれかのようになります。</span><span class="sxs-lookup"><span data-stu-id="e3735-112">Your full request URI will look like one of these examples:</span></span>

- `https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sections`
- `https://graph.microsoft.com/v1.0/me/onenote/notes/pages`
- `https://graph.microsoft.com/v1.0/me/onenote/pages?select=title,self`

> <span data-ttu-id="e3735-113">**注:** [サービス ルート URL](../api-reference/v1.0/resources/onenote-api-overview.md#root-url) の詳細についてはリンク先をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="e3735-113">**Note:** Learn more about the [service root URL](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span></span>

<a name="resource-paths"></a>

## <a name="resource-paths-for-get-requests"></a><span data-ttu-id="e3735-114">GET 要求のリソース パス</span><span class="sxs-lookup"><span data-stu-id="e3735-114">Resource paths for GET requests</span></span>

<span data-ttu-id="e3735-115">次のリソース パスを使用して、ページ、セクション、セクション グループ、ノートブック、画像、またはファイル リソースを取得します。</span><span class="sxs-lookup"><span data-stu-id="e3735-115">Use the following resource paths to get pages, sections, section groups, notebooks, and image or file resources.</span></span>

- [<span data-ttu-id="e3735-116">ページ コレクション</span><span class="sxs-lookup"><span data-stu-id="e3735-116">Page collection</span></span>](#page-collection)
- [<span data-ttu-id="e3735-117">ページ エンティティ</span><span class="sxs-lookup"><span data-stu-id="e3735-117">Page entity</span></span>](#page-entity)
- [<span data-ttu-id="e3735-118">ページ プレビュー</span><span class="sxs-lookup"><span data-stu-id="e3735-118">Page preview</span></span>](#page-preview)
- [<span data-ttu-id="e3735-119">ページ HTML コンテンツ</span><span class="sxs-lookup"><span data-stu-id="e3735-119">Page HTML content</span></span>](#page-html-content)
- [<span data-ttu-id="e3735-120">セクション コレクション</span><span class="sxs-lookup"><span data-stu-id="e3735-120">Section collection</span></span>](#section-collection)
- [<span data-ttu-id="e3735-121">セクション エンティティ</span><span class="sxs-lookup"><span data-stu-id="e3735-121">Section entity</span></span>](#section-entity)
- [<span data-ttu-id="e3735-122">SectionGroup コレクション</span><span class="sxs-lookup"><span data-stu-id="e3735-122">SectionGroup collection</span></span>](#sectiongroup-collection)
- [<span data-ttu-id="e3735-123">SectionGroup エンティティ</span><span class="sxs-lookup"><span data-stu-id="e3735-123">SectionGroup entity</span></span>](#sectiongroup-entity)
- [<span data-ttu-id="e3735-124">ノートブック コレクション</span><span class="sxs-lookup"><span data-stu-id="e3735-124">Notebook collection</span></span>](#notebook-collection)
- [<span data-ttu-id="e3735-125">ノートブック エンティティ</span><span class="sxs-lookup"><span data-stu-id="e3735-125">Notebook entity</span></span>](#notebook-entity)
- [<span data-ttu-id="e3735-126">画像またはその他のファイル リソース</span><span class="sxs-lookup"><span data-stu-id="e3735-126">Image or other file resource</span></span>](#image-or-other-file-resource)

<a name="get-pages"></a>

### <a name="page-collection"></a><span data-ttu-id="e3735-127">ページ コレクション</span><span class="sxs-lookup"><span data-stu-id="e3735-127">Page collection</span></span>

<span data-ttu-id="e3735-128">すべてのノートブックのページ (メタデータ) を取得する。</span><span class="sxs-lookup"><span data-stu-id="e3735-128">Get pages (metadata) across all notebooks</span></span>

`../pages[?filter,orderby,select,expand,top,skip,search,count]`

<br/>

<span data-ttu-id="e3735-129">特定のセクションからページ (メタデータ) を取得する。</span><span class="sxs-lookup"><span data-stu-id="e3735-129">Get pages (metadata) from a specific section</span></span>

`../sections/{section-id}/pages[?filter,orderby,select,expand,top,skip,search,count,pagelevel]`

<br/>
 
<span data-ttu-id="e3735-130">`search`クエリ文字列オプションは、コンシューマー ノートパソコンでのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="e3735-130">The `search` query string option is available for consumer notebooks only.</span></span>

<span data-ttu-id="e3735-131">ページの既定の並べ替え順序は `lastModifiedTime desc` です。</span><span class="sxs-lookup"><span data-stu-id="e3735-131">The default sort order for pages is `lastModifiedTime desc`.</span></span>

<span data-ttu-id="e3735-132">既定のクエリは、親セクションを展開し、セクションの `id`、`name`、および `self` プロパティを選択します。</span><span class="sxs-lookup"><span data-stu-id="e3735-132">The default query expands the parent section and selects the section's `id`, `name`, and `self` properties.</span></span>

<span data-ttu-id="e3735-133">既定では、*GET ページ*要求に対して上位 20 のエントリのみが返されます。</span><span class="sxs-lookup"><span data-stu-id="e3735-133">By default, only the top 20 entries are returned for *GET pages* requests.</span></span> <span data-ttu-id="e3735-134">**上位**クエリ文字列オプションを指定しない要求を行った場合、次の 20 エントリを取得するために使用できる `@odata.nextLink` リンクが応答で返されます。</span><span class="sxs-lookup"><span data-stu-id="e3735-134">Requests that don't specify a **top** query string option return an `@odata.nextLink` link in the response that you can use to get the next 20 entries.</span></span>

<span data-ttu-id="e3735-135">セクションのページ コレクションの場合、**pagelevel** を使用して、ページのインデント レベルとセクション内でのその順序を返します。</span><span class="sxs-lookup"><span data-stu-id="e3735-135">For the pages collection in a section, use **pagelevel** to return the indentation level of pages and their order within the section.</span></span> 

#### <a name="example"></a><span data-ttu-id="e3735-136">例</span><span class="sxs-lookup"><span data-stu-id="e3735-136">Example</span></span>

`GET ../sections/{section-id}/pages?pagelevel=true`



<a name="get-page"></a> 

### <a name="page-entity"></a><span data-ttu-id="e3735-137">ページ エンティティ</span><span class="sxs-lookup"><span data-stu-id="e3735-137">Page entity</span></span>

<span data-ttu-id="e3735-138">特定のページのメタデータを取得する</span><span class="sxs-lookup"><span data-stu-id="e3735-138">Get the metadata for a specific page.</span></span> 

`../pages/{page-id}[?select,expand,pagelevel]` 

<br/>

<span data-ttu-id="e3735-139">ページは、**parentNotebook** プロパティと **parentSection** プロパティを展開できます。</span><span class="sxs-lookup"><span data-stu-id="e3735-139">Pages can expand the **parentNotebook** and **parentSection** properties.</span></span>

<span data-ttu-id="e3735-140">既定のクエリは、親セクションを展開し、セクションの `id`、`name`、および `self` プロパティを選択します。</span><span class="sxs-lookup"><span data-stu-id="e3735-140">The default query expands the parent section and selects the section's `id`, `name`, and `self` properties.</span></span>

<span data-ttu-id="e3735-141">**pagelevel** を使用して、ページのインデント レベルと親セクション内でのその順序を返します。</span><span class="sxs-lookup"><span data-stu-id="e3735-141">Use **pagelevel** to return the indentation level of the page and its order within its parent section.</span></span> 

#### <a name="example"></a><span data-ttu-id="e3735-142">例</span><span class="sxs-lookup"><span data-stu-id="e3735-142">Example</span></span>

`GET ../pages/{page-id}?pagelevel=true`



<a name="get-page-preview"></a> 

### <a name="page-preview"></a><span data-ttu-id="e3735-143">ページ プレビュー</span><span class="sxs-lookup"><span data-stu-id="e3735-143">Page preview</span></span>

<span data-ttu-id="e3735-144">ページのテキストと画像のプレビュー コンテンツを取得する。</span><span class="sxs-lookup"><span data-stu-id="e3735-144">Get text and image preview content for a page</span></span>

`../pages/{page-id}/preview`

<br/>


<span data-ttu-id="e3735-145">JSON 応答には、ページに含まれているものを特定するために使用できる、プレビュー コンテンツが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e3735-145">The JSON response contains the preview content, which you can use to help users identify what's in the page.</span></span>

```json
{
  "@odata.context":"https://www.onenote.com/api/v1.0/$metadata#Microsoft.OneNote.Api.PagePreview",
  "previewText":"text-snippet",
  "links":{
    "previewImageUrl":{
      "href":"https://www.onenote.com/api/v1.0/resources/{id}/content?publicAuth=true&mimeType=image/png"
    }
  }
}
```

<span data-ttu-id="e3735-146">**previewText** プロパティには、ページからのテキスト スニペットが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e3735-146">The **previewText** property contains a text snippet from the page.</span></span> <span data-ttu-id="e3735-147">Microsoft Graph は、最大 300 文字の完全な文字列を返します。</span><span class="sxs-lookup"><span data-stu-id="e3735-147">Microsoft Graph returns complete phrases, up to a maximum of 300 characters.</span></span> 

<span data-ttu-id="e3735-148">ページにプレビュー UI のビルドに使用できる画像が含まれている場合、**previewImageUrl** オブジェクトの **href** プロパティには、事前認証されたパブリックの [image resource](#image-or-other-file-resource) のリンクが含まれます。</span><span class="sxs-lookup"><span data-stu-id="e3735-148">If the page has an image that can be used to build a preview UI, the **href** property in the **previewImageUrl** object contains a link to a public, pre-authenticated [image resource](#image-or-other-file-resource).</span></span> <span data-ttu-id="e3735-149">このリンクは HTML で使用できます。</span><span class="sxs-lookup"><span data-stu-id="e3735-149">You can use this link in HTML,</span></span> <span data-ttu-id="e3735-150">それ以外の場合、**href** は、null 値を返します。</span><span class="sxs-lookup"><span data-stu-id="e3735-150">Otherwise, **href** returns null.</span></span>

#### <a name="example"></a><span data-ttu-id="e3735-151">例</span><span class="sxs-lookup"><span data-stu-id="e3735-151">Example</span></span> 

`<img src="https://www.onenote.com/api/v1.0/resources/{id}/content?publicAuth=true&mimeType=image/png" />`


<a name="get-page-content"></a> 

### <a name="page-html-content"></a><span data-ttu-id="e3735-152">ページ HTML コンテンツ</span><span class="sxs-lookup"><span data-stu-id="e3735-152">Page HTML content</span></span>

<span data-ttu-id="e3735-153">ページの HTML コンテンツを取得する。</span><span class="sxs-lookup"><span data-stu-id="e3735-153">Get the HTML content of a page </span></span>

`../pages/{page-id}/content[?includeIDs,preAuthenticated]`

<span data-ttu-id="e3735-154">(*[返される HTML コンテンツ](onenote_input_output_html.md)の詳細についてはリンク先をご覧ください*)</span><span class="sxs-lookup"><span data-stu-id="e3735-154">(*learn more about [returned HTML content](onenote_input_output_html.md)*)</span></span> 

<br/>

<span data-ttu-id="e3735-155">**includeIDs=true** クエリ文字列オプションを使用して、[ページを更新](onenote_update_page.md)するために使用する生成 ID を取得します。</span><span class="sxs-lookup"><span data-stu-id="e3735-155">Use the **includeIDs=true** query string option to get generated IDs used to [update the page](onenote_update_page.md).</span></span>

<span data-ttu-id="e3735-p107">**preAuthenticated=true** クエリ文字列オプションを使用して、ページ上の[画像リソース](#image-or-other-file-resource)のパブリック URL を取得します。パブリック URL は 1 時間有効です。</span><span class="sxs-lookup"><span data-stu-id="e3735-p107">Use the **preAuthenticated=true** query string option to get public URLs to the [image resources](#image-or-other-file-resource) that are on the page. The public URLs are valid for one hour.</span></span> 



<a name="get-sections"></a>

### <a name="section-collection"></a><span data-ttu-id="e3735-158">セクション コレクション</span><span class="sxs-lookup"><span data-stu-id="e3735-158">Section collection</span></span>

<span data-ttu-id="e3735-159">ユーザーが所有するすべてのノートブックから、ネストされたセクション グループのセクションを含む、すべてのセクションを取得する。</span><span class="sxs-lookup"><span data-stu-id="e3735-159">Get all sections from all notebooks that are owned by the user, including sections in nested section groups </span></span>

`../sections[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="e3735-160">特定のセクション グループの直下にあるすべてのセクションを取得する。</span><span class="sxs-lookup"><span data-stu-id="e3735-160">Get all sections that are directly under a specific section group</span></span>

`../sectionGroups/{sectiongroup-id}/sections[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="e3735-161">特定のノートブックの直下にあるすべてのセクションを取得する。</span><span class="sxs-lookup"><span data-stu-id="e3735-161">Get all sections that are directly under a specific notebook </span></span>

`../notebooks/{notebook-id}/sections[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="e3735-162">セクションは、**parentNotebook** プロパティと **parentSectionGroup** プロパティを展開できます。</span><span class="sxs-lookup"><span data-stu-id="e3735-162">Sections can expand the **parentNotebook** and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="e3735-163">セクションの既定の並べ替え順序は `name asc` です。</span><span class="sxs-lookup"><span data-stu-id="e3735-163">The default sort order for sections is `name asc`.</span></span>

<span data-ttu-id="e3735-164">既定のクエリは、親ノートブックおよび親セクション グループを展開し、`id`、`name`、および `self` プロパティを選択します。</span><span class="sxs-lookup"><span data-stu-id="e3735-164">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>



<a name="get-section"></a>

### <a name="section-entity"></a><span data-ttu-id="e3735-165">セクション エンティティ</span><span class="sxs-lookup"><span data-stu-id="e3735-165">Section entity</span></span>

<span data-ttu-id="e3735-166">特定のセクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="e3735-166">Get a specific section.</span></span>

`../sections/{section-id}[?select,expand]` 

<br/>

<span data-ttu-id="e3735-167">セクションは、**parentNotebook** プロパティと **parentSectionGroup** プロパティを展開できます。</span><span class="sxs-lookup"><span data-stu-id="e3735-167">Sections can expand the **parentNotebook** and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="e3735-168">既定のクエリは、親ノートブックおよび親セクション グループを展開し、`id`、`name`、および `self` プロパティを選択します。</span><span class="sxs-lookup"><span data-stu-id="e3735-168">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>



<a name="get-section-groups"></a>

### <a name="sectiongroup-collection"></a><span data-ttu-id="e3735-169">SectionGroup コレクション</span><span class="sxs-lookup"><span data-stu-id="e3735-169">SectionGroup collection</span></span>

<span data-ttu-id="e3735-170">ユーザーが所有するすべてのノートブックから、ネストされたセクション グループを含む、すべてのセクション グループを取得する。</span><span class="sxs-lookup"><span data-stu-id="e3735-170">Get all section groups from all notebooks that are owned by the user, including nested section groups</span></span>

`../sectionGroups[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="e3735-171">特定のノートブックの直下にあるすべてのセクション グループを取得する。</span><span class="sxs-lookup"><span data-stu-id="e3735-171">Get all section groups that are directly under a specific notebook</span></span> 

`../notebooks/{notebook-id}/sectionGroups[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="e3735-172">セクション グループは、**セクション**、**sectionGroups**、**parentNotebook**、および **parentSectionGroup** プロパティを展開できます。</span><span class="sxs-lookup"><span data-stu-id="e3735-172">Section groups can expand the **sections**, **sectionGroups**, **parentNotebook**, and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="e3735-173">セクション グループの既定の並べ替え順序は `name asc` です。</span><span class="sxs-lookup"><span data-stu-id="e3735-173">The default sort order for section groups is `name asc`.</span></span>

<span data-ttu-id="e3735-174">既定のクエリは、親ノートブックおよび親セクション グループを展開し、`id`、`name`、および `self` プロパティを選択します。</span><span class="sxs-lookup"><span data-stu-id="e3735-174">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>



<a name="get-section-group"></a>

### <a name="sectiongroup-entity"></a><span data-ttu-id="e3735-175">SectionGroup エンティティ</span><span class="sxs-lookup"><span data-stu-id="e3735-175">SectionGroup entity</span></span>

<span data-ttu-id="e3735-176">特定のセクション グループを取得します。</span><span class="sxs-lookup"><span data-stu-id="e3735-176">Get a specific section group.</span></span>

`../sectionGroups/{sectiongroup-id}[?select,expand]` 

<br/>

<span data-ttu-id="e3735-177">セクション グループは、**セクション**、**sectionGroups**、**parentNotebook**、および **parentSectionGroup** プロパティを展開できます。</span><span class="sxs-lookup"><span data-stu-id="e3735-177">Section groups can expand the **sections**, **sectionGroups**, **parentNotebook**, and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="e3735-178">既定のクエリは、親ノートブックおよび親セクション グループを展開し、`id`、`name`、および `self` プロパティを選択します。</span><span class="sxs-lookup"><span data-stu-id="e3735-178">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>



<a name="get-notebooks"></a>

### <a name="notebook-collection"></a><span data-ttu-id="e3735-179">ノートブック コレクション</span><span class="sxs-lookup"><span data-stu-id="e3735-179">Notebook collection</span></span>

<span data-ttu-id="e3735-180">ユーザーによって所有されるすべてのノートブックを取得する。</span><span class="sxs-lookup"><span data-stu-id="e3735-180">Get all the notebooks that are owned by the user</span></span> 

`../notebooks[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="e3735-181">ノートブックは、**セクション**および **sectionGroups** プロパティを展開できます。</span><span class="sxs-lookup"><span data-stu-id="e3735-181">Notebooks can expand the **sections** and **sectionGroups** properties.</span></span>

<span data-ttu-id="e3735-182">ノートブックの既定の並べ替え順序は `name asc` です。</span><span class="sxs-lookup"><span data-stu-id="e3735-182">The default sort order for notebooks is `name asc`.</span></span> 



<a name="get-notebook"></a>

### <a name="notebook-entity"></a><span data-ttu-id="e3735-183">ノートブック エンティティ</span><span class="sxs-lookup"><span data-stu-id="e3735-183">Notebook entity</span></span>

<span data-ttu-id="e3735-184">特定のノートブックを取得します。</span><span class="sxs-lookup"><span data-stu-id="e3735-184">Get a specific notebook.</span></span>

`../notebooks/{notebook-id}[?select,expand]` 

<br/>

<span data-ttu-id="e3735-185">ノートブックは、**セクション**および **sectionGroups** プロパティを展開できます。</span><span class="sxs-lookup"><span data-stu-id="e3735-185">Notebooks can expand the **sections** and **sectionGroups** properties.</span></span>



<a name="get-resource"></a>

### <a name="image-or-other-file-resource"></a><span data-ttu-id="e3735-186">画像またはその他のファイル リソース</span><span class="sxs-lookup"><span data-stu-id="e3735-186">Image or other file resource</span></span>

<span data-ttu-id="e3735-187">特定のリソースのバイナリ データを取得する。</span><span class="sxs-lookup"><span data-stu-id="e3735-187">Get the binary data of a specific resource</span></span> 

`../resources/{resource-id}/$value` 

<br/>

<span data-ttu-id="e3735-188">ファイルのリソース URI は、ページの[出力 HTML](onenote_input_output_html.md) にあります。</span><span class="sxs-lookup"><span data-stu-id="e3735-188">You can find the file's resource URI in the page's [output HTML](onenote_input_output_html.md).</span></span>

<span data-ttu-id="e3735-189">たとえば、**img** タグには、**data-fullres-src** 属性に元の画像のエンドポイント、**src** 属性に最適化された画像のエンドポイントが含まれます。</span><span class="sxs-lookup"><span data-stu-id="e3735-189">For example, an **img** tag includes endpoints for the original image in the **data-fullres-src** attribute and the optimized image in the **src** attribute.</span></span> 

#### <a name="example"></a><span data-ttu-id="e3735-190">例</span><span class="sxs-lookup"><span data-stu-id="e3735-190">Example</span></span>

```html
<img 
    src="https://www.onenote.com/api/v1.0/me/notes/resources/{image-id}/$value"  
    data-src-type="image/png"
    data-fullres-src="https://www.onenote.com/api/v1.0/resources/{image-id}/$value"  
    data-fullres-src-type="image/png" ... />
```

<span data-ttu-id="e3735-191">**object** タグには、**data** 属性のファイル リソースのエンドポイントが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e3735-191">And an **object** tag includes the endpoint for the file resource in the **data** attribute.</span></span> 

#### <a name="example"></a><span data-ttu-id="e3735-192">例</span><span class="sxs-lookup"><span data-stu-id="e3735-192">Example</span></span>

```html
<object
    data="http://www.onenote.com/api/v1.0/me/notes/resources/{file-id}/$value"
    data-attachment="fileName.pdf" 
    type="application/pdf" ... />
```

<span data-ttu-id="e3735-193">ページにある画像リソースへの事前認証された公開 URL を取得するには、[ページのコンテンツを取得する](#page-html-content)際にクエリ文字列に `preAuthenticated=true` を含めます (**例:**  `GET ../pages/{page-id}/content?preAuthenticated=true`)。</span><span class="sxs-lookup"><span data-stu-id="e3735-193">To get public, pre-authenticated URLs to the image resources on a page, include `preAuthenticated=true` in the query string when you [retrieve the page content](#page-html-content) (**example:**  `GET ../pages/{page-id}/content?preAuthenticated=true`).</span></span> <span data-ttu-id="e3735-194">[出力 HTML](onenote_input_output_html.md#output-html-examples-for-images) に返されるパブリック URL は 1 時間有効です。</span><span class="sxs-lookup"><span data-stu-id="e3735-194">The public URLs that are returned in the [output HTML](onenote_input_output_html.md#output-html-examples-for-images) are valid for one hour.</span></span> <span data-ttu-id="e3735-195">このフラグを設定していない場合、取得された画像は非公開で、またページのコンテンツの残りの部分と同様、それらを取得するために承認を必要とするため、ブラウザーで直接レンダリングすることはありません。</span><span class="sxs-lookup"><span data-stu-id="e3735-195">Without this flag, retrieved images won't render directly in a browser because they are private and require authorization to retrieve them, like the rest of the page contents.</span></span> 

> <span data-ttu-id="e3735-196">**注:** リソースのコレクションの取得はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3735-196">**Note:** Getting a collection of resources is not supported.</span></span> 

<span data-ttu-id="e3735-197">ファイル リソースを取得する場合、**Accept** コンテンツ タイプを要求に含める必要はありません。</span><span class="sxs-lookup"><span data-stu-id="e3735-197">When you get a file resource, you don't need to include an **Accept** content type in the request.</span></span>

<span data-ttu-id="e3735-198">GET 要求の詳細については、Microsoft Graph API REST リファレンスの中の次のリソースを参照してください。</span><span class="sxs-lookup"><span data-stu-id="e3735-198">For more information about GET requests, see the following resources in the Microsoft Graph API REST reference:</span></span>

- [<span data-ttu-id="e3735-199">ページを取得する</span><span class="sxs-lookup"><span data-stu-id="e3735-199">GET Pages</span></span>](../api-reference/v1.0/api/page_get.md)
- [<span data-ttu-id="e3735-200">Get section</span><span class="sxs-lookup"><span data-stu-id="e3735-200">GET Sections</span></span>](../api-reference/v1.0/api/section_get.md)
- [<span data-ttu-id="e3735-201">Get sectionGroup</span><span class="sxs-lookup"><span data-stu-id="e3735-201">GET SectionGroups</span></span>](../api-reference/v1.0/api/sectiongroup_get.md)
- [<span data-ttu-id="e3735-202">ノートブックを取得する</span><span class="sxs-lookup"><span data-stu-id="e3735-202">GET Notebooks</span></span>](../api-reference/v1.0/api/notebook_get.md) 




<a name="example"></a>

## <a name="example-get-requests"></a><span data-ttu-id="e3735-203">GET 要求の例</span><span class="sxs-lookup"><span data-stu-id="e3735-203">Example GET requests</span></span>

<span data-ttu-id="e3735-204">OneNote のエンティティおよび検索ページ コンテンツを照会して、必要な情報だけを取得することができます。</span><span class="sxs-lookup"><span data-stu-id="e3735-204">You can query for OneNote entities and search page content to get just the information you need.</span></span> <span data-ttu-id="e3735-205">次の例は、Microsoft Graph への GET 要求で、[サポートされているクエリ文字列オプション](#supported-odata-query-string-options)を使用するいくつかの方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="e3735-205">The following examples show some ways you can use [supported query string options](#supported-odata-query-string-options) in GET requests to Microsoft Graph.</span></span> 

<span data-ttu-id="e3735-206">**次の点にご注意ください。**</span><span class="sxs-lookup"><span data-stu-id="e3735-206">**Remember:**</span></span>

- <span data-ttu-id="e3735-207">GET 要求はすべて、[サービス ルート URL](../api-reference/v1.0/resources/onenote-api-overview.md#root-url) で始まります。</span><span class="sxs-lookup"><span data-stu-id="e3735-207">All GET requests start with the [service root URL](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span></span> <br/><br/><span data-ttu-id="e3735-208">**例**: `https://www.onenote.com/api/v1.0/me/notes` および `https://www.onenote.com/api/v1.0/myOrganization/siteCollections/{id}/sites/{id}/notes/`</span><span class="sxs-lookup"><span data-stu-id="e3735-208">**Examples**: `https://www.onenote.com/api/v1.0/me/notes` and `https://www.onenote.com/api/v1.0/myOrganization/siteCollections/{id}/sites/{id}/notes/`</span></span>

- <span data-ttu-id="e3735-209">URL クエリ文字列のスペースには %20 エンコードを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e3735-209">Spaces in the URL query string must use %20 encoding.</span></span><br/><br/><span data-ttu-id="e3735-210">**例**: `filter=title%20eq%20'biology'`</span><span class="sxs-lookup"><span data-stu-id="e3735-210">Example: </span></span>

- <span data-ttu-id="e3735-211">プロパティ名と OData 文字列比較では大文字と小文字が区別されます。</span><span class="sxs-lookup"><span data-stu-id="e3735-211">Property names and OData string comparisons are case sensitive.</span></span> <span data-ttu-id="e3735-212">文字列比較には OData **tolower** 関数を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="e3735-212">We recommend using the OData **tolower** function for string comparisons.</span></span><br/><br/><span data-ttu-id="e3735-213">**例**: `filter=tolower(name) eq 'spring'`</span><span class="sxs-lookup"><span data-stu-id="e3735-213">Example: </span></span>
 

### <a name="search--filter"></a><span data-ttu-id="e3735-214">search & filter</span><span class="sxs-lookup"><span data-stu-id="e3735-214">search & filter</span></span>  

<span data-ttu-id="e3735-215">特定のアプリによって作成された、*recipe* という用語が含まれるページすべてを取得します (`search` はコンシューマー ノートブックでのみ使用可能)。</span><span class="sxs-lookup"><span data-stu-id="e3735-215">Get all pages that contain the term *recipe* that were created by a specific app.  (`search` is available for consumer notebooks only)</span></span>

```
[GET] ../pages?search=recipe&filter=createdByAppId eq 'WLID-000000004C12821A'
```
 
### <a name="search--select"></a><span data-ttu-id="e3735-216">search & select</span><span class="sxs-lookup"><span data-stu-id="e3735-216">search & select</span></span>  

<span data-ttu-id="e3735-217">*golgi app* という用語が含まれるすべてのページの、タイトル、OneNote クライアントのリンク、**contentUrl** リンクを取得します (`search` はコンシューマー ノートブックでのみ使用可能)。</span><span class="sxs-lookup"><span data-stu-id="e3735-217">Get the title, OneNote client links, and **contentUrl** link for all pages that contain the term *golgi app*.  (`search` is available for consumer notebooks only)</span></span>

```
[GET] ../pages?search=golgi app&select=title,links,contentUrl
```
 
### <a name="expand"></a><span data-ttu-id="e3735-218">expand</span><span class="sxs-lookup"><span data-stu-id="e3735-218">expand</span></span> 

<span data-ttu-id="e3735-219">すべてのノートブックを取得し、そのセクションとセクション グループを展開します。</span><span class="sxs-lookup"><span data-stu-id="e3735-219">Get all notebooks and expand their sections and section groups.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups
```

<br/>

<span data-ttu-id="e3735-220">特定のセクション グループを取得し、そのセクションとセクション グループを展開します。</span><span class="sxs-lookup"><span data-stu-id="e3735-220">Get a specific section group and expand its sections and section groups.</span></span>  

```
[GET] ../sectionGroups/{sectiongroup-id}?expand=sections,sectionGroups
```

<br/>

<span data-ttu-id="e3735-221">ページを取得し、その親セクションと親ノートブックを展開します。</span><span class="sxs-lookup"><span data-stu-id="e3735-221">Get a page and expand its parent section and parent notebook.</span></span>

```
[GET] ../pages/{page-id}?expand=parentSection,parentNotebook
```

### <a name="expand-multiple-levels"></a><span data-ttu-id="e3735-222">expand (複数レベル)</span><span class="sxs-lookup"><span data-stu-id="e3735-222">expand (multiple levels)</span></span>  

<span data-ttu-id="e3735-223">すべてのノートブックを取得してセクションとセクション グループを展開し、各セクション グループのすべてのセクションを展開します。</span><span class="sxs-lookup"><span data-stu-id="e3735-223">Get all notebooks and expand their sections and section groups, and expand all sections in each section group.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups(expand=sections)
```
 
> <span data-ttu-id="e3735-224">**注:** 子エンティティの親を展開、または親エンティティの子を展開すると、循環参照が作成されますが、これはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3735-224">Expanding parents of child entities or expanding children of parent entities creates a circular reference and is not supported.</span></span>

 
### <a name="expand--select-multiple-levels"></a><span data-ttu-id="e3735-225">expand & select (複数レベル)</span><span class="sxs-lookup"><span data-stu-id="e3735-225">expand & select (multiple levels)</span></span>  

<span data-ttu-id="e3735-226">特定のセクション グループの名前と **self** リンクを取得し、そのすべてのセクションの名前と **self** リンクを取得します。</span><span class="sxs-lookup"><span data-stu-id="e3735-226">Get the name and **self** link for a specific section group, and get the name and **self** links for all its sections.</span></span>  

```
[GET] ../sectionGroups/{sectiongroup-id}?expand=sections(select=name,self)&select=name,self
```

<br/>

<span data-ttu-id="e3735-227">すべてのセクションの名前と **self** リンクを取得し、各セクションの親ノートブックの名前と作成時刻を取得します。</span><span class="sxs-lookup"><span data-stu-id="e3735-227">Get the name and **self** link for all sections, and get the name and created time of each section's parent notebook.</span></span>  

```
[GET] ../sections?expand=parentNotebook(select=name,createdTime)&select=name,self
```

<br/>
 
<span data-ttu-id="e3735-228">すべてのページのタイトルと ID を取得し、親セクションと親ノートブックの名前を取得します。</span><span class="sxs-lookup"><span data-stu-id="e3735-228">Get the title and ID for all pages, and get the name of the parent section and parent notebook.</span></span>

```
[GET] ../pages?select=id,title&expand=parentSection(select=name),parentNotebook(select=name)
```

### <a name="expand--levels-multiple-levels"></a><span data-ttu-id="e3735-229">expand & levels (複数レベル)</span><span class="sxs-lookup"><span data-stu-id="e3735-229">expand & levels (multiple levels)</span></span>  

<span data-ttu-id="e3735-230">すべてのノートブック、セクション、セクション グループを取得します。</span><span class="sxs-lookup"><span data-stu-id="e3735-230">Get all notebooks, sections, and section groups.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups(expand=sections,sectionGroups(levels=max;expand=sections))
```
 
### <a name="filter"></a><span data-ttu-id="e3735-231">filter</span><span class="sxs-lookup"><span data-stu-id="e3735-231">filter</span></span>

<span data-ttu-id="e3735-232">2014 年 10 月に作成されたセクションすべてを取得します。</span><span class="sxs-lookup"><span data-stu-id="e3735-232">Get all sections that were created in October 2014.</span></span>

```
[GET] ../sections?filter=createdTime ge 2014-10-01 and createdTime le 2014-10-31
```

<br/>

<span data-ttu-id="e3735-233">2015 年 1 月 1 日以降に特定のアプリによって作成されたページを取得します。</span><span class="sxs-lookup"><span data-stu-id="e3735-233">Get the pages that were created by a specific app since January 1, 2015.</span></span>

```
[GET] ../pages?filter=createdByAppId eq 'WLID-0000000048118631' and createdTime ge 2015-01-01
```

### <a name="filter--expand"></a><span data-ttu-id="e3735-234">filter & expand</span><span class="sxs-lookup"><span data-stu-id="e3735-234">filter & expand</span></span>  

<span data-ttu-id="e3735-p111">特定のノートブックに含まれるすべてのページを取得します。既定では、この API は 20 エントリを戻します。</span><span class="sxs-lookup"><span data-stu-id="e3735-p111">Get all pages in a specific notebook. The API returns 20 entries by default.</span></span>

```
[GET] ../pages?filter=parentNotebook/id eq '{notebook-id}'&expand=parentNotebook
```

<br/>

<span data-ttu-id="e3735-237">*学校*のノートブックにあるすべてのセクションの名前と **pagesUrl** リンクを取得します。</span><span class="sxs-lookup"><span data-stu-id="e3735-237">Get the name and **pagesUrl** link for all sections from the *School* notebook.</span></span> <span data-ttu-id="e3735-238">OData の文字列比較は大文字小文字が区別されるので、ベスト プラクティスとして **tolower** 関数を使用します。</span><span class="sxs-lookup"><span data-stu-id="e3735-238">OData string comparisons are case sensitive, so use the **tolower** function as a best practice.</span></span>

```
[GET] ../notebooks?filter=tolower(name) eq 'school'&expand=sections(select=name,pagesUrl)
```

### <a name="filter--select--orderby"></a><span data-ttu-id="e3735-239">filter & select & orderby</span><span class="sxs-lookup"><span data-stu-id="e3735-239">filter & select & orderby</span></span>   

<span data-ttu-id="e3735-p113">セクション名に *spring* という語が含まれるすべてのセクションの名前と **pagesUrl** リンクを取得します。セクションを最終変更日で並べ替えます。</span><span class="sxs-lookup"><span data-stu-id="e3735-p113">Get the name and **pagesUrl** link for all sections that contain the term *spring* in the section name. Order sections by last modified date.</span></span>

```
[GET] ../sections?filter=contains(tolower(name),'spring')&select=name,pagesUrl&orderby=lastModifiedTime desc
```
 
### <a name="orderby"></a><span data-ttu-id="e3735-242">orderby</span><span class="sxs-lookup"><span data-stu-id="e3735-242">orderby</span></span>

<span data-ttu-id="e3735-p114">**createdByAppId** プロパティ、次に作成時刻を基準に順序を並べ替えて、最初の 20 ページを取得します。既定では、この API は 20 エントリを戻します。</span><span class="sxs-lookup"><span data-stu-id="e3735-p114">Get the first 20 pages ordered by **createdByAppId** property and then by most recent created time. The API returns 20 entries by default.</span></span>

```
[GET] ../pages?orderby=createdByAppId,createdTime desc
```

### <a name="search--filter--top"></a><span data-ttu-id="e3735-245">search & filter & top</span><span class="sxs-lookup"><span data-stu-id="e3735-245">search & filter & top</span></span> 

<span data-ttu-id="e3735-246">*cell division* という語句を含む、2015 年 1 月 1 日以降に作成されたページで新しいものを 5 つ取得します。</span><span class="sxs-lookup"><span data-stu-id="e3735-246">Get the five newest pages created since January 1, 2015 that contain the phrase *cell division*.</span></span> <span data-ttu-id="e3735-247">既定ではこの API は 20 エントリを返します。最大では 100 エントリを返します。</span><span class="sxs-lookup"><span data-stu-id="e3735-247">The API returns 20 entries by default with a maximum of 100.</span></span> <span data-ttu-id="e3735-248">ページの既定の並べ替え順序は `lastModifiedTime desc` です (`search` は、コンシューマー ノートブックでのみ使用可能)。</span><span class="sxs-lookup"><span data-stu-id="e3735-248">The default sort order for pages is `lastModifiedTime desc` (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search="cell division"&filter=createdTime ge 2015-01-01&top=5
```

### <a name="search--filter--top--skip"></a><span data-ttu-id="e3735-249">search & filter & top & skip</span><span class="sxs-lookup"><span data-stu-id="e3735-249">search & filter & top & skip</span></span>  

<span data-ttu-id="e3735-250">結果セット内の次の 5 ページを取得します (`search` は、コンシューマー ノートブックでのみ使用可能)。</span><span class="sxs-lookup"><span data-stu-id="e3735-250">Get the next five pages in the result set. (`search` is available for consumer notebooks only)</span></span>

```
[GET] ../pages?search=biology&filter=createdTime ge 2015-01-01&top=5&skip=5
```

<br/>

<span data-ttu-id="e3735-251">それから次の 5 ページを取得します (`search` は、コンシューマー ノートブックでのみ使用可能)。</span><span class="sxs-lookup"><span data-stu-id="e3735-251">And the next five. (`search` is available for consumer notebooks only)</span></span>

```
[GET] ../pages?search=biology&filter=createdTime ge 2015-01-01&top=5&skip=10
```

> <span data-ttu-id="e3735-252">**注:** **search** と **filter** がどちらも同じ要求に適用される場合、結果には両方の条件に一致するエンティティのみが含まれます。</span><span class="sxs-lookup"><span data-stu-id="e3735-252">**Note:** If both **search** and **filter** are applied to the same request, the results include only those entities that match both criteria.</span></span>
 
### <a name="select"></a><span data-ttu-id="e3735-253">select</span><span class="sxs-lookup"><span data-stu-id="e3735-253">select</span></span>

<span data-ttu-id="e3735-254">ユーザーのノートブック内にあるすべてのセクションの名前、作成時刻、**self** リンクを取得します。</span><span class="sxs-lookup"><span data-stu-id="e3735-254">Get the name, created time, and **self** link for all sections in the user's notebooks.</span></span>

```
[GET] ../sections?select=name,createdTime,self
```

<br/>

<span data-ttu-id="e3735-255">特定のページのタイトル、作成時刻、OneNote クライアント リンクを取得します。</span><span class="sxs-lookup"><span data-stu-id="e3735-255">Get the title, created time, and OneNote client links for a specific page.</span></span>

```
[GET] ../pages/{page-id}?select=title,createdTime,links
```

### <a name="select--expand--filter-multiple-levels"></a><span data-ttu-id="e3735-256">select & expand & filter (複数レベル)</span><span class="sxs-lookup"><span data-stu-id="e3735-256">select & expand & filter (multiple levels)</span></span>  

<span data-ttu-id="e3735-257">ユーザーの既定ノートブックにあるすべてのセクションの名前と **pagesUrl** リンクを取得します。</span><span class="sxs-lookup"><span data-stu-id="e3735-257">Get the name and **pagesUrl** link for all sections in the user's default notebook.</span></span>

```
[GET] ../notebooks?select=name&expand=sections(select=name,pagesUrl)&filter=isDefault eq true
```

### <a name="top--select--orderby"></a><span data-ttu-id="e3735-258">top & select & orderby</span><span class="sxs-lookup"><span data-stu-id="e3735-258">top & select & orderby</span></span> 

<span data-ttu-id="e3735-p116">最初の 50 ページのタイトルと **self** リンクを取得します。タイトルのアルファベット順に並べられます。既定ではこの API は 20 エントリを返します。最大では 100 エントリを返します。ページの既定の並べ替え順序は `lastModifiedTime desc` です。</span><span class="sxs-lookup"><span data-stu-id="e3735-p116">Get the title and **self** link for the first 50 pages, ordered alphabetically by title. The API returns 20 entries by default with a maximum of 100. The default sort order for pages is `lastModifiedTime desc`.</span></span>

```
[GET] ../pages?top=50&select=title,self&orderby=title
```

### <a name="skip--top--select--orderby"></a><span data-ttu-id="e3735-262">skip & top & select & orderby</span><span class="sxs-lookup"><span data-stu-id="e3735-262">skip & top & select & orderby</span></span>  

<span data-ttu-id="e3735-p117">51 ページ目から 100 ページ目までを取得します。既定ではこの API は 20 エントリを返します。最大では 100 エントリを返します。</span><span class="sxs-lookup"><span data-stu-id="e3735-p117">Get pages 51 to 100. The API returns 20 entries by default with a maximum of 100.</span></span>

```
[GET] ../pages?skip=50&top=50&select=title,self&orderby=title
```

> <span data-ttu-id="e3735-265">**注:** 既定のエントリ数を取得する pages に対する GET 要求 (つまり、**top** 式を指定しない要求) は、応答で次の 20 エントリを取得するために使用できる **@odata.nextLink** リンクを戻します。</span><span class="sxs-lookup"><span data-stu-id="e3735-265">**Note:** GET requests for pages that retrieve the default number of entries (that is, they don't specify a **top** expression) return an **@odata.nextLink** link in the response that you can use to get the next 20 entries.</span></span>
 

<a name="supported-odata-query-string-options"></a>

## <a name="supported-odata-query-string-options"></a><span data-ttu-id="e3735-266">サポートされている OData クエリ文字列オプション</span><span class="sxs-lookup"><span data-stu-id="e3735-266">Supported OData query string options</span></span>

<span data-ttu-id="e3735-267">Microsoft Graph に GET 要求を送信する場合、OData クエリ文字列オプションを使用してクエリをカスタマイズして、必要な情報だけを取得できます。</span><span class="sxs-lookup"><span data-stu-id="e3735-267">When sending GET requests to Microsoft Graph, you can use OData query string options to customize your query and get just the information you need.</span></span> <span data-ttu-id="e3735-268">このオプションを使用することにより、サービスへの呼び出し回数が減り、応答ペイロードのサイズが小さくなるので、パフォーマンスも向上します。</span><span class="sxs-lookup"><span data-stu-id="e3735-268">They can also improve performance by reducing the number of calls to the service and the size of the response payload.</span></span>

> <span data-ttu-id="e3735-269">**注:** この記事の例では読みやすくするために、URL クエリ文字列内のスペースで必要な %20 パーセント エンコードを使用していません: `filter=isDefault%20eq%20true`</span><span class="sxs-lookup"><span data-stu-id="e3735-269">**Note:** For readability, the examples in this article don't use the %20 percent-encoding required for spaces in the URL query string: `filter=isDefault%20eq%20true`</span></span>
 
| <span data-ttu-id="e3735-270">クエリ オプション</span><span class="sxs-lookup"><span data-stu-id="e3735-270">Query option</span></span> | <span data-ttu-id="e3735-271">例と説明</span><span class="sxs-lookup"><span data-stu-id="e3735-271">Example and description</span></span> |  
|------|------|  
| <span data-ttu-id="e3735-272">count</span><span class="sxs-lookup"><span data-stu-id="e3735-272">count</span></span> | <p>`count=true`</p><p><span data-ttu-id="e3735-p119">コレクション内のエンティティのカウントです。この値は、応答の **@odata.count** プロパティで戻ります。</span><span class="sxs-lookup"><span data-stu-id="e3735-p119">The count of entities in the collection. The value is returned in the **@odata.count** property in the response.</span></span></p> |  
| <span data-ttu-id="e3735-275">expand</span><span class="sxs-lookup"><span data-stu-id="e3735-275">expand</span></span> | <p>`expand=sections,sectionGroups`</p><p><span data-ttu-id="e3735-p120">応答でインラインを返すナビゲーション プロパティ。**expand** 式には次のプロパティがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="e3735-p120">The navigation properties to return inline in the response. The following properties are supported for **expand** expressions:</span></span><br /> <span data-ttu-id="e3735-278">- ページ: **parentNotebook**、**parentSection**</span><span class="sxs-lookup"><span data-stu-id="e3735-278">- Pages: **parentNotebook**, **parentSection**</span></span><br /> <span data-ttu-id="e3735-279">- セクション: **parentNotebook**、**parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="e3735-279">- Sections: **parentNotebook**, **parentSectionGroup**</span></span><br /> <span data-ttu-id="e3735-280">- セクション グループ: **sections**、**sectionGroups**、**parentNotebook**、**parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="e3735-280">- Section groups: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**</span></span><br /> <span data-ttu-id="e3735-281">- ノートブック: **sections**、**sectionGroups**</span><span class="sxs-lookup"><span data-stu-id="e3735-281">- Notebooks: **sections**, **sectionGroups**</span></span></p><p><span data-ttu-id="e3735-p121">既定では、ページの GET 要求は **parentSection** を展開し、セクションの **id**、**name**、**self** の各プロパティを選択します。セクションとセクションのグループの既定の GET 要求は **parentNotebook** と **parentSectionGroup** の両方を展開し、親の **id**、**name**、**self** の各プロパティを選択します。</span><span class="sxs-lookup"><span data-stu-id="e3735-p121">By default, GET requests for pages expands **parentSection** and select the section's **id**, **name**, and **self** properties. Default GET requests for sections and section groups expand both **parentNotebook** and **parentSectionGroup**, and select the parents' **id**, **name**, and **self** properties. </span></span></p><p><span data-ttu-id="e3735-284">1 つのエンティティまたはコレクションに使用できます。</span><span class="sxs-lookup"><span data-stu-id="e3735-284">Can be used for a single entity or a collection.</span></span><br /><span data-ttu-id="e3735-285">コンマを使用して複数のプロパティを区切ります。</span><span class="sxs-lookup"><span data-stu-id="e3735-285">Separate multiple properties with commas.</span></span><br /><span data-ttu-id="e3735-286">プロパティ名では、大文字と小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="e3735-286">Property names are not case-sensitive</span></span></p> |   
| <span data-ttu-id="e3735-287">filter</span><span class="sxs-lookup"><span data-stu-id="e3735-287">filter</span></span> | <p>`filter=isDefault eq true`</p><p><span data-ttu-id="e3735-p122">結果セットの入力に含めるかどうかを決めるブール式。サポートされている OData 演算子と関数:</span><span class="sxs-lookup"><span data-stu-id="e3735-p122">A Boolean expression for whether to include an entry in the result set. Supports the following OData operators and functions:</span></span><br /> <span data-ttu-id="e3735-290">- 比較演算子: **eq**、**ne**、**gt**、**ge**、**lt**、**le**</span><span class="sxs-lookup"><span data-stu-id="e3735-290">- Comparison operators: **eq**, **ne**, **gt**, **ge**, **lt**, **le**</span></span><br /> <span data-ttu-id="e3735-291">- 論理演算子: **and**、**or**、**not**</span><span class="sxs-lookup"><span data-stu-id="e3735-291">- Logical operators: **and**, **or**, **not**</span></span><br /> <span data-ttu-id="e3735-292">- 文字列関数: **contains**、**endswith**、**startswith**、**length**、**indexof**、**substring**、**tolower**、**toupper**、**trim**、**concat**</span><span class="sxs-lookup"><span data-stu-id="e3735-292">- String functions: **contains**, **endswith**, **startswith**, **length**, **indexof**, **substring**, **tolower**, **toupper**, **trim**, **concat**</span></span></p><p><span data-ttu-id="e3735-293">[プロパティ](#onenote-entity-properties)名と OData 文字列比較では大文字と小文字が区別されます。</span><span class="sxs-lookup"><span data-stu-id="e3735-293">[Property](#onenote-entity-properties) names and OData string comparisons are case sensitive.</span></span> <span data-ttu-id="e3735-294">文字列比較には OData **tolower** 関数を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="e3735-294">We recommend using the OData **tolower** function for string comparisons.</span></span><br /><br /><span data-ttu-id="e3735-295">**例**: `filter=tolower(name) eq 'spring'`</span><span class="sxs-lookup"><span data-stu-id="e3735-295">Example: </span></span></p> |  
| <span data-ttu-id="e3735-296">orderby</span><span class="sxs-lookup"><span data-stu-id="e3735-296">orderby</span></span> | <p>`orderby=title,createdTime desc`</p><p><span data-ttu-id="e3735-p124">並べ替え基準を示す[プロパティ](#onenote-entity-properties)です。オプションで、**asc** (既定) または **desc** 並べ替え順序を指定します。要求対象コレクション内のエンティティの任意のプロパティで並べ替えが可能です。</span><span class="sxs-lookup"><span data-stu-id="e3735-p124">The [properties](#onenote-entity-properties) to sort by, with an optional **asc** (default) or **desc** sort order. You can sort by any property of the entity in the requested collection.</span></span></p><p><span data-ttu-id="e3735-299">ノートブック、セクション グループ、セクションの既定の並べ替え順序は `name asc` で、ページの場合には `lastModifiedTime desc` (最新の変更ページが先頭になります)。</span><span class="sxs-lookup"><span data-stu-id="e3735-299">The default sort order for notebooks, section groups, and sections is `name asc`, and for pages is `lastModifiedTime desc` (last modified page first).</span></span></p><p><span data-ttu-id="e3735-300">複数のプロパティはコンマで区切り、任意の順序で一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="e3735-300">Separate multiple properties with commas, and list them in the order that you want them applied.</span></span> <span data-ttu-id="e3735-301">プロパティ名では、大文字と小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="e3735-301">Property names are not case-sensitive</span></span></p> |  
| <span data-ttu-id="e3735-302">search</span><span class="sxs-lookup"><span data-stu-id="e3735-302">search</span></span> | <p>`search=cell div`</p><p><span data-ttu-id="e3735-303">コンシューマー ノートパソコンでのみ使用可能。</span><span class="sxs-lookup"><span data-stu-id="e3735-303">Available for consumer notebooks only.</span></span></p><p><span data-ttu-id="e3735-p126">ページ タイトル、ページ本文、画像の代替テキスト、画像の OCR テキストで検索する用語または語句です。既定では、検索クエリは関連度で並べ替えて結果を返します。</span><span class="sxs-lookup"><span data-stu-id="e3735-p126">The term or phrase to search for in the page title, page body, image alt text, and image OCR text. By default, search queries return results sorted by relevance.</span></span></p><p><span data-ttu-id="e3735-306">OneNote は、Bing のフルテキスト検索を使用して、語句の検索、語形変化、スペルの曖昧さ、関連性とランキング、単語分割、複数の言語、他のフルテキスト検索機能をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e3735-306">OneNote uses Bing full-text search to support phrase search, stemming, spelling forgiveness, relevance and ranking, word breaking, multiple languages, and other full-text search features.</span></span> <span data-ttu-id="e3735-307">検索文字列では、大文字と小文字が区別されません。</span><span class="sxs-lookup"><span data-stu-id="e3735-307">Search strings are case-insensitive.</span></span></p><p><span data-ttu-id="e3735-308">ユーザーが所有しているノートブック内のページにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="e3735-308">Applies only to pages in notebooks owned by the user (not shared with the user).</span></span> <span data-ttu-id="e3735-309">インデックス付けされたコンテンツは非公開であり、所有者のみがアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="e3735-309">Indexed content is private and can only be accessed by the owner.</span></span> <span data-ttu-id="e3735-310">パスワードで保護されたページにはインデックスは付けられません。</span><span class="sxs-lookup"><span data-stu-id="e3735-310">Password-protected pages are not indexed.</span></span> <span data-ttu-id="e3735-311">`pages` エンドポイントにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="e3735-311">Applies only to the `pages` endpoint.</span></span></p> |  
| <span data-ttu-id="e3735-312">select</span><span class="sxs-lookup"><span data-stu-id="e3735-312">select</span></span> | <p>`select=id,title`</p><p><span data-ttu-id="e3735-313">返す[プロパティ](#onenote-entity-properties)。</span><span class="sxs-lookup"><span data-stu-id="e3735-313">The [properties](#onenote-entity-properties) to return.</span></span> <span data-ttu-id="e3735-314">1 つのエンティティまたはコレクションに使用できます。</span><span class="sxs-lookup"><span data-stu-id="e3735-314">Can be used for a single entity or for a collection.</span></span> <span data-ttu-id="e3735-315">コンマを使用して複数のプロパティを区切ります。</span><span class="sxs-lookup"><span data-stu-id="e3735-315">Separate multiple properties with commas.</span></span> <span data-ttu-id="e3735-316">プロパティ名では、大文字と小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="e3735-316">Property names are not case-sensitive</span></span></p> |  
| <span data-ttu-id="e3735-317">skip</span><span class="sxs-lookup"><span data-stu-id="e3735-317">skip</span></span> | <p>`skip=10`</p><p><span data-ttu-id="e3735-p130">結果セットでスキップするエントリの数。通常、結果のページングに使用されます。</span><span class="sxs-lookup"><span data-stu-id="e3735-p130">The number of entries to skip in the result set. Typically used for paging results.</span></span></p> |  
| <span data-ttu-id="e3735-320">top</span><span class="sxs-lookup"><span data-stu-id="e3735-320">top</span></span> | <p>`top=50`</p><p><span data-ttu-id="e3735-p131">結果セット内で返すエントリ数で、最大数は 100 です。既定値は 20 です。</span><span class="sxs-lookup"><span data-stu-id="e3735-p131">The number of entries to return in the result set, up to a maximum of 100. The default value is 20.</span></span></p> |  

<span data-ttu-id="e3735-323">Microsoft Graph にも、親セクション内でページのレベルと順序を取得する `pagelevel` クエリ文字列オプションが用意されています。</span><span class="sxs-lookup"><span data-stu-id="e3735-323">Microsoft Graph also provides the `pagelevel` query string option you can use to get the level and order of pages within the parent section.</span></span> <span data-ttu-id="e3735-324">特定のセクションのページのクエリ、または特定のページのクエリにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="e3735-324">Applies only to queries for pages in a specific section or queries for a specific page.</span></span> 

#### <a name="examples"></a><span data-ttu-id="e3735-325">例</span><span class="sxs-lookup"><span data-stu-id="e3735-325">Examples</span></span> 

- `GET ../sections/{section-id}/pages?pagelevel=true` 
- `GET ../pages/{page-id}?pagelevel=true` 

### <a name="supported-odata-operators-and-functions"></a><span data-ttu-id="e3735-326">サポートされている OData 演算子と関数</span><span class="sxs-lookup"><span data-stu-id="e3735-326">Supported OData operators and functions</span></span>

<span data-ttu-id="e3735-327">Microsoft Graph は、**フィルター**式で次の OData 演算子および関数をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="e3735-327">Microsoft Graph supports the following OData operators and functions in **filter** expressions.</span></span> <span data-ttu-id="e3735-328">OData 式を使用する場合には、次の点に注意してください。</span><span class="sxs-lookup"><span data-stu-id="e3735-328">When using OData expressions, remember:</span></span>

- <span data-ttu-id="e3735-329">URL クエリ文字列のスペースは `%20` エンコードで置換する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e3735-329">Spaces in the URL query string must be replaced with the `%20` encoding.</span></span><br/><br/><span data-ttu-id="e3735-330">**例:** `filter=isDefault%20eq%20true`</span><span class="sxs-lookup"><span data-stu-id="e3735-330">**Example:** `filter=isDefault%20eq%20true`</span></span>

- <span data-ttu-id="e3735-331">プロパティ名と OData 文字列比較では大文字と小文字が区別されます。</span><span class="sxs-lookup"><span data-stu-id="e3735-331">Property names and OData string comparisons are case sensitive.</span></span> <span data-ttu-id="e3735-332">文字列比較には OData **tolower** 関数を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="e3735-332">We recommend using the OData **tolower** function for string comparisons.</span></span><br/><br/><span data-ttu-id="e3735-333">**例:** `filter=tolower(name) eq 'spring'`</span><span class="sxs-lookup"><span data-stu-id="e3735-333">**Example:** `filter=tolower(name) eq 'spring'`</span></span>


| <span data-ttu-id="e3735-334">比較演算子</span><span class="sxs-lookup"><span data-stu-id="e3735-334">Comparison operator</span></span> | <span data-ttu-id="e3735-335">例</span><span class="sxs-lookup"><span data-stu-id="e3735-335">Example</span></span> |  
|------|------|  
| <span data-ttu-id="e3735-336">eq</span><span class="sxs-lookup"><span data-stu-id="e3735-336">eq</span></span><br /><span data-ttu-id="e3735-337">(等しい)</span><span class="sxs-lookup"><span data-stu-id="e3735-337">(equal to)</span></span> | `createdByAppId eq '{app-id}'` |  
| <span data-ttu-id="e3735-338">ne</span><span class="sxs-lookup"><span data-stu-id="e3735-338">ne</span></span><br /><span data-ttu-id="e3735-339">(等しくない)</span><span class="sxs-lookup"><span data-stu-id="e3735-339">(not equal to)</span></span> | `userRole ne 'Owner'` |  
| <span data-ttu-id="e3735-340">gt</span><span class="sxs-lookup"><span data-stu-id="e3735-340">gt</span></span><br /><span data-ttu-id="e3735-341">(より大きい)</span><span class="sxs-lookup"><span data-stu-id="e3735-341">(greater than)</span></span> | `createdTime gt 2014-02-23` |  
| <span data-ttu-id="e3735-342">ge</span><span class="sxs-lookup"><span data-stu-id="e3735-342">ge</span></span><br /><span data-ttu-id="e3735-343">(以上)</span><span class="sxs-lookup"><span data-stu-id="e3735-343">(greater than or equal to)</span></span> | `lastModifiedTime ge 2014-05-05T07:00:00Z` |  
| <span data-ttu-id="e3735-344">lt</span><span class="sxs-lookup"><span data-stu-id="e3735-344">lt</span></span><br /><span data-ttu-id="e3735-345">(より小さい)</span><span class="sxs-lookup"><span data-stu-id="e3735-345">(less than)</span></span> | `createdTime lt 2014-02-23` |  
| <span data-ttu-id="e3735-346">le</span><span class="sxs-lookup"><span data-stu-id="e3735-346">le</span></span><br /><span data-ttu-id="e3735-347">(以下)</span><span class="sxs-lookup"><span data-stu-id="e3735-347">(less than or equal to)</span></span> | `lastModifiedTime le 2014-02-23` |  

<br/>

| <span data-ttu-id="e3735-348">論理演算子</span><span class="sxs-lookup"><span data-stu-id="e3735-348">Logical operator</span></span> | <span data-ttu-id="e3735-349">例</span><span class="sxs-lookup"><span data-stu-id="e3735-349">Example</span></span> |  
|------|------|  
| <span data-ttu-id="e3735-350">and</span><span class="sxs-lookup"><span data-stu-id="e3735-350">and</span></span> | `createdTime le 2014-01-30 and createdTime gt 2014-01-23` |  
| <span data-ttu-id="e3735-351">or</span><span class="sxs-lookup"><span data-stu-id="e3735-351">or</span></span> | `createdByAppId eq '{app-id}' or createdByAppId eq '{app-id}'` |  
| <span data-ttu-id="e3735-352">not</span><span class="sxs-lookup"><span data-stu-id="e3735-352">not</span></span> | `not contains(tolower(title),'school')` |  

<br/>
  
| <span data-ttu-id="e3735-353">String 関数</span><span class="sxs-lookup"><span data-stu-id="e3735-353">String function</span></span> | <span data-ttu-id="e3735-354">例</span><span class="sxs-lookup"><span data-stu-id="e3735-354">Example</span></span> |  
|------|------|   
| <span data-ttu-id="e3735-355">contains</span><span class="sxs-lookup"><span data-stu-id="e3735-355">contains</span></span> | `contains(tolower(title),'spring')` |  
| <span data-ttu-id="e3735-356">endswith</span><span class="sxs-lookup"><span data-stu-id="e3735-356">endswith</span></span> | `endswith(tolower(title),'spring')` |  
| <span data-ttu-id="e3735-357">startswith</span><span class="sxs-lookup"><span data-stu-id="e3735-357">startswith</span></span> | `startswith(tolower(title),'spring')` |  
| <span data-ttu-id="e3735-358">length</span><span class="sxs-lookup"><span data-stu-id="e3735-358">length</span></span> | `length(title) eq 19` |  
| <span data-ttu-id="e3735-359">indexof</span><span class="sxs-lookup"><span data-stu-id="e3735-359">indexof</span></span> | `indexof(tolower(title),'spring') eq 1` |  
| <span data-ttu-id="e3735-360">substring</span><span class="sxs-lookup"><span data-stu-id="e3735-360">substring</span></span> | `substring(tolower(title),1) eq 'spring'` |  
| <span data-ttu-id="e3735-361">tolower</span><span class="sxs-lookup"><span data-stu-id="e3735-361">tolower</span></span> | `tolower(title) eq 'spring'` |  
| <span data-ttu-id="e3735-362">toupper</span><span class="sxs-lookup"><span data-stu-id="e3735-362">toupper</span></span> | `toupper(title) eq 'SPRING'` |  
| <span data-ttu-id="e3735-363">trim</span><span class="sxs-lookup"><span data-stu-id="e3735-363">trim</span></span> | `trim(tolower(title)) eq 'spring'` |  
| <span data-ttu-id="e3735-364">concat</span><span class="sxs-lookup"><span data-stu-id="e3735-364">concat</span></span> | `concat(title,'- by MyRecipesApp') eq 'Carrot Cake Recipe - by MyRecipesApp'` |  
 

<a name="properties"></a>

## <a name="onenote-entity-properties"></a><span data-ttu-id="e3735-365">OneNote エンティティのプロパティ</span><span class="sxs-lookup"><span data-stu-id="e3735-365">OneNote entity properties</span></span>

<span data-ttu-id="e3735-366">**filter**、**select**、**expand**、および **orderby** クエリ式には、OneNote エンティティのプロパティを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="e3735-366">The **filter**, **select**, **expand**, and **orderby** query expressions can include properties of OneNote entities.</span></span> 

#### <a name="example"></a><span data-ttu-id="e3735-367">例</span><span class="sxs-lookup"><span data-stu-id="e3735-367">Example</span></span>

`../sections?filter=createdTime ge 2015-01-01&select=name,pagesUrl&orderby=lastModifiedTime desc` 

<span data-ttu-id="e3735-368">クエリ式のプロパティ名は大文字小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="e3735-368">Property names are case sensitive in query expressions.</span></span>

<span data-ttu-id="e3735-369">プロパティとプロパティの種類の一覧については、Microsoft Graph API REST リファレンスの中の次のリソースを参照してください。</span><span class="sxs-lookup"><span data-stu-id="e3735-369">For the list of properties and property types, see the following resources in the Microsoft Graph API REST reference:</span></span>

- [<span data-ttu-id="e3735-370">ページを取得する</span><span class="sxs-lookup"><span data-stu-id="e3735-370">GET Pages</span></span>](../api-reference/v1.0/api/page_get.md)
- [<span data-ttu-id="e3735-371">Get section</span><span class="sxs-lookup"><span data-stu-id="e3735-371">GET Sections</span></span>](../api-reference/v1.0/api/section_get.md)
- [<span data-ttu-id="e3735-372">Get sectionGroup</span><span class="sxs-lookup"><span data-stu-id="e3735-372">GET SectionGroups</span></span>](../api-reference/v1.0/api/sectiongroup_get.md)
- [<span data-ttu-id="e3735-373">ノートブックを取得する</span><span class="sxs-lookup"><span data-stu-id="e3735-373">GET Notebooks</span></span>](../api-reference/v1.0/api/notebook_get.md) 



<span data-ttu-id="e3735-374">**expand** クエリ文字列オプションは、以下のナビゲーション プロパティとともに使用できます。</span><span class="sxs-lookup"><span data-stu-id="e3735-374">The **expand** query string option can be used with the following navigation properties:</span></span>

- <span data-ttu-id="e3735-375">ページ: **parentNotebook**、**parentSection**</span><span class="sxs-lookup"><span data-stu-id="e3735-375">Pages: **parentNotebook**, **parentSection**</span></span>
- <span data-ttu-id="e3735-376">セクション: **parentNotebook**、**parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="e3735-376">Sections: **parentNotebook**, **parentSectionGroup**</span></span>
- <span data-ttu-id="e3735-377">セクション グループ: **sections**、**sectionGroups**、**parentNotebook**、**parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="e3735-377">Section groups: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**</span></span>
- <span data-ttu-id="e3735-378">ノートブック: **sections**、**sectionGroups**</span><span class="sxs-lookup"><span data-stu-id="e3735-378">Notebooks: **sections**, **sectionGroups**</span></span>


<a name="request-response-info"></a>

## <a name="request-and-response-information-for-get-requests"></a><span data-ttu-id="e3735-379">要求および *GET* 要求の応答に関する情報</span><span class="sxs-lookup"><span data-stu-id="e3735-379">Request and response information for *GET* requests</span></span>

| <span data-ttu-id="e3735-380">要求データ</span><span class="sxs-lookup"><span data-stu-id="e3735-380">Request data</span></span> | <span data-ttu-id="e3735-381">説明</span><span class="sxs-lookup"><span data-stu-id="e3735-381">Description</span></span> |  
|------|------|  
| <span data-ttu-id="e3735-382">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e3735-382">Protocol</span></span> | <span data-ttu-id="e3735-383">すべての要求は SSL/TLS HTTPS プロトコルを使用します。</span><span class="sxs-lookup"><span data-stu-id="e3735-383">All requests use the SSL/TLS HTTPS protocol.</span></span> |  
| <span data-ttu-id="e3735-384">承認ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3735-384">Authorization header</span></span> | <p><span data-ttu-id="e3735-385">`Bearer {token}`。`{token}` は、登録済みアプリの有効な OAuth 2.0 アクセス トークンです。</span><span class="sxs-lookup"><span data-stu-id="e3735-385">`Bearer {token}`, where `{token}` is a valid OAuth 2.0 access token for your registered app.</span></span></p><p><span data-ttu-id="e3735-p135">これがないか、無効の場合、401 ステータス コードで要求は失敗します。「[認証とアクセス許可](permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e3735-p135">If missing or invalid, the request fails with a 401 status code. See [Authentication and permissions](permissions_reference.md).</span></span></p> |  
| <span data-ttu-id="e3735-388">Accept ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3735-388">Accept header</span></span> | <p> <span data-ttu-id="e3735-389">OneNote エンティティとエンティティ セットの場合、`application/json`</span><span class="sxs-lookup"><span data-stu-id="e3735-389">`application/json` for OneNote entities and entity sets</span></span></p><p> <span data-ttu-id="e3735-390">ページ コンテンツの場合、`text/html`</span><span class="sxs-lookup"><span data-stu-id="e3735-390">`text/html` for page content</span></span></p> | 

<br/>

| <span data-ttu-id="e3735-391">応答データ</span><span class="sxs-lookup"><span data-stu-id="e3735-391">Response data</span></span> | <span data-ttu-id="e3735-392">説明</span><span class="sxs-lookup"><span data-stu-id="e3735-392">Description</span></span> |  
|------|------|  
| <span data-ttu-id="e3735-393">成功コード</span><span class="sxs-lookup"><span data-stu-id="e3735-393">Success code</span></span> | <span data-ttu-id="e3735-394">200 HTTP ステータス コード。</span><span class="sxs-lookup"><span data-stu-id="e3735-394">A 200 HTTP status code.</span></span> |  
| <span data-ttu-id="e3735-395">応答本文</span><span class="sxs-lookup"><span data-stu-id="e3735-395">Response body</span></span> | <span data-ttu-id="e3735-396">JSON 形式のエンティティまたはエンティティ セット、ページ HTML、またはファイル リソースのバイナリ データの OData 表現。</span><span class="sxs-lookup"><span data-stu-id="e3735-396">An OData representation of the entity or entity set in JSON format, the page HTML, or file resource binary data.</span></span>  |  
| <span data-ttu-id="e3735-397">エラー</span><span class="sxs-lookup"><span data-stu-id="e3735-397">Errors</span></span> | <span data-ttu-id="e3735-398">要求が失敗すると、API は応答本文の **@api.diagnostics** オブジェクトに[エラー](onenote_error_codes.md)を返します。</span><span class="sxs-lookup"><span data-stu-id="e3735-398">If the request fails, the API returns [errors](onenote_error_codes.md) in the **@api.diagnostics** object in the response body.</span></span> |  
| <span data-ttu-id="e3735-399">X-CorrelationId ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3735-399">X-CorrelationId header</span></span> | <span data-ttu-id="e3735-p136">要求を一意に識別する GUID。Microsoft サポートと問題のトラブルシューティングを行う際に、この値を Date ヘッダーの値とともに使用できます。</span><span class="sxs-lookup"><span data-stu-id="e3735-p136">A GUID that uniquely identifies the request. You can use this value along with the value of the Date header when working with Microsoft support to troubleshoot issues.</span></span> |  


<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-notes-service-root-url"></a><span data-ttu-id="e3735-402">Microsoft Graph のノート サービスのルート URL の構築</span><span class="sxs-lookup"><span data-stu-id="e3735-402">Constructing the Microsoft Graph notes service root URL</span></span>

<span data-ttu-id="e3735-403">Microsoft Graph ノートのルート URL は、Microsoft Graph ノートへのすべての呼び出しで次の形式を使用します。</span><span class="sxs-lookup"><span data-stu-id="e3735-403">The Microsoft Graph notes root URL uses the following format for all calls to Microsoft Graph notes.</span></span>

`https://graph.microsoft.com/{version}/me/onenote/`  

<span data-ttu-id="e3735-404">URL の `version` セグメントは、使用する Microsoft Graph のバージョンを示しています。</span><span class="sxs-lookup"><span data-stu-id="e3735-404">The `version` segment in the URL represents the version of Microsoft Graph that you want to use.</span></span> <span data-ttu-id="e3735-405">安定した運用コードには `v1.0` を使用します。</span><span class="sxs-lookup"><span data-stu-id="e3735-405">Use `v1.0` for stable production code.</span></span> <span data-ttu-id="e3735-406">開発中の機能を試すには `beta` を使用します。</span><span class="sxs-lookup"><span data-stu-id="e3735-406">Use `beta` to try out a feature that's in development.</span></span> <span data-ttu-id="e3735-407">ベータ版の機能は変更される可能性があるため、運用コードでは使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="e3735-407">Features and functionality in beta may change, so you shouldn't use it in your production code.</span></span> 

<span data-ttu-id="e3735-408">現在のユーザーがアクセスできる OneNote コンテンツには `me` を使用します (所有と共有)。</span><span class="sxs-lookup"><span data-stu-id="e3735-408">Use `me` for OneNote content that the current user can access (owned and shared).</span></span> <span data-ttu-id="e3735-409">指定されたユーザー (URL 内) が現在のユーザーと共有している OneNote コンテンツには `users/{id}` を使用します。</span><span class="sxs-lookup"><span data-stu-id="e3735-409">Use `users/{id}` for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="e3735-410">ユーザー ID を取得するには [Microsoft Graph](https://graph.microsoft.com/v1.0/users) を使用します。</span><span class="sxs-lookup"><span data-stu-id="e3735-410">Use the [Microsoft Graph](https://graph.microsoft.com/v1.0/users) to get user IDs.</span></span> 


<a name="permissions"></a>

## <a name="permissions-for-get-requests"></a><span data-ttu-id="e3735-411">GET 要求のアクセス許可</span><span class="sxs-lookup"><span data-stu-id="e3735-411">Permissions for GET requests</span></span>

<span data-ttu-id="e3735-412">OneNote のコンテンツまたは構造を取得するには、適切なアクセス許可を要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e3735-412">To get OneNote content or structure, you'll need to request appropriate permissions.</span></span> 

<span data-ttu-id="e3735-413">次のスコープは、Microsoft Graph に対する GET 要求を許可します。</span><span class="sxs-lookup"><span data-stu-id="e3735-413">The following scopes allow GET requests to Microsoft Graph.</span></span> <span data-ttu-id="e3735-414">アプリの動作に必要な最低限のアクセス許可を選択してください。</span><span class="sxs-lookup"><span data-stu-id="e3735-414">Choose the lowest level of permissions that your app needs to do its work.</span></span>

<span data-ttu-id="e3735-415">次から選択します。</span><span class="sxs-lookup"><span data-stu-id="e3735-415">Choose from:</span></span>

- <span data-ttu-id="e3735-416">Notes.read</span><span class="sxs-lookup"><span data-stu-id="e3735-416">Notes.read</span></span>
- <span data-ttu-id="e3735-417">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e3735-417">Notes.ReadWrite</span></span>
- <span data-ttu-id="e3735-418">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3735-418">Notes.ReadWrite.All</span></span>

<span data-ttu-id="e3735-419">アクセス許可の範囲とその動作方法の詳細については、「[Microsoft Graph のアクセス許可のリファレンス](permissions_reference.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="e3735-419">For more information about permission scopes and how they work, see [Microsoft Graph permissions reference](permissions_reference.md).</span></span>

<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="e3735-420">関連項目</span><span class="sxs-lookup"><span data-stu-id="e3735-420">See also</span></span>

- [<span data-ttu-id="e3735-421">OneNote ページの入出力 HTML</span><span class="sxs-lookup"><span data-stu-id="e3735-421">Input and output HTML for OneNote pages</span></span>](onenote_input_output_html.md)
- [<span data-ttu-id="e3735-422">OneNote との統合</span><span class="sxs-lookup"><span data-stu-id="e3735-422">Integrate with OneNote</span></span>](integrate_with_onenote.md)
- [<span data-ttu-id="e3735-423">OneNote の開発者ブログ</span><span class="sxs-lookup"><span data-stu-id="e3735-423">OneNote Developer Blog</span></span>](http://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="e3735-424">Stack Overflow 掲載の OneNote の開発に関する質問</span><span class="sxs-lookup"><span data-stu-id="e3735-424">OneNote development questions on Stack Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="e3735-425">OneNote GitHub のリポジトリ</span><span class="sxs-lookup"><span data-stu-id="e3735-425">OneNote GitHub repos</span></span>](http://go.microsoft.com/fwlink/?LinkID=390178)  
