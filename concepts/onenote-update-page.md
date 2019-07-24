---
title: OneNote ページ コンテンツを更新する
description: " Office 365 のエンタープライズ ノートブック"
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 939875ce060abeb4a76d33bea68b3e3bbb49a203
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840762"
---
# <a name="update-onenote-page-content"></a><span data-ttu-id="a2041-103">OneNote ページ コンテンツを更新する</span><span class="sxs-lookup"><span data-stu-id="a2041-103">Update OneNote page content</span></span>

<span data-ttu-id="a2041-104">**適用対象** OneDrive のコンシューマー ノートブック | Office 365 のエンタープライズ ノートブック</span><span class="sxs-lookup"><span data-stu-id="a2041-104">**Applies to** Consumer notebooks on OneDrive | Enterprise notebooks on Office 365</span></span>


<span data-ttu-id="a2041-105">OneNote ページのコンテンツを更新する場合は、ページの *content* エンドポイントに PATCH 要求を送信します。</span><span class="sxs-lookup"><span data-stu-id="a2041-105">To update the content of a OneNote page, you send a PATCH request to the page's *content* endpoint:</span></span>

`PATCH ../notes/pages/{id}/content`</p>

<span data-ttu-id="a2041-p101">メッセージの本文で JSON 変更オブジェクトを送信します。要求が成功すると、Microsoft Graph は 204 HTTP 状態コードを返します。</span><span class="sxs-lookup"><span data-stu-id="a2041-p101">Send a JSON change object in the message body. If the request is successful, Microsoft Graph returns a 204 HTTP status code.</span></span>


<a name="request-uri"></a>

## <a name="construct-the-request-uri"></a><span data-ttu-id="a2041-108">要求 URI の構築</span><span class="sxs-lookup"><span data-stu-id="a2041-108">Construct the request URI</span></span>

<span data-ttu-id="a2041-109">要求 URI を構築するには、サービス ルート URL から開始します。</span><span class="sxs-lookup"><span data-stu-id="a2041-109">To construct the request URI, start with the service root URL:</span></span>

`https://graph.microsoft.com/v1.0/me/onenote`

<br/>

<span data-ttu-id="a2041-110">次に、ページの *content* エンドポイントを追加します。</span><span class="sxs-lookup"><span data-stu-id="a2041-110">Then append the page's *content* endpoint:</span></span>

- <span data-ttu-id="a2041-111">**ページ HTML と、すべての定義済み *data-id* の値を取得する**</span><span class="sxs-lookup"><span data-stu-id="a2041-111">**Get the page HTML and all defined *data-id* values**</span></span><br/><br/>`../pages/{id}/content`   

- <span data-ttu-id="a2041-112">**ページ HTML、すべての定義済み *data-id* の値、およびすべての生成された *id* の値を取得する**</span><span class="sxs-lookup"><span data-stu-id="a2041-112">**Get the page HTML, all defined *data-id* values, and all generated *id* values**</span></span><br/><br/>`../pages/{page-id}/content?includeIDs=true` 

<span data-ttu-id="a2041-113">**data-id** と **id** の値は、更新する要素の **target** 識別子として使用されます。</span><span class="sxs-lookup"><span data-stu-id="a2041-113">The **data-id** and **id** values are used as **target** identifiers for the elements you want to update.</span></span>

 
<span data-ttu-id="a2041-114">完全な要求 URI は、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="a2041-114">Your full request URI will look like this:</span></span><br/><br/>`https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/content`


<span data-ttu-id="a2041-115">[サービス ルート URL](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url) の詳細についてはリンク先をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="a2041-115">Learn more about the [service root URL](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).</span></span>


<a name="message-body"></a>

## <a name="construct-the-message-body"></a><span data-ttu-id="a2041-116">メッセージ本文の構築</span><span class="sxs-lookup"><span data-stu-id="a2041-116">Construct the message body</span></span>

<span data-ttu-id="a2041-p102">OneNote ページの HTML には、**div** 要素、**img** 要素、**ol** 要素などの構造に編成されたテキスト、画像などのコンテンツが含まれています。OneNote ページのコンテンツを更新する場合は、ページ上で HTML 要素を追加および置換します。</span><span class="sxs-lookup"><span data-stu-id="a2041-p102">The HTML of a OneNote page contains text, images, and other content organized into structures such as **div**, **img**, and **ol** elements. To update OneNote page content, you add and replace HTML elements on the page.</span></span>

<span data-ttu-id="a2041-p103">変更内容は JSON 変更オブジェクトの配列としてメッセージ本文に入れて送信します。ターゲット要素、新しい HTML コンテンツ、コンテンツに対する操作が各オブジェクトにより指定されます。</span><span class="sxs-lookup"><span data-stu-id="a2041-p103">Your changes are sent in the message body as an array of JSON change objects. Each object specifies the target element, new HTML content, and what to do with the content.</span></span>

<span data-ttu-id="a2041-p104">2 つの変更を定義する配列を次に示します。最初の変更では画像が兄弟として段落の上に挿入され、2 番目の変更ではアイテムが最後の子としてリストに追加されます。</span><span class="sxs-lookup"><span data-stu-id="a2041-p104">The following array defines two changes. The first inserts an image above a paragraph as a sibling, and the second appends an item to a list as a last child.</span></span>

> [!NOTE]
> <span data-ttu-id="a2041-123">OneNote ページのイメージを更新する場合、www リンクは使用できません。</span><span class="sxs-lookup"><span data-stu-id="a2041-123">When updating an image on a OneNote page, you can't use www links.</span></span> <span data-ttu-id="a2041-124">このサービスは、ランダムなリソースのダウンロードを試行しません。</span><span class="sxs-lookup"><span data-stu-id="a2041-124">The service won't try to download random resources.</span></span> <span data-ttu-id="a2041-125">代わりに、画像が要求の一部である必要があります。イメージデータ url またはマルチパート要求のパーツ名を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a2041-125">Instead, the image must be part of the request, either by an image-data-url or a part-name of a multipart request.</span></span>

```json
[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-data-url-or-part-name" alt="Image above the target paragraph" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>Item at the end of the list</li>'
  }
]
```

