# <a name="get-onenote-content-and-structure-with-microsoft-graph"></a><span data-ttu-id="90ac2-101">Microsoft Graph によって OneNote コンテンツと構造を取得する</span><span class="sxs-lookup"><span data-stu-id="90ac2-101">Get OneNote content and structure with Microsoft Graph</span></span>

<span data-ttu-id="90ac2-102">*__適用対象:__ OneDrive のコンシューマー ノートブック | Office 365 のエンタープライズ ノートブック*</span><span class="sxs-lookup"><span data-stu-id="90ac2-102">*__Applies to:__ Consumer notebooks on OneDrive | Enterprise notebooks on Office 365*</span></span>

<span data-ttu-id="90ac2-p101">OneNote のコンテンツと構造を取得するには、ターゲット エンドポイントに GET 要求を送信します。たとえば次のようにします。</span><span class="sxs-lookup"><span data-stu-id="90ac2-p101">To get OneNote content and structure, you send a GET request to the target endpoint. For example:</span></span>

`GET ../onenote/pages/{id}`</p>

<span data-ttu-id="90ac2-105">要求が成功すると、Microsoft Graph は 200 HTTP 状態コードと、要求したエンティティまたはコンテンツを返します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-105">If the request is successful, the OneNote API returns a 200 HTTP status code and the entities or content that you requested. OneNote entities are returned as JSON objects that conform to the OData version 4.0 specification.</span></span> <span data-ttu-id="90ac2-106">OneNote のエンティティは、OData バージョン 4.0 仕様に準拠した JSON オブジェクトとして返されます。</span><span class="sxs-lookup"><span data-stu-id="90ac2-106">If the request is successful, the OneNote API returns a 200 HTTP status code and the entities or content that you requested. OneNote entities are returned as JSON objects that conform to the OData version 4.0 specification.</span></span>

<span data-ttu-id="90ac2-107">クエリ文字列オプションを使用すると、クエリをフィルターしてパフォーマンスを向上させることができます。</span><span class="sxs-lookup"><span data-stu-id="90ac2-107">By using query string options, you can filter your queries and improve performance.</span></span>


<a name="request-uri"></a>
## <a name="construct-the-request-uri"></a><span data-ttu-id="90ac2-108">要求 URI の構築</span><span class="sxs-lookup"><span data-stu-id="90ac2-108">Construct the request URI</span></span>

<span data-ttu-id="90ac2-109">要求 URI を構築するには、サービス ルート URL から開始します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-109">To construct the request URI, start with the service root URL:</span></span>

`https://graph.microsoft.com/v1.0/me/onenote`

