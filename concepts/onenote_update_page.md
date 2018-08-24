# <a name="update-onenote-page-content"></a><span data-ttu-id="f685e-101">OneNote ページ コンテンツを更新する</span><span class="sxs-lookup"><span data-stu-id="f685e-101">Update OneNote page content</span></span>

<span data-ttu-id="f685e-102">**適用対象** OneDrive のコンシューマー ノートブック | Office 365 のエンタープライズ ノートブック</span><span class="sxs-lookup"><span data-stu-id="f685e-102">**Applies to** Consumer notebooks on OneDrive | Enterprise notebooks on Office 365</span></span>


<span data-ttu-id="f685e-103">OneNote ページのコンテンツを更新する場合は、ページの *content* エンドポイントに PATCH 要求を送信します。</span><span class="sxs-lookup"><span data-stu-id="f685e-103">To update the content of a OneNote page, you send a PATCH request to the page's *content* endpoint:</span></span>

`PATCH ../notes/pages/{id}/content`</p>

<span data-ttu-id="f685e-104">メッセージの本文で JSON 変更オブジェクトを送信します。</span><span class="sxs-lookup"><span data-stu-id="f685e-104">Send a JSON change object in the message body.</span></span> <span data-ttu-id="f685e-105">要求が成功すると、Microsoft Graph は 204 HTTP 状態コードを返します。</span><span class="sxs-lookup"><span data-stu-id="f685e-105">If the request is successful, Microsoft Graph returns a 204 HTTP status code.</span></span>


<a name="request-uri"></a>

## <a name="construct-the-request-uri"></a><span data-ttu-id="f685e-106">要求 URI の構築</span><span class="sxs-lookup"><span data-stu-id="f685e-106">Construct the request URI</span></span>

<span data-ttu-id="f685e-107">要求 URI を構築するには、サービス ルート URL から開始します。</span><span class="sxs-lookup"><span data-stu-id="f685e-107">To construct the request URI, start with the service root URL:</span></span>

`https://graph.microsoft.com/v1.0/me/onenote`

<br/>

<span data-ttu-id="f685e-108">次に、ページの *content* エンドポイントを追加します。</span><span class="sxs-lookup"><span data-stu-id="f685e-108">Then append the page's *content* endpoint:</span></span>

- <span data-ttu-id="f685e-109">**ページ HTML と、すべての定義済み *data-id* の値を取得する**</span><span class="sxs-lookup"><span data-stu-id="f685e-109">**Get the page HTML and all defined *data-id* values**</span></span><br/><br/>`../pages/{id}/content`   

- <span data-ttu-id="f685e-110">**ページ HTML、すべての定義済み *data-id* の値、およびすべての生成された *id* の値を取得する**</span><span class="sxs-lookup"><span data-stu-id="f685e-110">**Get the page HTML, all defined *data-id* values, and all generated *id* values**</span></span><br/><br/>`../pages/{page-id}/content?includeIDs=true` 

<span data-ttu-id="f685e-111">**data-id** と **id** の値は、更新する要素の **target** 識別子として使用されます。</span><span class="sxs-lookup"><span data-stu-id="f685e-111">The **data-id** and **id** values are used as **target** identifiers for the elements you want to update.</span></span>

 
<span data-ttu-id="f685e-112">完全な要求 URI は、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="f685e-112">Your full request URI will look like this:</span></span><br/><br/>`https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/content`