<span data-ttu-id="a2041-126">[その他の例](#example-requests)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2041-126">See [more examples](#example-requests).</span></span>


### <a name="attributes-for-json-change-objects"></a><span data-ttu-id="a2041-127">JSON 変更オブジェクトの属性</span><span class="sxs-lookup"><span data-stu-id="a2041-127">Attributes for JSON change objects</span></span>

<span data-ttu-id="a2041-128">PATCH 要求の JSON オブジェクトの定義には、**target** 属性、**action** 属性、**position** 属性、および **content** 属性を使用します。</span><span class="sxs-lookup"><span data-stu-id="a2041-128">Use the **target**, **action**, **position**, and **content** attributes to define JSON objects for PATCH requests.</span></span>

#### <a name="target"></a><span data-ttu-id="a2041-129">ターゲット</span><span class="sxs-lookup"><span data-stu-id="a2041-129">target</span></span>

<span data-ttu-id="a2041-p106">更新する要素。値として次の ID のいずれかを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a2041-p106">The element to update. The value must be one of the following identifiers:</span></span>

| <span data-ttu-id="a2041-132">Identifier</span><span class="sxs-lookup"><span data-stu-id="a2041-132">Identifier</span></span> | <span data-ttu-id="a2041-133">説明</span><span class="sxs-lookup"><span data-stu-id="a2041-133">Description</span></span> |  
|------|------|  
| <span data-ttu-id="a2041-134">#{data-id}</span><span class="sxs-lookup"><span data-stu-id="a2041-134">#{data-id}</span></span> | <p><span data-ttu-id="a2041-p107">この ID は、[ページを作成](onenote-create-page.md)するときや[更新](onenote-update-page.md)するときに、入力 HTML の要素で任意で定義されます。値の先頭に # を付けます。</span><span class="sxs-lookup"><span data-stu-id="a2041-p107">This ID is optionally defined on elements in the input HTML when [creating a page](onenote-create-page.md) or [updating a page](onenote-update-page.md). Prefix the value with a #.</span></span></p><p> <span data-ttu-id="a2041-137">例:</span><span class="sxs-lookup"><span data-stu-id="a2041-137">Example:</span></span><br/><span data-ttu-id="a2041-138">`'target':'#intro'` は要素 `<div data-id="intro" ...>` をターゲットとします</span><span class="sxs-lookup"><span data-stu-id="a2041-138">`'target':'#intro'` targets the element `<div data-id="intro" ...>`</span></span></p> |  
| <span data-ttu-id="a2041-139">ID</span><span class="sxs-lookup"><span data-stu-id="a2041-139">id</span></span> | <p><span data-ttu-id="a2041-140">これは、Microsoft Graph から得られる[生成済み ID](#generated-ids) であり、ほとんどの置換操作で必要になります。</span><span class="sxs-lookup"><span data-stu-id="a2041-140">This is the [generated ID](#generated-ids) from Microsoft Graph, and is required for most replace operations.</span></span> <span data-ttu-id="a2041-141">プレフィックス # を追加しないでください。</span><span class="sxs-lookup"><span data-stu-id="a2041-141">Do not prefix with a #.</span></span></p><p> <span data-ttu-id="a2041-142">例:</span><span class="sxs-lookup"><span data-stu-id="a2041-142">Example:</span></span><br/><span data-ttu-id="a2041-143">`'target':'div:{33f8a2...}{37}'` は要素 `<div id="div:{33f8a2...}{37}" ...>` をターゲットとします</span><span class="sxs-lookup"><span data-stu-id="a2041-143">`'target':'div:{33f8a2...}{37}'` targets the element `<div id="div:{33f8a2...}{37}" ...>`</span></span></p><p><span data-ttu-id="a2041-p109">[入力 HTML](onenote-input-output-html.md) に定義されている **id** 値とこれらを混同しないでください。入力 HTML で送信される **id** 値は、すべて破棄されます。</span><span class="sxs-lookup"><span data-stu-id="a2041-p109">Don't confuse these with any **id** values defined in the [input HTML](onenote-input-output-html.md). All **id** values sent in the input HTML are discarded.</span></span></p> |  
| <span data-ttu-id="a2041-146">body</span><span class="sxs-lookup"><span data-stu-id="a2041-146">body</span></span> | <span data-ttu-id="a2041-p110">ページ上で最初の div をターゲットにするキーワード。プレフィックス # を追加してはいけません。</span><span class="sxs-lookup"><span data-stu-id="a2041-p110">The keyword that targets the first div on the page. Do not prefix with a #.</span></span> |  
| <span data-ttu-id="a2041-149">title</span><span class="sxs-lookup"><span data-stu-id="a2041-149">title</span></span> | <span data-ttu-id="a2041-p111">ページ タイトルをターゲットにするキーワード。プレフィックス # を追加してはなりません。</span><span class="sxs-lookup"><span data-stu-id="a2041-p111">The keyword that targets the page title. Do not prefix with a #.</span></span> |  
 
#### <a name="action"></a><span data-ttu-id="a2041-152">action</span><span class="sxs-lookup"><span data-stu-id="a2041-152">action</span></span>

<span data-ttu-id="a2041-p112">ターゲット要素に対して実行するアクション。「[サポートされる要素とアクション](#supported-elements-and-actions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2041-p112">The action to perform on the target element. See [supported actions for elements](#supported-elements-and-actions).</span></span>

| <span data-ttu-id="a2041-155">アクション</span><span class="sxs-lookup"><span data-stu-id="a2041-155">Action</span></span> | <span data-ttu-id="a2041-156">説明</span><span class="sxs-lookup"><span data-stu-id="a2041-156">Description</span></span> |  
|------|------|  
| <span data-ttu-id="a2041-157">append</span><span class="sxs-lookup"><span data-stu-id="a2041-157">append</span></span> | <p><span data-ttu-id="a2041-158">指定されたコンテンツを最初または最後の子としてターゲットに追加します。追加される位置 (最初または最後) は、**position** 属性によって決まります。</span><span class="sxs-lookup"><span data-stu-id="a2041-158">Adds the supplied content to the target as a first or last child, as determined by the **position** attribute.</span></span></p><p><span data-ttu-id="a2041-159">**body**、**div**、**ol**、**ul** 要素にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="a2041-159">Applies only to **body**, **div**, **ol**, and **ul** elements.</span></span></p> |  
| <span data-ttu-id="a2041-160">insert</span><span class="sxs-lookup"><span data-stu-id="a2041-160">insert</span></span> | <span data-ttu-id="a2041-161">指定されたコンテンツを兄弟としてターゲットの前または後に追加します。追加される位置 (前または後) は、**position** 属性によって決まります。</span><span class="sxs-lookup"><span data-stu-id="a2041-161">Adds the supplied content as a sibling before or after the target, as determined by the **position** attribute.</span></span> |  
| <span data-ttu-id="a2041-162">prepend</span><span class="sxs-lookup"><span data-stu-id="a2041-162">prepend</span></span> | <p><span data-ttu-id="a2041-p113">指定されたコンテンツを最初の子としてターゲットに追加します。**append** + **before** のショートカット。</span><span class="sxs-lookup"><span data-stu-id="a2041-p113">Adds the supplied content to the target as a first child. Shortcut for **append** + **before**.</span></span></p><p><span data-ttu-id="a2041-165">**body**、**div**、**ol**、**ul** 要素にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="a2041-165">Applies only to **body**, **div**, **ol**, and **ul** elements.</span></span></p> |  
| <span data-ttu-id="a2041-166">replace</span><span class="sxs-lookup"><span data-stu-id="a2041-166">replace</span></span> | <p><span data-ttu-id="a2041-167">指定したコンテンツでターゲットを置換します。</span><span class="sxs-lookup"><span data-stu-id="a2041-167">Replaces the target with the supplied content.</span></span></p><p><span data-ttu-id="a2041-168">ほとんどの **replace** アクションは、ターゲットの[生成された ID](#generated-ids) を使用する必要があります (ただし、div 内の **img** 要素と **object** 要素を除きます。これらは、**data-id** の使用もサポートしています)。</span><span class="sxs-lookup"><span data-stu-id="a2041-168">Most **replace** actions require using the [generated ID](#generated-ids) for the target (except **img** and **object** elements within a div, which also support using **data-id**).</span></span></p> |  
 
#### <a name="position"></a><span data-ttu-id="a2041-169">position</span><span class="sxs-lookup"><span data-stu-id="a2041-169">position</span></span>

<span data-ttu-id="a2041-p114">指定されたコンテンツを追加する位置。ターゲット要素を基準とした相対位置です。省略すると、既定値として **after** が使用されます。</span><span class="sxs-lookup"><span data-stu-id="a2041-p114">The location to add the supplied content, relative to the target element. Defaults to **after** if omitted.</span></span>

| <span data-ttu-id="a2041-172">位置</span><span class="sxs-lookup"><span data-stu-id="a2041-172">Position</span></span> | <span data-ttu-id="a2041-173">説明</span><span class="sxs-lookup"><span data-stu-id="a2041-173">Description</span></span> |  
|------|------|  
| <span data-ttu-id="a2041-174">after (既定値)</span><span class="sxs-lookup"><span data-stu-id="a2041-174">after (default)</span></span> |<p><span data-ttu-id="a2041-175">**append** の場合: ターゲット要素の最後の子。</span><span class="sxs-lookup"><span data-stu-id="a2041-175">With **append**: The last child of the target element.</span></span></p><p><span data-ttu-id="a2041-176">**insert** の場合: ターゲット要素の後続の兄弟。</span><span class="sxs-lookup"><span data-stu-id="a2041-176">With **insert**: The subsequent sibling of the target element.</span></span></p> |
| <span data-ttu-id="a2041-177">before</span><span class="sxs-lookup"><span data-stu-id="a2041-177">before</span></span> | <p><span data-ttu-id="a2041-178">**append** の場合: ターゲット要素の最初の子。</span><span class="sxs-lookup"><span data-stu-id="a2041-178">With **append**: The first child of the target element.</span></span></p><p><span data-ttu-id="a2041-179">**insert** の場合: ターゲット要素の先行の兄弟。</span><span class="sxs-lookup"><span data-stu-id="a2041-179">With **insert**: The preceding sibling of the target element.</span></span></p> |

#### <a name="content"></a><span data-ttu-id="a2041-180">content</span><span class="sxs-lookup"><span data-stu-id="a2041-180">content</span></span>

<span data-ttu-id="a2041-p115">ページに追加する整形式 HTML の文字列と画像またはファイル バイナリ データ。コンテンツにバイナリ データが含まれている場合、コンテンツ タイプとして `multipart/form-data` を利用し、"Commands" パートを含む要求を送信する必要があります ([例](#multipart-request-with-binary-content)参照)。</span><span class="sxs-lookup"><span data-stu-id="a2041-p115">A string of well-formed HTML to add to the page, and any image or file binary data. If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part (see an [example](#multipart-request-with-binary-content)).</span></span> 
 

<a name="generated-ids"></a>

### <a name="generated-ids"></a><span data-ttu-id="a2041-183">生成された ID</span><span class="sxs-lookup"><span data-stu-id="a2041-183">Generated IDs</span></span>
<span data-ttu-id="a2041-184">Microsoft Graph は、更新可能なページで要素に対して **id** 値を生成します。</span><span class="sxs-lookup"><span data-stu-id="a2041-184">Microsoft Graph generates **id** values for the elements on the page that can be updated.</span></span> <span data-ttu-id="a2041-185">生成された ID を取得するには、GET 要求で `includeIDs=true` クエリ文字列を使用します。</span><span class="sxs-lookup"><span data-stu-id="a2041-185">To get generated IDs, use the `includeIDs=true` query string expression in your GET request:</span></span>

`GET ../notes/pages/{page-id}/content?includeIDs=true` 

> <span data-ttu-id="a2041-186">**注:** API は、ページ作成要求およびページ更新要求の[入力 HTML](onenote-input-output-html.md) で定義された **id** の値をすべて破棄します。</span><span class="sxs-lookup"><span data-stu-id="a2041-186">**Note:** The API discards all **id** values that are defined in the [input HTML](onenote-input-output-html.md) of create-page and update-page requests.</span></span>

<span data-ttu-id="a2041-187">次の例は、ページの[出力 HTML](onenote-input-output-html.md) の段落と画像に対して生成された ID を示します。</span><span class="sxs-lookup"><span data-stu-id="a2041-187">The following example shows generated IDs for a paragraph and an image in the [output HTML](onenote-input-output-html.md) of a page.</span></span>

```html
<p id="p:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{40}">Some text on the page</p>
<img id="img:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{45}" ... />
```

<span data-ttu-id="a2041-188">生成された **id** 値はページ更新後に変更されることがあるため、これらの値を使用する PATCH 要求を作成する前に、現行値を取得する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a2041-188">Generated **id** values might change after a page update, so you should get the current values before building a PATCH request that uses them.</span></span>
 
<span data-ttu-id="a2041-189">ターゲット要素は、**data-id** または **id** 値を使用して次のように指定できます。</span><span class="sxs-lookup"><span data-stu-id="a2041-189">You can specify target elements by using the **data-id** or **id** value, as follows:</span></span>

- <span data-ttu-id="a2041-190">**append** アクションと **insert** アクションでは、いずれの ID もターゲット値として使用できます。</span><span class="sxs-lookup"><span data-stu-id="a2041-190">For **append** and **insert** actions, you can use either ID as the target value.</span></span>
- <span data-ttu-id="a2041-191">**replace** アクションでは、すべての要素について、生成された IDを使用する必要があります。ただし、ページ タイトル、および div 内の画像とオブジェクトを除きます。</span><span class="sxs-lookup"><span data-stu-id="a2041-191">For **replace** actions, you must use the generated ID for all elements except for the page title and images and objects that are within a div.</span></span> 
  - <span data-ttu-id="a2041-192">タイトルを置換する場合は、**title** キーワードを使用します。</span><span class="sxs-lookup"><span data-stu-id="a2041-192">To replace a title, use the **title** keyword.</span></span> 
  - <span data-ttu-id="a2041-193">div 内の画像とオブジェクトを置換する場合は、**data-id** または **id** のどちらかを使用します。</span><span class="sxs-lookup"><span data-stu-id="a2041-193">To replace images and objects that are within a div, use either **data-id** or **id**.</span></span>

<span data-ttu-id="a2041-p117">次の例では、ターゲットに **id** 値を使用します。生成された ID と共に # プレフィックスを使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="a2041-p117">The following example uses the **id** value for the target. Don't use the # prefix with a generated ID.</span></span>

```json
[
   {
    'target':'p:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{40}',
    'action':'insert',
    'position':'before',
    'content':'<p>This paragraph goes above the target paragraph.</p>'
  }
]
```

<a name="support-matrix"></a>

## <a name="supported-elements-and-actions"></a><span data-ttu-id="a2041-196">サポートされる要素とアクション</span><span class="sxs-lookup"><span data-stu-id="a2041-196">Supported elements and actions</span></span>

<span data-ttu-id="a2041-p118">ページ上の要素の多くは更新可能ですが、要素の種類ごとに特定のアクションがサポートされています。サポートされるターゲット要素と、各要素でサポートされる更新アクションを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="a2041-p118">Many elements on the page can be updated, but each element type supports specific actions. The following table shows supported target elements and the update actions that they support.</span></span>

| <span data-ttu-id="a2041-199">要素</span><span class="sxs-lookup"><span data-stu-id="a2041-199">Element</span></span> | <span data-ttu-id="a2041-200">置換</span><span class="sxs-lookup"><span data-stu-id="a2041-200">Replace</span></span> | <span data-ttu-id="a2041-201">子の追加</span><span class="sxs-lookup"><span data-stu-id="a2041-201">Append child</span></span> | <span data-ttu-id="a2041-202">兄弟の挿入</span><span class="sxs-lookup"><span data-stu-id="a2041-202">Insert sibling</span></span> |  
|------|:------:|:------:|:------:|  
| <span data-ttu-id="a2041-203">body</span><span class="sxs-lookup"><span data-stu-id="a2041-203">body</span></span><br /> <span data-ttu-id="a2041-204">(ページの最初の div をターゲットとする)</span><span class="sxs-lookup"><span data-stu-id="a2041-204">(targets first div on the page)</span></span> | <span data-ttu-id="a2041-205">いいえ</span><span class="sxs-lookup"><span data-stu-id="a2041-205">no</span></span> | <span data-ttu-id="a2041-206">**はい**</span><span class="sxs-lookup"><span data-stu-id="a2041-206">**yes**</span></span> | <span data-ttu-id="a2041-207">いいえ</span><span class="sxs-lookup"><span data-stu-id="a2041-207">no</span></span> |  
| <span data-ttu-id="a2041-208">div</span><span class="sxs-lookup"><span data-stu-id="a2041-208">div</span></span><br /> <span data-ttu-id="a2041-209">([絶対配置](onenote-abs-pos.md))</span><span class="sxs-lookup"><span data-stu-id="a2041-209">([absolute positioned](onenote-abs-pos.md))</span></span> | <span data-ttu-id="a2041-210">いいえ</span><span class="sxs-lookup"><span data-stu-id="a2041-210">no</span></span> | <span data-ttu-id="a2041-211">**はい**</span><span class="sxs-lookup"><span data-stu-id="a2041-211">**yes**</span></span> | <span data-ttu-id="a2041-212">いいえ</span><span class="sxs-lookup"><span data-stu-id="a2041-212">no</span></span> |  
| <span data-ttu-id="a2041-213">div</span><span class="sxs-lookup"><span data-stu-id="a2041-213">div</span></span><br /> <span data-ttu-id="a2041-214">(div 内)</span><span class="sxs-lookup"><span data-stu-id="a2041-214">(within a div)</span></span> | <span data-ttu-id="a2041-215">**はい**</span><span class="sxs-lookup"><span data-stu-id="a2041-215">**yes**</span></span><br/><span data-ttu-id="a2041-216">(id のみ)</span><span class="sxs-lookup"><span data-stu-id="a2041-216">(id only)</span></span> | <span data-ttu-id="a2041-217">**はい**</span><span class="sxs-lookup"><span data-stu-id="a2041-217">**yes**</span></span> | <span data-ttu-id="a2041-218">**はい**</span><span class="sxs-lookup"><span data-stu-id="a2041-218">**yes**</span></span> |   
| <span data-ttu-id="a2041-219">img、object</span><span class="sxs-lookup"><span data-stu-id="a2041-219">img, object</span></span><br /> <span data-ttu-id="a2041-220">(div 内)</span><span class="sxs-lookup"><span data-stu-id="a2041-220">(within a div)</span></span> | <span data-ttu-id="a2041-221">**はい**</span><span class="sxs-lookup"><span data-stu-id="a2041-221">**yes**</span></span> | <span data-ttu-id="a2041-222">no</span><span class="sxs-lookup"><span data-stu-id="a2041-222">no</span></span> | <span data-ttu-id="a2041-223">**はい**</span><span class="sxs-lookup"><span data-stu-id="a2041-223">**yes**</span></span> |   
| <span data-ttu-id="a2041-224">ol、ul</span><span class="sxs-lookup"><span data-stu-id="a2041-224">ol, ul</span></span> | <span data-ttu-id="a2041-225">**はい**</span><span class="sxs-lookup"><span data-stu-id="a2041-225">**yes**</span></span><br/><span data-ttu-id="a2041-226">(id のみ)</span><span class="sxs-lookup"><span data-stu-id="a2041-226">(id only)</span></span> | <span data-ttu-id="a2041-227">**はい**</span><span class="sxs-lookup"><span data-stu-id="a2041-227">**yes**</span></span> | <span data-ttu-id="a2041-228">**はい**</span><span class="sxs-lookup"><span data-stu-id="a2041-228">**yes**</span></span> |   
| <span data-ttu-id="a2041-229">table</span><span class="sxs-lookup"><span data-stu-id="a2041-229">table</span></span> | <span data-ttu-id="a2041-230">**はい**</span><span class="sxs-lookup"><span data-stu-id="a2041-230">**yes**</span></span><br/><span data-ttu-id="a2041-231">(id のみ)</span><span class="sxs-lookup"><span data-stu-id="a2041-231">(id only)</span></span> | <span data-ttu-id="a2041-232">いいえ</span><span class="sxs-lookup"><span data-stu-id="a2041-232">no</span></span> | <span data-ttu-id="a2041-233">**はい**</span><span class="sxs-lookup"><span data-stu-id="a2041-233">**yes**</span></span> |   
| <span data-ttu-id="a2041-234">p、li、h1-h6</span><span class="sxs-lookup"><span data-stu-id="a2041-234">p, li, h1-h6</span></span> | <span data-ttu-id="a2041-235">**はい**</span><span class="sxs-lookup"><span data-stu-id="a2041-235">**yes**</span></span><br/><span data-ttu-id="a2041-236">(id のみ)</span><span class="sxs-lookup"><span data-stu-id="a2041-236">(id only)</span></span> | <span data-ttu-id="a2041-237">いいえ</span><span class="sxs-lookup"><span data-stu-id="a2041-237">no</span></span> | <span data-ttu-id="a2041-238">**はい**</span><span class="sxs-lookup"><span data-stu-id="a2041-238">**yes**</span></span> |   
| <span data-ttu-id="a2041-239">title</span><span class="sxs-lookup"><span data-stu-id="a2041-239">title</span></span> | <span data-ttu-id="a2041-240">**はい**</span><span class="sxs-lookup"><span data-stu-id="a2041-240">**yes**</span></span> | <span data-ttu-id="a2041-241">いいえ</span><span class="sxs-lookup"><span data-stu-id="a2041-241">no</span></span> | <span data-ttu-id="a2041-242">no</span><span class="sxs-lookup"><span data-stu-id="a2041-242">no</span></span> |  
 
<br/>

<span data-ttu-id="a2041-243">次の要素では更新アクションはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2041-243">The following elements do not support any update actions.</span></span>

- <span data-ttu-id="a2041-244">img ([絶対配置](onenote-abs-pos.md))</span><span class="sxs-lookup"><span data-stu-id="a2041-244">img ([absolute positioned](onenote-abs-pos.md))</span></span>
- <span data-ttu-id="a2041-245">object ([絶対配置](onenote-abs-pos.md))</span><span class="sxs-lookup"><span data-stu-id="a2041-245">object ([absolute positioned](onenote-abs-pos.md))</span></span>
- <span data-ttu-id="a2041-246">tr、td</span><span class="sxs-lookup"><span data-stu-id="a2041-246">tr, td</span></span>
- <span data-ttu-id="a2041-247">meta</span><span class="sxs-lookup"><span data-stu-id="a2041-247">meta</span></span>
- <span data-ttu-id="a2041-248">head</span><span class="sxs-lookup"><span data-stu-id="a2041-248">head</span></span>
- <span data-ttu-id="a2041-249">span</span><span class="sxs-lookup"><span data-stu-id="a2041-249">span</span></span>
- <span data-ttu-id="a2041-250">a</span><span class="sxs-lookup"><span data-stu-id="a2041-250">a</span></span>
- <span data-ttu-id="a2041-251">style タグ</span><span class="sxs-lookup"><span data-stu-id="a2041-251">style tags</span></span>


<a name="examples"></a>

## <a name="example-requests"></a><span data-ttu-id="a2041-252">要求の例</span><span class="sxs-lookup"><span data-stu-id="a2041-252">Example requests</span></span>

<span data-ttu-id="a2041-p119">更新要求には、JSON 変更オブジェクトとして表現される変更が 1 つ以上含まれています。これらのオブジェクトでは、ページ上のさまざまなターゲットや、ターゲットに対するさまざまなアクションとコンテンツを定義できます。</span><span class="sxs-lookup"><span data-stu-id="a2041-p119">An update request contains one or more changes represented as JSON change objects. These objects can define different targets on the page and different actions and content for the targets.</span></span>

<span data-ttu-id="a2041-255">次の例に、PATCH 要求で使用される JSON オブジェクトと完全な PATCH 要求を示します。</span><span class="sxs-lookup"><span data-stu-id="a2041-255">The following examples include JSON objects used in PATCH requests and complete PATCH requests:</span></span>

- [<span data-ttu-id="a2041-256">子要素の追加</span><span class="sxs-lookup"><span data-stu-id="a2041-256">Append child elements</span></span>](#append-child-elements)
- [<span data-ttu-id="a2041-257">兄弟要素の挿入</span><span class="sxs-lookup"><span data-stu-id="a2041-257">Insert sibling elements</span></span>](#insert-sibling-elements)
- [<span data-ttu-id="a2041-258">要素の置換</span><span class="sxs-lookup"><span data-stu-id="a2041-258">Replace elements</span></span>](#replace-elements)
- [<span data-ttu-id="a2041-259">完全な PATCH 要求</span><span class="sxs-lookup"><span data-stu-id="a2041-259">Complete PATCH requests</span></span>](#complete-patch-request-examples)


<a name="append-examples"></a>

### <a name="append-child-elements"></a><span data-ttu-id="a2041-260">子要素の追加</span><span class="sxs-lookup"><span data-stu-id="a2041-260">Append child elements</span></span>

<span data-ttu-id="a2041-p120">**append** アクションでは、**body**、**div** (div 内)、**ol**、**ul** 要素に子が追加されます。**position** 属性により、ターゲットの前または後に子を追加することが決定されます。既定の位置は**後**です。</span><span class="sxs-lookup"><span data-stu-id="a2041-p120">The **append** action adds a child to a **body**, **div** (within a div), **ol**, or **ul** element. The **position** attribute determines whether to append the child before or after the target. The default position is **after**.</span></span>

#### <a name="append-to-a-div"></a><span data-ttu-id="a2041-264">div への追加</span><span class="sxs-lookup"><span data-stu-id="a2041-264">Append to a div</span></span>

<span data-ttu-id="a2041-p121">次の例では、2 つの子ノードが **div1** 要素に追加されます。画像が最初の子として追加され、段落が 2 番目の子として追加されます。</span><span class="sxs-lookup"><span data-stu-id="a2041-p121">The following example adds two child nodes to the **div1** element. It adds an image as the first child and a paragraph as the last child.</span></span> 

```json
[
 {
    'target':'#div1',
    'action':'append',
    'position':'before',
    'content':'<img data-id="first-child" src="image-url-or-part-name" />'
  },
  {
    'target':'#div1',
    'action':'append',
    'content':'<p data-id="last-child">New paragraph appended to the div</p>'
  }
]
```
 

#### <a name="append-to-the-body-element"></a><span data-ttu-id="a2041-267">*body* 要素への追加</span><span class="sxs-lookup"><span data-stu-id="a2041-267">Append to the *body* element</span></span>

<span data-ttu-id="a2041-268">**body** は、任意のページ上の最初の div 内に子要素を追加するためのショートカットとして使用できます。</span><span class="sxs-lookup"><span data-stu-id="a2041-268">You can use the **body** shortcut to append a child element inside the first div on any page.</span></span>

<span data-ttu-id="a2041-p122">次の例では、ページの最初の div に 2 つの段落を最初の子と最後の子として追加しています。**body** ターゲットと共に # を使用しないでください。この例では、**prepend** アクションを **append** + **before** のショートカットとして使用しています。</span><span class="sxs-lookup"><span data-stu-id="a2041-p122">The following example adds two paragraphs as the first child and the last child to the first div on the page. Don't use a # with the **body** target. This example uses the **prepend** action as a shortcut for **append** + **before**.</span></span>

```json
[
  {
    'target':'body',
    'action':'prepend',
    'content':'<p data-id="first-child">New paragraph as first child in the first div</p>'
  },
  {
    'target':'body',
    'action':'append',
    'content':'<p data-id="last-child">New paragraph as last child in the first div</p>'
  }
]
```
 

#### <a name="append-to-a-list"></a><span data-ttu-id="a2041-272">リストへの追加</span><span class="sxs-lookup"><span data-stu-id="a2041-272">Append to a list</span></span>

<span data-ttu-id="a2041-p123">次の例では、リスト項目がターゲット リストに最後の子として追加されます。この項目では既定以外のリスト スタイルが使用されるため、**list-style-type** プロパティが定義されます。</span><span class="sxs-lookup"><span data-stu-id="a2041-p123">The following example adds a list item as a last child to the target list. The **list-style-type** property is defined because the item uses a non-default list style.</span></span>

```json
[
  {
    'target':'#circle-ul',
    'action':'append',
    'content':'<li style="list-style-type:circle">Item at the end of the list</li>'
  }
]
```
 

<a name="insert-examples"></a>

### <a name="insert-sibling-elements"></a><span data-ttu-id="a2041-275">兄弟要素の挿入</span><span class="sxs-lookup"><span data-stu-id="a2041-275">Insert sibling elements</span></span>

<span data-ttu-id="a2041-p124">**insert** アクションでは、兄弟がターゲット要素に追加されます。**position** 属性により、ターゲットの前または後に兄弟を挿入することが決定されます。既定の位置は**後**です。「[**insert** をサポートする要素](#supported-elements-and-actions)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="a2041-p124">The **insert** action adds a sibling to the target element. The **position** attribute determines whether to insert the sibling before or after the target. The default position is **after**. See [elements that support **insert**](#supported-elements-and-actions).</span></span>

#### <a name="insert-siblings"></a><span data-ttu-id="a2041-280">兄弟の挿入</span><span class="sxs-lookup"><span data-stu-id="a2041-280">Insert siblings</span></span>

<span data-ttu-id="a2041-p125">次の例では、ページに 2 つの兄弟ノードが挿入されます。**para1** 要素の上に画像が追加され、**para2** 要素の下に段落が追加されます。</span><span class="sxs-lookup"><span data-stu-id="a2041-p125">The following example adds two sibling nodes to the page. It adds an image above the **para1** element and a paragraph below the **para2** element.</span></span>

```json
[
  {
     'target':'#para1',
     'action':'insert',
     'position':'before',
     'content':'<img src="image-data-url-or-part-name" alt="Image inserted above the target" />'
  },
  {
    'target':'#para2',
     'action':'insert',
     'content':'<p data-id="next-sibling">Paragraph inserted below the target</p>'
  }
]
```
 

<a name="replace-examples"></a>

### <a name="replace-elements"></a><span data-ttu-id="a2041-283">要素の置換</span><span class="sxs-lookup"><span data-stu-id="a2041-283">Replace elements</span></span>

<span data-ttu-id="a2041-p126">**data-id** と生成された **id** のいずれかをターゲット値として使用し、div 内にある **img** 要素および **object** 要素を置換できます。ページ タイトルを置換する場合は、**title** キーワードを使用します。[**replace** をサポートするその他すべての要素](#supported-elements-and-actions)については、生成された ID を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a2041-p126">You can use either the **data-id** or generated **id** as the target value to replace **img** and **object** elements that are within a div. To replace the page title, use the **title** keyword. For all other [elements that support **replace**](#supported-elements-and-actions), you must use the generated ID.</span></span>

#### <a name="replace-an-image"></a><span data-ttu-id="a2041-287">画像の置換</span><span class="sxs-lookup"><span data-stu-id="a2041-287">Replace an image</span></span>

<span data-ttu-id="a2041-288">次の例では、画像の **data-id** をターゲットとして使用して、div 内の画像が置換されます。</span><span class="sxs-lookup"><span data-stu-id="a2041-288">The following example replaces an image with a div by using the image's **data-id** as the target.</span></span> 

```json
[
  {
    'target':'#img1',
    'action':'replace',
    'content':'<div data-id="new-div"><p>This div replaces the image</p></div>'
  }
]
```
 

#### <a name="update-a-table"></a><span data-ttu-id="a2041-289">表の更新</span><span class="sxs-lookup"><span data-stu-id="a2041-289">Update a table</span></span> 

<span data-ttu-id="a2041-p127">次の例は、生成された ID を使用して表を更新する方法を示します。**tr** 要素と **td** 要素の置換はサポートされていませんが、表全体を置換することができます。</span><span class="sxs-lookup"><span data-stu-id="a2041-p127">This example shows how to update a table by using its generated ID. Replacing **tr** and **td** elements is not supported, but you can replace the entire table.</span></span>

```json
[
  {
    'target':'table:{de3e0977-94e4-4bb0-8fee-0379eaf47486}{11}',
    'action':'replace',
    'content':'<table data-id="football">
      <tr><td><p><b>Brazil</b></p></td><td><p>Germany</p></td></tr>
      <tr><td><p>France</p></td><td><p><b>Italy</b></p></td></tr>
      <tr><td><p>Netherlands</p></td><td><p><b>Spain</b></p></td></tr>
      <tr><td><p>Argentina</p></td><td><p><b>Germany</b></p></td></tr></table>'
  }
]
```
 

#### <a name="change-the-title"></a><span data-ttu-id="a2041-292">タイトルの変更</span><span class="sxs-lookup"><span data-stu-id="a2041-292">Change the title</span></span> 

<span data-ttu-id="a2041-p128">次の例は、ページのタイトルを変更する方法を示します。タイトルを変更するには、ターゲット値として **title** キーワードを使用します。title ターゲットでは # は使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="a2041-p128">This example shows how to change the title of a page. To change the title, use the **title** keyword as the target value. Don't use a # with the title target.</span></span>

```json
[
  {
    'target':'title',
    'action':'replace',
    'content':'New title'
  }
]
```
 

#### <a name="update-a-to-do-item"></a><span data-ttu-id="a2041-296">To Do アイテムの更新</span><span class="sxs-lookup"><span data-stu-id="a2041-296">Update a to-do item</span></span>

<span data-ttu-id="a2041-297">次に示す例では、replace アクションを使用して、To Do チェック ボックス アイテムを完了状態に変更します。</span><span class="sxs-lookup"><span data-stu-id="a2041-297">The following example uses the replace action to change a to-do check box item to a completed state.</span></span>

```json
[
  {
    'target':'#task1',
    'action':'replace',
    'content':'<p data-tag="to-do:completed" data-id="task1">First task</p>'
  }
]
```

<span data-ttu-id="a2041-298">**data-tag** 属性の使用法の詳細については、「[ノート シールを使用する](onenote-note-tags.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2041-298">See [Use note tags](onenote-note-tags.md) for more about using the **data-tag** attribute.</span></span>


<a name="complete-requests"></a>

### <a name="complete-patch-request-examples"></a><span data-ttu-id="a2041-299">完全な PATCH 要求の例</span><span class="sxs-lookup"><span data-stu-id="a2041-299">Complete PATCH request examples</span></span>

<span data-ttu-id="a2041-300">次の例に、完全な PATCH 要求を示します。</span><span class="sxs-lookup"><span data-stu-id="a2041-300">The following examples show complete PATCH requests.</span></span>

#### <a name="request-with-text-content-only"></a><span data-ttu-id="a2041-301">テキスト コンテンツのみの要求</span><span class="sxs-lookup"><span data-stu-id="a2041-301">Request with text content only</span></span>

<span data-ttu-id="a2041-p129">次の例では、PATCH 要求でコンテンツ タイプとして **application/json** が使用されています。 コンテンツにバイナリ データが含まれていないとき、この形式を使用できます。</span><span class="sxs-lookup"><span data-stu-id="a2041-p129">The following example shows a PATCH request that uses the **application/json** content type. You can use this format when your content doesn't contain binary data.</span></span>

```json
PATCH https://graph.microsoft.com/v1.0/me/onenote/notebooks/pages/{page-id}/content

Content-Type: application/json
Authorization: Bearer {token}

[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-data-url" alt="New image from a URL" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>Item at the bottom of the list</li>'
  }
]
```
 
<a name="multipart"></a>

#### <a name="multipart-request-with-binary-content"></a><span data-ttu-id="a2041-304">バイナリ コンテンツを含むマルチパート要求</span><span class="sxs-lookup"><span data-stu-id="a2041-304">Multipart request with binary content</span></span> 

<span data-ttu-id="a2041-p130">次の例は、バイナリ データを含んでいるマルチパート PATCH 要求を示しています。マルチパート要求には、**application/json** コンテンツ タイプを指定し、JSON 変更オブジェクトの配列を含める "Commands" 部分が必要になります。その他のデータ部分に、バイナリ データを含めることができます。部分の名前は、通常、ミリ秒単位での現在の時刻、またはランダムな GUID が付加された文字列になります。</span><span class="sxs-lookup"><span data-stu-id="a2041-p130">The following example shows a multipart PATCH request that includes binary data. Multipart requests require a "Commands" part that specifies the **application/json** content type and contains the array of JSON change objects. Other data parts can contain binary data. Part names typically are strings appended with the current time in milliseconds or a random GUID.</span></span>

```json
PATCH https://graph.microsoft.com/v1.0/me/onenote/notebooks/pages/{page-id}/content

Content-Type: multipart/form-data; boundary=PartBoundary123
Authorization: Bearer {token}

--PartBoundary123
Content-Disposition: form-data; name="Commands"
Content-Type: application/json

[
  {
    'target':'img:{2998967e-69b3-413f-a221-c1a3b5cbe0fc}{42}',
    'action':'replace',
    'content':'<img src="name:image-part-name" alt="New binary image" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>Item at the bottom of the list</li>'
  }
]

--PartBoundary123
Content-Disposition: form-data; name="image-part-name"
Content-Type: image/png

... binary image data ...

--PartBoundary123--
```

<a name="request-response-info"></a>

## <a name="request-and-response-information-for-patch-requests"></a><span data-ttu-id="a2041-309">PATCH 要求の要求情報と応答情報</span><span class="sxs-lookup"><span data-stu-id="a2041-309">Request and response information for PATCH requests</span></span>

| <span data-ttu-id="a2041-310">要求データ</span><span class="sxs-lookup"><span data-stu-id="a2041-310">Request data</span></span> | <span data-ttu-id="a2041-311">説明</span><span class="sxs-lookup"><span data-stu-id="a2041-311">Description</span></span> |  
|------|------|  
| <span data-ttu-id="a2041-312">プロトコル</span><span class="sxs-lookup"><span data-stu-id="a2041-312">Protocol</span></span> | <span data-ttu-id="a2041-313">すべての要求は SSL/TLS HTTPS プロトコルを使用します。</span><span class="sxs-lookup"><span data-stu-id="a2041-313">All requests use the SSL/TLS HTTPS protocol.</span></span> |  
| <span data-ttu-id="a2041-314">承認ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a2041-314">Authorization header</span></span> | <p><span data-ttu-id="a2041-315">`Bearer {token}`。`{token}` は、登録済みアプリの有効な OAuth 2.0 アクセス トークンです。</span><span class="sxs-lookup"><span data-stu-id="a2041-315">`Bearer {token}`, where `{token}` is a valid OAuth 2.0 access token for your registered app.</span></span></p><p><span data-ttu-id="a2041-p131">これがないか、無効の場合、401 ステータス コードで要求は失敗します。「[認証とアクセス許可](permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2041-p131">If missing or invalid, the request fails with a 401 status code. See [Authentication and permissions](permissions-reference.md).</span></span></p> |  
| <span data-ttu-id="a2041-318">Content-Type ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a2041-318">Content-Type header</span></span> | <p><span data-ttu-id="a2041-319">JSON 変更オブジェクトの配列の `application/json`。メッセージ本文または[マルチパート要求](#multipart-request-with-binary-content)の必須の "Commands" パートで直接送信。</span><span class="sxs-lookup"><span data-stu-id="a2041-319">`application/json` for the array of JSON change objects, whether sent directly in the message body or in the required "Commands" part of [multipart requests](#multipart-request-with-binary-content).</span></span></p><p><span data-ttu-id="a2041-320">マルチパート要求はバイナリ データを送信するときに必須であり、コンテンツ タイプとして `multipart/form-data; boundary=part-boundary` を使用します。`{part-boundary}` は、各データ パートの開始と終了を伝える文字列です。</span><span class="sxs-lookup"><span data-stu-id="a2041-320">Multipart requests are required when sending binary data, and use the `multipart/form-data; boundary=part-boundary` content type, where `{part-boundary}` is a string that signals the start and end of each data part.</span></span></p> |  

<br/> 

| <span data-ttu-id="a2041-321">応答データ</span><span class="sxs-lookup"><span data-stu-id="a2041-321">Response data</span></span> | <span data-ttu-id="a2041-322">説明</span><span class="sxs-lookup"><span data-stu-id="a2041-322">Description</span></span> |  
|------|------|  
| <span data-ttu-id="a2041-323">成功コード</span><span class="sxs-lookup"><span data-stu-id="a2041-323">Success code</span></span> | <span data-ttu-id="a2041-p132">204 HTTP ステータス コード。PATCH 要求に対して JSON データは返されません。</span><span class="sxs-lookup"><span data-stu-id="a2041-p132">A 204 HTTP status code. No JSON data is returned for a PATCH request.</span></span> |  
| <span data-ttu-id="a2041-326">エラー</span><span class="sxs-lookup"><span data-stu-id="a2041-326">Errors</span></span> | <span data-ttu-id="a2041-327">Microsoft Graph から返されることのある OneNote エラーに関する詳細については、「[Microsoft Graph の OneNote API のエラー コード](onenote-error-codes.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="a2041-327">Read [Error codes for OneNote APIs in Microsoft Graph](onenote-error-codes.md) to learn about OneNote errors that Microsoft Graph can return.</span></span> |  
 
 

<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-service-root-url"></a><span data-ttu-id="a2041-328">Microsoft Graph サービスのルート URL の構築</span><span class="sxs-lookup"><span data-stu-id="a2041-328">Constructing the Microsoft Graph service root URL</span></span>

<span data-ttu-id="a2041-329">OneNote サービスのルート URL は、OneNote API へのすべての呼び出しで次の形式を使用します。</span><span class="sxs-lookup"><span data-stu-id="a2041-329">The OneNote service root URL uses the following format for all calls to the OneNote API:</span></span>

`https://graph.microsoft.com/{version}/me/onenote/`

<span data-ttu-id="a2041-330">URL の `version` セグメントは、使用する Microsoft Graph のバージョンを示しています。</span><span class="sxs-lookup"><span data-stu-id="a2041-330">The `version` segment in the URL represents the version of Microsoft Graph that you want to use.</span></span> <span data-ttu-id="a2041-331">安定した運用コードには `v1.0` を使用します。</span><span class="sxs-lookup"><span data-stu-id="a2041-331">`v1.0` is for stable production code.</span></span> <span data-ttu-id="a2041-332">開発中の機能を試すには `beta` を使用します。</span><span class="sxs-lookup"><span data-stu-id="a2041-332">`beta` is to try out a feature that's in development.</span></span> <span data-ttu-id="a2041-333">ベータ版の機能は変更される可能性があるため、運用コードでは使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="a2041-333">Features and functionality in beta may change, so you shouldn't use it in your production code.</span></span>

<span data-ttu-id="a2041-334">現在のユーザーがアクセスできる OneNote コンテンツには `me` を使用します (所有と共有)。</span><span class="sxs-lookup"><span data-stu-id="a2041-334">`me` is for OneNote content that the current user can access (owned and shared).</span></span> <span data-ttu-id="a2041-335">指定されたユーザー (URL 内) が現在のユーザーと共有している OneNote コンテンツには `users/{id}` を使用します。</span><span class="sxs-lookup"><span data-stu-id="a2041-335">`users/{id}` is for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="a2041-336">[Azure AD Graph API](https://msdn.microsoft.com/library/azure/ad/graph/api/api-catalog) の使用。</span><span class="sxs-lookup"><span data-stu-id="a2041-336">Use the [Azure AD Graph API](https://msdn.microsoft.com/library/azure/ad/graph/api/api-catalog).</span></span>


> <span data-ttu-id="a2041-337">**注:** `https://graph.microsoft.com/v1.0/users`で GET 要求を行うことにより、ユーザー ID を取得できます。</span><span class="sxs-lookup"><span data-stu-id="a2041-337">**Note:** You can get user ids by making a GET request on `https://graph.microsoft.com/v1.0/users`.</span></span>



<a name="permissions"></a>

## <a name="permissions"></a><span data-ttu-id="a2041-338">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a2041-338">Permissions</span></span>

<span data-ttu-id="a2041-p135">OneNote ページを更新するには、適切なアクセス許可を要求する必要があります。アプリの動作に必要な最低限のアクセス許可を選択してください。</span><span class="sxs-lookup"><span data-stu-id="a2041-p135">To update OneNote pages, you'll need to request appropriate permissions. Choose the lowest level of permissions that your app needs to do its work.</span></span>

- <span data-ttu-id="a2041-341">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a2041-341">Notes.ReadWrite</span></span>
- <span data-ttu-id="a2041-342">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2041-342">Notes.ReadWrite.All</span></span>

<span data-ttu-id="a2041-343">アクセス許可のスコープと動作のしくみの詳細については、「[OneNote のアクセス許可のスコープ](permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2041-343">For more information about permission scopes and how they work, see [OneNote permission scopes](permissions-reference.md).</span></span>
   

<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="a2041-344">関連項目</span><span class="sxs-lookup"><span data-stu-id="a2041-344">See also</span></span>

- [<span data-ttu-id="a2041-345">画像とファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="a2041-345">Add images and files</span></span>](onenote-images-files.md)
- [<span data-ttu-id="a2041-346">OneNote との統合</span><span class="sxs-lookup"><span data-stu-id="a2041-346">Integrate with OneNote</span></span>](integrate-with-onenote.md)
- [<span data-ttu-id="a2041-347">OneNote の開発者ブログ</span><span class="sxs-lookup"><span data-stu-id="a2041-347">OneNote Developer Blog</span></span>](https://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="a2041-348">Stack Overflow 掲載の OneNote の開発に関する質問</span><span class="sxs-lookup"><span data-stu-id="a2041-348">OneNote development questions on Stack Overflow</span></span>](https://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="a2041-349">OneNote GitHub のリポジトリ</span><span class="sxs-lookup"><span data-stu-id="a2041-349">OneNote GitHub repos</span></span>](https://go.microsoft.com/fwlink/?LinkID=390178)  