<span data-ttu-id="90ac2-110">次に、取得するリソースのエンドポイントを追加します </span><span class="sxs-lookup"><span data-stu-id="90ac2-110">Then append the endpoint of the resource you want to retrieve.</span></span> <span data-ttu-id="90ac2-111">([リソース パス](#resource-paths-for-get-requests)が次のセクションに表示されます)。</span><span class="sxs-lookup"><span data-stu-id="90ac2-111">([Resource paths](#resource-paths-for-get-requests) are shown in the next section.)</span></span>


<span data-ttu-id="90ac2-112">完全な要求 URI は、次に示す例のいずれかのようになります。</span><span class="sxs-lookup"><span data-stu-id="90ac2-112">Your full request URI will look like one of these examples:</span></span>
- `https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sections`</p>
- `https://graph.microsoft.com/v1.0/me/onenote/notes/pages`</p>
- `https://graph.microsoft.com/v1.0/me/onenote/pages?select=title,self`</p>

> <span data-ttu-id="90ac2-113">**注:** [サービス ルート URL](../api-reference/v1.0/resources/onenote-api-overview.md#root-url) の詳細についてはリンク先をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="90ac2-113">Learn more about the [service root URL](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span></span>

<a name="resource-paths"></a>
## <a name="resource-paths-for-get-requests"></a><span data-ttu-id="90ac2-114">GET 要求のリソース パス</span><span class="sxs-lookup"><span data-stu-id="90ac2-114">Resource paths for GET requests</span></span>

<span data-ttu-id="90ac2-115">次のリソース パスを使用して、ページ、セクション、セクション グループ、ノートブック、画像、またはファイル リソースを取得します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-115">Use the following resource paths to get pages, sections, section groups, notebooks, and image or file resources.</span></span>

<span data-ttu-id="90ac2-116">[ページ コレクション](#page-collection)&nbsp;&nbsp;|&nbsp;&nbsp;[ページ エンティティ](#page-entity)&nbsp;&nbsp;|&nbsp;&nbsp;[ページ プレビュー](#page-preview)&nbsp;&nbsp;|&nbsp;&nbsp;[ページ HTML コンテンツ](#page-html-content)&nbsp;&nbsp;|&nbsp;&nbsp; [セクション コレクション](#section-collection)&nbsp;&nbsp;|&nbsp;&nbsp;[セクション エンティティ](#section-entity)&nbsp;&nbsp;|&nbsp;&nbsp;[SectionGroup コレクション](#sectiongroup-collection)&nbsp;&nbsp;|&nbsp;&nbsp; [SectionGroup エンティティ](#sectiongroup-entity)&nbsp;&nbsp;|&nbsp;&nbsp;[ノートブック コレクション](#notebook-collection)&nbsp;&nbsp;|&nbsp;&nbsp;[ノートブック エンティティ](#notebook-entity)&nbsp;&nbsp;|&nbsp;&nbsp; [画像またはその他のファイル リソース](#image-or-other-file-resource)</span><span class="sxs-lookup"><span data-stu-id="90ac2-116">[Page collection](#page-collection)&nbsp;&nbsp;|&nbsp;&nbsp;[Page entity](#page-entity)&nbsp;&nbsp;|&nbsp;&nbsp;[Page preview](#page-preview)&nbsp;&nbsp;|&nbsp;&nbsp;[Page HTML content](#page-html-content)&nbsp;&nbsp;|&nbsp;&nbsp; [Section collection](#section-collection)&nbsp;&nbsp;|&nbsp;&nbsp;[Section entity](#section-entity)&nbsp;&nbsp;|&nbsp;&nbsp;[SectionGroup collection](#sectiongroup-collection)&nbsp;&nbsp;|&nbsp;&nbsp; [SectionGroup entity](#sectiongroup-entity)&nbsp;&nbsp;|&nbsp;&nbsp;[Notebook collection](#notebook-collection)&nbsp;&nbsp;|&nbsp;&nbsp;[Notebook entity](#notebook-entity)&nbsp;&nbsp;|&nbsp;&nbsp; [Image or other file resource](#image-or-other-file-resource)</span></span>

<a name="get-pages"></a>
### <a name="page-collection"></a><span data-ttu-id="90ac2-117">ページ コレクション</span><span class="sxs-lookup"><span data-stu-id="90ac2-117">Page collection</span></span>

<span data-ttu-id="90ac2-118">すべてのノートブックのページ (メタデータ) を取得する</span><span class="sxs-lookup"><span data-stu-id="90ac2-118">Get pages (metadata) across all notebooks</span></span>

`../pages[?filter,orderby,select,expand,top,skip,search,count]`

<span data-ttu-id="90ac2-119">特定のセクションからページ (メタデータ) を取得する</span><span class="sxs-lookup"><span data-stu-id="90ac2-119">Get pages (metadata) from a specific section</span></span>

`../sections/{section-id}/pages[?filter,orderby,select,expand,top,skip,search,count,pagelevel]`

 
<span data-ttu-id="90ac2-120">`search`クエリ文字列オプションは、コンシューマー ノートパソコンでのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="90ac2-120">The `search` query string option is available for consumer notebooks only.</span></span>

<span data-ttu-id="90ac2-121">ページの既定の並べ替え順序は `lastModifiedTime desc` です。</span><span class="sxs-lookup"><span data-stu-id="90ac2-121">The default sort order for pages is `lastModifiedTime desc`.</span></span>

<span data-ttu-id="90ac2-122">既定のクエリは、親セクションを展開し、セクションの `id`、`name`、および `self` プロパティを選択します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-122">The default query expands the parent section and selects the section's `id`, `name`, and `self` properties.</span></span>

<span data-ttu-id="90ac2-123">既定では、*GET ページ*要求に対して上位 20 のエントリのみが返されます。</span><span class="sxs-lookup"><span data-stu-id="90ac2-123">By default, only the top 20 entries are returned for *GET pages* requests.</span></span> <span data-ttu-id="90ac2-124">**上位**クエリ文字列オプションを指定しない要求を行った場合、次の 20 エントリを取得するために使用できる **@odata.nextLink** リンクが応答で返されます。</span><span class="sxs-lookup"><span data-stu-id="90ac2-124">Requests that don't specify a **top** query string option return an **@odata.nextLink** link in the response that you can use to get the next 20 entries.</span></span>

<span data-ttu-id="90ac2-125">セクションのページ コレクションの場合、**pagelevel** を使用して、ページのインデント レベルとセクション内でのその順序を返します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-125">For the pages collection in a section, use **pagelevel** to return the indentation level of pages and their order within the section.</span></span> 

<span data-ttu-id="90ac2-126">**例:**  `GET ../sections/{section-id}/pages?pagelevel=true`。</span><span class="sxs-lookup"><span data-stu-id="90ac2-126">Example</span></span>

- - -

<a name="get-page"></a> 
### <a name="page-entity"></a><span data-ttu-id="90ac2-127">ページ エンティティ</span><span class="sxs-lookup"><span data-stu-id="90ac2-127">Page entity</span></span>

<span data-ttu-id="90ac2-128">特定のページのメタデータを取得する</span><span class="sxs-lookup"><span data-stu-id="90ac2-128">Get the metadata for a specific page.</span></span> 

`../pages/{page-id}[?select,expand,pagelevel]` 


<span data-ttu-id="90ac2-129">ページは、**parentNotebook** プロパティと **parentSection** プロパティを展開できます。</span><span class="sxs-lookup"><span data-stu-id="90ac2-129">Pages can expand the **parentNotebook** and **parentSection** properties.</span></span>

<span data-ttu-id="90ac2-130">既定のクエリは、親セクションを展開し、セクションの `id`、`name`、および `self` プロパティを選択します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-130">The default query expands the parent section and selects the section's `id`, `name`, and `self` properties.</span></span>

<span data-ttu-id="90ac2-131">**pagelevel** を使用して、ページのインデント レベルと親セクション内でのその順序を返します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-131">Use **pagelevel** to return the indentation level of the page and its order within its parent section.</span></span> <span data-ttu-id="90ac2-132">例: `GET ../pages/{page-id}?pagelevel=true`</span><span class="sxs-lookup"><span data-stu-id="90ac2-132">Example: `GET ../pages/{page-id}?pagelevel=true`.</span></span>

- - -

<a name="get-page-preview"></a> 
### <a name="page-preview"></a><span data-ttu-id="90ac2-133">ページ プレビュー</span><span class="sxs-lookup"><span data-stu-id="90ac2-133">Page preview</span></span>

<span data-ttu-id="90ac2-134">ページのテキストと画像のプレビュー コンテンツを取得する</span><span class="sxs-lookup"><span data-stu-id="90ac2-134">Get text and image preview content for a page</span></span>

`../pages/{page-id}/preview`


<span data-ttu-id="90ac2-135">JSON 応答には、ページに含まれているものを特定するために使用できる、プレビュー コンテンツが含まれています。</span><span class="sxs-lookup"><span data-stu-id="90ac2-135">The JSON response contains the preview content, which you can use to help users identify what's in the page.</span></span>

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

<span data-ttu-id="90ac2-136">**previewText** プロパティには、ページからのテキスト スニペットが含まれています。</span><span class="sxs-lookup"><span data-stu-id="90ac2-136">The **previewText** property contains a text snippet from the page.</span></span> <span data-ttu-id="90ac2-137">Microsoft Graph は、最大 300 文字の完全な文字列を返します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-137">The OneNote API returns complete phrases, up to a maximum of 300 characters.</span></span> 

<span data-ttu-id="90ac2-138">ページにプレビュー UI のビルドに使用できる画像が含まれている場合、**previewImageUrl** オブジェクトの **href** プロパティには、事前認証されたパブリックの [image resource](#image-or-other-file-resource) のリンクが含まれます。</span><span class="sxs-lookup"><span data-stu-id="90ac2-138">If the page has an image that can be used to build a preview UI, the **href** property in the **previewImageUrl** object contains a link to a public, pre-authenticated [image resource](#image-or-other-file-resource).</span></span> <span data-ttu-id="90ac2-139">このリンクは HTML で使用できます。</span><span class="sxs-lookup"><span data-stu-id="90ac2-139">You can use this link in HTML, for example: .</span></span>

<span data-ttu-id="90ac2-140">**例:** `<img src="https://www.onenote.com/api/v1.0/resources/{id}/content?publicAuth=true&mimeType=image/png" />`。</span><span class="sxs-lookup"><span data-stu-id="90ac2-140">Example</span></span> <span data-ttu-id="90ac2-141">それ以外の場合、**href** は、null 値を返します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-141">Otherwise, **href** returns null.</span></span>

- - -

<a name="get-page-content"></a> 
### <a name="page-html-content"></a><span data-ttu-id="90ac2-142">ページ HTML コンテンツ</span><span class="sxs-lookup"><span data-stu-id="90ac2-142">Page HTML content</span></span>

<span data-ttu-id="90ac2-143">ページ (`../pages/{page-id}/content[?includeIDs,preAuthenticated]`) の HTML コンテンツを取得する</span><span class="sxs-lookup"><span data-stu-id="90ac2-143">Get the HTML content of a page`../pages/{page-id}/content[?includeIDs,preAuthenticated]`</span></span>

<span data-ttu-id="90ac2-144">(*[返される HTML コンテンツ](onenote_input_output_html.md)の詳細についてはリンク先をご覧ください*)</span><span class="sxs-lookup"><span data-stu-id="90ac2-144">(*learn more about [returned HTML content](onenote_input_output_html.md)*)</span></span> 

 
<span data-ttu-id="90ac2-145">**includeIDs=true** クエリ文字列オプションを使用して、[ページを更新](onenote_update_page.md)するために使用する生成 ID を取得します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-145">Use the **includeIDs=true** query string option to get generated IDs used to [update the page](onenote_update_page.md).</span></span>

<span data-ttu-id="90ac2-146">**preAuthenticated=true** クエリ文字列オプションを使用して、ページ上の[画像リソース](#image-or-other-file-resource)のパブリック URL を取得します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-146">Use the **preAuthenticated=true** query string option to get public URLs to the [image resources](#image-or-other-file-resource) that are on the page.</span></span> <span data-ttu-id="90ac2-147">パブリック URL は 1 時間有効です。</span><span class="sxs-lookup"><span data-stu-id="90ac2-147">The public URLs are valid for one hour.</span></span> 

- - -

<a name="get-sections"></a>
### <a name="section-collection"></a><span data-ttu-id="90ac2-148">セクション コレクション</span><span class="sxs-lookup"><span data-stu-id="90ac2-148">Section collection</span></span>

<span data-ttu-id="90ac2-149">ユーザーが所有するすべてのノートブックから、ネストされたセクション グループのセクションを含む、すべてのセクションを取得する `../sections[?filter,orderby,select,top,skip,expand,count]`</span><span class="sxs-lookup"><span data-stu-id="90ac2-149">Get all sections from all notebooks that are owned by the user, including sections in nested section groups`../sections[?filter,orderby,select,top,skip,expand,count]`</span></span> 

<span data-ttu-id="90ac2-150">特定のセクション グループの直下にあるすべてのセクションを取得する</span><span class="sxs-lookup"><span data-stu-id="90ac2-150">Get all sections that are directly under a specific section group</span></span>

`../sectionGroups/{sectiongroup-id}/sections[?filter,orderby,select,top,skip,expand,count]` 

<span data-ttu-id="90ac2-151">特定のノートブックの直下にあるすべてのセクションを取得する `../notebooks/{notebook-id}/sections[?filter,orderby,select,top,skip,expand,count]`</span><span class="sxs-lookup"><span data-stu-id="90ac2-151">Get all sections that are directly under a specific notebook`../notebooks/{notebook-id}/sections[?filter,orderby,select,top,skip,expand,count]`</span></span> 

 
<span data-ttu-id="90ac2-152">セクションは、**parentNotebook** プロパティと **parentSectionGroup** プロパティを展開できます。</span><span class="sxs-lookup"><span data-stu-id="90ac2-152">Sections can expand the **parentNotebook** and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="90ac2-153">セクションの既定の並べ替え順序は `name asc` です。</span><span class="sxs-lookup"><span data-stu-id="90ac2-153">The default sort order for sections is `name asc`.</span></span>

<span data-ttu-id="90ac2-154">既定のクエリは、親ノートブックおよび親セクション グループを展開し、`id`、`name`、および `self` プロパティを選択します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-154">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>

- - -

<a name="get-section"></a>
### <a name="section-entity"></a><span data-ttu-id="90ac2-155">セクション エンティティ</span><span class="sxs-lookup"><span data-stu-id="90ac2-155">Section entity</span></span>

<span data-ttu-id="90ac2-156">特定のセクションを取得する</span><span class="sxs-lookup"><span data-stu-id="90ac2-156">Get a specific section</span></span>

`../sections/{section-id}[?select,expand]` 

 
<span data-ttu-id="90ac2-157">セクションは、**parentNotebook** プロパティと **parentSectionGroup** プロパティを展開できます。</span><span class="sxs-lookup"><span data-stu-id="90ac2-157">Sections can expand the **parentNotebook** and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="90ac2-158">既定のクエリは、親ノートブックおよび親セクション グループを展開し、`id`、`name`、および `self` プロパティを選択します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-158">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>

- - -

<a name="get-section-groups"></a>
### <a name="sectiongroup-collection"></a><span data-ttu-id="90ac2-159">SectionGroup コレクション</span><span class="sxs-lookup"><span data-stu-id="90ac2-159">SectionGroup collection</span></span>

<span data-ttu-id="90ac2-160">ユーザーが所有するすべてのノートブックから、ネストされたセクション グループを含む、すべてのセクション グループを取得する</span><span class="sxs-lookup"><span data-stu-id="90ac2-160">Get all section groups from all notebooks that are owned by the user, including nested section groups</span></span>

`../sectionGroups[?filter,orderby,select,top,skip,expand,count]` 

<span data-ttu-id="90ac2-161">特定のノートブックの直下にあるすべてのセクション グループを取得する</span><span class="sxs-lookup"><span data-stu-id="90ac2-161">Get all section groups that are directly under a specific notebook</span></span> 

`../notebooks/{notebook-id}/sectionGroups[?filter,orderby,select,top,skip,expand,count]` 

<span data-ttu-id="90ac2-162">セクション グループは、**セクション**、**sectionGroups**、**parentNotebook**、および **parentSectionGroup** プロパティを展開できます。</span><span class="sxs-lookup"><span data-stu-id="90ac2-162">Section groups can expand the **sections**, **sectionGroups**, **parentNotebook**, and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="90ac2-163">セクション グループの既定の並べ替え順序は `name asc` です。</span><span class="sxs-lookup"><span data-stu-id="90ac2-163">The default sort order for section groups is `name asc`.</span></span>

<span data-ttu-id="90ac2-164">既定のクエリは、親ノートブックおよび親セクション グループを展開し、`id`、`name`、および `self` プロパティを選択します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-164">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>

- - -

<a name="get-section-group"></a>
### <a name="sectiongroup-entity"></a><span data-ttu-id="90ac2-165">SectionGroup エンティティ</span><span class="sxs-lookup"><span data-stu-id="90ac2-165">SectionGroup entity</span></span>

<span data-ttu-id="90ac2-166">特定のセクション グループを取得する</span><span class="sxs-lookup"><span data-stu-id="90ac2-166">Get a specific section group</span></span>

`../sectionGroups/{sectiongroup-id}[?select,expand]` 


<span data-ttu-id="90ac2-167">セクション グループは、**セクション**、**sectionGroups**、**parentNotebook**、および **parentSectionGroup** プロパティを展開できます。</span><span class="sxs-lookup"><span data-stu-id="90ac2-167">Section groups can expand the **sections**, **sectionGroups**, **parentNotebook**, and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="90ac2-168">既定のクエリは、親ノートブックおよび親セクション グループを展開し、`id`、`name`、および `self` プロパティを選択します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-168">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>

- - -

<a name="get-notebooks"></a>
### <a name="notebook-collection"></a><span data-ttu-id="90ac2-169">ノートブック コレクション</span><span class="sxs-lookup"><span data-stu-id="90ac2-169">Notebook collection</span></span>

<span data-ttu-id="90ac2-170">ユーザーによって所有されるすべてのノートブックを取得する</span><span class="sxs-lookup"><span data-stu-id="90ac2-170">Get all the notebooks that are owned by the user</span></span> 

`../notebooks[?filter,orderby,select,top,skip,expand,count]` 

 
<span data-ttu-id="90ac2-171">ノートブックは、**セクション**および **sectionGroups** プロパティを展開できます。</span><span class="sxs-lookup"><span data-stu-id="90ac2-171">Notebooks can expand the **sections** and **sectionGroups** properties.</span></span>

<span data-ttu-id="90ac2-172">ノートブックの既定の並べ替え順序は `name asc` です。</span><span class="sxs-lookup"><span data-stu-id="90ac2-172">The default sort order for notebooks is `name asc`.</span></span> 

- - -

<a name="get-notebook"></a>
### <a name="notebook-entity"></a><span data-ttu-id="90ac2-173">ノートブック エンティティ</span><span class="sxs-lookup"><span data-stu-id="90ac2-173">Notebook entity</span></span>

<span data-ttu-id="90ac2-174">特定のノートブックを取得する `../notebooks/{notebook-id}[?select,expand]`</span><span class="sxs-lookup"><span data-stu-id="90ac2-174">Get a specific notebook`../notebooks/{notebook-id}[?select,expand]`</span></span> 


<span data-ttu-id="90ac2-175">ノートブックは、**セクション**および **sectionGroups** プロパティを展開できます。</span><span class="sxs-lookup"><span data-stu-id="90ac2-175">Notebooks can expand the **sections** and **sectionGroups** properties.</span></span>

- - -

<a name="get-resource"></a>
### <a name="image-or-other-file-resource"></a><span data-ttu-id="90ac2-176">画像またはその他のファイル リソース</span><span class="sxs-lookup"><span data-stu-id="90ac2-176">Image or other file resource</span></span>

<span data-ttu-id="90ac2-177">特定のリソースのバイナリ データを取得する</span><span class="sxs-lookup"><span data-stu-id="90ac2-177">Get the binary data of a specific resource</span></span> 

`../resources/{resource-id}/$value` 


<span data-ttu-id="90ac2-178">ファイルのリソース URI は、ページの[出力 HTML](onenote_input_output_html.md) にあります。</span><span class="sxs-lookup"><span data-stu-id="90ac2-178">You can find the file's resource URI in the page's [output HTML](onenote_input_output_html.md).</span></span>

<span data-ttu-id="90ac2-179">たとえば、**img** タグには、**data-fullres-src** 属性の元の画像のエンドポイントと、**src** 属性の最適化された画像のエンドポイントが含まれます。</span><span class="sxs-lookup"><span data-stu-id="90ac2-179">For example, an **img** tag includes endpoints for the original image in the **data-fullres-src** attribute and the optimized image in the **src** attribute.</span></span> 

<span data-ttu-id="90ac2-180">**例:**</span><span class="sxs-lookup"><span data-stu-id="90ac2-180">**Example:**</span></span>

```
<img 
    src="https://www.onenote.com/api/v1.0/me/notes/resources/{image-id}/$value"  
    data-src-type="image/png"
    data-fullres-src="https://www.onenote.com/api/v1.0/resources/{image-id}/$value"  
    data-fullres-src-type="image/png" ... />
```

<span data-ttu-id="90ac2-181">**object** タグには、**data** 属性のファイル リソースのエンドポイントが含まれています。</span><span class="sxs-lookup"><span data-stu-id="90ac2-181">And an **object** tag includes the endpoint for the file resource in the **data** attribute.</span></span> 

<span data-ttu-id="90ac2-182">**例:**</span><span class="sxs-lookup"><span data-stu-id="90ac2-182">**Example:**</span></span>

```
<object
    data="http://www.onenote.com/api/v1.0/me/notes/resources/{file-id}/$value"
    data-attachment="fileName.pdf" 
    type="application/pdf" ... />
```

<span data-ttu-id="90ac2-183">ページにある画像リソースへの事前認証された公開 URL を取得するには、[ページのコンテンツを取得する](#page-html-content)際にクエリ文字列に **preAuthenticated=true** を含めます (**例:**  `GET ../pages/{page-id}/content?preAuthenticated=true`)。</span><span class="sxs-lookup"><span data-stu-id="90ac2-183">To get public, pre-authenticated URLs to the image resources on a page, include preAuthenticated=true in the query string when you retrieve the page content (example: ).</span></span> <span data-ttu-id="90ac2-184">[出力 HTML](onenote_input_output_html.md#output-html-examples-for-images) に返されるパブリック URL は 1 時間有効です。</span><span class="sxs-lookup"><span data-stu-id="90ac2-184">The public URLs that are returned in the [output HTML](onenote_input_output_html.md#output-html-examples-for-images) are valid for one hour.</span></span> <span data-ttu-id="90ac2-185">このフラグを設定していない場合、取得された画像は非公開で、またページのコンテンツの残りの部分と同様、それらを取得するために承認を必要とするため、ブラウザーで直接レンダリングすることはありません。</span><span class="sxs-lookup"><span data-stu-id="90ac2-185">Without this flag, retrieved images won't render directly in a browser because they are private and require authorization to retrieve them, like the rest of the page contents.</span></span> 

> <span data-ttu-id="90ac2-186">**注:** リソースのコレクションの取得はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="90ac2-186">Getting a collection of resources is not supported.</span></span> 

<span data-ttu-id="90ac2-187">ファイル リソースを取得する場合、**Accept** コンテンツ タイプを要求に含める必要はありません。</span><span class="sxs-lookup"><span data-stu-id="90ac2-187">When you get a file resource, you don't need to include an **Accept** content type in the request.</span></span>

<span data-ttu-id="90ac2-188">GET 要求の詳細については、Microsoft Graph API REST リファレンス内の</span><span class="sxs-lookup"><span data-stu-id="90ac2-188">For more information about GET requests, see:</span></span> 
- [<span data-ttu-id="90ac2-189">ページを取得する</span><span class="sxs-lookup"><span data-stu-id="90ac2-189">Get pages</span></span>](../api-reference/v1.0/api/page_get.md)
- [<span data-ttu-id="90ac2-190">Get section</span><span class="sxs-lookup"><span data-stu-id="90ac2-190">Get sections</span></span>](../api-reference/v1.0/api/section_get.md)
- [<span data-ttu-id="90ac2-191">Get sectionGroup</span><span class="sxs-lookup"><span data-stu-id="90ac2-191">GET sectiongroups</span></span>](../api-reference/v1.0/api/sectiongroup_get.md)
- [<span data-ttu-id="90ac2-192">ノートブックを取得する</span><span class="sxs-lookup"><span data-stu-id="90ac2-192">GET notebooks</span></span>](../api-reference/v1.0/api/notebook_get.md) 

<span data-ttu-id="90ac2-193">をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="90ac2-193">in the Microsoft Graph API REST reference.</span></span>


<a name="example"></a>
## <a name="example-get-requests"></a><span data-ttu-id="90ac2-194">GET 要求の例</span><span class="sxs-lookup"><span data-stu-id="90ac2-194">Example GET requests</span></span>
<span data-ttu-id="90ac2-195">OneNote のエンティティおよび検索ページ コンテンツを照会して、必要な情報だけを取得することができます。</span><span class="sxs-lookup"><span data-stu-id="90ac2-195">You can query for OneNote entities and search page content to get just the information you need.</span></span> <span data-ttu-id="90ac2-196">次の例は、Microsoft Graph への GET 要求で、[サポートされているクエリ文字列オプション](#supported-odata-query-string-options)を使用するいくつかの方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="90ac2-196">The following examples show some ways you can use [supported query string options](#supported-odata-query-string-options) in GET requests to the OneNote API.</span></span> 

<span data-ttu-id="90ac2-197">**次の点にご注意ください。**</span><span class="sxs-lookup"><span data-stu-id="90ac2-197">**Remember:**</span></span>

- <span data-ttu-id="90ac2-198">GET 要求はすべて、[サービス ルート URL](../api-reference/v1.0/resources/onenote-api-overview.md#root-url) で始まります。</span><span class="sxs-lookup"><span data-stu-id="90ac2-198">All GET requests start with the [service root URL](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span></span>

  <span data-ttu-id="90ac2-199">**例:**</span><span class="sxs-lookup"><span data-stu-id="90ac2-199">**Examples: **</span></span> 
  - `https://www.onenote.com/api/v1.0/me/notes`
  - `https://www.onenote.com/api/v1.0/myOrganization/siteCollections/{id}/sites/{id}/notes/`

- <span data-ttu-id="90ac2-200">URL クエリ文字列のスペースには %20 エンコードを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="90ac2-200">Spaces in the URL query string must use %20 encoding.</span></span>

<span data-ttu-id="90ac2-201">例: `filter=title%20eq%20'biology'`</span><span class="sxs-lookup"><span data-stu-id="90ac2-201">Example: `filter=title%20eq%20'biology'`</span></span>

- <span data-ttu-id="90ac2-202">プロパティ名と OData 文字列比較では大文字と小文字が区別されます。</span><span class="sxs-lookup"><span data-stu-id="90ac2-202">Property names and OData string comparisons are case sensitive.</span></span> <span data-ttu-id="90ac2-203">文字列比較には OData **tolower** 関数を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="90ac2-203">We recommend using the OData **tolower** function for string comparisons.</span></span>

   <span data-ttu-id="90ac2-204">例: `filter=tolower(name) eq 'spring'`</span><span class="sxs-lookup"><span data-stu-id="90ac2-204">Example: `filter=tolower(name) eq 'spring'`</span></span>
 

<span data-ttu-id="90ac2-205">**search & filter**</span><span class="sxs-lookup"><span data-stu-id="90ac2-205">**search & filter**</span></span>  

<span data-ttu-id="90ac2-206">特定のアプリによって作成された、*recipe* という用語が含まれるページすべてを取得します </span><span class="sxs-lookup"><span data-stu-id="90ac2-206">Get all pages that contain the term *recipe* that were created by a specific app.</span></span>  <span data-ttu-id="90ac2-207">(`search` は、コンシューマー ノートパソコンでのみ使用可能)。</span><span class="sxs-lookup"><span data-stu-id="90ac2-207">(`search` is available for consumer notebooks only)</span></span>

```
[GET] ../pages?search=recipe&filter=createdByAppId eq 'WLID-000000004C12821A'
```
 
<span data-ttu-id="90ac2-208">**search & select**</span><span class="sxs-lookup"><span data-stu-id="90ac2-208">**search & select**</span></span>  

<span data-ttu-id="90ac2-209">*golgi app* という用語が含まれるすべてのページの、タイトル、OneNote クライアントのリンク、および **contentUrl** リンクを取得します </span><span class="sxs-lookup"><span data-stu-id="90ac2-209">Get the title, OneNote client links, and **contentUrl** link for all pages that contain the term *golgi app*.</span></span>  <span data-ttu-id="90ac2-210">(`search` は、コンシューマー ノートパソコンでのみ使用可能)。</span><span class="sxs-lookup"><span data-stu-id="90ac2-210">(`search` is available for consumer notebooks only)</span></span>

```
[GET] ../pages?search=golgi app&select=title,links,contentUrl
```
 
<span data-ttu-id="90ac2-211">**expand**</span><span class="sxs-lookup"><span data-stu-id="90ac2-211">**expand**</span></span>  

<span data-ttu-id="90ac2-212">すべてのノートブックを取得し、そのセクションとセクション グループを展開します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-212">Get all notebooks and expand their sections and section groups.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups
```
 
<span data-ttu-id="90ac2-213">特定のセクション グループを取得し、そのセクションとセクション グループを展開します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-213">Get a specific section group and expand its sections and section groups.</span></span>  

```
[GET] ../sectionGroups/{sectiongroup-id}?expand=sections,sectionGroups
```

<span data-ttu-id="90ac2-214">ページを取得し、その親セクションと親ノートブックを展開します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-214">Get a page and expand its parent section and parent notebook.</span></span>

```
[GET] ../pages/{page-id}?expand=parentSection,parentNotebook
```

<span data-ttu-id="90ac2-215">**expand** (複数レベル)</span><span class="sxs-lookup"><span data-stu-id="90ac2-215">**expand** (multiple levels)</span></span>  

<span data-ttu-id="90ac2-216">すべてのノートブックを取得してセクションとセクション グループを展開し、各セクション グループのすべてのセクションを展開します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-216">Get all notebooks and expand their sections and section groups, and expand all sections in each section group.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups(expand=sections)
```
 
><span data-ttu-id="90ac2-217">子エンティティの親を展開、または親エンティティの子を展開すると、循環参照が作成されますが、これはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="90ac2-217">Expanding parents of child entities or expanding children of parent entities creates a circular reference and is not supported.</span></span>

 
<span data-ttu-id="90ac2-218">**expand & select** (複数レベル)</span><span class="sxs-lookup"><span data-stu-id="90ac2-218">**expand & select** (multiple levels)</span></span>  

<span data-ttu-id="90ac2-219">特定のセクション グループの名前と **self** リンクを取得し、そのすべてのセクションの名前と **self** リンクを取得します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-219">Get the name and **self** link for a specific section group, and get the name and **self** links for all its sections.</span></span>  

```
[GET] ../sectionGroups/{sectiongroup-id}?expand=sections(select=name,self)&select=name,self
```
 
<span data-ttu-id="90ac2-220">すべてのセクションの名前と **self** リンクを取得し、各セクションの親ノートブックの名前と作成時刻を取得します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-220">Get the name and **self** link for all sections, and get the name and created time of each section's parent notebook.</span></span>  

```
[GET] ../sections?expand=parentNotebook(select=name,createdTime)&select=name,self
```
 
<span data-ttu-id="90ac2-221">すべてのページのタイトルと ID を取得し、親セクションと親ノートブックの名前を取得します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-221">Get the title and ID for all pages, and get the name of the parent section and parent notebook.</span></span>

```
[GET] ../pages?select=id,title&expand=parentSection(select=name),parentNotebook(select=name)
```

<span data-ttu-id="90ac2-222">**expand & levels** (複数レベル)</span><span class="sxs-lookup"><span data-stu-id="90ac2-222">**expand & levels** (multiple levels)</span></span>  

<span data-ttu-id="90ac2-223">すべてのノートブック、セクション、セクション グループを取得します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-223">Get all notebooks, sections, and section groups.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups(expand=sections,sectionGroups(levels=max;expand=sections))
```
 
<span data-ttu-id="90ac2-224">**filter**</span><span class="sxs-lookup"><span data-stu-id="90ac2-224">**filter**</span></span>  

<span data-ttu-id="90ac2-225">2014 年 10 月に作成されたセクションすべてを取得します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-225">Get all sections that were created in October 2014.</span></span>

```
[GET] ../sections?filter=createdTime ge 2014-10-01 and createdTime le 2014-10-31
```

<span data-ttu-id="90ac2-226">2015 年 1 月 1 日以降に特定のアプリによって作成されたページを取得します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-226">Get the pages that were created by a specific app since January 1, 2015.</span></span>

```
[GET] ../pages?filter=createdByAppId eq 'WLID-0000000048118631' and createdTime ge 2015-01-01
```

<span data-ttu-id="90ac2-227">**filter & expand**</span><span class="sxs-lookup"><span data-stu-id="90ac2-227">**filter & expand**</span></span>  

<span data-ttu-id="90ac2-p115">特定のノートブックに含まれるすべてのページを取得します。既定では、この API は 20 エントリを戻します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-p115">Get all pages in a specific notebook. The API returns 20 entries by default.</span></span>

```
[GET] ../pages?filter=parentNotebook/id eq '{notebook-id}'&expand=parentNotebook
```

<span data-ttu-id="90ac2-230">*学校*のノートブックにあるすべてのセクションの名前と **pagesUrl** リンクを取得します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-230">Get the name and **pagesUrl** link for all sections from the *School* notebook.</span></span> <span data-ttu-id="90ac2-231">OData の文字列比較は大文字小文字が区別されるので、ベスト プラクティスとして **tolower** 関数を使用します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-231">OData string comparisons are case sensitive, so use the **tolower** function as a best practice.</span></span>

```
[GET] ../notebooks?filter=tolower(name) eq 'school'&expand=sections(select=name,pagesUrl)
```

<span data-ttu-id="90ac2-232">**filter & select & orderby**</span><span class="sxs-lookup"><span data-stu-id="90ac2-232">**filter & select & orderby**</span></span>   

<span data-ttu-id="90ac2-233">セクション名に *spring* という語が含まれるすべてのセクションの名前と **pagesUrl** リンクを取得します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-233">Get the name and **pagesUrl** link for all sections that contain the term *spring* in the section name.</span></span> <span data-ttu-id="90ac2-234">セクションを最終変更日で並べ替えます。</span><span class="sxs-lookup"><span data-stu-id="90ac2-234">Order sections by last modified date.</span></span>

```
[GET] ../sections?filter=contains(tolower(name),'spring')&select=name,pagesUrl&orderby=lastModifiedTime desc
```
 
<span data-ttu-id="90ac2-235">**orderby**</span><span class="sxs-lookup"><span data-stu-id="90ac2-235">**orderby**</span></span>  

<span data-ttu-id="90ac2-236">**createdByAppId** プロパティ、次に作成時刻を基準に順序を並べ替えて、最初の 20 ページを取得します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-236">Get the first 20 pages ordered by **createdByAppId** property and then by most recent created time.</span></span> <span data-ttu-id="90ac2-237">既定では、この API は 20 エントリを戻します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-237">The API returns 20 entries by default.</span></span>

```
[GET] ../pages?orderby=createdByAppId,createdTime desc
```

<span data-ttu-id="90ac2-238">**search & filter & top**</span><span class="sxs-lookup"><span data-stu-id="90ac2-238">**search & filter & top**</span></span>  

<span data-ttu-id="90ac2-239">*cell division* という語句を含む、2015 年 1 月 1 日以降に作成されたページで新しいものを 5 つ取得します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-239">Get the five newest pages created since January 1, 2015 that contain the phrase *cell division*.</span></span> <span data-ttu-id="90ac2-240">既定ではこの API は 20 エントリを返します。最大では 100 エントリを返します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-240">The API returns 20 entries by default with a maximum of 100.</span></span> <span data-ttu-id="90ac2-241">ページの既定の並べ替え順序は `lastModifiedTime desc` です </span><span class="sxs-lookup"><span data-stu-id="90ac2-241">The default sort order for pages is `lastModifiedTime desc`.</span></span> <span data-ttu-id="90ac2-242">(`search` は、コンシューマー ノートパソコンでのみ使用可能)。</span><span class="sxs-lookup"><span data-stu-id="90ac2-242">(`search` is available for consumer notebooks only)</span></span>

```
[GET] ../pages?search="cell division"&filter=createdTime ge 2015-01-01&top=5
```

<span data-ttu-id="90ac2-243">**search & filter & top & skip**</span><span class="sxs-lookup"><span data-stu-id="90ac2-243">**search & filter & top & skip**</span></span>  

<span data-ttu-id="90ac2-244">結果セットの次の 5 ページを取得します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-244">Get the next five pages in the result set.</span></span> <span data-ttu-id="90ac2-245">(`search` は、コンシューマー ノートパソコンでのみ使用可能)。</span><span class="sxs-lookup"><span data-stu-id="90ac2-245">(`search` is available for consumer notebooks only)</span></span>

```
[GET] ../pages?search=biology&filter=createdTime ge 2015-01-01&top=5&skip=5
```

<span data-ttu-id="90ac2-246">さらに次の 5 つを取得します </span><span class="sxs-lookup"><span data-stu-id="90ac2-246">And the next five.</span></span> <span data-ttu-id="90ac2-247">(`search` は、コンシューマー ノートパソコンでのみ使用可能)。</span><span class="sxs-lookup"><span data-stu-id="90ac2-247">(`search` is available for consumer notebooks only)</span></span>

```
[GET] ../pages?search=biology&filter=createdTime ge 2015-01-01&top=5&skip=10
```

> <span data-ttu-id="90ac2-248">**注:** **search** と **filter** がどちらも同じ要求に適用される場合、結果には両方の条件に一致するエンティティのみが含まれます。</span><span class="sxs-lookup"><span data-stu-id="90ac2-248">If both **search** and **filter** are applied to the same request, the results include only those entities that match both criteria.</span></span>
 
<span data-ttu-id="90ac2-249">**select**</span><span class="sxs-lookup"><span data-stu-id="90ac2-249">**select**</span></span>  

<span data-ttu-id="90ac2-250">ユーザーのノートブック内にあるすべてのセクションの名前、作成時刻、**self** リンクを取得します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-250">Get the name, created time, and **self** link for all sections in the user's notebooks.</span></span>

```
[GET] ../sections?select=name,createdTime,self
```

<span data-ttu-id="90ac2-251">特定のページのタイトル、作成時刻、OneNote クライアント リンクを取得します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-251">Get the title, created time, and OneNote client links for a specific page.</span></span>

```
[GET] ../pages/{page-id}?select=title,createdTime,links
```

<span data-ttu-id="90ac2-252">**select & expand & filter** (複数レベル)</span><span class="sxs-lookup"><span data-stu-id="90ac2-252">**select & expand & filter** (multiple levels)</span></span>  

<span data-ttu-id="90ac2-253">ユーザーの既定ノートブックにあるすべてのセクションの名前と **pagesUrl** リンクを取得します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-253">Get the name and **pagesUrl** link for all sections in the user's default notebook.</span></span>

```
[GET] ../notebooks?select=name&expand=sections(select=name,pagesUrl)&filter=isDefault eq true
```

<span data-ttu-id="90ac2-254">**top & select & orderby**</span><span class="sxs-lookup"><span data-stu-id="90ac2-254">**top & select & orderby**</span></span>  

<span data-ttu-id="90ac2-255">最初の 50 ページのタイトルと **self** リンクを取得します。タイトルのアルファベット順に並べられます。</span><span class="sxs-lookup"><span data-stu-id="90ac2-255">Get the title and **self** link for the first 50 pages, ordered alphabetically by title.</span></span> <span data-ttu-id="90ac2-256">既定ではこの API は 20 エントリを返します。最大では 100 エントリを返します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-256">The API returns 20 entries by default with a maximum of 100.</span></span> <span data-ttu-id="90ac2-257">ページの既定の並べ替え順序は `lastModifiedTime desc` です。</span><span class="sxs-lookup"><span data-stu-id="90ac2-257">The default sort order for pages is `lastModifiedTime desc`.</span></span>

```
[GET] ../pages?top=50&select=title,self&orderby=title
```

<span data-ttu-id="90ac2-258">**skip & top & select & orderby**</span><span class="sxs-lookup"><span data-stu-id="90ac2-258">**skip & top & select & orderby**</span></span>  

<span data-ttu-id="90ac2-p123">51 ページ目から 100 ページ目までを取得します。既定ではこの API は 20 エントリを返します。最大では 100 エントリを返します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-p123">Get pages 51 to 100. The API returns 20 entries by default with a maximum of 100.</span></span>

```
[GET] ../pages?skip=50&top=50&select=title,self&orderby=title
```

> <span data-ttu-id="90ac2-261">**注:** 既定のエントリ数を取得する pages に対する GET 要求 (つまり、**top** 式を指定しない要求) は、応答で次の 20 エントリを取得するために使用できる **@odata.nextLink** リンクを戻します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-261">GET requests for pages that retrieve the default number of entries (that is, they don't specify a **top** expression) return an **@odata.nextLink** link in the response that you can use to get the next 20 entries.</span></span>
 

<a name="query-options"></a>
## <a name="supported-odata-query-string-options"></a><span data-ttu-id="90ac2-262">サポートされている OData クエリ文字列オプション</span><span class="sxs-lookup"><span data-stu-id="90ac2-262">Supported OData query string options</span></span>

<span data-ttu-id="90ac2-263">Microsoft Graph に GET 要求を送信する場合、OData クエリ文字列オプションを使用してクエリをカスタマイズして、必要な情報だけを取得できます。</span><span class="sxs-lookup"><span data-stu-id="90ac2-263">When sending GET requests to the OneNote API, you can use OData query string options to customize your query and get just the information you need. They can also improve performance by reducing the number of calls to the service and the size of the response payload.</span></span> <span data-ttu-id="90ac2-264">このオプションを使用することにより、サービスへの呼び出し回数が減り、応答ペイロードのサイズが小さくなるので、パフォーマンスも向上します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-264">When sending GET requests to the OneNote API, you can use OData query string options to customize your query and get just the information you need. They can also improve performance by reducing the number of calls to the service and the size of the response payload.</span></span>

> <span data-ttu-id="90ac2-265">**注:** この記事の例では読みやすくするために、URL クエリ文字列内のスペースで必要な %20 パーセント エンコードを使用していません: `filter=isDefault%20eq%20true`</span><span class="sxs-lookup"><span data-stu-id="90ac2-265">For readability, the examples in this article don't use the %20 percent-encoding required for spaces in the URL query string: `filter=isDefault%20eq%20true`</span></span>
 
| <span data-ttu-id="90ac2-266">クエリ オプション</span><span class="sxs-lookup"><span data-stu-id="90ac2-266">Query option</span></span> | <span data-ttu-id="90ac2-267">例と説明</span><span class="sxs-lookup"><span data-stu-id="90ac2-267">Example and description</span></span> |  
|------|------|  
| <span data-ttu-id="90ac2-268">count</span><span class="sxs-lookup"><span data-stu-id="90ac2-268">count</span></span> | <p>`count=true`</p><p><span data-ttu-id="90ac2-269">コレクション内のエンティティのカウントです。</span><span class="sxs-lookup"><span data-stu-id="90ac2-269">The count of entities in the collection.</span></span> <span data-ttu-id="90ac2-270">この値は、応答の **@odata.count** プロパティで戻ります。</span><span class="sxs-lookup"><span data-stu-id="90ac2-270">The value is returned in the **@odata.count** property in the response.</span></span></p> |  
| <span data-ttu-id="90ac2-271">expand</span><span class="sxs-lookup"><span data-stu-id="90ac2-271">expand</span></span> | <p>`expand=sections,sectionGroups`</p><p><span data-ttu-id="90ac2-272">応答でインラインを返すナビゲーション プロパティ。</span><span class="sxs-lookup"><span data-stu-id="90ac2-272">The navigation properties to return inline in the response.</span></span> <span data-ttu-id="90ac2-273">**expand** 式には次のプロパティがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="90ac2-273">The following properties are supported for **expand** expressions:</span></span><br /> <span data-ttu-id="90ac2-274">- ページ: **parentNotebook**、**parentSection**</span><span class="sxs-lookup"><span data-stu-id="90ac2-274">- Pages: **parentNotebook**, **parentSection**</span></span><br /> <span data-ttu-id="90ac2-275">- セクション: **parentNotebook**、**parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="90ac2-275">- Sections: **parentNotebook**, **parentSectionGroup**</span></span><br /> <span data-ttu-id="90ac2-276">- セクション グループ: **sections**、**sectionGroups**、**parentNotebook**、**parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="90ac2-276">- Section groups: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**</span></span><br /> <span data-ttu-id="90ac2-277">- ノートブック: **sections**、**sectionGroups**</span><span class="sxs-lookup"><span data-stu-id="90ac2-277">- Notebooks: **sections**, **sectionGroups**</span></span></p><p><span data-ttu-id="90ac2-278">既定では、ページの GET 要求は **parentSection** を展開し、セクションの **id**、**name**、**self** プロパティを選択します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-278">By default, GET requests for pages expands **parentSection** and select the section's **id**, **name**, and **self** properties.</span></span> <span data-ttu-id="90ac2-279">セクションおよびセクション グループの既定の GET 要求では、**parentNotebook** と **parentSectionGroup** の両方を展開し、親の **id**、**name**、**self** プロパティを選択します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-279">Default GET requests for sections and section groups expand both **parentNotebook** and **parentSectionGroup**, and select the parents' **id**, **name**, and **self** properties.</span></span> </p><p><span data-ttu-id="90ac2-p128">1 つのエンティティまたはコレクションに使用できます。コンマを使用して複数のプロパティを区切ります。プロパティ名では、大文字と小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-p128">Can be used for a single entity or a collection. Separate multiple properties with commas. Property names are case sensitive.</span></span></p> |   
| <span data-ttu-id="90ac2-283">filter</span><span class="sxs-lookup"><span data-stu-id="90ac2-283">filter</span></span> | <p>`filter=isDefault eq true`</p><p><span data-ttu-id="90ac2-p129">結果セットの入力に含めるかどうかを決めるブール式。サポートされている OData 演算子と関数:</span><span class="sxs-lookup"><span data-stu-id="90ac2-p129">A Boolean expression for whether to include an entry in the result set. Supports the following OData operators and functions:</span></span><br /> <span data-ttu-id="90ac2-286">- 比較演算子: **eq**、**ne**、**gt**、**ge**、**lt**、**le**</span><span class="sxs-lookup"><span data-stu-id="90ac2-286">- Comparison operators: **eq**, **ne**, **gt**, **ge**, **lt**, **le**</span></span><br /> <span data-ttu-id="90ac2-287">- 論理演算子: **and**、**or**、**not**</span><span class="sxs-lookup"><span data-stu-id="90ac2-287">- Logical operators: **and**, **or**, **not**</span></span><br /> <span data-ttu-id="90ac2-288">- 文字列関数: **contains**、**endswith**、**startswith**、**length**、**indexof**、**substring**、**tolower**、**toupper**、**trim**、**concat**</span><span class="sxs-lookup"><span data-stu-id="90ac2-288">- String functions: **contains**, **endswith**, **startswith**, **length**, **indexof**, **substring**, **tolower**, **toupper**, **trim**, **concat**</span></span></p><p><span data-ttu-id="90ac2-289">[プロパティ](#onenote-entity-properties)名と OData 文字列比較では大文字と小文字が区別されます。</span><span class="sxs-lookup"><span data-stu-id="90ac2-289">[Property](#onenote-entity-properties) names and OData string comparisons are case sensitive.</span></span> <span data-ttu-id="90ac2-290">文字列比較には OData **tolower** 関数を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="90ac2-290">We recommend using the OData **tolower** function for string comparisons.</span></span> <span data-ttu-id="90ac2-291">例: `filter=tolower(name) eq 'spring'`</span><span class="sxs-lookup"><span data-stu-id="90ac2-291">Example: `filter=tolower(name) eq 'spring'`</span></span></p> |  
| <span data-ttu-id="90ac2-292">orderby</span><span class="sxs-lookup"><span data-stu-id="90ac2-292">orderby</span></span> | <p>`orderby=title,createdTime desc`</p><p><span data-ttu-id="90ac2-293">オプションの **asc** (既定) または **desc** 並べ替え順序で並べ替える[プロパティ](#onenote-entity-properties)。</span><span class="sxs-lookup"><span data-stu-id="90ac2-293">The [properties](#onenote-entity-properties) to sort by, with an optional **asc** (default) or **desc** sort order.</span></span> <span data-ttu-id="90ac2-294">要求対象コレクション内のエンティティの任意のプロパティで並べ替えが可能です。</span><span class="sxs-lookup"><span data-stu-id="90ac2-294">You can sort by any property of the entity in the requested collection.</span></span></p><p><span data-ttu-id="90ac2-295">ノートブック、セクション グループ、セクションの既定の並べ替え順序は `name asc` で、ページの場合には `lastModifiedTime desc` (最新の変更ページが先頭になります)。</span><span class="sxs-lookup"><span data-stu-id="90ac2-295">The default sort order for notebooks, section groups, and sections is `name asc`, and for pages is `lastModifiedTime desc` (last modified page first).</span></span></p><p><span data-ttu-id="90ac2-p132">複数のプロパティはコンマで区切り、任意の順序で一覧表示します。プロパティ名では、大文字と小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-p132">Separate multiple properties with commas, and list them in the order that you want them applied. Property names are case sensitive.</span></span></p> |  
| <span data-ttu-id="90ac2-298">search</span><span class="sxs-lookup"><span data-stu-id="90ac2-298">search</span></span> | <p>`search=cell div`</p><p><span data-ttu-id="90ac2-299">コンシューマー ノートパソコンでのみ使用可能。</span><span class="sxs-lookup"><span data-stu-id="90ac2-299">Available for consumer notebooks only.</span></span></p><p><span data-ttu-id="90ac2-p133">ページ タイトル、ページ本文、画像の代替テキスト、画像の OCR テキストで検索する用語または語句です。既定では、検索クエリは関連度で並べ替えて結果を返します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-p133">The term or phrase to search for in the page title, page body, image alt text, and image OCR text. By default, search queries return results sorted by relevance.</span></span></p><p><span data-ttu-id="90ac2-p134">OneNote は、Bing のフルテキスト検索を使用して、語句の検索、語形変化、スペルの曖昧さ、関連性とランキング、単語分割、複数の言語、他のフルテキスト検索機能をサポートします。検索文字列では、大文字と小文字が区別されます。</span><span class="sxs-lookup"><span data-stu-id="90ac2-p134">OneNote uses Bing full-text search to support phrase search, stemming, spelling forgiveness, relevance and ranking, word breaking, multiple languages, and other full-text search features. Search strings are case insensitive.</span></span></p><p><span data-ttu-id="90ac2-304">ユーザーが所有しているノートブック内のページにのみ適用されます (ユーザーとは共有されません)。</span><span class="sxs-lookup"><span data-stu-id="90ac2-304">Applies only to pages in notebooks owned by the user (not shared with the user).</span></span> <span data-ttu-id="90ac2-305">インデックス付けされたコンテンツは非公開であり、所有者のみがアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="90ac2-305">Indexed content is private and can only be accessed by the owner.</span></span> <span data-ttu-id="90ac2-306">パスワードで保護されたページにはインデックスは付けられません。</span><span class="sxs-lookup"><span data-stu-id="90ac2-306">Password-protected pages are not indexed.</span></span> <span data-ttu-id="90ac2-307">`pages` エンドポイントにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="90ac2-307">Applies only to the `pages` endpoint.</span></span></p> |  
| <span data-ttu-id="90ac2-308">select</span><span class="sxs-lookup"><span data-stu-id="90ac2-308">select</span></span> | <p>`select=id,title`</p><p><span data-ttu-id="90ac2-309">返す[プロパティ](#onenote-entity-properties)。</span><span class="sxs-lookup"><span data-stu-id="90ac2-309">The [properties](#onenote-entity-properties) to return.</span></span> <span data-ttu-id="90ac2-310">1 つのエンティティまたはコレクションに使用できます。</span><span class="sxs-lookup"><span data-stu-id="90ac2-310">Can be used for a single entity or for a collection.</span></span> <span data-ttu-id="90ac2-311">コンマを使用して複数のプロパティを区切ります。</span><span class="sxs-lookup"><span data-stu-id="90ac2-311">Separate multiple properties with commas.</span></span> <span data-ttu-id="90ac2-312">プロパティ名では、大文字と小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-312">Property names are case sensitive.</span></span></p> |  
| <span data-ttu-id="90ac2-313">skip</span><span class="sxs-lookup"><span data-stu-id="90ac2-313">skip</span></span> | <p>`skip=10`</p><p><span data-ttu-id="90ac2-p137">結果セットでスキップするエントリの数。通常、結果のページングに使用されます。</span><span class="sxs-lookup"><span data-stu-id="90ac2-p137">The number of entries to skip in the result set. Typically used for paging results.</span></span></p> |  
| <span data-ttu-id="90ac2-316">top</span><span class="sxs-lookup"><span data-stu-id="90ac2-316">top</span></span> | <p>`top=50`</p><p><span data-ttu-id="90ac2-p138">結果セット内で返すエントリ数で、最大数は 100 です。既定値は 20 です。</span><span class="sxs-lookup"><span data-stu-id="90ac2-p138">The number of entries to return in the result set, up to a maximum of 100. The default value is 20.</span></span></p> |  

<span data-ttu-id="90ac2-319">Microsoft Graph にも、親セクション内でページのレベルと順序を取得する `pagelevel` クエリ文字列オプションが用意されています。</span><span class="sxs-lookup"><span data-stu-id="90ac2-319">OneNote also provides the `pagelevel` query string option you can use to get the level and order of pages within the parent section.</span></span> <span data-ttu-id="90ac2-320">特定のセクションのページのクエリ、または特定のページのクエリのにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="90ac2-320">Applies only to queries for pages in a specific section or queries for a specific page.</span></span> 

<span data-ttu-id="90ac2-321">**例:**</span><span class="sxs-lookup"><span data-stu-id="90ac2-321">**Example:**</span></span> 

- `GET ../sections/{section-id}/pages?pagelevel=true` 
- `GET ../pages/{page-id}?pagelevel=true` 

### <a name="supported-odata-operators-and-functions"></a><span data-ttu-id="90ac2-322">サポートされている OData 演算子と関数</span><span class="sxs-lookup"><span data-stu-id="90ac2-322">Supported OData operators and functions</span></span>

<span data-ttu-id="90ac2-323">Microsoft Graph は、**フィルター**式で次の OData 演算子および関数をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="90ac2-323">The OneNote API supports the following OData operators and functions in **filter** expressions.</span></span> <span data-ttu-id="90ac2-324">OData 式を使用する場合には、次の点に注意してください。</span><span class="sxs-lookup"><span data-stu-id="90ac2-324">When using OData expressions, remember:</span></span>  
- <span data-ttu-id="90ac2-325">URL クエリ文字列のスペースは `%20` エンコードで置換する必要があります。</span><span class="sxs-lookup"><span data-stu-id="90ac2-325">Spaces in the URL query string must be replaced with the `%20` encoding.</span></span>

   <span data-ttu-id="90ac2-326">**例:** `filter=isDefault%20eq%20true`</span><span class="sxs-lookup"><span data-stu-id="90ac2-326">**Example: ** `filter=isDefault%20eq%20true`</span></span>
- <span data-ttu-id="90ac2-327">プロパティ名と OData 文字列比較では大文字と小文字が区別されます。</span><span class="sxs-lookup"><span data-stu-id="90ac2-327">Property names and OData string comparisons are case sensitive.</span></span> <span data-ttu-id="90ac2-328">文字列比較には OData **tolower** 関数を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="90ac2-328">We recommend using the OData **tolower** function for string comparisons.</span></span>
   
   <span data-ttu-id="90ac2-329">**例:** `filter=tolower(name) eq 'spring'`</span><span class="sxs-lookup"><span data-stu-id="90ac2-329">**Example: ** `filter=tolower(name) eq 'spring'`</span></span>

| <span data-ttu-id="90ac2-330">比較演算子</span><span class="sxs-lookup"><span data-stu-id="90ac2-330">Comparison operator</span></span> | <span data-ttu-id="90ac2-331">例</span><span class="sxs-lookup"><span data-stu-id="90ac2-331">Example</span></span> |  
|------|------|  
| <span data-ttu-id="90ac2-332">eq</span><span class="sxs-lookup"><span data-stu-id="90ac2-332">eq</span></span><br /><span data-ttu-id="90ac2-333">(等しい)</span><span class="sxs-lookup"><span data-stu-id="90ac2-333">(equal to)</span></span> | `createdByAppId eq '{app-id}'` |  
| <span data-ttu-id="90ac2-334">ne</span><span class="sxs-lookup"><span data-stu-id="90ac2-334">ne</span></span><br /><span data-ttu-id="90ac2-335">(等しくない)</span><span class="sxs-lookup"><span data-stu-id="90ac2-335">(not equal to)</span></span> | `userRole ne 'Owner'` |  
| <span data-ttu-id="90ac2-336">gt</span><span class="sxs-lookup"><span data-stu-id="90ac2-336">gt</span></span><br /><span data-ttu-id="90ac2-337">(より大きい)</span><span class="sxs-lookup"><span data-stu-id="90ac2-337">(greater than)</span></span> | `createdTime gt 2014-02-23` |  
| <span data-ttu-id="90ac2-338">ge</span><span class="sxs-lookup"><span data-stu-id="90ac2-338">ge</span></span><br /><span data-ttu-id="90ac2-339">(以上)</span><span class="sxs-lookup"><span data-stu-id="90ac2-339">(greater than or equal to)</span></span> | `lastModifiedTime ge 2014-05-05T07:00:00Z` |  
| <span data-ttu-id="90ac2-340">lt</span><span class="sxs-lookup"><span data-stu-id="90ac2-340">lt</span></span><br /><span data-ttu-id="90ac2-341">(より小さい)</span><span class="sxs-lookup"><span data-stu-id="90ac2-341">(less than)</span></span> | `createdTime lt 2014-02-23` |  
| <span data-ttu-id="90ac2-342">le</span><span class="sxs-lookup"><span data-stu-id="90ac2-342">le</span></span><br /><span data-ttu-id="90ac2-343">(以下)</span><span class="sxs-lookup"><span data-stu-id="90ac2-343">(less than or equal to)</span></span> | `lastModifiedTime le 2014-02-23` |  
 
| <span data-ttu-id="90ac2-344">論理演算子</span><span class="sxs-lookup"><span data-stu-id="90ac2-344">Logical operator</span></span> | <span data-ttu-id="90ac2-345">例</span><span class="sxs-lookup"><span data-stu-id="90ac2-345">Example</span></span> |  
|------|------|  
| <span data-ttu-id="90ac2-346">and</span><span class="sxs-lookup"><span data-stu-id="90ac2-346">and</span></span> | `createdTime le 2014-01-30 and createdTime gt 2014-01-23` |  
| <span data-ttu-id="90ac2-347">or</span><span class="sxs-lookup"><span data-stu-id="90ac2-347">or</span></span> | `createdByAppId eq '{app-id}' or createdByAppId eq '{app-id}'` |  
| <span data-ttu-id="90ac2-348">not</span><span class="sxs-lookup"><span data-stu-id="90ac2-348">not</span></span> | `not contains(tolower(title),'school')` |  
 
| <span data-ttu-id="90ac2-349">String 関数</span><span class="sxs-lookup"><span data-stu-id="90ac2-349">String function</span></span> | <span data-ttu-id="90ac2-350">例</span><span class="sxs-lookup"><span data-stu-id="90ac2-350">Example</span></span> |  
|------|------|   
| <span data-ttu-id="90ac2-351">contains</span><span class="sxs-lookup"><span data-stu-id="90ac2-351">contains</span></span> | `contains(tolower(title),'spring')` |  
| <span data-ttu-id="90ac2-352">endswith</span><span class="sxs-lookup"><span data-stu-id="90ac2-352">endswith</span></span> | `endswith(tolower(title),'spring')` |  
| <span data-ttu-id="90ac2-353">startswith</span><span class="sxs-lookup"><span data-stu-id="90ac2-353">startswith</span></span> | `startswith(tolower(title),'spring')` |  
| <span data-ttu-id="90ac2-354">length</span><span class="sxs-lookup"><span data-stu-id="90ac2-354">length</span></span> | `length(title) eq 19` |  
| <span data-ttu-id="90ac2-355">indexof</span><span class="sxs-lookup"><span data-stu-id="90ac2-355">indexof</span></span> | `indexof(tolower(title),'spring') eq 1` |  
| <span data-ttu-id="90ac2-356">substring</span><span class="sxs-lookup"><span data-stu-id="90ac2-356">substring</span></span> | `substring(tolower(title),1) eq 'spring'` |  
| <span data-ttu-id="90ac2-357">tolower</span><span class="sxs-lookup"><span data-stu-id="90ac2-357">tolower</span></span> | `tolower(title) eq 'spring'` |  
| <span data-ttu-id="90ac2-358">toupper</span><span class="sxs-lookup"><span data-stu-id="90ac2-358">toupper</span></span> | `toupper(title) eq 'SPRING'` |  
| <span data-ttu-id="90ac2-359">trim</span><span class="sxs-lookup"><span data-stu-id="90ac2-359">trim</span></span> | `trim(tolower(title)) eq 'spring'` |  
| <span data-ttu-id="90ac2-360">concat</span><span class="sxs-lookup"><span data-stu-id="90ac2-360">concat</span></span> | `concat(title,'- by MyRecipesApp') eq 'Carrot Cake Recipe - by MyRecipesApp'` |  
 

<a name="properties"></a>
## <a name="onenote-entity-properties"></a><span data-ttu-id="90ac2-361">OneNote エンティティのプロパティ</span><span class="sxs-lookup"><span data-stu-id="90ac2-361">OneNote entity properties</span></span>

<span data-ttu-id="90ac2-362">**filter**、**select**、**expand**、および **orderby** クエリ式には、OneNote エンティティのプロパティを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="90ac2-362">The **filter**, **select**, **expand**, and **orderby** query expressions can include properties of OneNote entities.</span></span> 

<span data-ttu-id="90ac2-363">**例:**</span><span class="sxs-lookup"><span data-stu-id="90ac2-363">**Example:**</span></span>

`../sections?filter=createdTime ge 2015-01-01&select=name,pagesUrl&orderby=lastModifiedTime desc` 

<span data-ttu-id="90ac2-364">クエリ式のプロパティ名は大文字小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-364">Property names are case sensitive in query expressions.</span></span>

<span data-ttu-id="90ac2-365">プロパティおよびプロパティの種類のリストについては、次をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="90ac2-365">For the list of properties and property types, see:</span></span>

- [<span data-ttu-id="90ac2-366">ページを取得する</span><span class="sxs-lookup"><span data-stu-id="90ac2-366">Get pages</span></span>](../api-reference/v1.0/api/page_get.md)
- [<span data-ttu-id="90ac2-367">Get section</span><span class="sxs-lookup"><span data-stu-id="90ac2-367">Get sections</span></span>](../api-reference/v1.0/api/section_get.md)
- [<span data-ttu-id="90ac2-368">Get sectionGroup</span><span class="sxs-lookup"><span data-stu-id="90ac2-368">GET sectiongroups</span></span>](../api-reference/v1.0/api/sectiongroup_get.md)
- [<span data-ttu-id="90ac2-369">ノートブックを取得する</span><span class="sxs-lookup"><span data-stu-id="90ac2-369">GET notebooks</span></span>](../api-reference/v1.0/api/notebook_get.md) 

<span data-ttu-id="90ac2-370">をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="90ac2-370">in the Microsoft Graph API REST reference.</span></span>

<span data-ttu-id="90ac2-371">**expand** クエリ文字列オプションは、以下のナビゲーション プロパティとともに使用できます。</span><span class="sxs-lookup"><span data-stu-id="90ac2-371">The **expand** query string option can be used with the following navigation properties:</span></span>

- <span data-ttu-id="90ac2-372">ページ: **parentNotebook**、**parentSection**</span><span class="sxs-lookup"><span data-stu-id="90ac2-372">Pages: **parentNotebook**, **parentSection**</span></span>
- <span data-ttu-id="90ac2-373">セクション: **parentNotebook**、**parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="90ac2-373">Sections: **parentNotebook**, **parentSectionGroup**</span></span>
- <span data-ttu-id="90ac2-374">セクション グループ: **sections**、**sectionGroups**、**parentNotebook**、**parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="90ac2-374">Section groups: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**</span></span>
- <span data-ttu-id="90ac2-375">ノートブック: **sections**、**sectionGroups**</span><span class="sxs-lookup"><span data-stu-id="90ac2-375">Notebooks: **sections**, **sectionGroups**</span></span>


<a name="request-response-info"></a>
## <a name="request-and-response-information-for-get-requests"></a><span data-ttu-id="90ac2-376">要求および *GET* 要求の応答に関する情報</span><span class="sxs-lookup"><span data-stu-id="90ac2-376">Request and response information for *GET* requests</span></span>

| <span data-ttu-id="90ac2-377">要求データ</span><span class="sxs-lookup"><span data-stu-id="90ac2-377">Request data</span></span> | <span data-ttu-id="90ac2-378">説明</span><span class="sxs-lookup"><span data-stu-id="90ac2-378">Description</span></span> |  
|------|------|  
| <span data-ttu-id="90ac2-379">プロトコル</span><span class="sxs-lookup"><span data-stu-id="90ac2-379">Protocol</span></span> | <span data-ttu-id="90ac2-380">すべての要求は SSL/TLS HTTPS プロトコルを使用します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-380">All requests use the SSL/TLS HTTPS protocol.</span></span> |  
| <span data-ttu-id="90ac2-381">承認ヘッダー</span><span class="sxs-lookup"><span data-stu-id="90ac2-381">Authorization header</span></span> | <p><span data-ttu-id="90ac2-382">`Bearer {token}`。*{token}* は、登録済みアプリの有効な OAuth 2.0 アクセス トークンになります。</span><span class="sxs-lookup"><span data-stu-id="90ac2-382">`Bearer {token}`, where *{token}* is a valid OAuth 2.0 access token for your registered app.</span></span></p><p><span data-ttu-id="90ac2-383">これがないか、無効の場合、要求は失敗し、401 ステータス コードが表示されます。</span><span class="sxs-lookup"><span data-stu-id="90ac2-383">If missing or invalid, the request fails with a 401 status code.</span></span> <span data-ttu-id="90ac2-384">「[認証とアクセス許可](permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="90ac2-384">See [Authentication and permissions](permissions_reference.md).</span></span></p> |  
| <span data-ttu-id="90ac2-385">Accept ヘッダー</span><span class="sxs-lookup"><span data-stu-id="90ac2-385">Accept header</span></span> | <p><span data-ttu-id="90ac2-386">-  OneNote エンティティとエンティティ セットの `application/json`</span><span class="sxs-lookup"><span data-stu-id="90ac2-386">- `application/json` for OneNote entities and entity sets</span></span></p><p><span data-ttu-id="90ac2-387">-  ページ コンテンツの `text/html`</span><span class="sxs-lookup"><span data-stu-id="90ac2-387">- `text/html` for page content</span></span></p> | 

| <span data-ttu-id="90ac2-388">応答データ</span><span class="sxs-lookup"><span data-stu-id="90ac2-388">Response data</span></span> | <span data-ttu-id="90ac2-389">説明</span><span class="sxs-lookup"><span data-stu-id="90ac2-389">Description</span></span> |  
|------|------|  
| <span data-ttu-id="90ac2-390">成功コード</span><span class="sxs-lookup"><span data-stu-id="90ac2-390">Success code</span></span> | <span data-ttu-id="90ac2-391">200 HTTP ステータス コード。</span><span class="sxs-lookup"><span data-stu-id="90ac2-391">A 200 HTTP status code.</span></span> |  
| <span data-ttu-id="90ac2-392">応答本文</span><span class="sxs-lookup"><span data-stu-id="90ac2-392">Response body</span></span> | <span data-ttu-id="90ac2-393">JSON 形式のエンティティまたはエンティティ セット、ページ HTML、またはファイル リソースのバイナリ データの OData 表現。</span><span class="sxs-lookup"><span data-stu-id="90ac2-393">An OData representation of the entity or entity set in JSON format, the page HTML, or file resource binary data.</span></span>  |  
| <span data-ttu-id="90ac2-394">エラー</span><span class="sxs-lookup"><span data-stu-id="90ac2-394">Errors</span></span> | <span data-ttu-id="90ac2-395">要求が失敗すると、API は応答本文の **@api.diagnostics** オブジェクトに[エラー](onenote_error_codes.md)を返します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-395">If the request fails, the API returns [errors](onenote_error_codes.md) in the **@api.diagnostics** object in the response body.</span></span> |  
| <span data-ttu-id="90ac2-396">X-CorrelationId ヘッダー</span><span class="sxs-lookup"><span data-stu-id="90ac2-396">X-CorrelationId header</span></span> | <span data-ttu-id="90ac2-p143">要求を一意に識別する GUID。Microsoft サポートと問題のトラブルシューティングを行う際に、この値を Date ヘッダーの値とともに使用できます。</span><span class="sxs-lookup"><span data-stu-id="90ac2-p143">A GUID that uniquely identifies the request. You can use this value along with the value of the Date header when working with Microsoft support to troubleshoot issues.</span></span> |  


<a name="root-url"></a>
### <a name="constructing-the-microsoft-graph-notes-service-root-url"></a><span data-ttu-id="90ac2-399">Microsoft Graph のノート サービスのルート URL の構築</span><span class="sxs-lookup"><span data-stu-id="90ac2-399">Constructing the Microsoft Graph notes service root URL</span></span>

<span data-ttu-id="90ac2-400">Microsoft Graph ノートのルート URL は、Microsoft Graph ノートへのすべての呼び出しで次の形式を使用します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-400">The Microsoft Graph notes root URL uses the following format for all calls to Microsoft Graph notes.</span></span> <span data-ttu-id="90ac2-401">`https://graph.microsoft.com/{version}/me/onenote/`  URL の `version` セグメントは、使用する Microsoft Graph のバージョンを示しています。</span><span class="sxs-lookup"><span data-stu-id="90ac2-401">The `https://graph.microsoft.com/{version}/me/onenote/` segment in the URL represents the version of the OneNote API that you want to use.</span></span> <span data-ttu-id="90ac2-402">安定した運用コードには `v1.0` を使用します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-402">Use `v1.0` for stable production code.</span></span> <span data-ttu-id="90ac2-403">開発中の機能を試すには `beta` を使用します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-403">Use `beta` to try out a feature that's in development.</span></span> <span data-ttu-id="90ac2-404">ベータ版の機能は変更される可能性があるため、運用コードでは使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="90ac2-404">Features and functionality in beta may change, so you shouldn't use it in your production code.</span></span> <span data-ttu-id="90ac2-405">現在のユーザーがアクセスできる OneNote コンテンツには `me` を使用します (所有と共有)。</span><span class="sxs-lookup"><span data-stu-id="90ac2-405">Use `me` for OneNote content that the current user can access (owned and shared).</span></span> <span data-ttu-id="90ac2-406">指定されたユーザー (URL 内) が現在のユーザーと共有している OneNote コンテンツには `users/{id}` を使用します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-406">Use `users/{id}` for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="90ac2-407">ユーザー ID を取得するには [Microsoft Graph](https://graph.microsoft.com/v1.0/users) を使用します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-407">Use the [Azure AD Graph API](https://graph.microsoft.com/v1.0/users) to get user IDs.</span></span> 


<a name="permissions"></a>
## <a name="permissions-for-get-requests"></a><span data-ttu-id="90ac2-408">GET 要求のアクセス許可</span><span class="sxs-lookup"><span data-stu-id="90ac2-408">Permissions for GET requests</span></span>

<span data-ttu-id="90ac2-409">OneNote のコンテンツまたは構造を取得するには、適切なアクセス許可を要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="90ac2-409">To get OneNote content or structure, you'll need to request appropriate permissions.</span></span> 

<span data-ttu-id="90ac2-410">次のスコープは、Microsoft Graph に対する GET 要求を許可します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-410">The following scopes allow GET requests to Microsoft Graph.</span></span> <span data-ttu-id="90ac2-411">アプリの動作に必要な最低限のアクセス許可を選択してください。</span><span class="sxs-lookup"><span data-stu-id="90ac2-411">Choose the lowest level of permissions that your app needs to do its work.</span></span>

<span data-ttu-id="90ac2-412">次から選択します。</span><span class="sxs-lookup"><span data-stu-id="90ac2-412">Choose from:</span></span> 
- <span data-ttu-id="90ac2-413">Notes.read</span><span class="sxs-lookup"><span data-stu-id="90ac2-413">Notes.Read</span></span>
- <span data-ttu-id="90ac2-414">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="90ac2-414">Notes.ReadWrite</span></span>
- <span data-ttu-id="90ac2-415">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90ac2-415">Notes.ReadWrite.All</span></span>


<span data-ttu-id="90ac2-416">アクセス許可の範囲とその動作方法の詳細については、「[Microsoft Graph のアクセス許可のリファレンス](permissions_reference.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="90ac2-416">For more information about permission scopes and how they work, see [OneNote permission scopes](permissions_reference.md).</span></span>

<a name="see-also"></a>
## <a name="additional-resources"></a><span data-ttu-id="90ac2-417">その他のリソース</span><span class="sxs-lookup"><span data-stu-id="90ac2-417">Additional resources</span></span>

- [<span data-ttu-id="90ac2-418">OneNote ページの入出力 HTML</span><span class="sxs-lookup"><span data-stu-id="90ac2-418">Input and output HTML for OneNote pages</span></span>](onenote_input_output_html.md)
- [<span data-ttu-id="90ac2-419">OneNote との統合</span><span class="sxs-lookup"><span data-stu-id="90ac2-419">Integrate with OneNote</span></span>](integrate_with_onenote.md)
- [<span data-ttu-id="90ac2-420">OneNote の開発者ブログ</span><span class="sxs-lookup"><span data-stu-id="90ac2-420">OneNote Developer Blog</span></span>](http://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="90ac2-421">Stack Overflow 掲載の OneNote の開発に関する質問</span><span class="sxs-lookup"><span data-stu-id="90ac2-421">OneNote development questions on Stack Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="90ac2-422">OneNote GitHub のリポジトリ</span><span class="sxs-lookup"><span data-stu-id="90ac2-422">OneNote GitHub repos</span></span>](http://go.microsoft.com/fwlink/?LinkID=390178)  