<span data-ttu-id="f685e-113">[サービス ルート URL](../api-reference/v1.0/resources/onenote-api-overview.md#root-url) の詳細についてはリンク先をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="f685e-113">Learn more about the [service root URL](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span></span>


<a name="message-body"></a>

## <a name="construct-the-message-body"></a><span data-ttu-id="f685e-114">メッセージ本文の構築</span><span class="sxs-lookup"><span data-stu-id="f685e-114">Construct the message body</span></span>

<span data-ttu-id="f685e-p102">OneNote ページの HTML には、**div** 要素、**img** 要素、**ol** 要素などの構造に編成されたテキスト、画像などのコンテンツが含まれています。OneNote ページのコンテンツを更新する場合は、ページ上で HTML 要素を追加および置換します。</span><span class="sxs-lookup"><span data-stu-id="f685e-p102">The HTML of a OneNote page contains text, images, and other content organized into structures such as **div**, **img**, and **ol** elements. To update OneNote page content, you add and replace HTML elements on the page.</span></span>

<span data-ttu-id="f685e-p103">変更内容は JSON 変更オブジェクトの配列としてメッセージ本文に入れて送信します。ターゲット要素、新しい HTML コンテンツ、コンテンツに対する操作が各オブジェクトにより指定されます。</span><span class="sxs-lookup"><span data-stu-id="f685e-p103">Your changes are sent in the message body as an array of JSON change objects. Each object specifies the target element, new HTML content, and what to do with the content.</span></span>

<span data-ttu-id="f685e-p104">2 つの変更を定義する配列を次に示します。最初の変更では画像が兄弟として段落の上に挿入され、2 番目の変更ではアイテムが最後の子としてリストに追加されます。</span><span class="sxs-lookup"><span data-stu-id="f685e-p104">The following array defines two changes. The first inserts an image above a paragraph as a sibling, and the second appends an item to a list as a last child.</span></span>

```json
[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-url-or-part-name" alt="Image above the target paragraph" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>Item at the end of the list</li>'
  }
]
```

<span data-ttu-id="f685e-121">[その他の例](#example-requests)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f685e-121">See [more examples](#example-requests).</span></span>


### <a name="attributes-for-json-change-objects"></a><span data-ttu-id="f685e-122">JSON 変更オブジェクトの属性</span><span class="sxs-lookup"><span data-stu-id="f685e-122">Attributes for JSON change objects</span></span>

<span data-ttu-id="f685e-123">PATCH 要求の JSON オブジェクトの定義には、**target** 属性、**action** 属性、**position** 属性、および **content** 属性を使用します。</span><span class="sxs-lookup"><span data-stu-id="f685e-123">Use the **target**, **action**, **position**, and **content** attributes to define JSON objects for PATCH requests.</span></span>

#### <a name="target"></a><span data-ttu-id="f685e-124">ターゲット</span><span class="sxs-lookup"><span data-stu-id="f685e-124">target</span></span>

<span data-ttu-id="f685e-p105">更新する要素。値として次の ID のいずれかを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f685e-p105">The element to update. The value must be one of the following identifiers:</span></span>

| <span data-ttu-id="f685e-127">識別子</span><span class="sxs-lookup"><span data-stu-id="f685e-127">Identifier</span></span> | <span data-ttu-id="f685e-128">説明</span><span class="sxs-lookup"><span data-stu-id="f685e-128">Description</span></span> |  
|------|------|  
| <span data-ttu-id="f685e-129">#{data-id}</span><span class="sxs-lookup"><span data-stu-id="f685e-129">#{data-id}</span></span> | <p><span data-ttu-id="f685e-p106">この ID は、[ページを作成](onenote-create-page.md)するときや[更新](onenote_update_page.md)するときに、入力 HTML の要素で任意で定義されます。値の先頭に # を付けます。</span><span class="sxs-lookup"><span data-stu-id="f685e-p106">This ID is optionally defined on elements in the input HTML when [creating a page](onenote-create-page.md) or [updating a page](onenote_update_page.md). Prefix the value with a #.</span></span></p><p> <span data-ttu-id="f685e-132">例:</span><span class="sxs-lookup"><span data-stu-id="f685e-132">Example:</span></span><br/><span data-ttu-id="f685e-133">`'target':'#intro'` は要素 `<div data-id="intro" ...>` をターゲットとします `<div data-id="intro" ...>`</span><span class="sxs-lookup"><span data-stu-id="f685e-133">`'target':'#intro'` targets the element `<div data-id="intro" ...>`</span></span></p> |  
| <span data-ttu-id="f685e-134">ID</span><span class="sxs-lookup"><span data-stu-id="f685e-134">id</span></span> | <p><span data-ttu-id="f685e-135">これは、Microsoft Graph から得られる[生成済み ID](#generated-ids) であり、ほとんどの置換操作で必要になります。</span><span class="sxs-lookup"><span data-stu-id="f685e-135">This is the [generated ID](#generated-ids) from Microsoft Graph, and is required for most replace operations.</span></span> <span data-ttu-id="f685e-136">プレフィックス # を追加しないでください。</span><span class="sxs-lookup"><span data-stu-id="f685e-136">Do not prefix with a #.</span></span></p><p> <span data-ttu-id="f685e-137">例:</span><span class="sxs-lookup"><span data-stu-id="f685e-137">Example:</span></span><br/><span data-ttu-id="f685e-138">`'target':'div:{33f8a2...}{37}'` は要素 `<div id="div:{33f8a2...}{37}" ...>` をターゲットとします `<div id="div:{33f8a2...}{37}" ...>`</span><span class="sxs-lookup"><span data-stu-id="f685e-138">`'target':'div:{33f8a2...}{37}'` targets the element `<div id="div:{33f8a2...}{37}" ...>`</span></span></p><p><span data-ttu-id="f685e-p108">[入力 HTML](onenote_input_output_html.md) に定義されている **id** 値とこれらを混同しないでください。入力 HTML で送信される **id** 値は、すべて破棄されます。</span><span class="sxs-lookup"><span data-stu-id="f685e-p108">Don't confuse these with any **id** values defined in the [input HTML](onenote_input_output_html.md). All **id** values sent in the input HTML are discarded.</span></span></p> |  
| <span data-ttu-id="f685e-141">本文</span><span class="sxs-lookup"><span data-stu-id="f685e-141">body</span></span> | <span data-ttu-id="f685e-p109">ページ上で最初の div をターゲットにするキーワード。プレフィックス # を追加してはいけません。</span><span class="sxs-lookup"><span data-stu-id="f685e-p109">The keyword that targets the first div on the page. Do not prefix with a #.</span></span> |  
| <span data-ttu-id="f685e-144">タイトル</span><span class="sxs-lookup"><span data-stu-id="f685e-144">title</span></span> | <span data-ttu-id="f685e-p110">ページ タイトルをターゲットにするキーワード。プレフィックス # を追加してはなりません。</span><span class="sxs-lookup"><span data-stu-id="f685e-p110">The keyword that targets the page title. Do not prefix with a #.</span></span> |  
 
#### <a name="action"></a><span data-ttu-id="f685e-147">操作</span><span class="sxs-lookup"><span data-stu-id="f685e-147">action</span></span>

<span data-ttu-id="f685e-p111">ターゲット要素に対して実行するアクション。「[サポートされる要素とアクション](#supported-elements-and-actions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f685e-p111">The action to perform on the target element. See [supported actions for elements](#supported-elements-and-actions).</span></span>

| <span data-ttu-id="f685e-150">アクション</span><span class="sxs-lookup"><span data-stu-id="f685e-150">Action</span></span> | <span data-ttu-id="f685e-151">説明</span><span class="sxs-lookup"><span data-stu-id="f685e-151">Description</span></span> |  
|------|------|  
| <span data-ttu-id="f685e-152">追加</span><span class="sxs-lookup"><span data-stu-id="f685e-152">append</span></span> | <p><span data-ttu-id="f685e-153">指定されたコンテンツを最初または最後の子としてターゲットに追加します。追加される位置 (最初または最後) は、**position** 属性によって決まります。</span><span class="sxs-lookup"><span data-stu-id="f685e-153">Adds the supplied content to the target as a first or last child, as determined by the **position** attribute.</span></span></p><p><span data-ttu-id="f685e-154">**body**、**div**、**ol**、**ul** 要素にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="f685e-154">Applies only to **body**, **div**, **ol**, and **ul** elements.</span></span></p> |  
| <span data-ttu-id="f685e-155">挿入</span><span class="sxs-lookup"><span data-stu-id="f685e-155">insert</span></span> | <span data-ttu-id="f685e-156">指定されたコンテンツを兄弟としてターゲットの前または後に追加します。追加される位置 (前または後) は、**position** 属性によって決まります。</span><span class="sxs-lookup"><span data-stu-id="f685e-156">Adds the supplied content as a sibling before or after the target, as determined by the **position** attribute.</span></span> |  
| <span data-ttu-id="f685e-157">先頭に追加</span><span class="sxs-lookup"><span data-stu-id="f685e-157">prepend</span></span> | <p><span data-ttu-id="f685e-p112">指定されたコンテンツを最初の子としてターゲットに追加します。**append** + **before** のショートカット。</span><span class="sxs-lookup"><span data-stu-id="f685e-p112">Adds the supplied content to the target as a first child. Shortcut for **append** + **before**.</span></span></p><p><span data-ttu-id="f685e-160">**body**、**div**、**ol**、**ul** 要素にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="f685e-160">Applies only to **body**, **div**, **ol**, and **ul** elements.</span></span></p> |  
| <span data-ttu-id="f685e-161">置換え</span><span class="sxs-lookup"><span data-stu-id="f685e-161">replace</span></span> | <p><span data-ttu-id="f685e-162">指定したコンテンツでターゲットを置換します。</span><span class="sxs-lookup"><span data-stu-id="f685e-162">Replaces the target with the supplied content.</span></span></p><p><span data-ttu-id="f685e-163">ほとんどの **replace** アクションは、ターゲットの[生成された ID](#generated-ids) を使用する必要があります (ただし、div 内の **img** 要素と **object** 要素を除きます。これらは、**data-id** の使用もサポートしています)。</span><span class="sxs-lookup"><span data-stu-id="f685e-163">Most **replace** actions require using the [generated ID](#generated-ids) for the target (except **img** and **object** elements within a div, which also support using **data-id**).</span></span></p> |  
 
#### <a name="position"></a><span data-ttu-id="f685e-164">位置</span><span class="sxs-lookup"><span data-stu-id="f685e-164">position</span></span>

<span data-ttu-id="f685e-p113">指定されたコンテンツを追加する位置。ターゲット要素を基準とした相対位置です。省略すると、既定値として **after** が使用されます。</span><span class="sxs-lookup"><span data-stu-id="f685e-p113">The location to add the supplied content, relative to the target element. Defaults to **after** if omitted.</span></span>

| <span data-ttu-id="f685e-167">位置</span><span class="sxs-lookup"><span data-stu-id="f685e-167">Position</span></span> | <span data-ttu-id="f685e-168">説明</span><span class="sxs-lookup"><span data-stu-id="f685e-168">Description</span></span> |  
|------|------|  
| <span data-ttu-id="f685e-169">after (既定値)</span><span class="sxs-lookup"><span data-stu-id="f685e-169">after (default)</span></span> |<p><span data-ttu-id="f685e-170">**append** の場合: ターゲット要素の最後の子。</span><span class="sxs-lookup"><span data-stu-id="f685e-170">With **append**: The last child of the target element.</span></span></p><p><span data-ttu-id="f685e-171">**insert** の場合: ターゲット要素の後続の兄弟。</span><span class="sxs-lookup"><span data-stu-id="f685e-171">With **insert**: The subsequent sibling of the target element.</span></span></p> |
| <span data-ttu-id="f685e-172">before</span><span class="sxs-lookup"><span data-stu-id="f685e-172">before</span></span> | <p><span data-ttu-id="f685e-173">**append** の場合: ターゲット要素の最初の子。</span><span class="sxs-lookup"><span data-stu-id="f685e-173">With **append**: The first child of the target element.</span></span></p><p><span data-ttu-id="f685e-174">**insert** の場合: ターゲット要素の先行の兄弟。</span><span class="sxs-lookup"><span data-stu-id="f685e-174">With **insert**: The preceding sibling of the target element.</span></span></p> |

#### <a name="content"></a><span data-ttu-id="f685e-175">コンテンツ</span><span class="sxs-lookup"><span data-stu-id="f685e-175">content</span></span>

<span data-ttu-id="f685e-p114">ページに追加する整形式 HTML の文字列と画像またはファイル バイナリ データ。コンテンツにバイナリ データが含まれている場合、コンテンツ タイプとして `multipart/form-data` を利用し、"Commands" パートを含む要求を送信する必要があります ([例](#multipart-request-with-binary-content)参照)。</span><span class="sxs-lookup"><span data-stu-id="f685e-p114">A string of well-formed HTML to add to the page, and any image or file binary data. If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part (see an [example](#multipart-request-with-binary-content)).</span></span> 
 

<a name="generated-ids"></a>

### <a name="generated-ids"></a><span data-ttu-id="f685e-178">生成された ID</span><span class="sxs-lookup"><span data-stu-id="f685e-178">Generated IDs</span></span>
<span data-ttu-id="f685e-179">Microsoft Graph は、更新可能なページで要素に対して **id** 値を生成します。</span><span class="sxs-lookup"><span data-stu-id="f685e-179">Microsoft Graph generates **id** values for the elements on the page that can be updated.</span></span> <span data-ttu-id="f685e-180">生成された ID を取得するには、GET 要求で `includeIDs=true` クエリ文字列を使用します。</span><span class="sxs-lookup"><span data-stu-id="f685e-180">To get generated IDs, use the `includeIDs=true` query string expression in your GET request:</span></span>

`GET ../notes/pages/{page-id}/content?includeIDs=true` 

> <span data-ttu-id="f685e-181">**注:** API は、ページ作成要求およびページ更新要求の[入力 HTML](onenote_input_output_html.md) で定義された **id** の値をすべて破棄します。</span><span class="sxs-lookup"><span data-stu-id="f685e-181">**Note:** The API discards all **id** values that are defined in the [input HTML](onenote_input_output_html.md) of create-page and update-page requests.</span></span>

<span data-ttu-id="f685e-182">次の例は、ページの[出力 HTML](onenote_input_output_html.md) の段落と画像に対して生成された ID を示します。</span><span class="sxs-lookup"><span data-stu-id="f685e-182">The following example shows generated IDs for a paragraph and an image in the [output HTML](onenote_input_output_html.md) of a page.</span></span>

```html
<p id="p:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{40}">Some text on the page</p>
<img id="img:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{45}" ... />
```

<span data-ttu-id="f685e-183">生成された **id** 値はページ更新後に変更されることがあるため、これらの値を使用する PATCH 要求を作成する前に、現行値を取得する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f685e-183">Generated **id** values might change after a page update, so you should get the current values before building a PATCH request that uses them.</span></span>
 
<span data-ttu-id="f685e-184">ターゲット要素は、**data-id** または **id** 値を使用して次のように指定できます。</span><span class="sxs-lookup"><span data-stu-id="f685e-184">You can specify target elements by using the **data-id** or **id** value, as follows:</span></span>

- <span data-ttu-id="f685e-185">**append** アクションと **insert** アクションでは、いずれの ID もターゲット値として使用できます。</span><span class="sxs-lookup"><span data-stu-id="f685e-185">For **append** and **insert** actions, you can use either ID as the target value.</span></span>
- <span data-ttu-id="f685e-186">**replace** アクションでは、すべての要素について、生成された IDを使用する必要があります。ただし、ページ タイトル、および div 内の画像とオブジェクトを除きます。</span><span class="sxs-lookup"><span data-stu-id="f685e-186">For **replace** actions, you must use the generated ID for all elements except for the page title and images and objects that are within a div.</span></span> 
    - <span data-ttu-id="f685e-187">タイトルを置換する場合は、**title** キーワードを使用します。</span><span class="sxs-lookup"><span data-stu-id="f685e-187">To replace a title, use the **title** keyword.</span></span> 
    - <span data-ttu-id="f685e-188">div 内の画像とオブジェクトを置換する場合は、**data-id** または **id** のどちらかを使用します。</span><span class="sxs-lookup"><span data-stu-id="f685e-188">To replace images and objects that are within a div, use either **data-id** or **id**.</span></span>

<span data-ttu-id="f685e-p116">次の例では、ターゲットに **id** 値を使用します。生成された ID と共に # プレフィックスを使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="f685e-p116">The following example uses the **id** value for the target. Don't use the # prefix with a generated ID.</span></span>

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

## <a name="supported-elements-and-actions"></a><span data-ttu-id="f685e-191">サポートされる要素とアクション</span><span class="sxs-lookup"><span data-stu-id="f685e-191">Supported elements and actions</span></span>

<span data-ttu-id="f685e-p117">ページ上の要素の多くは更新可能ですが、要素の種類ごとに特定のアクションがサポートされています。サポートされるターゲット要素と、各要素でサポートされる更新アクションを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="f685e-p117">Many elements on the page can be updated, but each element type supports specific actions. The following table shows supported target elements and the update actions that they support.</span></span>

| <span data-ttu-id="f685e-194">要素</span><span class="sxs-lookup"><span data-stu-id="f685e-194">Element</span></span> | <span data-ttu-id="f685e-195">置換</span><span class="sxs-lookup"><span data-stu-id="f685e-195">Replace</span></span> | <span data-ttu-id="f685e-196">子の追加</span><span class="sxs-lookup"><span data-stu-id="f685e-196">Append child</span></span> | <span data-ttu-id="f685e-197">兄弟の挿入</span><span class="sxs-lookup"><span data-stu-id="f685e-197">Insert sibling</span></span> |  
|------|:------:|:------:|:------:|  
| <span data-ttu-id="f685e-198">本文</span><span class="sxs-lookup"><span data-stu-id="f685e-198">body</span></span><br /> <span data-ttu-id="f685e-199">(ページの最初の div をターゲットとする)</span><span class="sxs-lookup"><span data-stu-id="f685e-199">(targets first div on the page)</span></span> | <span data-ttu-id="f685e-200">いいえ</span><span class="sxs-lookup"><span data-stu-id="f685e-200">no</span></span> | <span data-ttu-id="f685e-201">**はい**</span><span class="sxs-lookup"><span data-stu-id="f685e-201">**yes**</span></span> | <span data-ttu-id="f685e-202">いいえ</span><span class="sxs-lookup"><span data-stu-id="f685e-202">no</span></span> |  
| <span data-ttu-id="f685e-203">div</span><span class="sxs-lookup"><span data-stu-id="f685e-203">div</span></span><br /> <span data-ttu-id="f685e-204">([絶対配置](onenote-abs-pos.md))</span><span class="sxs-lookup"><span data-stu-id="f685e-204">([absolute positioned](onenote-abs-pos.md))</span></span> | <span data-ttu-id="f685e-205">いいえ</span><span class="sxs-lookup"><span data-stu-id="f685e-205">no</span></span> | <span data-ttu-id="f685e-206">**はい**</span><span class="sxs-lookup"><span data-stu-id="f685e-206">**yes**</span></span> | <span data-ttu-id="f685e-207">いいえ</span><span class="sxs-lookup"><span data-stu-id="f685e-207">no</span></span> |  
| <span data-ttu-id="f685e-208">div</span><span class="sxs-lookup"><span data-stu-id="f685e-208">div</span></span><br /> <span data-ttu-id="f685e-209">(div 内)</span><span class="sxs-lookup"><span data-stu-id="f685e-209">(within a div)</span></span> | <span data-ttu-id="f685e-210">**はい**</span><span class="sxs-lookup"><span data-stu-id="f685e-210">**yes**</span></span><br/><span data-ttu-id="f685e-211">(id のみ)</span><span class="sxs-lookup"><span data-stu-id="f685e-211">(id only)</span></span> | <span data-ttu-id="f685e-212">**はい**</span><span class="sxs-lookup"><span data-stu-id="f685e-212">**yes**</span></span> | <span data-ttu-id="f685e-213">**はい**</span><span class="sxs-lookup"><span data-stu-id="f685e-213">**yes**</span></span> |   
| <span data-ttu-id="f685e-214">img、object</span><span class="sxs-lookup"><span data-stu-id="f685e-214">img, object</span></span><br /> <span data-ttu-id="f685e-215">(div 内)</span><span class="sxs-lookup"><span data-stu-id="f685e-215">(within a div)</span></span> | <span data-ttu-id="f685e-216">**はい**</span><span class="sxs-lookup"><span data-stu-id="f685e-216">**yes**</span></span> | <span data-ttu-id="f685e-217">いいえ</span><span class="sxs-lookup"><span data-stu-id="f685e-217">no</span></span> | <span data-ttu-id="f685e-218">**はい**</span><span class="sxs-lookup"><span data-stu-id="f685e-218">**yes**</span></span> |   
| <span data-ttu-id="f685e-219">ol、ul</span><span class="sxs-lookup"><span data-stu-id="f685e-219">ol, ul</span></span> | <span data-ttu-id="f685e-220">**はい**</span><span class="sxs-lookup"><span data-stu-id="f685e-220">**yes**</span></span><br/><span data-ttu-id="f685e-221">(id のみ)</span><span class="sxs-lookup"><span data-stu-id="f685e-221">(id only)</span></span> | <span data-ttu-id="f685e-222">**はい**</span><span class="sxs-lookup"><span data-stu-id="f685e-222">**yes**</span></span> | <span data-ttu-id="f685e-223">**はい**</span><span class="sxs-lookup"><span data-stu-id="f685e-223">**yes**</span></span> |   
| <span data-ttu-id="f685e-224">テーブル</span><span class="sxs-lookup"><span data-stu-id="f685e-224">table</span></span> | <span data-ttu-id="f685e-225">**はい**</span><span class="sxs-lookup"><span data-stu-id="f685e-225">**yes**</span></span><br/><span data-ttu-id="f685e-226">(id のみ)</span><span class="sxs-lookup"><span data-stu-id="f685e-226">(id only)</span></span> | <span data-ttu-id="f685e-227">いいえ</span><span class="sxs-lookup"><span data-stu-id="f685e-227">no</span></span> | <span data-ttu-id="f685e-228">**はい**</span><span class="sxs-lookup"><span data-stu-id="f685e-228">**yes**</span></span> |   
| <span data-ttu-id="f685e-229">p、li、h1-h6</span><span class="sxs-lookup"><span data-stu-id="f685e-229">p, li, h1-h6</span></span> | <span data-ttu-id="f685e-230">**はい**</span><span class="sxs-lookup"><span data-stu-id="f685e-230">**yes**</span></span><br/><span data-ttu-id="f685e-231">(id のみ)</span><span class="sxs-lookup"><span data-stu-id="f685e-231">(id only)</span></span> | <span data-ttu-id="f685e-232">いいえ</span><span class="sxs-lookup"><span data-stu-id="f685e-232">no</span></span> | <span data-ttu-id="f685e-233">**はい**</span><span class="sxs-lookup"><span data-stu-id="f685e-233">**yes**</span></span> |   
| <span data-ttu-id="f685e-234">タイトル</span><span class="sxs-lookup"><span data-stu-id="f685e-234">title</span></span> | <span data-ttu-id="f685e-235">**はい**</span><span class="sxs-lookup"><span data-stu-id="f685e-235">**yes**</span></span> | <span data-ttu-id="f685e-236">いいえ</span><span class="sxs-lookup"><span data-stu-id="f685e-236">no</span></span> | <span data-ttu-id="f685e-237">いいえ</span><span class="sxs-lookup"><span data-stu-id="f685e-237">no</span></span> |  
 
<br/>

<span data-ttu-id="f685e-238">次の要素では更新アクションはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f685e-238">The following elements do not support any update actions.</span></span>

- <span data-ttu-id="f685e-239">img ([絶対配置](onenote-abs-pos.md))</span><span class="sxs-lookup"><span data-stu-id="f685e-239">img ([absolute positioned](onenote-abs-pos.md))</span></span>
- <span data-ttu-id="f685e-240">object ([絶対配置](onenote-abs-pos.md))</span><span class="sxs-lookup"><span data-stu-id="f685e-240">object ([absolute positioned](onenote-abs-pos.md))</span></span>
- <span data-ttu-id="f685e-241">tr、td</span><span class="sxs-lookup"><span data-stu-id="f685e-241">tr, td</span></span>
- <span data-ttu-id="f685e-242">メタ</span><span class="sxs-lookup"><span data-stu-id="f685e-242">meta</span></span>
- <span data-ttu-id="f685e-243">見出し</span><span class="sxs-lookup"><span data-stu-id="f685e-243">head</span></span>
- <span data-ttu-id="f685e-244">スパン</span><span class="sxs-lookup"><span data-stu-id="f685e-244">span</span></span>
- <span data-ttu-id="f685e-245">a</span><span class="sxs-lookup"><span data-stu-id="f685e-245">a</span></span>
- <span data-ttu-id="f685e-246">style タグ</span><span class="sxs-lookup"><span data-stu-id="f685e-246">style tags</span></span>


<a name="examples"></a>

## <a name="example-requests"></a><span data-ttu-id="f685e-247">要求の例</span><span class="sxs-lookup"><span data-stu-id="f685e-247">Example requests</span></span>

<span data-ttu-id="f685e-p118">更新要求には、JSON 変更オブジェクトとして表現される変更が 1 つ以上含まれています。これらのオブジェクトでは、ページ上のさまざまなターゲットや、ターゲットに対するさまざまなアクションとコンテンツを定義できます。</span><span class="sxs-lookup"><span data-stu-id="f685e-p118">An update request contains one or more changes represented as JSON change objects. These objects can define different targets on the page and different actions and content for the targets.</span></span>

<span data-ttu-id="f685e-250">次の例に、PATCH 要求で使用される JSON オブジェクトと完全な PATCH 要求を示します。</span><span class="sxs-lookup"><span data-stu-id="f685e-250">The following examples include JSON objects used in PATCH requests and complete PATCH requests:</span></span>

- [<span data-ttu-id="f685e-251">子要素の追加</span><span class="sxs-lookup"><span data-stu-id="f685e-251">Append child elements</span></span>](#append-child-elements)
- [<span data-ttu-id="f685e-252">兄弟要素の挿入</span><span class="sxs-lookup"><span data-stu-id="f685e-252">Insert sibling elements</span></span>](#insert-sibling-elements)
- [<span data-ttu-id="f685e-253">要素の置換</span><span class="sxs-lookup"><span data-stu-id="f685e-253">Replace elements</span></span>](#replace-elements)
- [<span data-ttu-id="f685e-254">完全な PATCH 要求</span><span class="sxs-lookup"><span data-stu-id="f685e-254">Complete PATCH requests</span></span>](#complete-patch-request-examples)


<a name="append-examples"></a>

### <a name="append-child-elements"></a><span data-ttu-id="f685e-255">子要素の追加</span><span class="sxs-lookup"><span data-stu-id="f685e-255">Append child elements</span></span>

<span data-ttu-id="f685e-p119">**append** アクションでは、**body**、**div** (div 内)、**ol**、**ul** 要素に子が追加されます。**position** 属性により、ターゲットの前または後に子を追加することが決定されます。既定の位置は**後**です。</span><span class="sxs-lookup"><span data-stu-id="f685e-p119">The **append** action adds a child to a **body**, **div** (within a div), **ol**, or **ul** element. The **position** attribute determines whether to append the child before or after the target. The default position is **after**.</span></span>

#### <a name="append-to-a-div"></a><span data-ttu-id="f685e-259">div への追加</span><span class="sxs-lookup"><span data-stu-id="f685e-259">Append to a div</span></span>

<span data-ttu-id="f685e-p120">次の例では、2 つの子ノードが **div1** 要素に追加されます。画像が最初の子として追加され、段落が 2 番目の子として追加されます。</span><span class="sxs-lookup"><span data-stu-id="f685e-p120">The following example adds two child nodes to the **div1** element. It adds an image as the first child and a paragraph as the last child.</span></span> 

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
 

#### <a name="append-to-the-body-element"></a><span data-ttu-id="f685e-262">*body* 要素への追加</span><span class="sxs-lookup"><span data-stu-id="f685e-262">Append to the *body* element</span></span>

<span data-ttu-id="f685e-263">**body** は、任意のページ上の最初の div 内に子要素を追加するためのショートカットとして使用できます。</span><span class="sxs-lookup"><span data-stu-id="f685e-263">You can use the **body** shortcut to append a child element inside the first div on any page.</span></span>

<span data-ttu-id="f685e-p121">次の例では、ページの最初の div に 2 つの段落を最初の子と最後の子として追加しています。**body** ターゲットと共に # を使用しないでください。この例では、**prepend** アクションを **append** + **before** のショートカットとして使用しています。</span><span class="sxs-lookup"><span data-stu-id="f685e-p121">The following example adds two paragraphs as the first child and the last child to the first div on the page. Don't use a # with the **body** target. This example uses the **prepend** action as a shortcut for **append** + **before**.</span></span>

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
 

#### <a name="append-to-a-list"></a><span data-ttu-id="f685e-267">リストへの追加</span><span class="sxs-lookup"><span data-stu-id="f685e-267">Append to a list</span></span>

<span data-ttu-id="f685e-p122">次の例では、リスト項目がターゲット リストに最後の子として追加されます。この項目では既定以外のリスト スタイルが使用されるため、**list-style-type** プロパティが定義されます。</span><span class="sxs-lookup"><span data-stu-id="f685e-p122">The following example adds a list item as a last child to the target list. The **list-style-type** property is defined because the item uses a non-default list style.</span></span>

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

### <a name="insert-sibling-elements"></a><span data-ttu-id="f685e-270">兄弟要素の挿入</span><span class="sxs-lookup"><span data-stu-id="f685e-270">Insert sibling elements</span></span>

<span data-ttu-id="f685e-p123">**insert** アクションでは、兄弟がターゲット要素に追加されます。**position** 属性により、ターゲットの前または後に兄弟を挿入することが決定されます。既定の位置は**後**です。「[**insert** をサポートする要素](#supported-elements-and-actions)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="f685e-p123">The **insert** action adds a sibling to the target element. The **position** attribute determines whether to insert the sibling before or after the target. The default position is **after**. See [elements that support **insert**](#supported-elements-and-actions).</span></span>

#### <a name="insert-siblings"></a><span data-ttu-id="f685e-275">兄弟の挿入</span><span class="sxs-lookup"><span data-stu-id="f685e-275">Insert siblings</span></span>

<span data-ttu-id="f685e-p124">次の例では、ページに 2 つの兄弟ノードが挿入されます。**para1** 要素の上に画像が追加され、**para2** 要素の下に段落が追加されます。</span><span class="sxs-lookup"><span data-stu-id="f685e-p124">The following example adds two sibling nodes to the page. It adds an image above the **para1** element and a paragraph below the **para2** element.</span></span>

```json
[
  {
     'target':'#para1',
     'action':'insert',
     'position':'before',
     'content':'<img src="image-url-or-part-name" alt="Image inserted above the target" />'
  },
  {
    'target':'#para2',
     'action':'insert',
     'content':'<p data-id="next-sibling">Paragraph inserted below the target</p>'
  }
]
```
 

<a name="replace-examples"></a>

### <a name="replace-elements"></a><span data-ttu-id="f685e-278">要素の置換</span><span class="sxs-lookup"><span data-stu-id="f685e-278">Replace elements</span></span>

<span data-ttu-id="f685e-p125">**data-id** と生成された **id** のいずれかをターゲット値として使用し、div 内にある **img** 要素および **object** 要素を置換できます。ページ タイトルを置換する場合は、**title** キーワードを使用します。[**replace** をサポートするその他すべての要素](#supported-elements-and-actions)については、生成された ID を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f685e-p125">You can use either the **data-id** or generated **id** as the target value to replace **img** and **object** elements that are within a div. To replace the page title, use the **title** keyword. For all other [elements that support **replace**](#supported-elements-and-actions), you must use the generated ID.</span></span>

#### <a name="replace-an-image"></a><span data-ttu-id="f685e-282">画像の置換</span><span class="sxs-lookup"><span data-stu-id="f685e-282">Replace an image</span></span>

<span data-ttu-id="f685e-283">次の例では、画像の **data-id** をターゲットとして使用して、div 内の画像が置換されます。</span><span class="sxs-lookup"><span data-stu-id="f685e-283">The following example replaces an image with a div by using the image's **data-id** as the target.</span></span> 

```json
[
  {
    'target':'#img1',
    'action':'replace',
    'content':'<div data-id="new-div"><p>This div replaces the image</p></div>'
  }
]
```
 

#### <a name="update-a-table"></a><span data-ttu-id="f685e-284">表の更新</span><span class="sxs-lookup"><span data-stu-id="f685e-284">Update a table</span></span> 

<span data-ttu-id="f685e-p126">次の例は、生成された ID を使用して表を更新する方法を示します。**tr** 要素と **td** 要素の置換はサポートされていませんが、表全体を置換することができます。</span><span class="sxs-lookup"><span data-stu-id="f685e-p126">This example shows how to update a table by using its generated ID. Replacing **tr** and **td** elements is not supported, but you can replace the entire table.</span></span>

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
 

#### <a name="change-the-title"></a><span data-ttu-id="f685e-287">タイトルの変更</span><span class="sxs-lookup"><span data-stu-id="f685e-287">Change the title</span></span> 

<span data-ttu-id="f685e-p127">次の例は、ページのタイトルを変更する方法を示します。タイトルを変更するには、ターゲット値として **title** キーワードを使用します。title ターゲットでは # は使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="f685e-p127">This example shows how to change the title of a page. To change the title, use the **title** keyword as the target value. Don't use a # with the title target.</span></span>

```json
[
  {
    'target':'title',
    'action':'replace',
    'content':'New title'
  }
]
```
 

#### <a name="update-a-to-do-item"></a><span data-ttu-id="f685e-291">To Do アイテムの更新</span><span class="sxs-lookup"><span data-stu-id="f685e-291">Update a to-do item</span></span>

<span data-ttu-id="f685e-292">次に示す例では、replace アクションを使用して、To Do チェック ボックス アイテムを完了状態に変更します。</span><span class="sxs-lookup"><span data-stu-id="f685e-292">The following example uses the replace action to change a to-do check box item to a completed state.</span></span>

```json
[
  {
    'target':'#task1',
    'action':'replace',
    'content':'<p data-tag="to-do:completed" data-id="task1">First task</p>'
  }
]
```

<span data-ttu-id="f685e-293">**data-tag** 属性の使用法の詳細については、「[ノート シールを使用する](onenote-note-tags.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f685e-293">See [Use note tags](onenote-note-tags.md) for more about using the **data-tag** attribute.</span></span>


<a name="complete-requests"></a>

### <a name="complete-patch-request-examples"></a><span data-ttu-id="f685e-294">完全な PATCH 要求の例</span><span class="sxs-lookup"><span data-stu-id="f685e-294">Complete PATCH request examples</span></span>

<span data-ttu-id="f685e-295">次の例に、完全な PATCH 要求を示します。</span><span class="sxs-lookup"><span data-stu-id="f685e-295">The following examples show complete PATCH requests.</span></span>

#### <a name="request-with-text-content-only"></a><span data-ttu-id="f685e-296">テキスト コンテンツのみの要求</span><span class="sxs-lookup"><span data-stu-id="f685e-296">Request with text content only</span></span>

<span data-ttu-id="f685e-p128">次の例は、**application/json** コンテンツ タイプを使用する PATCH 要求を示しています。コンテンツにバイナリ データが含まれていない場合にこの形式を使用できます。</span><span class="sxs-lookup"><span data-stu-id="f685e-p128">The following example shows a PATCH request that uses the **application/json** content type. You can use this format when your content doesn't contain binary data.</span></span>

```json
PATCH https://graph.microsoft.com/v1.0/me/onenote/notebooks/pages/{page-id}/content

Content-Type: application/json
Authorization: Bearer {token}

[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-url" alt="New image from a URL" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>Item at the bottom of the list</li>'
  }
]
```
 
<a name="multipart"></a>

#### <a name="multipart-request-with-binary-content"></a><span data-ttu-id="f685e-299">バイナリ コンテンツを含むマルチパート要求</span><span class="sxs-lookup"><span data-stu-id="f685e-299">Multipart request with binary content</span></span> 

<span data-ttu-id="f685e-p129">次の例は、バイナリ データを含んでいるマルチパート PATCH 要求を示しています。マルチパート要求には、**application/json** コンテンツ タイプを指定し、JSON 変更オブジェクトの配列を含める "Commands" 部分が必要になります。その他のデータ部分に、バイナリ データを含めることができます。部分の名前は、通常、ミリ秒単位での現在の時刻、またはランダムな GUID が付加された文字列になります。</span><span class="sxs-lookup"><span data-stu-id="f685e-p129">The following example shows a multipart PATCH request that includes binary data. Multipart requests require a "Commands" part that specifies the **application/json** content type and contains the array of JSON change objects. Other data parts can contain binary data. Part names typically are strings appended with the current time in milliseconds or a random GUID.</span></span>

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

## <a name="request-and-response-information-for-patch-requests"></a><span data-ttu-id="f685e-304">PATCH 要求の要求情報と応答情報</span><span class="sxs-lookup"><span data-stu-id="f685e-304">Request and response information for PATCH requests</span></span>

| <span data-ttu-id="f685e-305">要求データ</span><span class="sxs-lookup"><span data-stu-id="f685e-305">Request data</span></span> | <span data-ttu-id="f685e-306">説明</span><span class="sxs-lookup"><span data-stu-id="f685e-306">Description</span></span> |  
|------|------|  
| <span data-ttu-id="f685e-307">プロトコル</span><span class="sxs-lookup"><span data-stu-id="f685e-307">Protocol</span></span> | <span data-ttu-id="f685e-308">すべての要求は SSL/TLS HTTPS プロトコルを使用します。</span><span class="sxs-lookup"><span data-stu-id="f685e-308">All requests use the SSL/TLS HTTPS protocol.</span></span> |  
| <span data-ttu-id="f685e-309">承認ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f685e-309">Authorization header</span></span> | <p><span data-ttu-id="f685e-310">`Bearer {token}`。`{token}` は、登録済みアプリの有効な OAuth 2.0 アクセス トークンです。</span><span class="sxs-lookup"><span data-stu-id="f685e-310">`Bearer {token}`, where `{token}` is a valid OAuth 2.0 access token for your registered app.</span></span></p><p><span data-ttu-id="f685e-p130">これがないか、無効の場合、401 ステータス コードで要求は失敗します。「[認証とアクセス許可](permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f685e-p130">If missing or invalid, the request fails with a 401 status code. See [Authentication and permissions](permissions_reference.md).</span></span></p> |  
| <span data-ttu-id="f685e-313">Content-Type ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f685e-313">Content-Type header</span></span> | <p><span data-ttu-id="f685e-314">`application/json` JSON 変更オブジェクトの配列の `application/json`。メッセージ本文または[マルチパート要求](#multipart-request-with-binary-content)の必須の "Commands" パートで直接送信。</span><span class="sxs-lookup"><span data-stu-id="f685e-314">`application/json` for the array of JSON change objects, whether sent directly in the message body or in the required "Commands" part of [multipart requests](#multipart-request-with-binary-content).</span></span></p><p><span data-ttu-id="f685e-315">マルチパート要求はバイナリ データを送信するときに必須であり、コンテンツ タイプとして `multipart/form-data; boundary=part-boundary` を使用します。`{part-boundary}` は、各データ パートの開始と終了を伝える文字列です。</span><span class="sxs-lookup"><span data-stu-id="f685e-315">Multipart requests are required when sending binary data, and use the `multipart/form-data; boundary=part-boundary` content type, where `{part-boundary}` is a string that signals the start and end of each data part.</span></span></p> |  

<br/> 

| <span data-ttu-id="f685e-316">応答データ</span><span class="sxs-lookup"><span data-stu-id="f685e-316">Response data</span></span> | <span data-ttu-id="f685e-317">説明</span><span class="sxs-lookup"><span data-stu-id="f685e-317">Description</span></span> |  
|------|------|  
| <span data-ttu-id="f685e-318">成功コード</span><span class="sxs-lookup"><span data-stu-id="f685e-318">Success code</span></span> | <span data-ttu-id="f685e-p131">204 HTTP ステータス コード。PATCH 要求に対して JSON データは返されません。</span><span class="sxs-lookup"><span data-stu-id="f685e-p131">A 204 HTTP status code. No JSON data is returned for a PATCH request.</span></span> |  
| <span data-ttu-id="f685e-321">エラー</span><span class="sxs-lookup"><span data-stu-id="f685e-321">Errors</span></span> | <span data-ttu-id="f685e-322">Microsoft Graph から返されることのある OneNote エラーに関する詳細については、「[Microsoft Graph の OneNote API のエラー コード](onenote_error_codes.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="f685e-322">Read [Error codes for OneNote APIs in Microsoft Graph](onenote_error_codes.md) to learn about OneNote errors that Microsoft Graph can return.</span></span> |  
 
 

<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-service-root-url"></a><span data-ttu-id="f685e-323">Microsoft Graph サービスのルート URL の構築</span><span class="sxs-lookup"><span data-stu-id="f685e-323">Constructing the Microsoft Graph service root URL</span></span>

<span data-ttu-id="f685e-324">OneNote サービスのルート URL は、OneNote API へのすべての呼び出しで次の形式を使用します。</span><span class="sxs-lookup"><span data-stu-id="f685e-324">The OneNote service root URL uses the following format for all calls to the OneNote API:</span></span>

`https://graph.microsoft.com/{version}/me/onenote/`

<span data-ttu-id="f685e-325">URL の `version` セグメントは、使用する Microsoft Graph のバージョンを示しています。</span><span class="sxs-lookup"><span data-stu-id="f685e-325">The `version` segment in the URL represents the version of Microsoft Graph that you want to use.</span></span> <span data-ttu-id="f685e-326">`v1.0` 安定した運用コードには `v1.0` を使用します。</span><span class="sxs-lookup"><span data-stu-id="f685e-326">`v1.0` is for stable production code.</span></span> <span data-ttu-id="f685e-327">`beta` 開発中の機能を試すには `beta` を使用します。</span><span class="sxs-lookup"><span data-stu-id="f685e-327">`beta` is to try out a feature that's in development.</span></span> <span data-ttu-id="f685e-328">ベータ版の機能は変更される可能性があるため、運用コードでは使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="f685e-328">Features and functionality in beta may change, so you shouldn't use it in your production code.</span></span>

<span data-ttu-id="f685e-329">`me` 現在のユーザーがアクセスできる OneNote コンテンツには `me` を使用します (所有と共有)。</span><span class="sxs-lookup"><span data-stu-id="f685e-329">`me` is for OneNote content that the current user can access (owned and shared).</span></span> <span data-ttu-id="f685e-330">`users/{id}` 指定されたユーザー (URL 内) が現在のユーザーと共有している OneNote コンテンツには `users/{id}` を使用します。</span><span class="sxs-lookup"><span data-stu-id="f685e-330">`users/{id}` is for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="f685e-331">[Azure AD Graph API](https://msdn.microsoft.com/library/azure/ad/graph/api/api-catalog) の使用。</span><span class="sxs-lookup"><span data-stu-id="f685e-331">Use the [Azure AD Graph API](https://msdn.microsoft.com/library/azure/ad/graph/api/api-catalog).</span></span>


> <span data-ttu-id="f685e-332">**注:** `https://graph.microsoft.com/v1.0/users`で GET 要求を行うことにより、ユーザー ID を取得できます。</span><span class="sxs-lookup"><span data-stu-id="f685e-332">**Note:** You can get user ids by making a GET request on `https://graph.microsoft.com/v1.0/users`.</span></span>



<a name="permissions"></a>

## <a name="permissions"></a><span data-ttu-id="f685e-333">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f685e-333">Permissions</span></span>

<span data-ttu-id="f685e-p134">OneNote ページを更新するには、適切なアクセス許可を要求する必要があります。アプリの動作に必要な最低限のアクセス許可を選択してください。</span><span class="sxs-lookup"><span data-stu-id="f685e-p134">To update OneNote pages, you'll need to request appropriate permissions. Choose the lowest level of permissions that your app needs to do its work.</span></span>

- <span data-ttu-id="f685e-336">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f685e-336">Notes.ReadWrite</span></span>
- <span data-ttu-id="f685e-337">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f685e-337">Notes.ReadWrite.All</span></span>

<span data-ttu-id="f685e-338">アクセス許可のスコープと動作のしくみの詳細については、「[OneNote のアクセス許可のスコープ](permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f685e-338">For more information about permission scopes and how they work, see [OneNote permission scopes](permissions_reference.md).</span></span>
   

<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="f685e-339">関連項目</span><span class="sxs-lookup"><span data-stu-id="f685e-339">See also</span></span>

- [<span data-ttu-id="f685e-340">画像とファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="f685e-340">Add images and files</span></span>](onenote_images_files.md)
- [<span data-ttu-id="f685e-341">OneNote との統合</span><span class="sxs-lookup"><span data-stu-id="f685e-341">Integrate with OneNote</span></span>](integrate_with_onenote.md)
- [<span data-ttu-id="f685e-342">OneNote の開発者ブログ</span><span class="sxs-lookup"><span data-stu-id="f685e-342">OneNote Developer Blog</span></span>](http://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="f685e-343">Stack Overflow 掲載の OneNote の開発に関する質問</span><span class="sxs-lookup"><span data-stu-id="f685e-343">OneNote development questions on Stack Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="f685e-344">OneNote GitHub のリポジトリ</span><span class="sxs-lookup"><span data-stu-id="f685e-344">OneNote GitHub repos</span></span>](http://go.microsoft.com/fwlink/?LinkID=390178)  
