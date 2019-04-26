---
title: Microsoft Graph によって OneNote コンテンツと構造を取得する
description: " Office 365 のエンタープライズ ノートブック"
author: jewan-microsoft
localization_priority: Priority
ms.prod: onenote
ms.openlocfilehash: 835cd7ba930c7e8ea2d26f750a85e097db2399f0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555438"
---
# <a name="get-onenote-content-and-structure-with-microsoft-graph"></a><span data-ttu-id="368d7-103">Microsoft Graph によって OneNote コンテンツと構造を取得する</span><span class="sxs-lookup"><span data-stu-id="368d7-103">Get OneNote content and structure with Microsoft Graph</span></span>

<span data-ttu-id="368d7-104">**適用対象**: OneDrive のコンシューマー ノートブック | Office 365 のエンタープライズ ノートブック</span><span class="sxs-lookup"><span data-stu-id="368d7-104">**Applies to**: Consumer notebooks on OneDrive | Enterprise notebooks on Office 365</span></span>

<span data-ttu-id="368d7-p101">OneNote のコンテンツと構造を取得するには、ターゲット エンドポイントに GET 要求を送信します。たとえば次のようにします。</span><span class="sxs-lookup"><span data-stu-id="368d7-p101">To get OneNote content and structure, you send a GET request to the target endpoint. For example:</span></span>

`GET ../onenote/pages/{id}`

<span data-ttu-id="368d7-107">要求が成功すると、Microsoft Graph は 200 HTTP 状態コードと、要求したエンティティまたはコンテンツを返します。</span><span class="sxs-lookup"><span data-stu-id="368d7-107">If the request is successful, Microsoft Graph returns a 200 HTTP status code and the entities or content that you requested.</span></span> <span data-ttu-id="368d7-108">OneNote のエンティティは、OData バージョン 4.0 仕様に準拠した JSON オブジェクトとして返されます。</span><span class="sxs-lookup"><span data-stu-id="368d7-108">OneNote entities are returned as JSON objects that conform to the OData version 4.0 specification.</span></span>

<span data-ttu-id="368d7-109">クエリ文字列オプションを使用すると、クエリをフィルターしてパフォーマンスを向上させることができます。</span><span class="sxs-lookup"><span data-stu-id="368d7-109">By using query string options, you can filter your queries and improve performance.</span></span>


<a name="request-uri"></a>

## <a name="construct-the-request-uri"></a><span data-ttu-id="368d7-110">要求 URI の構築</span><span class="sxs-lookup"><span data-stu-id="368d7-110">Construct the request URI</span></span>

<span data-ttu-id="368d7-111">要求 URI を構築するには、サービス ルート URL から開始します。</span><span class="sxs-lookup"><span data-stu-id="368d7-111">To construct the request URI, start with the service root URL:</span></span>

`https://graph.microsoft.com/v1.0/me/onenote`

<br/>

<span data-ttu-id="368d7-p103">次に、取得するリソースのエンドポイントを追加します ([リソース パス](#resource-paths-for-get-requests)については次のセクションを参照してください)。</span><span class="sxs-lookup"><span data-stu-id="368d7-p103">Then append the endpoint of the resource you want to retrieve. ([Resource paths](#resource-paths-for-get-requests) are shown in the next section.)</span></span>

<span data-ttu-id="368d7-114">完全な要求 URI は、次に示す例のいずれかのようになります。</span><span class="sxs-lookup"><span data-stu-id="368d7-114">Your full request URI will look like one of these examples:</span></span>

- `https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sections`
- `https://graph.microsoft.com/v1.0/me/onenote/notes/pages`
- `https://graph.microsoft.com/v1.0/me/onenote/pages?select=title,self`

> <span data-ttu-id="368d7-115">**注:** [サービス ルート URL](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url) の詳細についてはリンク先をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="368d7-115">**Note:** Learn more about the [service root URL](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).</span></span>

<a name="resource-paths"></a>

## <a name="resource-paths-for-get-requests"></a><span data-ttu-id="368d7-116">GET 要求のリソース パス</span><span class="sxs-lookup"><span data-stu-id="368d7-116">Resource paths for GET requests</span></span>

<span data-ttu-id="368d7-117">次のリソース パスを使用して、ページ、セクション、セクション グループ、ノートブック、画像、またはファイル リソースを取得します。</span><span class="sxs-lookup"><span data-stu-id="368d7-117">Use the following resource paths to get pages, sections, section groups, notebooks, and image or file resources.</span></span>

- [<span data-ttu-id="368d7-118">ページ コレクション</span><span class="sxs-lookup"><span data-stu-id="368d7-118">Page collection</span></span>](#page-collection)
- [<span data-ttu-id="368d7-119">ページ エンティティ</span><span class="sxs-lookup"><span data-stu-id="368d7-119">Page entity</span></span>](#page-entity)
- [<span data-ttu-id="368d7-120">ページ プレビュー</span><span class="sxs-lookup"><span data-stu-id="368d7-120">Page preview</span></span>](#page-preview)
- [<span data-ttu-id="368d7-121">ページ HTML コンテンツ</span><span class="sxs-lookup"><span data-stu-id="368d7-121">Page HTML content</span></span>](#page-html-content)
- [<span data-ttu-id="368d7-122">セクション コレクション</span><span class="sxs-lookup"><span data-stu-id="368d7-122">Section collection</span></span>](#section-collection)
- [<span data-ttu-id="368d7-123">セクション エンティティ</span><span class="sxs-lookup"><span data-stu-id="368d7-123">Section entity</span></span>](#section-entity)
- [<span data-ttu-id="368d7-124">SectionGroup コレクション</span><span class="sxs-lookup"><span data-stu-id="368d7-124">SectionGroup collection</span></span>](#sectiongroup-collection)
- [<span data-ttu-id="368d7-125">SectionGroup エンティティ</span><span class="sxs-lookup"><span data-stu-id="368d7-125">SectionGroup entity</span></span>](#sectiongroup-entity)
- [<span data-ttu-id="368d7-126">ノートブック コレクション</span><span class="sxs-lookup"><span data-stu-id="368d7-126">Notebook collection</span></span>](#notebook-collection)
- [<span data-ttu-id="368d7-127">ノートブック エンティティ</span><span class="sxs-lookup"><span data-stu-id="368d7-127">Notebook entity</span></span>](#notebook-entity)
- [<span data-ttu-id="368d7-128">画像またはその他のファイル リソース</span><span class="sxs-lookup"><span data-stu-id="368d7-128">Image or other file resource</span></span>](#image-or-other-file-resource)

<a name="get-pages"></a>

### <a name="page-collection"></a><span data-ttu-id="368d7-129">ページ コレクション</span><span class="sxs-lookup"><span data-stu-id="368d7-129">Page collection</span></span>

<span data-ttu-id="368d7-130">すべてのノートブックのページ (メタデータ) を取得する。</span><span class="sxs-lookup"><span data-stu-id="368d7-130">Get pages (metadata) across all notebooks.</span></span>

`../pages[?filter,orderby,select,expand,top,skip,search,count]`

<br/>

<span data-ttu-id="368d7-131">特定のセクションからページ (メタデータ) を取得する。</span><span class="sxs-lookup"><span data-stu-id="368d7-131">Get pages (metadata) from a specific section.</span></span>

`../sections/{section-id}/pages[?filter,orderby,select,expand,top,skip,search,count,pagelevel]`

<br/>
 
<span data-ttu-id="368d7-132">`search`クエリ文字列オプションは、コンシューマー ノートパソコンでのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="368d7-132">The `search` query string option is available for consumer notebooks only.</span></span>

<span data-ttu-id="368d7-133">ページの既定の並べ替え順序は `lastModifiedTime desc` です。</span><span class="sxs-lookup"><span data-stu-id="368d7-133">The default sort order for pages is `lastModifiedTime desc`.</span></span>

<span data-ttu-id="368d7-134">既定のクエリは、親セクションを展開し、セクションの `id`、`name`、および `self` プロパティを選択します。</span><span class="sxs-lookup"><span data-stu-id="368d7-134">The default query expands the parent section and selects the section's `id`, `name`, and `self` properties.</span></span>

<span data-ttu-id="368d7-135">既定では、*GET ページ*要求に対して上位 20 のエントリのみが返されます。</span><span class="sxs-lookup"><span data-stu-id="368d7-135">By default, only the top 20 entries are returned for *GET pages* requests.</span></span> <span data-ttu-id="368d7-136">**上位**クエリ文字列オプションを指定しない要求を行った場合、次の 20 エントリを取得するために使用できる `@odata.nextLink` リンクが応答で返されます。</span><span class="sxs-lookup"><span data-stu-id="368d7-136">Requests that don't specify a **top** query string option return an `@odata.nextLink` link in the response that you can use to get the next 20 entries.</span></span>

<span data-ttu-id="368d7-137">セクションのページ コレクションの場合、**pagelevel** を使用して、ページのインデント レベルとセクション内でのその順序を返します。</span><span class="sxs-lookup"><span data-stu-id="368d7-137">For the pages collection in a section, use **pagelevel** to return the indentation level of pages and their order within the section.</span></span> 

#### <a name="example"></a><span data-ttu-id="368d7-138">例</span><span class="sxs-lookup"><span data-stu-id="368d7-138">Example</span></span>

`GET ../sections/{section-id}/pages?pagelevel=true`



<a name="get-page"></a> 

### <a name="page-entity"></a><span data-ttu-id="368d7-139">ページ エンティティ</span><span class="sxs-lookup"><span data-stu-id="368d7-139">Page entity</span></span>

<span data-ttu-id="368d7-140">特定のページのメタデータを取得する</span><span class="sxs-lookup"><span data-stu-id="368d7-140">Get the metadata for a specific page.</span></span> 

`../pages/{page-id}[?select,expand,pagelevel]` 

<br/>

<span data-ttu-id="368d7-141">ページは、**parentNotebook** プロパティと **parentSection** プロパティを展開できます。</span><span class="sxs-lookup"><span data-stu-id="368d7-141">Pages can expand the **parentNotebook** and **parentSection** properties.</span></span>

<span data-ttu-id="368d7-142">既定のクエリは、親セクションを展開し、セクションの `id`、`name`、および `self` プロパティを選択します。</span><span class="sxs-lookup"><span data-stu-id="368d7-142">The default query expands the parent section and selects the section's `id`, `name`, and `self` properties.</span></span>

<span data-ttu-id="368d7-143">**pagelevel** を使用して、ページのインデント レベルと親セクション内でのその順序を返します。</span><span class="sxs-lookup"><span data-stu-id="368d7-143">Use **pagelevel** to return the indentation level of the page and its order within its parent section.</span></span> 

#### <a name="example"></a><span data-ttu-id="368d7-144">例</span><span class="sxs-lookup"><span data-stu-id="368d7-144">Example</span></span>

`GET ../pages/{page-id}?pagelevel=true`



<a name="get-page-preview"></a> 

### <a name="page-preview"></a><span data-ttu-id="368d7-145">ページ プレビュー</span><span class="sxs-lookup"><span data-stu-id="368d7-145">Page preview</span></span>

<span data-ttu-id="368d7-146">ページのテキストと画像のプレビュー コンテンツを取得する。</span><span class="sxs-lookup"><span data-stu-id="368d7-146">Get text and image preview content for a page.</span></span>

`../pages/{page-id}/preview`

<br/>


<span data-ttu-id="368d7-147">JSON 応答には、ページに含まれているものを特定するために使用できる、プレビュー コンテンツが含まれています。</span><span class="sxs-lookup"><span data-stu-id="368d7-147">The JSON response contains the preview content, which you can use to help users identify what's in the page.</span></span>

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

<span data-ttu-id="368d7-148">**previewText** プロパティには、ページからのテキスト スニペットが含まれています。</span><span class="sxs-lookup"><span data-stu-id="368d7-148">The **previewText** property contains a text snippet from the page.</span></span> <span data-ttu-id="368d7-149">Microsoft Graph は、最大 300 文字の完全な文字列を返します。</span><span class="sxs-lookup"><span data-stu-id="368d7-149">Microsoft Graph returns complete phrases, up to a maximum of 300 characters.</span></span> 

<span data-ttu-id="368d7-150">ページにプレビュー UI のビルドに使用できる画像が含まれている場合、**previewImageUrl** オブジェクトの **href** プロパティには、事前認証されたパブリックの [image resource](#image-or-other-file-resource) のリンクが含まれます。</span><span class="sxs-lookup"><span data-stu-id="368d7-150">If the page has an image that can be used to build a preview UI, the **href** property in the **previewImageUrl** object contains a link to a public, pre-authenticated [image resource](#image-or-other-file-resource).</span></span> <span data-ttu-id="368d7-151">このリンクは HTML で使用できます。</span><span class="sxs-lookup"><span data-stu-id="368d7-151">You can use this link in HTML.</span></span> <span data-ttu-id="368d7-152">それ以外の場合、**href** は、null 値を返します。</span><span class="sxs-lookup"><span data-stu-id="368d7-152">Otherwise, **href** returns null.</span></span>

#### <a name="example"></a><span data-ttu-id="368d7-153">例</span><span class="sxs-lookup"><span data-stu-id="368d7-153">Example</span></span> 

`<img src="https://www.onenote.com/api/v1.0/resources/{id}/content?publicAuth=true&mimeType=image/png" />`


<a name="get-page-content"></a> 

### <a name="page-html-content"></a><span data-ttu-id="368d7-154">ページ HTML コンテンツ</span><span class="sxs-lookup"><span data-stu-id="368d7-154">Page HTML content</span></span>

<span data-ttu-id="368d7-155">ページの HTML コンテンツを取得する。</span><span class="sxs-lookup"><span data-stu-id="368d7-155">Get the HTML content of a page.</span></span>

`../pages/{page-id}/content[?includeIDs]`

<span data-ttu-id="368d7-156">(*[返される HTML コンテンツ](onenote-input-output-html.md)の詳細についてはリンク先をご覧ください*)</span><span class="sxs-lookup"><span data-stu-id="368d7-156">(*learn more about [returned HTML content](onenote-input-output-html.md)*)</span></span> 

<br/>

<span data-ttu-id="368d7-157">**includeIDs=true** クエリ文字列オプションを使用して、[ページを更新](onenote-update-page.md)するために使用する生成 ID を取得します。</span><span class="sxs-lookup"><span data-stu-id="368d7-157">Use the **includeIDs=true** query string option to get generated IDs used to [update the page](onenote-update-page.md).</span></span>



<a name="get-sections"></a>

### <a name="section-collection"></a><span data-ttu-id="368d7-158">セクション コレクション</span><span class="sxs-lookup"><span data-stu-id="368d7-158">Section collection</span></span>

<span data-ttu-id="368d7-159">ユーザーが所有するすべてのノートブックから、ネストされたセクション グループのセクションを含む、すべてのセクションを取得する。</span><span class="sxs-lookup"><span data-stu-id="368d7-159">Get all sections from all notebooks that are owned by the user, including sections in nested section groups.</span></span>

`../sections[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="368d7-160">特定のセクション グループの直下にあるすべてのセクションを取得する。</span><span class="sxs-lookup"><span data-stu-id="368d7-160">Get all sections that are directly under a specific section group.</span></span>

`../sectionGroups/{sectiongroup-id}/sections[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="368d7-161">特定のノートブックの直下にあるすべてのセクションを取得する。</span><span class="sxs-lookup"><span data-stu-id="368d7-161">Get all sections that are directly under a specific notebook.</span></span>

`../notebooks/{notebook-id}/sections[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="368d7-162">セクションは、**parentNotebook** プロパティと **parentSectionGroup** プロパティを展開できます。</span><span class="sxs-lookup"><span data-stu-id="368d7-162">Sections can expand the **parentNotebook** and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="368d7-163">セクションの既定の並べ替え順序は `name asc` です。</span><span class="sxs-lookup"><span data-stu-id="368d7-163">The default sort order for sections is `name asc`.</span></span>

<span data-ttu-id="368d7-164">既定のクエリは、親ノートブックおよび親セクション グループを展開し、`id`、`name`、および `self` プロパティを選択します。</span><span class="sxs-lookup"><span data-stu-id="368d7-164">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>



<a name="get-section"></a>

### <a name="section-entity"></a><span data-ttu-id="368d7-165">セクション エンティティ</span><span class="sxs-lookup"><span data-stu-id="368d7-165">Section entity</span></span>

<span data-ttu-id="368d7-166">特定のセクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="368d7-166">Get a specific section.</span></span>

`../sections/{section-id}[?select,expand]` 

<br/>

<span data-ttu-id="368d7-167">セクションは、**parentNotebook** プロパティと **parentSectionGroup** プロパティを展開できます。</span><span class="sxs-lookup"><span data-stu-id="368d7-167">Sections can expand the **parentNotebook** and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="368d7-168">既定のクエリは、親ノートブックおよび親セクション グループを展開し、`id`、`name`、および `self` プロパティを選択します。</span><span class="sxs-lookup"><span data-stu-id="368d7-168">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>



<a name="get-section-groups"></a>

### <a name="sectiongroup-collection"></a><span data-ttu-id="368d7-169">SectionGroup コレクション</span><span class="sxs-lookup"><span data-stu-id="368d7-169">SectionGroup collection</span></span>

<span data-ttu-id="368d7-170">ユーザーが所有するすべてのノートブックから、ネストされたセクション グループを含む、すべてのセクション グループを取得する。</span><span class="sxs-lookup"><span data-stu-id="368d7-170">Get all section groups from all notebooks that are owned by the user, including nested section groups.</span></span>

`../sectionGroups[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="368d7-171">特定のノートブックの直下にあるすべてのセクション グループを取得する。</span><span class="sxs-lookup"><span data-stu-id="368d7-171">Get all section groups that are directly under a specific notebook.</span></span> 

`../notebooks/{notebook-id}/sectionGroups[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="368d7-172">セクション グループは、**セクション**、**sectionGroups**、**parentNotebook**、および **parentSectionGroup** プロパティを展開できます。</span><span class="sxs-lookup"><span data-stu-id="368d7-172">Section groups can expand the **sections**, **sectionGroups**, **parentNotebook**, and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="368d7-173">セクション グループの既定の並べ替え順序は `name asc` です。</span><span class="sxs-lookup"><span data-stu-id="368d7-173">The default sort order for section groups is `name asc`.</span></span>

<span data-ttu-id="368d7-174">既定のクエリは、親ノートブックおよび親セクション グループを展開し、`id`、`name`、および `self` プロパティを選択します。</span><span class="sxs-lookup"><span data-stu-id="368d7-174">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>



<a name="get-section-group"></a>

### <a name="sectiongroup-entity"></a><span data-ttu-id="368d7-175">SectionGroup エンティティ</span><span class="sxs-lookup"><span data-stu-id="368d7-175">SectionGroup entity</span></span>

<span data-ttu-id="368d7-176">特定のセクション グループを取得します。</span><span class="sxs-lookup"><span data-stu-id="368d7-176">Get a specific section group.</span></span>

`../sectionGroups/{sectiongroup-id}[?select,expand]` 

<br/>

<span data-ttu-id="368d7-177">セクション グループは、**セクション**、**sectionGroups**、**parentNotebook**、および **parentSectionGroup** プロパティを展開できます。</span><span class="sxs-lookup"><span data-stu-id="368d7-177">Section groups can expand the **sections**, **sectionGroups**, **parentNotebook**, and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="368d7-178">既定のクエリは、親ノートブックおよび親セクション グループを展開し、`id`、`name`、および `self` プロパティを選択します。</span><span class="sxs-lookup"><span data-stu-id="368d7-178">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>



<a name="get-notebooks"></a>

### <a name="notebook-collection"></a><span data-ttu-id="368d7-179">ノートブック コレクション</span><span class="sxs-lookup"><span data-stu-id="368d7-179">Notebook collection</span></span>

<span data-ttu-id="368d7-180">ユーザーによって所有されるすべてのノートブックを取得する。</span><span class="sxs-lookup"><span data-stu-id="368d7-180">Get all the notebooks that are owned by the user.</span></span> 

`../notebooks[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="368d7-181">ノートブックは、**セクション**および **sectionGroups** プロパティを展開できます。</span><span class="sxs-lookup"><span data-stu-id="368d7-181">Notebooks can expand the **sections** and **sectionGroups** properties.</span></span>

<span data-ttu-id="368d7-182">ノートブックの既定の並べ替え順序は `name asc` です。</span><span class="sxs-lookup"><span data-stu-id="368d7-182">The default sort order for notebooks is `name asc`.</span></span> 



<a name="get-notebook"></a>

### <a name="notebook-entity"></a><span data-ttu-id="368d7-183">ノートブック エンティティ</span><span class="sxs-lookup"><span data-stu-id="368d7-183">Notebook entity</span></span>

<span data-ttu-id="368d7-184">特定のノートブックを取得します。</span><span class="sxs-lookup"><span data-stu-id="368d7-184">Get a specific notebook.</span></span>

`../notebooks/{notebook-id}[?select,expand]` 

<br/>

<span data-ttu-id="368d7-185">ノートブックは、**セクション**および **sectionGroups** プロパティを展開できます。</span><span class="sxs-lookup"><span data-stu-id="368d7-185">Notebooks can expand the **sections** and **sectionGroups** properties.</span></span>



<a name="get-resource"></a>

### <a name="image-or-other-file-resource"></a><span data-ttu-id="368d7-186">画像またはその他のファイル リソース</span><span class="sxs-lookup"><span data-stu-id="368d7-186">Image or other file resource</span></span>

<span data-ttu-id="368d7-187">特定のリソースのバイナリ データを取得する。</span><span class="sxs-lookup"><span data-stu-id="368d7-187">Get the binary data of a specific resource.</span></span> 

`../resources/{resource-id}/$value` 

<br/>

<span data-ttu-id="368d7-188">ファイルのリソース URI は、ページの[出力 HTML](onenote-input-output-html.md) にあります。</span><span class="sxs-lookup"><span data-stu-id="368d7-188">You can find the file's resource URI in the page's [output HTML](onenote-input-output-html.md).</span></span>

<span data-ttu-id="368d7-189">たとえば、**img** タグには、**data-fullres-src** 属性に元の画像のエンドポイント、**src** 属性に最適化された画像のエンドポイントが含まれます。</span><span class="sxs-lookup"><span data-stu-id="368d7-189">For example, an **img** tag includes endpoints for the original image in the **data-fullres-src** attribute and the optimized image in the **src** attribute.</span></span> 

#### <a name="example"></a><span data-ttu-id="368d7-190">例</span><span class="sxs-lookup"><span data-stu-id="368d7-190">Example</span></span>

```html
<img 
    src="https://www.onenote.com/api/v1.0/me/notes/resources/{image-id}/$value"  
    data-src-type="image/png"
    data-fullres-src="https://www.onenote.com/api/v1.0/resources/{image-id}/$value"  
    data-fullres-src-type="image/png" ... />
```

<span data-ttu-id="368d7-191">**object** タグには、**data** 属性のファイル リソースのエンドポイントが含まれています。</span><span class="sxs-lookup"><span data-stu-id="368d7-191">And an **object** tag includes the endpoint for the file resource in the **data** attribute.</span></span> 

#### <a name="example"></a><span data-ttu-id="368d7-192">例</span><span class="sxs-lookup"><span data-stu-id="368d7-192">Example</span></span>

```html
<object
    data="https://www.onenote.com/api/v1.0/me/notes/resources/{file-id}/$value"
    data-attachment="fileName.pdf" 
    type="application/pdf" ... />
```

> <span data-ttu-id="368d7-193">**注:** リソースのコレクションの取得はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="368d7-193">**Note:** Getting a collection of resources is not supported.</span></span> 

<span data-ttu-id="368d7-194">ファイル リソースを取得する場合、**Accept** コンテンツ タイプを要求に含める必要はありません。</span><span class="sxs-lookup"><span data-stu-id="368d7-194">When you get a file resource, you don't need to include an **Accept** content type in the request.</span></span>

<span data-ttu-id="368d7-195">GET 要求の詳細については、Microsoft Graph API REST リファレンスの中の次のリソースを参照してください。</span><span class="sxs-lookup"><span data-stu-id="368d7-195">For more information about GET requests, see the following resources in the Microsoft Graph API REST reference:</span></span>

- [<span data-ttu-id="368d7-196">ページを取得する</span><span class="sxs-lookup"><span data-stu-id="368d7-196">GET Pages</span></span>](/graph/api/page-get?view=graph-rest-1.0)
- [<span data-ttu-id="368d7-197">Get section</span><span class="sxs-lookup"><span data-stu-id="368d7-197">GET Sections</span></span>](/graph/api/section-get?view=graph-rest-1.0)
- [<span data-ttu-id="368d7-198">Get sectionGroup</span><span class="sxs-lookup"><span data-stu-id="368d7-198">GET SectionGroups</span></span>](/graph/api/sectiongroup-get?view=graph-rest-1.0)
- [<span data-ttu-id="368d7-199">ノートブックを取得する</span><span class="sxs-lookup"><span data-stu-id="368d7-199">GET Notebooks</span></span>](/graph/api/notebook-get?view=graph-rest-1.0) 




<a name="example"></a>

## <a name="example-get-requests"></a><span data-ttu-id="368d7-200">GET 要求の例</span><span class="sxs-lookup"><span data-stu-id="368d7-200">Example GET requests</span></span>

<span data-ttu-id="368d7-201">OneNote のエンティティおよび検索ページ コンテンツを照会して、必要な情報だけを取得することができます。</span><span class="sxs-lookup"><span data-stu-id="368d7-201">You can query for OneNote entities and search page content to get just the information you need.</span></span> <span data-ttu-id="368d7-202">次の例は、Microsoft Graph への GET 要求で、[サポートされているクエリ文字列オプション](#supported-odata-query-string-options)を使用するいくつかの方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="368d7-202">The following examples show some ways you can use [supported query string options](#supported-odata-query-string-options) in GET requests to Microsoft Graph.</span></span> 

<span data-ttu-id="368d7-203">**次の点にご注意ください。**</span><span class="sxs-lookup"><span data-stu-id="368d7-203">**Remember:**</span></span>

- <span data-ttu-id="368d7-204">GET 要求はすべて、[サービス ルート URL](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url) で始まります。</span><span class="sxs-lookup"><span data-stu-id="368d7-204">All GET requests start with the [service root URL](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).</span></span> <br/><br/><span data-ttu-id="368d7-205">**例**: `https://www.onenote.com/api/v1.0/me/notes` および `https://www.onenote.com/api/v1.0/myOrganization/siteCollections/{id}/sites/{id}/notes/`</span><span class="sxs-lookup"><span data-stu-id="368d7-205">**Examples**: `https://www.onenote.com/api/v1.0/me/notes` and `https://www.onenote.com/api/v1.0/myOrganization/siteCollections/{id}/sites/{id}/notes/`</span></span>

- <span data-ttu-id="368d7-206">URL クエリ文字列のスペースには %20 エンコードを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="368d7-206">Spaces in the URL query string must use %20 encoding.</span></span><br/><br/><span data-ttu-id="368d7-207">**例**: `filter=title%20eq%20'biology'`</span><span class="sxs-lookup"><span data-stu-id="368d7-207">**Example**: `filter=title%20eq%20'biology'`</span></span>

- <span data-ttu-id="368d7-208">プロパティ名と OData 文字列比較では大文字と小文字が区別されます。</span><span class="sxs-lookup"><span data-stu-id="368d7-208">Property names and OData string comparisons are case-sensitive.</span></span> <span data-ttu-id="368d7-209">文字列比較には OData **tolower** 関数を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="368d7-209">We recommend using the OData **tolower** function for string comparisons.</span></span><br/><br/><span data-ttu-id="368d7-210">**例**: `filter=tolower(name) eq 'spring'`</span><span class="sxs-lookup"><span data-stu-id="368d7-210">**Example**: `filter=tolower(name) eq 'spring'`</span></span>
 

### <a name="search--filter"></a><span data-ttu-id="368d7-211">search & filter</span><span class="sxs-lookup"><span data-stu-id="368d7-211">search & filter</span></span>  

<span data-ttu-id="368d7-212">特定のアプリによって作成された、*recipe* という用語が含まれるページすべてを取得します (`search` はコンシューマー ノートブックでのみ使用可能)。</span><span class="sxs-lookup"><span data-stu-id="368d7-212">Get all pages that contain the term *recipe* that were created by a specific app (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search=recipe&filter=createdByAppId eq 'WLID-000000004C12821A'
```
 
### <a name="search--select"></a><span data-ttu-id="368d7-213">search & select</span><span class="sxs-lookup"><span data-stu-id="368d7-213">search & select</span></span>  

<span data-ttu-id="368d7-214">*golgi app* という用語が含まれるすべてのページの、タイトル、OneNote クライアントのリンク、**contentUrl** リンクを取得します (`search` はコンシューマー ノートブックでのみ使用可能)。</span><span class="sxs-lookup"><span data-stu-id="368d7-214">Get the title, OneNote client links, and **contentUrl** link for all pages that contain the term *golgi app* (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search=golgi app&select=title,links,contentUrl
```
 
### <a name="expand"></a><span data-ttu-id="368d7-215">expand</span><span class="sxs-lookup"><span data-stu-id="368d7-215">expand</span></span> 

<span data-ttu-id="368d7-216">すべてのノートブックを取得し、そのセクションとセクション グループを展開します。</span><span class="sxs-lookup"><span data-stu-id="368d7-216">Get all notebooks and expand their sections and section groups.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups
```

<br/>

<span data-ttu-id="368d7-217">特定のセクション グループを取得し、そのセクションとセクション グループを展開します。</span><span class="sxs-lookup"><span data-stu-id="368d7-217">Get a specific section group and expand its sections and section groups.</span></span>  

```
[GET] ../sectionGroups/{sectiongroup-id}?expand=sections,sectionGroups
```

<br/>

<span data-ttu-id="368d7-218">ページを取得し、その親セクションと親ノートブックを展開します。</span><span class="sxs-lookup"><span data-stu-id="368d7-218">Get a page and expand its parent section and parent notebook.</span></span>

```
[GET] ../pages/{page-id}?expand=parentSection,parentNotebook
```

### <a name="expand-multiple-levels"></a><span data-ttu-id="368d7-219">expand (複数レベル)</span><span class="sxs-lookup"><span data-stu-id="368d7-219">expand (multiple levels)</span></span>  

<span data-ttu-id="368d7-220">すべてのノートブックを取得してセクションとセクション グループを展開し、各セクション グループのすべてのセクションを展開します。</span><span class="sxs-lookup"><span data-stu-id="368d7-220">Get all notebooks and expand their sections and section groups, and expand all sections in each section group.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups(expand=sections)
```
 
> <span data-ttu-id="368d7-221">**注:** 子エンティティの親を展開、または親エンティティの子を展開すると、循環参照が作成されますが、これはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="368d7-221">**Note:** Expanding parents of child entities or expanding children of parent entities creates a circular reference and is not supported.</span></span>

 
### <a name="expand--select-multiple-levels"></a><span data-ttu-id="368d7-222">expand & select (複数レベル)</span><span class="sxs-lookup"><span data-stu-id="368d7-222">expand & select (multiple levels)</span></span>  

<span data-ttu-id="368d7-223">特定のセクション グループの名前と **self** リンクを取得し、そのすべてのセクションの名前と **self** リンクを取得します。</span><span class="sxs-lookup"><span data-stu-id="368d7-223">Get the name and **self** link for a specific section group, and get the name and **self** links for all its sections.</span></span>  

```
[GET] ../sectionGroups/{sectiongroup-id}?expand=sections(select=name,self)&select=name,self
```

<br/>

<span data-ttu-id="368d7-224">すべてのセクションの名前と **self** リンクを取得し、各セクションの親ノートブックの名前と作成時刻を取得します。</span><span class="sxs-lookup"><span data-stu-id="368d7-224">Get the name and **self** link for all sections, and get the name and created time of each section's parent notebook.</span></span>  

```
[GET] ../sections?expand=parentNotebook(select=name,createdTime)&select=name,self
```

<br/>
 
<span data-ttu-id="368d7-225">すべてのページのタイトルと ID を取得し、親セクションと親ノートブックの名前を取得します。</span><span class="sxs-lookup"><span data-stu-id="368d7-225">Get the title and ID for all pages, and get the name of the parent section and parent notebook.</span></span>

```
[GET] ../pages?select=id,title&expand=parentSection(select=name),parentNotebook(select=name)
```

### <a name="expand--levels-multiple-levels"></a><span data-ttu-id="368d7-226">expand & levels (複数レベル)</span><span class="sxs-lookup"><span data-stu-id="368d7-226">expand & levels (multiple levels)</span></span>  

<span data-ttu-id="368d7-227">すべてのノートブック、セクション、セクション グループを取得します。</span><span class="sxs-lookup"><span data-stu-id="368d7-227">Get all notebooks, sections, and section groups.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups(expand=sections,sectionGroups(levels=max;expand=sections))
```
 
### <a name="filter"></a><span data-ttu-id="368d7-228">filter</span><span class="sxs-lookup"><span data-stu-id="368d7-228">filter</span></span>

<span data-ttu-id="368d7-229">2014 年 10 月に作成されたセクションすべてを取得します。</span><span class="sxs-lookup"><span data-stu-id="368d7-229">Get all sections that were created in October 2014.</span></span>

```
[GET] ../sections?filter=createdTime ge 2014-10-01 and createdTime le 2014-10-31
```

<br/>

<span data-ttu-id="368d7-230">2015 年 1 月 1 日以降に特定のアプリによって作成されたページを取得します。</span><span class="sxs-lookup"><span data-stu-id="368d7-230">Get the pages that were created by a specific app since January 1, 2015.</span></span>

```
[GET] ../pages?filter=createdByAppId eq 'WLID-0000000048118631' and createdTime ge 2015-01-01
```

### <a name="filter--expand"></a><span data-ttu-id="368d7-231">filter & expand</span><span class="sxs-lookup"><span data-stu-id="368d7-231">filter & expand</span></span>  

<span data-ttu-id="368d7-p109">特定のノートブックに含まれるすべてのページを取得します。既定では、この API は 20 エントリを戻します。</span><span class="sxs-lookup"><span data-stu-id="368d7-p109">Get all pages in a specific notebook. The API returns 20 entries by default.</span></span>

```
[GET] ../pages?filter=parentNotebook/id eq '{notebook-id}'&expand=parentNotebook
```

<br/>

<span data-ttu-id="368d7-234">*学校*のノートブックにあるすべてのセクションの名前と **pagesUrl** リンクを取得します。</span><span class="sxs-lookup"><span data-stu-id="368d7-234">Get the name and **pagesUrl** link for all sections from the *School* notebook.</span></span> <span data-ttu-id="368d7-235">OData の文字列比較は大文字小文字が区別されるので、ベスト プラクティスとして **tolower** 関数を使用します。</span><span class="sxs-lookup"><span data-stu-id="368d7-235">OData string comparisons are case-sensitive, so use the **tolower** function as a best practice.</span></span>

```
[GET] ../notebooks?filter=tolower(name) eq 'school'&expand=sections(select=name,pagesUrl)
```

### <a name="filter--select--orderby"></a><span data-ttu-id="368d7-236">filter & select & orderby</span><span class="sxs-lookup"><span data-stu-id="368d7-236">filter & select & orderby</span></span>   

<span data-ttu-id="368d7-p111">セクション名に *spring* という語が含まれるすべてのセクションの名前と **pagesUrl** リンクを取得します。セクションを最終変更日で並べ替えます。</span><span class="sxs-lookup"><span data-stu-id="368d7-p111">Get the name and **pagesUrl** link for all sections that contain the term *spring* in the section name. Order sections by last modified date.</span></span>

```
[GET] ../sections?filter=contains(tolower(name),'spring')&select=name,pagesUrl&orderby=lastModifiedTime desc
```
 
### <a name="orderby"></a><span data-ttu-id="368d7-239">orderby</span><span class="sxs-lookup"><span data-stu-id="368d7-239">orderby</span></span>

<span data-ttu-id="368d7-p112">**createdByAppId** プロパティ、次に作成時刻を基準に順序を並べ替えて、最初の 20 ページを取得します。既定では、この API は 20 エントリを戻します。</span><span class="sxs-lookup"><span data-stu-id="368d7-p112">Get the first 20 pages ordered by **createdByAppId** property and then by most recent created time. The API returns 20 entries by default.</span></span>

```
[GET] ../pages?orderby=createdByAppId,createdTime desc
```

### <a name="search--filter--top"></a><span data-ttu-id="368d7-242">search & filter & top</span><span class="sxs-lookup"><span data-stu-id="368d7-242">search & filter & top</span></span> 

<span data-ttu-id="368d7-243">*cell division* という語句を含む、2015 年 1 月 1 日以降に作成されたページで新しいものを 5 つ取得します。</span><span class="sxs-lookup"><span data-stu-id="368d7-243">Get the five newest pages created since January 1, 2015 that contain the phrase *cell division*.</span></span> <span data-ttu-id="368d7-244">既定ではこの API は 20 エントリを返します。最大では 100 エントリを返します。</span><span class="sxs-lookup"><span data-stu-id="368d7-244">The API returns 20 entries by default with a maximum of 100.</span></span> <span data-ttu-id="368d7-245">ページの既定の並べ替え順序は `lastModifiedTime desc` です (`search` は、コンシューマー ノートブックでのみ使用可能)。</span><span class="sxs-lookup"><span data-stu-id="368d7-245">The default sort order for pages is `lastModifiedTime desc` (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search="cell division"&filter=createdTime ge 2015-01-01&top=5
```

### <a name="search--filter--top--skip"></a><span data-ttu-id="368d7-246">search & filter & top & skip</span><span class="sxs-lookup"><span data-stu-id="368d7-246">search & filter & top & skip</span></span>  

<span data-ttu-id="368d7-247">結果セット内の次の 5 ページを取得します (`search` は、コンシューマー ノートブックでのみ使用可能)。</span><span class="sxs-lookup"><span data-stu-id="368d7-247">Get the next five pages in the result set (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search=biology&filter=createdTime ge 2015-01-01&top=5&skip=5
```

<br/>

<span data-ttu-id="368d7-248">それから次の 5 ページを取得します (`search` は、コンシューマー ノートブックでのみ使用可能)。</span><span class="sxs-lookup"><span data-stu-id="368d7-248">And the next five (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search=biology&filter=createdTime ge 2015-01-01&top=5&skip=10
```

> <span data-ttu-id="368d7-249">**注:** **search** と **filter** がどちらも同じ要求に適用される場合、結果には両方の条件に一致するエンティティのみが含まれます。</span><span class="sxs-lookup"><span data-stu-id="368d7-249">**Note:** If both **search** and **filter** are applied to the same request, the results include only those entities that match both criteria.</span></span>
 
### <a name="select"></a><span data-ttu-id="368d7-250">select</span><span class="sxs-lookup"><span data-stu-id="368d7-250">select</span></span>

<span data-ttu-id="368d7-251">ユーザーのノートブック内にあるすべてのセクションの名前、作成時刻、**self** リンクを取得します。</span><span class="sxs-lookup"><span data-stu-id="368d7-251">Get the name, created time, and **self** link for all sections in the user's notebooks.</span></span>

```
[GET] ../sections?select=name,createdTime,self
```

<br/>

<span data-ttu-id="368d7-252">特定のページのタイトル、作成時刻、OneNote クライアント リンクを取得します。</span><span class="sxs-lookup"><span data-stu-id="368d7-252">Get the title, created time, and OneNote client links for a specific page.</span></span>

```
[GET] ../pages/{page-id}?select=title,createdTime,links
```

### <a name="select--expand--filter-multiple-levels"></a><span data-ttu-id="368d7-253">select & expand & filter (複数レベル)</span><span class="sxs-lookup"><span data-stu-id="368d7-253">select & expand & filter (multiple levels)</span></span>  

<span data-ttu-id="368d7-254">ユーザーの既定ノートブックにあるすべてのセクションの名前と **pagesUrl** リンクを取得します。</span><span class="sxs-lookup"><span data-stu-id="368d7-254">Get the name and **pagesUrl** link for all sections in the user's default notebook.</span></span>

```
[GET] ../notebooks?select=name&expand=sections(select=name,pagesUrl)&filter=isDefault eq true
```

### <a name="top--select--orderby"></a><span data-ttu-id="368d7-255">top & select & orderby</span><span class="sxs-lookup"><span data-stu-id="368d7-255">top & select & orderby</span></span> 

<span data-ttu-id="368d7-p114">最初の 50 ページのタイトルと **self** リンクを取得します。タイトルのアルファベット順に並べられます。既定ではこの API は 20 エントリを返します。最大では 100 エントリを返します。ページの既定の並べ替え順序は `lastModifiedTime desc` です。</span><span class="sxs-lookup"><span data-stu-id="368d7-p114">Get the title and **self** link for the first 50 pages, ordered alphabetically by title. The API returns 20 entries by default with a maximum of 100. The default sort order for pages is `lastModifiedTime desc`.</span></span>

```
[GET] ../pages?top=50&select=title,self&orderby=title
```

### <a name="skip--top--select--orderby"></a><span data-ttu-id="368d7-259">skip & top & select & orderby</span><span class="sxs-lookup"><span data-stu-id="368d7-259">skip & top & select & orderby</span></span>  

<span data-ttu-id="368d7-p115">51 ページ目から 100 ページ目までを取得します。既定ではこの API は 20 エントリを返します。最大では 100 エントリを返します。</span><span class="sxs-lookup"><span data-stu-id="368d7-p115">Get pages 51 to 100. The API returns 20 entries by default with a maximum of 100.</span></span>

```
[GET] ../pages?skip=50&top=50&select=title,self&orderby=title
```

> <span data-ttu-id="368d7-262">**注:** 既定のエントリ数を取得する pages に対する GET 要求 (つまり、**top** 式を指定しない要求) は、応答で次の 20 エントリを取得するために使用できる **@odata.nextLink** リンクを戻します。</span><span class="sxs-lookup"><span data-stu-id="368d7-262">**Note:** GET requests for pages that retrieve the default number of entries (that is, they don't specify a **top** expression) return an **@odata.nextLink** link in the response that you can use to get the next 20 entries.</span></span>
 

<a name="supported-odata-query-string-options"></a>

## <a name="supported-odata-query-string-options"></a><span data-ttu-id="368d7-263">サポートされている OData クエリ文字列オプション</span><span class="sxs-lookup"><span data-stu-id="368d7-263">Supported OData query string options</span></span>

<span data-ttu-id="368d7-264">Microsoft Graph に GET 要求を送信する場合、OData クエリ文字列オプションを使用してクエリをカスタマイズして、必要な情報だけを取得できます。</span><span class="sxs-lookup"><span data-stu-id="368d7-264">When sending GET requests to Microsoft Graph, you can use OData query string options to customize your query and get just the information you need.</span></span> <span data-ttu-id="368d7-265">このオプションを使用することにより、サービスへの呼び出し回数が減り、応答ペイロードのサイズが小さくなるので、パフォーマンスも向上します。</span><span class="sxs-lookup"><span data-stu-id="368d7-265">They can also improve performance by reducing the number of calls to the service and the size of the response payload.</span></span>

> <span data-ttu-id="368d7-266">**注:** この記事の例では読みやすくするために、URL クエリ文字列内のスペースで必要な %20 パーセント エンコードを使用していません: `filter=isDefault%20eq%20true`</span><span class="sxs-lookup"><span data-stu-id="368d7-266">**Note:** For readability, the examples in this article don't use the %20 percent-encoding required for spaces in the URL query string: `filter=isDefault%20eq%20true`</span></span>
 
| <span data-ttu-id="368d7-267">クエリ オプション</span><span class="sxs-lookup"><span data-stu-id="368d7-267">Query option</span></span> | <span data-ttu-id="368d7-268">例と説明</span><span class="sxs-lookup"><span data-stu-id="368d7-268">Example and description</span></span> |  
|------|------|  
| <span data-ttu-id="368d7-269">count</span><span class="sxs-lookup"><span data-stu-id="368d7-269">count</span></span> | <p>`count=true`</p><p><span data-ttu-id="368d7-p117">コレクション内のエンティティのカウントです。この値は、応答の **@odata.count** プロパティで戻ります。</span><span class="sxs-lookup"><span data-stu-id="368d7-p117">The count of entities in the collection. The value is returned in the **@odata.count** property in the response.</span></span></p> |  
| <span data-ttu-id="368d7-272">expand</span><span class="sxs-lookup"><span data-stu-id="368d7-272">expand</span></span> | <p>`expand=sections,sectionGroups`</p><p><span data-ttu-id="368d7-p118">応答でインラインを返すナビゲーション プロパティ。**expand** 式には次のプロパティがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="368d7-p118">The navigation properties to return inline in the response. The following properties are supported for **expand** expressions:</span></span><br /> <span data-ttu-id="368d7-275">- ページ: **parentNotebook**、**parentSection**</span><span class="sxs-lookup"><span data-stu-id="368d7-275">- Pages: **parentNotebook**, **parentSection**</span></span><br /> <span data-ttu-id="368d7-276">- セクション: **parentNotebook**、**parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="368d7-276">- Sections: **parentNotebook**, **parentSectionGroup**</span></span><br /> <span data-ttu-id="368d7-277">- セクション グループ: **sections**、**sectionGroups**、**parentNotebook**、**parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="368d7-277">- Section groups: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**</span></span><br /> <span data-ttu-id="368d7-278">- ノートブック: **sections**、**sectionGroups**</span><span class="sxs-lookup"><span data-stu-id="368d7-278">- Notebooks: **sections**, **sectionGroups**</span></span></p><p><span data-ttu-id="368d7-p119">既定では、ページの GET 要求は **parentSection** を展開し、セクションの **id**、**name**、**self** の各プロパティを選択します。セクションとセクションのグループの既定の GET 要求は **parentNotebook** と **parentSectionGroup** の両方を展開し、親の **id**、**name**、**self** の各プロパティを選択します。</span><span class="sxs-lookup"><span data-stu-id="368d7-p119">By default, GET requests for pages expands **parentSection** and select the section's **id**, **name**, and **self** properties. Default GET requests for sections and section groups expand both **parentNotebook** and **parentSectionGroup**, and select the parents' **id**, **name**, and **self** properties. </span></span></p><p><span data-ttu-id="368d7-281">1 つのエンティティまたはコレクションに使用できます。</span><span class="sxs-lookup"><span data-stu-id="368d7-281">Can be used for a single entity or a collection.</span></span><br /><span data-ttu-id="368d7-282">コンマを使用して複数のプロパティを区切ります。</span><span class="sxs-lookup"><span data-stu-id="368d7-282">Separate multiple properties with commas.</span></span><br /><span data-ttu-id="368d7-283">プロパティ名では、大文字と小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="368d7-283">Property names are case-sensitive.</span></span></p> |   
| <span data-ttu-id="368d7-284">filter</span><span class="sxs-lookup"><span data-stu-id="368d7-284">filter</span></span> | <p>`filter=isDefault eq true`</p><p><span data-ttu-id="368d7-p120">結果セットの入力に含めるかどうかを決めるブール式。サポートされている OData 演算子と関数:</span><span class="sxs-lookup"><span data-stu-id="368d7-p120">A Boolean expression for whether to include an entry in the result set. Supports the following OData operators and functions:</span></span><br /> <span data-ttu-id="368d7-287">- 比較演算子: **eq**、**ne**、**gt**、**ge**、**lt**、**le**</span><span class="sxs-lookup"><span data-stu-id="368d7-287">- Comparison operators: **eq**, **ne**, **gt**, **ge**, **lt**, **le**</span></span><br /> <span data-ttu-id="368d7-288">- 論理演算子: **and**、**or**、**not**</span><span class="sxs-lookup"><span data-stu-id="368d7-288">- Logical operators: **and**, **or**, **not**</span></span><br /> <span data-ttu-id="368d7-289">- 文字列関数: **contains**、**endswith**、**startswith**、**length**、**indexof**、**substring**、**tolower**、**toupper**、**trim**、**concat**</span><span class="sxs-lookup"><span data-stu-id="368d7-289">- String functions: **contains**, **endswith**, **startswith**, **length**, **indexof**, **substring**, **tolower**, **toupper**, **trim**, **concat**</span></span></p><p><span data-ttu-id="368d7-290">[プロパティ](#onenote-entity-properties)名と OData 文字列比較では大文字と小文字が区別されます。</span><span class="sxs-lookup"><span data-stu-id="368d7-290">[Property](#onenote-entity-properties) names and OData string comparisons are case-sensitive.</span></span> <span data-ttu-id="368d7-291">文字列比較には OData **tolower** 関数を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="368d7-291">We recommend using the OData **tolower** function for string comparisons.</span></span><br /><br /><span data-ttu-id="368d7-292">**例**: `filter=tolower(name) eq 'spring'`</span><span class="sxs-lookup"><span data-stu-id="368d7-292">**Example**: `filter=tolower(name) eq 'spring'`</span></span></p> |  
| <span data-ttu-id="368d7-293">orderby</span><span class="sxs-lookup"><span data-stu-id="368d7-293">orderby</span></span> | <p>`orderby=title,createdTime desc`</p><p><span data-ttu-id="368d7-p122">並べ替え基準を示す[プロパティ](#onenote-entity-properties)です。オプションで、**asc** (既定) または **desc** 並べ替え順序を指定します。要求対象コレクション内のエンティティの任意のプロパティで並べ替えが可能です。</span><span class="sxs-lookup"><span data-stu-id="368d7-p122">The [properties](#onenote-entity-properties) to sort by, with an optional **asc** (default) or **desc** sort order. You can sort by any property of the entity in the requested collection.</span></span></p><p><span data-ttu-id="368d7-296">ノートブック、セクション グループ、セクションの既定の並べ替え順序は `name asc` で、ページの場合には `lastModifiedTime desc` (最新の変更ページが先頭になります)。</span><span class="sxs-lookup"><span data-stu-id="368d7-296">The default sort order for notebooks, section groups, and sections is `name asc`, and for pages is `lastModifiedTime desc` (last modified page first).</span></span></p><p><span data-ttu-id="368d7-297">複数のプロパティはコンマで区切り、任意の順序で一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="368d7-297">Separate multiple properties with commas, and list them in the order that you want them applied.</span></span> <span data-ttu-id="368d7-298">プロパティ名では、大文字と小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="368d7-298">Property names are case-sensitive.</span></span></p> |  
| <span data-ttu-id="368d7-299">search</span><span class="sxs-lookup"><span data-stu-id="368d7-299">search</span></span> | <p>`search=cell div`</p><p><span data-ttu-id="368d7-300">コンシューマー ノートパソコンでのみ使用可能。</span><span class="sxs-lookup"><span data-stu-id="368d7-300">Available for consumer notebooks only.</span></span></p><p><span data-ttu-id="368d7-p124">ページ タイトル、ページ本文、画像の代替テキスト、画像の OCR テキストで検索する用語または語句です。既定では、検索クエリは関連度で並べ替えて結果を返します。</span><span class="sxs-lookup"><span data-stu-id="368d7-p124">The term or phrase to search for in the page title, page body, image alt text, and image OCR text. By default, search queries return results sorted by relevance.</span></span></p><p><span data-ttu-id="368d7-303">OneNote は、Bing のフルテキスト検索を使用して、語句の検索、語形変化、スペルの曖昧さ、関連性とランキング、単語分割、複数の言語、他のフルテキスト検索機能をサポートします。</span><span class="sxs-lookup"><span data-stu-id="368d7-303">OneNote uses Bing full-text search to support phrase search, stemming, spelling forgiveness, relevance and ranking, word breaking, multiple languages, and other full-text search features.</span></span> <span data-ttu-id="368d7-304">検索文字列では、大文字と小文字が区別されません。</span><span class="sxs-lookup"><span data-stu-id="368d7-304">Search strings are case-insensitive.</span></span></p><p><span data-ttu-id="368d7-305">ユーザーが所有しているノートブック内のページにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="368d7-305">Applies only to pages in notebooks owned by the user.</span></span> <span data-ttu-id="368d7-306">インデックス付けされたコンテンツは非公開であり、所有者のみがアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="368d7-306">Indexed content is private and can only be accessed by the owner.</span></span> <span data-ttu-id="368d7-307">パスワードで保護されたページにはインデックスは付けられません。</span><span class="sxs-lookup"><span data-stu-id="368d7-307">Password-protected pages are not indexed.</span></span> <span data-ttu-id="368d7-308">`pages` エンドポイントにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="368d7-308">Applies only to the `pages` endpoint.</span></span></p> |  
| <span data-ttu-id="368d7-309">select</span><span class="sxs-lookup"><span data-stu-id="368d7-309">select</span></span> | <p>`select=id,title`</p><p><span data-ttu-id="368d7-310">返す[プロパティ](#onenote-entity-properties)。</span><span class="sxs-lookup"><span data-stu-id="368d7-310">The [properties](#onenote-entity-properties) to return.</span></span> <span data-ttu-id="368d7-311">1 つのエンティティまたはコレクションに使用できます。</span><span class="sxs-lookup"><span data-stu-id="368d7-311">Can be used for a single entity or for a collection.</span></span> <span data-ttu-id="368d7-312">コンマを使用して複数のプロパティを区切ります。</span><span class="sxs-lookup"><span data-stu-id="368d7-312">Separate multiple properties with commas.</span></span> <span data-ttu-id="368d7-313">プロパティ名では、大文字と小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="368d7-313">Property names are case-sensitive.</span></span></p> |  
| <span data-ttu-id="368d7-314">skip</span><span class="sxs-lookup"><span data-stu-id="368d7-314">skip</span></span> | <p>`skip=10`</p><p><span data-ttu-id="368d7-p128">結果セットでスキップするエントリの数。通常、結果のページングに使用されます。</span><span class="sxs-lookup"><span data-stu-id="368d7-p128">The number of entries to skip in the result set. Typically used for paging results.</span></span></p> |  
| <span data-ttu-id="368d7-317">top</span><span class="sxs-lookup"><span data-stu-id="368d7-317">top</span></span> | <p>`top=50`</p><p><span data-ttu-id="368d7-p129">結果セット内で返すエントリ数で、最大数は 100 です。既定値は 20 です。</span><span class="sxs-lookup"><span data-stu-id="368d7-p129">The number of entries to return in the result set, up to a maximum of 100. The default value is 20.</span></span></p> |  

<span data-ttu-id="368d7-320">Microsoft Graph にも、親セクション内でページのレベルと順序を取得する `pagelevel` クエリ文字列オプションが用意されています。</span><span class="sxs-lookup"><span data-stu-id="368d7-320">Microsoft Graph also provides the `pagelevel` query string option you can use to get the level and order of pages within the parent section.</span></span> <span data-ttu-id="368d7-321">特定のセクションのページのクエリ、または特定のページのクエリにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="368d7-321">Applies only to queries for pages in a specific section or queries for a specific page.</span></span> 

#### <a name="examples"></a><span data-ttu-id="368d7-322">例</span><span class="sxs-lookup"><span data-stu-id="368d7-322">Examples</span></span> 

- `GET ../sections/{section-id}/pages?pagelevel=true` 
- `GET ../pages/{page-id}?pagelevel=true` 

### <a name="supported-odata-operators-and-functions"></a><span data-ttu-id="368d7-323">サポートされている OData 演算子と関数</span><span class="sxs-lookup"><span data-stu-id="368d7-323">Supported OData operators and functions</span></span>

<span data-ttu-id="368d7-324">Microsoft Graph は、**フィルター**式で次の OData 演算子および関数をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="368d7-324">Microsoft Graph supports the following OData operators and functions in **filter** expressions.</span></span> <span data-ttu-id="368d7-325">OData 式を使用する場合には、次の点に注意してください。</span><span class="sxs-lookup"><span data-stu-id="368d7-325">When using OData expressions, remember:</span></span>

- <span data-ttu-id="368d7-326">URL クエリ文字列のスペースは `%20` エンコードで置換する必要があります。</span><span class="sxs-lookup"><span data-stu-id="368d7-326">Spaces in the URL query string must be replaced with the `%20` encoding.</span></span><br/><br/><span data-ttu-id="368d7-327">**例:** `filter=isDefault%20eq%20true`</span><span class="sxs-lookup"><span data-stu-id="368d7-327">**Example:** `filter=isDefault%20eq%20true`</span></span>

- <span data-ttu-id="368d7-328">プロパティ名と OData 文字列比較では大文字と小文字が区別されます。</span><span class="sxs-lookup"><span data-stu-id="368d7-328">Property names and OData string comparisons are case-sensitive.</span></span> <span data-ttu-id="368d7-329">文字列比較には OData **tolower** 関数を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="368d7-329">We recommend using the OData **tolower** function for string comparisons.</span></span><br/><br/><span data-ttu-id="368d7-330">**例:** `filter=tolower(name) eq 'spring'`</span><span class="sxs-lookup"><span data-stu-id="368d7-330">**Example:** `filter=tolower(name) eq 'spring'`</span></span>


| <span data-ttu-id="368d7-331">比較演算子</span><span class="sxs-lookup"><span data-stu-id="368d7-331">Comparison operator</span></span> | <span data-ttu-id="368d7-332">例</span><span class="sxs-lookup"><span data-stu-id="368d7-332">Example</span></span> |  
|------|------|  
| <span data-ttu-id="368d7-333">eq</span><span class="sxs-lookup"><span data-stu-id="368d7-333">eq</span></span><br /><span data-ttu-id="368d7-334">(等しい)</span><span class="sxs-lookup"><span data-stu-id="368d7-334">(equal to)</span></span> | `createdByAppId eq '{app-id}'` |  
| <span data-ttu-id="368d7-335">ne</span><span class="sxs-lookup"><span data-stu-id="368d7-335">ne</span></span><br /><span data-ttu-id="368d7-336">(等しくない)</span><span class="sxs-lookup"><span data-stu-id="368d7-336">(not equal to)</span></span> | `userRole ne 'Owner'` |  
| <span data-ttu-id="368d7-337">gt</span><span class="sxs-lookup"><span data-stu-id="368d7-337">gt</span></span><br /><span data-ttu-id="368d7-338">(より大きい)</span><span class="sxs-lookup"><span data-stu-id="368d7-338">(greater than)</span></span> | `createdTime gt 2014-02-23` |  
| <span data-ttu-id="368d7-339">ge</span><span class="sxs-lookup"><span data-stu-id="368d7-339">ge</span></span><br /><span data-ttu-id="368d7-340">(以上)</span><span class="sxs-lookup"><span data-stu-id="368d7-340">(greater than or equal to)</span></span> | `lastModifiedTime ge 2014-05-05T07:00:00Z` |  
| <span data-ttu-id="368d7-341">lt</span><span class="sxs-lookup"><span data-stu-id="368d7-341">lt</span></span><br /><span data-ttu-id="368d7-342">(より小さい)</span><span class="sxs-lookup"><span data-stu-id="368d7-342">(less than)</span></span> | `createdTime lt 2014-02-23` |  
| <span data-ttu-id="368d7-343">le</span><span class="sxs-lookup"><span data-stu-id="368d7-343">le</span></span><br /><span data-ttu-id="368d7-344">(以下)</span><span class="sxs-lookup"><span data-stu-id="368d7-344">(less than or equal to)</span></span> | `lastModifiedTime le 2014-02-23` |  

<br/>

| <span data-ttu-id="368d7-345">論理演算子</span><span class="sxs-lookup"><span data-stu-id="368d7-345">Logical operator</span></span> | <span data-ttu-id="368d7-346">例</span><span class="sxs-lookup"><span data-stu-id="368d7-346">Example</span></span> |  
|------|------|  
| <span data-ttu-id="368d7-347">and</span><span class="sxs-lookup"><span data-stu-id="368d7-347">and</span></span> | `createdTime le 2014-01-30 and createdTime gt 2014-01-23` |  
| <span data-ttu-id="368d7-348">or</span><span class="sxs-lookup"><span data-stu-id="368d7-348">or</span></span> | `createdByAppId eq '{app-id}' or createdByAppId eq '{app-id}'` |  
| <span data-ttu-id="368d7-349">not</span><span class="sxs-lookup"><span data-stu-id="368d7-349">not</span></span> | `not contains(tolower(title),'school')` |  

<br/>
  
| <span data-ttu-id="368d7-350">String 関数</span><span class="sxs-lookup"><span data-stu-id="368d7-350">String function</span></span> | <span data-ttu-id="368d7-351">例</span><span class="sxs-lookup"><span data-stu-id="368d7-351">Example</span></span> |  
|------|------|   
| <span data-ttu-id="368d7-352">contains</span><span class="sxs-lookup"><span data-stu-id="368d7-352">contains</span></span> | `contains(tolower(title),'spring')` |  
| <span data-ttu-id="368d7-353">endswith</span><span class="sxs-lookup"><span data-stu-id="368d7-353">endswith</span></span> | `endswith(tolower(title),'spring')` |  
| <span data-ttu-id="368d7-354">startswith</span><span class="sxs-lookup"><span data-stu-id="368d7-354">startswith</span></span> | `startswith(tolower(title),'spring')` |  
| <span data-ttu-id="368d7-355">length</span><span class="sxs-lookup"><span data-stu-id="368d7-355">length</span></span> | `length(title) eq 19` |  
| <span data-ttu-id="368d7-356">indexof</span><span class="sxs-lookup"><span data-stu-id="368d7-356">indexof</span></span> | `indexof(tolower(title),'spring') eq 1` |  
| <span data-ttu-id="368d7-357">substring</span><span class="sxs-lookup"><span data-stu-id="368d7-357">substring</span></span> | `substring(tolower(title),1) eq 'spring'` |  
| <span data-ttu-id="368d7-358">tolower</span><span class="sxs-lookup"><span data-stu-id="368d7-358">tolower</span></span> | `tolower(title) eq 'spring'` |  
| <span data-ttu-id="368d7-359">toupper</span><span class="sxs-lookup"><span data-stu-id="368d7-359">toupper</span></span> | `toupper(title) eq 'SPRING'` |  
| <span data-ttu-id="368d7-360">trim</span><span class="sxs-lookup"><span data-stu-id="368d7-360">trim</span></span> | `trim(tolower(title)) eq 'spring'` |  
| <span data-ttu-id="368d7-361">concat</span><span class="sxs-lookup"><span data-stu-id="368d7-361">concat</span></span> | `concat(title,'- by MyRecipesApp') eq 'Carrot Cake Recipe - by MyRecipesApp'` |  
 

<a name="properties"></a>

## <a name="onenote-entity-properties"></a><span data-ttu-id="368d7-362">OneNote エンティティのプロパティ</span><span class="sxs-lookup"><span data-stu-id="368d7-362">OneNote entity properties</span></span>

<span data-ttu-id="368d7-363">**filter**、**select**、**expand**、および **orderby** クエリ式には、OneNote エンティティのプロパティを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="368d7-363">The **filter**, **select**, **expand**, and **orderby** query expressions can include properties of OneNote entities.</span></span> 

#### <a name="example"></a><span data-ttu-id="368d7-364">例</span><span class="sxs-lookup"><span data-stu-id="368d7-364">Example</span></span>

`../sections?filter=createdTime ge 2015-01-01&select=name,pagesUrl&orderby=lastModifiedTime desc` 

<span data-ttu-id="368d7-365">クエリ式のプロパティ名は大文字小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="368d7-365">Property names are case-sensitive in query expressions.</span></span>

<span data-ttu-id="368d7-366">プロパティとプロパティの種類の一覧については、Microsoft Graph API REST リファレンスの中の次のリソースを参照してください。</span><span class="sxs-lookup"><span data-stu-id="368d7-366">For the list of properties and property types, see the following resources in the Microsoft Graph API REST reference:</span></span>

- [<span data-ttu-id="368d7-367">ページを取得する</span><span class="sxs-lookup"><span data-stu-id="368d7-367">GET Pages</span></span>](/graph/api/page-get?view=graph-rest-1.0)
- [<span data-ttu-id="368d7-368">Get section</span><span class="sxs-lookup"><span data-stu-id="368d7-368">GET Sections</span></span>](/graph/api/section-get?view=graph-rest-1.0)
- [<span data-ttu-id="368d7-369">Get sectionGroup</span><span class="sxs-lookup"><span data-stu-id="368d7-369">GET SectionGroups</span></span>](/graph/api/sectiongroup-get?view=graph-rest-1.0)
- [<span data-ttu-id="368d7-370">ノートブックを取得する</span><span class="sxs-lookup"><span data-stu-id="368d7-370">GET Notebooks</span></span>](/graph/api/notebook-get?view=graph-rest-1.0) 



<span data-ttu-id="368d7-371">**expand** クエリ文字列オプションは、以下のナビゲーション プロパティとともに使用できます。</span><span class="sxs-lookup"><span data-stu-id="368d7-371">The **expand** query string option can be used with the following navigation properties:</span></span>

- <span data-ttu-id="368d7-372">ページ: **parentNotebook**、**parentSection**</span><span class="sxs-lookup"><span data-stu-id="368d7-372">Pages: **parentNotebook**, **parentSection**</span></span>
- <span data-ttu-id="368d7-373">セクション: **parentNotebook**、**parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="368d7-373">Sections: **parentNotebook**, **parentSectionGroup**</span></span>
- <span data-ttu-id="368d7-374">セクション グループ: **sections**、**sectionGroups**、**parentNotebook**、**parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="368d7-374">Section groups: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**</span></span>
- <span data-ttu-id="368d7-375">ノートブック: **sections**、**sectionGroups**</span><span class="sxs-lookup"><span data-stu-id="368d7-375">Notebooks: **sections**, **sectionGroups**</span></span>


<a name="request-response-info"></a>

## <a name="request-and-response-information-for-get-requests"></a><span data-ttu-id="368d7-376">要求および *GET* 要求の応答に関する情報</span><span class="sxs-lookup"><span data-stu-id="368d7-376">Request and response information for *GET* requests</span></span>

| <span data-ttu-id="368d7-377">要求データ</span><span class="sxs-lookup"><span data-stu-id="368d7-377">Request data</span></span> | <span data-ttu-id="368d7-378">説明</span><span class="sxs-lookup"><span data-stu-id="368d7-378">Description</span></span> |  
|------|------|  
| <span data-ttu-id="368d7-379">プロトコル</span><span class="sxs-lookup"><span data-stu-id="368d7-379">Protocol</span></span> | <span data-ttu-id="368d7-380">すべての要求は SSL/TLS HTTPS プロトコルを使用します。</span><span class="sxs-lookup"><span data-stu-id="368d7-380">All requests use the SSL/TLS HTTPS protocol.</span></span> |  
| <span data-ttu-id="368d7-381">承認ヘッダー</span><span class="sxs-lookup"><span data-stu-id="368d7-381">Authorization header</span></span> | <p><span data-ttu-id="368d7-382">`Bearer {token}`。`{token}` は、登録済みアプリの有効な OAuth 2.0 アクセス トークンです。</span><span class="sxs-lookup"><span data-stu-id="368d7-382">`Bearer {token}`, where `{token}` is a valid OAuth 2.0 access token for your registered app.</span></span></p><p><span data-ttu-id="368d7-p133">これがないか、無効の場合、401 ステータス コードで要求は失敗します。「[認証とアクセス許可](permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="368d7-p133">If missing or invalid, the request fails with a 401 status code. See [Authentication and permissions](permissions-reference.md).</span></span></p> |  
| <span data-ttu-id="368d7-385">Accept ヘッダー</span><span class="sxs-lookup"><span data-stu-id="368d7-385">Accept header</span></span> | <p> <span data-ttu-id="368d7-386">OneNote エンティティとエンティティ セットの場合、`application/json`</span><span class="sxs-lookup"><span data-stu-id="368d7-386">`application/json` for OneNote entities and entity sets</span></span></p><p> <span data-ttu-id="368d7-387">ページ コンテンツの場合、`text/html`</span><span class="sxs-lookup"><span data-stu-id="368d7-387">`text/html` for page content</span></span></p> | 

<br/>

| <span data-ttu-id="368d7-388">応答データ</span><span class="sxs-lookup"><span data-stu-id="368d7-388">Response data</span></span> | <span data-ttu-id="368d7-389">説明</span><span class="sxs-lookup"><span data-stu-id="368d7-389">Description</span></span> |  
|------|------|  
| <span data-ttu-id="368d7-390">成功コード</span><span class="sxs-lookup"><span data-stu-id="368d7-390">Success code</span></span> | <span data-ttu-id="368d7-391">200 HTTP ステータス コード。</span><span class="sxs-lookup"><span data-stu-id="368d7-391">A 200 HTTP status code.</span></span> |  
| <span data-ttu-id="368d7-392">応答本文</span><span class="sxs-lookup"><span data-stu-id="368d7-392">Response body</span></span> | <span data-ttu-id="368d7-393">JSON 形式のエンティティまたはエンティティ セット、ページ HTML、またはファイル リソースのバイナリ データの OData 表現。</span><span class="sxs-lookup"><span data-stu-id="368d7-393">An OData representation of the entity or entity set in JSON format, the page HTML, or file resource binary data.</span></span>  |  
| <span data-ttu-id="368d7-394">エラー</span><span class="sxs-lookup"><span data-stu-id="368d7-394">Errors</span></span> | <span data-ttu-id="368d7-395">要求が失敗すると、API は応答本文の **@api.diagnostics** オブジェクトに[エラー](onenote-error-codes.md)を返します。</span><span class="sxs-lookup"><span data-stu-id="368d7-395">If the request fails, the API returns [errors](onenote-error-codes.md) in the **@api.diagnostics** object in the response body.</span></span> |  
| <span data-ttu-id="368d7-396">X-CorrelationId ヘッダー</span><span class="sxs-lookup"><span data-stu-id="368d7-396">X-CorrelationId header</span></span> | <span data-ttu-id="368d7-p134">要求を一意に識別する GUID。Microsoft サポートと問題のトラブルシューティングを行う際に、この値を Date ヘッダーの値とともに使用できます。</span><span class="sxs-lookup"><span data-stu-id="368d7-p134">A GUID that uniquely identifies the request. You can use this value along with the value of the Date header when working with Microsoft support to troubleshoot issues.</span></span> |  


<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-notes-service-root-url"></a><span data-ttu-id="368d7-399">Microsoft Graph のノート サービスのルート URL の構築</span><span class="sxs-lookup"><span data-stu-id="368d7-399">Constructing the Microsoft Graph notes service root URL</span></span>

<span data-ttu-id="368d7-400">Microsoft Graph ノートのルート URL は、Microsoft Graph ノートへのすべての呼び出しで次の形式を使用します。</span><span class="sxs-lookup"><span data-stu-id="368d7-400">The Microsoft Graph notes root URL uses the following format for all calls to Microsoft Graph notes:</span></span>

`https://graph.microsoft.com/{version}/me/onenote/`  

<span data-ttu-id="368d7-401">URL の `version` セグメントは、使用する Microsoft Graph のバージョンを示しています。</span><span class="sxs-lookup"><span data-stu-id="368d7-401">The `version` segment in the URL represents the version of Microsoft Graph that you want to use.</span></span> <span data-ttu-id="368d7-402">安定した運用コードには `v1.0` を使用します。</span><span class="sxs-lookup"><span data-stu-id="368d7-402">Use `v1.0` for stable production code.</span></span> <span data-ttu-id="368d7-403">開発中の機能を試すには `beta` を使用します。</span><span class="sxs-lookup"><span data-stu-id="368d7-403">Use `beta` to try out a feature that's in development.</span></span> <span data-ttu-id="368d7-404">ベータ版の機能は変更される可能性があるため、運用コードでは使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="368d7-404">Features and functionality in beta may change, so you shouldn't use it in your production code.</span></span> 

<span data-ttu-id="368d7-405">現在のユーザーがアクセスできる OneNote コンテンツには `me` を使用します (所有と共有)。</span><span class="sxs-lookup"><span data-stu-id="368d7-405">Use `me` for OneNote content that the current user can access (owned and shared).</span></span> <span data-ttu-id="368d7-406">指定されたユーザー (URL 内) が現在のユーザーと共有している OneNote コンテンツには `users/{id}` を使用します。</span><span class="sxs-lookup"><span data-stu-id="368d7-406">Use `users/{id}` for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="368d7-407">ユーザー ID を取得するには [Microsoft Graph](https://graph.microsoft.com/v1.0/users) を使用します。</span><span class="sxs-lookup"><span data-stu-id="368d7-407">Use [Microsoft Graph](https://graph.microsoft.com/v1.0/users) to get user IDs.</span></span> 


<a name="permissions"></a>

## <a name="permissions-for-get-requests"></a><span data-ttu-id="368d7-408">GET 要求のアクセス許可</span><span class="sxs-lookup"><span data-stu-id="368d7-408">Permissions for GET requests</span></span>

<span data-ttu-id="368d7-409">OneNote のコンテンツまたは構造を取得するには、適切なアクセス許可を要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="368d7-409">To get OneNote content or structure, you'll need to request appropriate permissions.</span></span> 

<span data-ttu-id="368d7-410">次のスコープは、Microsoft Graph に対する GET 要求を許可します。</span><span class="sxs-lookup"><span data-stu-id="368d7-410">The following scopes allow GET requests to Microsoft Graph.</span></span> <span data-ttu-id="368d7-411">アプリの動作に必要な最低限のアクセス許可を選択してください。</span><span class="sxs-lookup"><span data-stu-id="368d7-411">Choose the lowest level of permissions that your app needs to do its work.</span></span>

<span data-ttu-id="368d7-412">次から選択します。</span><span class="sxs-lookup"><span data-stu-id="368d7-412">Choose from:</span></span>

- <span data-ttu-id="368d7-413">Notes.read</span><span class="sxs-lookup"><span data-stu-id="368d7-413">Notes.read</span></span>
- <span data-ttu-id="368d7-414">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="368d7-414">Notes.ReadWrite</span></span>
- <span data-ttu-id="368d7-415">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="368d7-415">Notes.ReadWrite.All</span></span>

<span data-ttu-id="368d7-416">アクセス許可の範囲とその動作方法の詳細については、「[Microsoft Graph のアクセス許可のリファレンス](permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="368d7-416">For more information about permission scopes and how they work, see [Microsoft Graph permissions reference](permissions-reference.md).</span></span>

<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="368d7-417">関連項目</span><span class="sxs-lookup"><span data-stu-id="368d7-417">See also</span></span>

- [<span data-ttu-id="368d7-418">OneNote ページの入出力 HTML</span><span class="sxs-lookup"><span data-stu-id="368d7-418">Input and output HTML for OneNote pages</span></span>](onenote-input-output-html.md)
- [<span data-ttu-id="368d7-419">OneNote との統合</span><span class="sxs-lookup"><span data-stu-id="368d7-419">Integrate with OneNote</span></span>](integrate-with-onenote.md)
- [<span data-ttu-id="368d7-420">OneNote の開発者ブログ</span><span class="sxs-lookup"><span data-stu-id="368d7-420">OneNote Developer Blog</span></span>](https://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="368d7-421">Stack Overflow 掲載の OneNote の開発に関する質問</span><span class="sxs-lookup"><span data-stu-id="368d7-421">OneNote development questions on Stack Overflow</span></span>](https://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="368d7-422">OneNote GitHub のリポジトリ</span><span class="sxs-lookup"><span data-stu-id="368d7-422">OneNote GitHub repos</span></span>](https://go.microsoft.com/fwlink/?LinkID=390178)  
