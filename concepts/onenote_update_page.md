# <a name="update-onenote-page-content"></a><span data-ttu-id="3342e-101">OneNote ページ コンテンツを更新する</span><span class="sxs-lookup"><span data-stu-id="3342e-101">Update OneNote page content</span></span>

<span data-ttu-id="3342e-102">*__適用対象:__ OneDrive のコンシューマー ノートブック | Office 365 のエンタープライズ ノートブック*</span><span class="sxs-lookup"><span data-stu-id="3342e-102">*__Applies to:__ Consumer notebooks on OneDrive | Enterprise notebooks on Office 365*</span></span>


<span data-ttu-id="3342e-103">OneNote ページのコンテンツを更新する場合は、ページの *content* エンドポイントに PATCH 要求を送信します。</span><span class="sxs-lookup"><span data-stu-id="3342e-103">To update the content of a OneNote page, you send a PATCH request to the page's *content* endpoint:</span></span>

`PATCH ../notes/pages/{id}/content`</p>

<span data-ttu-id="3342e-104">メッセージの本文で JSON 変更オブジェクトを送信します。</span><span class="sxs-lookup"><span data-stu-id="3342e-104">Send a JSON change object in the message body.</span></span> <span data-ttu-id="3342e-105">要求が成功すると、Microsoft Graph は 204 HTTP 状態コードを返します。</span><span class="sxs-lookup"><span data-stu-id="3342e-105">If the request is successful, the OneNote API returns a 204 HTTP status code.</span></span>


<a name="request-uri"></a>
## <a name="construct-the-request-uri"></a><span data-ttu-id="3342e-106">要求 URI の構築</span><span class="sxs-lookup"><span data-stu-id="3342e-106">Construct the request URI</span></span>

<span data-ttu-id="3342e-107">要求 URI を構築するには、サービス ルート URL から開始します。</span><span class="sxs-lookup"><span data-stu-id="3342e-107">To construct the request URI, start with the service root URL:</span></span>

`https://graph.microsoft.com/v1.0/me/onenote`

<span data-ttu-id="3342e-108">次に、ページの *content* エンドポイントを追加します。</span><span class="sxs-lookup"><span data-stu-id="3342e-108">Then append the page's *content* endpoint:</span></span>

<span data-ttu-id="3342e-109">**ページ HTML と、すべての定義済み *data-id* の値を取得する**</span><span class="sxs-lookup"><span data-stu-id="3342e-109">**Get the page HTML and all defined *data-id* values**</span></span></p>
`../pages/{id}/content`   

<span data-ttu-id="3342e-110">**ページ HTML、すべての定義済み *data-id* の値、およびすべての生成された *id* の値を取得する**</span><span class="sxs-lookup"><span data-stu-id="3342e-110">**Get the page HTML, all defined *data-id* values, and all generated *id* values**</span></span>  
`../pages/{page-id}/content?includeIDs=true` 

<span data-ttu-id="3342e-111">**data-id** と **id** の値は、更新する要素の **target** 識別子として使用されます。</span><span class="sxs-lookup"><span data-stu-id="3342e-111">The **data-id** and **id** values are used as **target** identifiers for the elements you want to update.</span></span>

 
<span data-ttu-id="3342e-112">完全な要求 URI は、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="3342e-112">Your full request URI will look like one of these:</span></span>

`https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/content`


<span data-ttu-id="3342e-113">[サービス ルート URL](../api-reference/v1.0/resources/onenote-api-overview.md#root-url) の詳細についてはリンク先をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="3342e-113">Learn more about the [service root URL](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span></span>


<a name="message-body"></a>
## <a name="construct-the-message-body"></a><span data-ttu-id="3342e-114">メッセージ本文の構築</span><span class="sxs-lookup"><span data-stu-id="3342e-114">Construct the message body</span></span>

<span data-ttu-id="3342e-115">OneNote ページの HTML には、**div** 要素、**img** 要素、**ol** 要素などの構造に編成されたテキスト、画像などのコンテンツが含まれています。</span><span class="sxs-lookup"><span data-stu-id="3342e-115">The HTML of a OneNote page contains text, images, and other content organized into structures such as **div**, **img**, and **ol** elements.</span></span> <span data-ttu-id="3342e-116">OneNote ページのコンテンツを更新する場合は、ページ上で HTML 要素を追加および置換します。</span><span class="sxs-lookup"><span data-stu-id="3342e-116">To update OneNote page content, you add and replace HTML elements on the page.</span></span>

<span data-ttu-id="3342e-p103">変更内容は JSON 変更オブジェクトの配列としてメッセージ本文に入れて送信します。ターゲット要素、新しい HTML コンテンツ、コンテンツに対する操作が各オブジェクトにより指定されます。</span><span class="sxs-lookup"><span data-stu-id="3342e-p103">Your changes are sent in the message body as an array of JSON change objects. Each object specifies the target element, new HTML content, and what to do with the content.</span></span>

<span data-ttu-id="3342e-p104">2 つの変更を定義する配列を次に示します。最初の変更では画像が兄弟として段落の上に挿入され、2 番目の変更ではアイテムが最後の子としてリストに追加されます。</span><span class="sxs-lookup"><span data-stu-id="3342e-p104">The following array defines two changes. The first inserts an image above a paragraph as a sibling, and the second appends an item to a list as a last child.</span></span>

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

<span data-ttu-id="3342e-121">[その他の例](#example-requests)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3342e-121">See [more examples](#example-requests).</span></span>


### <a name="attributes-for-json-change-objects"></a><span data-ttu-id="3342e-122">JSON 変更オブジェクトの属性</span><span class="sxs-lookup"><span data-stu-id="3342e-122">Attributes for JSON change objects</span></span>

<span data-ttu-id="3342e-123">PATCH 要求の JSON オブジェクトの定義には、**target** 属性、**action** 属性、**position** 属性、**content** 属性を使用します。</span><span class="sxs-lookup"><span data-stu-id="3342e-123">Use the **target**, **action**, **position**, and **content** attributes to define JSON objects for PATCH requests.</span></span>

<span data-ttu-id="3342e-124">**target**</span><span class="sxs-lookup"><span data-stu-id="3342e-124">**target**</span></span>  
<span data-ttu-id="3342e-p105">更新する要素。値として次の ID のいずれかを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3342e-p105">The element to update. The value must be one of the following identifiers:</span></span>

| <span data-ttu-id="3342e-127">Identifier</span><span class="sxs-lookup"><span data-stu-id="3342e-127">Identifier</span></span> | <span data-ttu-id="3342e-128">説明</span><span class="sxs-lookup"><span data-stu-id="3342e-128">Description</span></span> |  
|------|------|  
| <span data-ttu-id="3342e-129">#{data-id}</span><span class="sxs-lookup"><span data-stu-id="3342e-129">#{data-id}</span></span> | <p><span data-ttu-id="3342e-130">この ID は、[ページを作成](onenote-create-page.md)するときや[更新](onenote_update_page.md)するときに、入力 HTML の要素で任意で定義されます。</span><span class="sxs-lookup"><span data-stu-id="3342e-130">This ID is optionally defined on elements in the input HTML when [creating a page](onenote-create-page.md) or [updating a page](onenote_update_page.md).</span></span> <span data-ttu-id="3342e-131">値の先頭に # を付けます。</span><span class="sxs-lookup"><span data-stu-id="3342e-131">Prefix the value with a #.</span></span></p><p> <span data-ttu-id="3342e-132">例: `'target':'#intro'` は要素 `<div data-id="intro" ...>` をターゲットとします</span><span class="sxs-lookup"><span data-stu-id="3342e-132">Example: `'target':'#intro'` targets the element `<div data-id="intro" ...>`</span></span></p> |  
| <span data-ttu-id="3342e-133">id</span><span class="sxs-lookup"><span data-stu-id="3342e-133">id</span></span> | <p><span data-ttu-id="3342e-134">これは、Microsoft Graph から得られる[生成済み ID](#generated-ids) であり、ほとんどの置換操作で必要になります。</span><span class="sxs-lookup"><span data-stu-id="3342e-134">This is the [generated ID](#generated-ids) from the OneNote API, and is required for most replace operations.</span></span> <span data-ttu-id="3342e-135">プレフィックス # を追加しないでください。</span><span class="sxs-lookup"><span data-stu-id="3342e-135">Do not prefix with a #.</span></span></p><p> <span data-ttu-id="3342e-136">例: `'target':'div:{33f8a2...}{37}'` は要素 `<div id="div:{33f8a2...}{37}" ...>` をターゲットとします</span><span class="sxs-lookup"><span data-stu-id="3342e-136">Example: `'target':'div:{33f8a2...}{37}'` targets the element `<div id="div:{33f8a2...}{37}" ...>`</span></span></p><p><span data-ttu-id="3342e-137">[入力 HTML](onenote_input_output_html.md) に定義されている **id** 値とこれらを混同しないでください。</span><span class="sxs-lookup"><span data-stu-id="3342e-137">Don't confuse these with any **id** values defined in the [input HTML](onenote_input_output_html.md).</span></span> <span data-ttu-id="3342e-138">入力 HTML で送信される **id** 値は、すべて破棄されます。</span><span class="sxs-lookup"><span data-stu-id="3342e-138">All **id** values sent in the input HTML are discarded.</span></span></p> |  
| <span data-ttu-id="3342e-139">body</span><span class="sxs-lookup"><span data-stu-id="3342e-139">body</span></span> | <span data-ttu-id="3342e-p109">ページ上で最初の div をターゲットにするキーワード。プレフィックス # を追加してはいけません。</span><span class="sxs-lookup"><span data-stu-id="3342e-p109">The keyword that targets the first div on the page. Do not prefix with a #.</span></span> |  
| <span data-ttu-id="3342e-142">title</span><span class="sxs-lookup"><span data-stu-id="3342e-142">title</span></span> | <span data-ttu-id="3342e-p110">ページ タイトルをターゲットにするキーワード。プレフィックス # を追加してはなりません。</span><span class="sxs-lookup"><span data-stu-id="3342e-p110">The keyword that targets the page title. Do not prefix with a #.</span></span> |  
 
<span data-ttu-id="3342e-145">**action**</span><span class="sxs-lookup"><span data-stu-id="3342e-145">**action**</span></span>  
<span data-ttu-id="3342e-146">ターゲット要素で実行するアクション。</span><span class="sxs-lookup"><span data-stu-id="3342e-146">The action to perform on the target element.</span></span> <span data-ttu-id="3342e-147">「[サポートされる要素とアクション](#supported-elements-and-actions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3342e-147">See [supported actions for elements](#supported-elements-and-actions).</span></span>

| <span data-ttu-id="3342e-148">アクション</span><span class="sxs-lookup"><span data-stu-id="3342e-148">Action</span></span> | <span data-ttu-id="3342e-149">説明</span><span class="sxs-lookup"><span data-stu-id="3342e-149">Description</span></span> |  
|------|------|  
| <span data-ttu-id="3342e-150">append</span><span class="sxs-lookup"><span data-stu-id="3342e-150">append</span></span> | <p><span data-ttu-id="3342e-151">指定されたコンテンツを最初または最後の子としてターゲットに追加します。追加される位置 (最初または最後) は、**position** 属性によって決まります。</span><span class="sxs-lookup"><span data-stu-id="3342e-151">Adds the supplied content to the target as a first or last child, as determined by the **position** attribute.</span></span></p><p><span data-ttu-id="3342e-152">**body**、**div**、**ol**、**ul** 要素にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="3342e-152">Applies only to **body**, **div**, **ol**, and **ul** elements.</span></span></p> |  
| <span data-ttu-id="3342e-153">insert</span><span class="sxs-lookup"><span data-stu-id="3342e-153">insert</span></span> | <span data-ttu-id="3342e-154">指定されたコンテンツを兄弟としてターゲットの前または後に追加します。追加される位置 (前または後) は、**position** 属性によって決まります。</span><span class="sxs-lookup"><span data-stu-id="3342e-154">Adds the supplied content as a sibling before or after the target, as determined by the **position** attribute.</span></span> |  
| <span data-ttu-id="3342e-155">prepend</span><span class="sxs-lookup"><span data-stu-id="3342e-155">prepend</span></span> | <p><span data-ttu-id="3342e-156">指定されたコンテンツを最初の子としてターゲットに追加します。</span><span class="sxs-lookup"><span data-stu-id="3342e-156">Adds the supplied content to the target as a first child.</span></span> <span data-ttu-id="3342e-157">**append** + **before** のショートカット。</span><span class="sxs-lookup"><span data-stu-id="3342e-157">Shortcut for **append** + **before**.</span></span></p><p><span data-ttu-id="3342e-158">**body**、**div**、**ol**、**ul** 要素にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="3342e-158">Applies only to **body**, **div**, **ol**, and **ul** elements.</span></span></p> |  
| <span data-ttu-id="3342e-159">replace</span><span class="sxs-lookup"><span data-stu-id="3342e-159">replace</span></span> | <p><span data-ttu-id="3342e-160">指定したコンテンツでターゲットを置換します。</span><span class="sxs-lookup"><span data-stu-id="3342e-160">Replaces the target with the supplied content.</span></span></p><p><span data-ttu-id="3342e-161">ほとんどの **replace** アクションは、ターゲットの[生成された ID](#generated-ids) を使用する必要があります (ただし、div 内の **img** 要素と **object** 要素を除きます。これらは、**data-id** の使用もサポートしています)。</span><span class="sxs-lookup"><span data-stu-id="3342e-161">Most **replace** actions require using the [generated ID](#generated-ids) for the target (except **img** and **object** elements within a div, which also support using **data-id**).</span></span></p> |  
 
<span data-ttu-id="3342e-162">**position**</span><span class="sxs-lookup"><span data-stu-id="3342e-162">**position**</span></span>  
<span data-ttu-id="3342e-163">指定されたコンテンツを追加する位置。ターゲット要素を基準とした相対位置です。</span><span class="sxs-lookup"><span data-stu-id="3342e-163">The location to add the supplied content, relative to the target element.</span></span> <span data-ttu-id="3342e-164">省略すると、既定値として **after** が使用されます。</span><span class="sxs-lookup"><span data-stu-id="3342e-164">Defaults to **after** if omitted.</span></span>

| <span data-ttu-id="3342e-165">位置</span><span class="sxs-lookup"><span data-stu-id="3342e-165">Position</span></span> | <span data-ttu-id="3342e-166">説明</span><span class="sxs-lookup"><span data-stu-id="3342e-166">Description</span></span> |  
|------|------|  
| <span data-ttu-id="3342e-167">after (既定値)</span><span class="sxs-lookup"><span data-stu-id="3342e-167">after (default)</span></span> | <p><span data-ttu-id="3342e-168">- **append** と共に:ターゲット要素の最後の子。</span><span class="sxs-lookup"><span data-stu-id="3342e-168">- With **append**: The last child of the target element.</span></span></p><p><span data-ttu-id="3342e-169">- **insert** と共に:ターゲット要素の後続の兄弟。</span><span class="sxs-lookup"><span data-stu-id="3342e-169">- With **insert**: The subsequent sibling of the target element.</span></span></p> |
| <span data-ttu-id="3342e-170">before</span><span class="sxs-lookup"><span data-stu-id="3342e-170">before</span></span> | <p><span data-ttu-id="3342e-171">- **append** と共に:ターゲット要素の最初の子。</span><span class="sxs-lookup"><span data-stu-id="3342e-171">- With **append**: The first child of the target element.</span></span></p><p><span data-ttu-id="3342e-172">- **insert** と共に:ターゲット要素の先行の兄弟。</span><span class="sxs-lookup"><span data-stu-id="3342e-172">- With **insert**: The preceding sibling of the target element.</span></span></p> |

<span data-ttu-id="3342e-173">**content**</span><span class="sxs-lookup"><span data-stu-id="3342e-173">**content**</span></span>  
<span data-ttu-id="3342e-174">ページに追加する整形式 HTML の文字列と画像またはファイル バイナリ データ。</span><span class="sxs-lookup"><span data-stu-id="3342e-174">A string of well-formed HTML to add to the page, and any image or file binary data.</span></span> <span data-ttu-id="3342e-175">コンテンツにバイナリ データが含まれている場合、コンテンツ タイプとして `multipart/form-data` を利用し、"Commands" パートを含む要求を送信する必要があります ([例](#multipart-request-with-binary-content)参照)。</span><span class="sxs-lookup"><span data-stu-id="3342e-175">If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part (see an [example](#multipart-request-with-binary-content)).</span></span> 
 

<a name="generated-ids"></a>

### <a name="generated-ids"></a><span data-ttu-id="3342e-176">生成された ID</span><span class="sxs-lookup"><span data-stu-id="3342e-176">Generated IDs</span></span>
<span data-ttu-id="3342e-177">Microsoft Graph は、更新可能なページで要素に対して **id** 値を生成します。</span><span class="sxs-lookup"><span data-stu-id="3342e-177">The OneNote API generates **id** values for the elements on the page that can be updated.</span></span> <span data-ttu-id="3342e-178">生成された ID を取得するには、GET 要求で `includeIDs=true` クエリ文字列を使用します。</span><span class="sxs-lookup"><span data-stu-id="3342e-178">To get generated IDs, use the `includeIDs=true` query string expression in your GET request:</span></span>

`GET ../notes/pages/{page-id}/content?includeIDs=true` 

> <span data-ttu-id="3342e-179">**注:** API は、ページ作成要求およびページ更新要求の[入力 HTML](onenote_input_output_html.md) で定義された **id** の値をすべて破棄します。</span><span class="sxs-lookup"><span data-stu-id="3342e-179">The API discards all **id** values that are defined in the [input HTML](onenote_input_output_html.md) of create-page and update-page requests.</span></span>

<span data-ttu-id="3342e-180">次の例は、ページの[出力 HTML](onenote_input_output_html.md) の段落と画像に対して生成された ID を示します。</span><span class="sxs-lookup"><span data-stu-id="3342e-180">The following example shows generated IDs for a paragraph and an image in the [output HTML](onenote_input_output_html.md) of a page.</span></span>

```html
<p id="p:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{40}">Some text on the page</p>
<img id="img:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{45}" ... />
```

<span data-ttu-id="3342e-181">生成された **id** 値はページ更新後に変更されることがあるため、これらの値を使用する PATCH 要求を作成する前に、現行値を取得する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3342e-181">Generated **id** values might change after a page update, so you should get the current values before building a PATCH request that uses them.</span></span>
 
<span data-ttu-id="3342e-182">ターゲット要素は、**data-id** または **id** 値を使用して次のように指定できます。</span><span class="sxs-lookup"><span data-stu-id="3342e-182">You can specify target elements by using the **data-id** or **id** value, as follows:</span></span>

- <span data-ttu-id="3342e-183">**append** アクションと **insert** アクションでは、いずれの ID もターゲット値として使用できます。</span><span class="sxs-lookup"><span data-stu-id="3342e-183">For **append** and **insert** actions, you can use either ID as the target value.</span></span>
- <span data-ttu-id="3342e-184">**replace** アクションでは、すべての要素について、生成された IDを使用する必要があります。ただし、ページ タイトル、および div 内の画像とオブジェクトを除きます。</span><span class="sxs-lookup"><span data-stu-id="3342e-184">For **replace** actions, you must use the generated ID for all elements except for the page title and images and objects that are within a div.</span></span> 
    - <span data-ttu-id="3342e-185">タイトルを置換する場合は、**title** キーワードを使用します。</span><span class="sxs-lookup"><span data-stu-id="3342e-185">To replace a title, use the **title** keyword.</span></span> 
    - <span data-ttu-id="3342e-186">div 内の画像とオブジェクトを置換する場合は、**data-id** または **id** のどちらかを使用します。</span><span class="sxs-lookup"><span data-stu-id="3342e-186">To replace images and objects that are within a div, use either **data-id** or **id**.</span></span>

<span data-ttu-id="3342e-187">次の例では、ターゲットに **id** 値を使用します。</span><span class="sxs-lookup"><span data-stu-id="3342e-187">The following example uses the **id** value for the target.</span></span> <span data-ttu-id="3342e-188">生成された ID と共に # プレフィックスを使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="3342e-188">Don't use the # prefix with a generated ID.</span></span>

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

## <a name="supported-elements-and-actions"></a><span data-ttu-id="3342e-189">サポートされる要素とアクション</span><span class="sxs-lookup"><span data-stu-id="3342e-189">Supported elements and actions</span></span>
<span data-ttu-id="3342e-p117">ページ上の要素の多くは更新可能ですが、要素の種類ごとに特定のアクションがサポートされています。サポートされるターゲット要素と、各要素でサポートされる更新アクションを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="3342e-p117">Many elements on the page can be updated, but each element type supports specific actions. The following table shows supported target elements and the update actions that they support.</span></span>

| <span data-ttu-id="3342e-192">要素</span><span class="sxs-lookup"><span data-stu-id="3342e-192">Element</span></span> | <span data-ttu-id="3342e-193">置換</span><span class="sxs-lookup"><span data-stu-id="3342e-193">Replace</span></span> | <span data-ttu-id="3342e-194">子の追加</span><span class="sxs-lookup"><span data-stu-id="3342e-194">Append child</span></span> | <span data-ttu-id="3342e-195">兄弟の挿入</span><span class="sxs-lookup"><span data-stu-id="3342e-195">Insert sibling</span></span> |  
|------|------|------|------|  
| <span data-ttu-id="3342e-196">body</span><span class="sxs-lookup"><span data-stu-id="3342e-196">body</span></span><br /> <span data-ttu-id="3342e-197">(ページの最初の div をターゲットとする)</span><span class="sxs-lookup"><span data-stu-id="3342e-197">(targets first div on the page)</span></span> | <span data-ttu-id="3342e-198">いいえ</span><span class="sxs-lookup"><span data-stu-id="3342e-198">no</span></span> | <span data-ttu-id="3342e-199">**はい**</span><span class="sxs-lookup"><span data-stu-id="3342e-199">**yes**</span></span> | <span data-ttu-id="3342e-200">いいえ</span><span class="sxs-lookup"><span data-stu-id="3342e-200">no</span></span> |  
| <span data-ttu-id="3342e-201">div</span><span class="sxs-lookup"><span data-stu-id="3342e-201">div</span></span><br /> <span data-ttu-id="3342e-202">([絶対配置](onenote-abs-pos.md))</span><span class="sxs-lookup"><span data-stu-id="3342e-202">([absolute positioned](onenote-abs-pos.md))</span></span> | <span data-ttu-id="3342e-203">いいえ</span><span class="sxs-lookup"><span data-stu-id="3342e-203">no</span></span> | <span data-ttu-id="3342e-204">**はい**</span><span class="sxs-lookup"><span data-stu-id="3342e-204">**yes**</span></span> | <span data-ttu-id="3342e-205">いいえ</span><span class="sxs-lookup"><span data-stu-id="3342e-205">no</span></span> |  
| <span data-ttu-id="3342e-206">div</span><span class="sxs-lookup"><span data-stu-id="3342e-206">div</span></span><br /> <span data-ttu-id="3342e-207">(div 内)</span><span class="sxs-lookup"><span data-stu-id="3342e-207">(within a div)</span></span> | <span data-ttu-id="3342e-208">**はい** (id のみ)</span><span class="sxs-lookup"><span data-stu-id="3342e-208">**yes** (id only)</span></span> | <span data-ttu-id="3342e-209">**はい**</span><span class="sxs-lookup"><span data-stu-id="3342e-209">**yes**</span></span> | <span data-ttu-id="3342e-210">**はい**</span><span class="sxs-lookup"><span data-stu-id="3342e-210">**yes**</span></span> |   
| <span data-ttu-id="3342e-211">img、object</span><span class="sxs-lookup"><span data-stu-id="3342e-211">img, object</span></span><br /> <span data-ttu-id="3342e-212">(div 内)</span><span class="sxs-lookup"><span data-stu-id="3342e-212">(within a div)</span></span> | <span data-ttu-id="3342e-213">**はい**</span><span class="sxs-lookup"><span data-stu-id="3342e-213">**yes**</span></span> | <span data-ttu-id="3342e-214">いいえ</span><span class="sxs-lookup"><span data-stu-id="3342e-214">no</span></span> | <span data-ttu-id="3342e-215">**はい**</span><span class="sxs-lookup"><span data-stu-id="3342e-215">**yes**</span></span> |   
| <span data-ttu-id="3342e-216">ol、ul</span><span class="sxs-lookup"><span data-stu-id="3342e-216">ol, ul</span></span> | <span data-ttu-id="3342e-217">**はい** (id のみ)</span><span class="sxs-lookup"><span data-stu-id="3342e-217">**yes** (id only)</span></span> | <span data-ttu-id="3342e-218">**はい**</span><span class="sxs-lookup"><span data-stu-id="3342e-218">**yes**</span></span> | <span data-ttu-id="3342e-219">**はい**</span><span class="sxs-lookup"><span data-stu-id="3342e-219">**yes**</span></span> |   
| <span data-ttu-id="3342e-220">table</span><span class="sxs-lookup"><span data-stu-id="3342e-220">table</span></span> | <span data-ttu-id="3342e-221">**はい** (id のみ)</span><span class="sxs-lookup"><span data-stu-id="3342e-221">**yes** (id only)</span></span> | <span data-ttu-id="3342e-222">いいえ</span><span class="sxs-lookup"><span data-stu-id="3342e-222">no</span></span> | <span data-ttu-id="3342e-223">**はい**</span><span class="sxs-lookup"><span data-stu-id="3342e-223">**yes**</span></span> |   
| <span data-ttu-id="3342e-224">p、li、h1-h6</span><span class="sxs-lookup"><span data-stu-id="3342e-224">p, li, h1-h6</span></span> | <span data-ttu-id="3342e-225">**はい** (id のみ)</span><span class="sxs-lookup"><span data-stu-id="3342e-225">**yes** (id only)</span></span> | <span data-ttu-id="3342e-226">いいえ</span><span class="sxs-lookup"><span data-stu-id="3342e-226">no</span></span> | <span data-ttu-id="3342e-227">**はい**</span><span class="sxs-lookup"><span data-stu-id="3342e-227">**yes**</span></span> |   
| <span data-ttu-id="3342e-228">title</span><span class="sxs-lookup"><span data-stu-id="3342e-228">title</span></span> | <span data-ttu-id="3342e-229">**はい**</span><span class="sxs-lookup"><span data-stu-id="3342e-229">**yes**</span></span> | <span data-ttu-id="3342e-230">いいえ</span><span class="sxs-lookup"><span data-stu-id="3342e-230">no</span></span> | <span data-ttu-id="3342e-231">いいえ</span><span class="sxs-lookup"><span data-stu-id="3342e-231">no</span></span> |  
 

<span data-ttu-id="3342e-232">次の要素では更新アクションはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3342e-232">The following elements do not support any update actions.</span></span>

- <span data-ttu-id="3342e-233">img ([絶対配置](onenote-abs-pos.md))</span><span class="sxs-lookup"><span data-stu-id="3342e-233">img ([absolute positioned](onenote-abs-pos.md))</span></span>
- <span data-ttu-id="3342e-234">object ([絶対配置](onenote-abs-pos.md))</span><span class="sxs-lookup"><span data-stu-id="3342e-234">object ([absolute positioned](onenote-abs-pos.md))</span></span>
- <span data-ttu-id="3342e-235">tr、td</span><span class="sxs-lookup"><span data-stu-id="3342e-235">tr, td</span></span>
- <span data-ttu-id="3342e-236">meta</span><span class="sxs-lookup"><span data-stu-id="3342e-236">meta</span></span>
- <span data-ttu-id="3342e-237">head</span><span class="sxs-lookup"><span data-stu-id="3342e-237">head</span></span>
- <span data-ttu-id="3342e-238">span</span><span class="sxs-lookup"><span data-stu-id="3342e-238">span</span></span>
- <span data-ttu-id="3342e-239">a</span><span class="sxs-lookup"><span data-stu-id="3342e-239">a</span></span>
- <span data-ttu-id="3342e-240">style タグ</span><span class="sxs-lookup"><span data-stu-id="3342e-240">style tags</span></span>


<a name="examples"></a>
## <a name="example-requests"></a><span data-ttu-id="3342e-241">要求の例</span><span class="sxs-lookup"><span data-stu-id="3342e-241">Example requests</span></span>
<span data-ttu-id="3342e-p118">更新要求には、JSON 変更オブジェクトとして表現される変更が 1 つ以上含まれています。これらのオブジェクトでは、ページ上のさまざまなターゲットや、ターゲットに対するさまざまなアクションとコンテンツを定義できます。</span><span class="sxs-lookup"><span data-stu-id="3342e-p118">An update request contains one or more changes represented as JSON change objects. These objects can define different targets on the page and different actions and content for the targets.</span></span>

<span data-ttu-id="3342e-244">次の例に、PATCH 要求で使用される JSON オブジェクトと完全な PATCH 要求を示します。</span><span class="sxs-lookup"><span data-stu-id="3342e-244">The following examples include JSON objects used in PATCH requests and complete PATCH requests:</span></span>

<span data-ttu-id="3342e-245">[子要素の追加](#append-child-elements)&nbsp;&nbsp;|&nbsp;&nbsp;[兄弟要素の挿入](#insert-sibling-elements)&nbsp;&nbsp;|&nbsp;&nbsp;[要素の置換](#replace-elements)&nbsp;&nbsp;|&nbsp;&nbsp;[完全な PATCH 要求](#complete-patch-request-examples)</span><span class="sxs-lookup"><span data-stu-id="3342e-245">[Append child elements](#append-child-elements)&nbsp;&nbsp;|&nbsp;&nbsp;[Insert sibling elements](#insert-sibling-elements)&nbsp;&nbsp;|&nbsp;&nbsp;[Replace elements](#replace-elements)&nbsp;&nbsp;|&nbsp;&nbsp;[Complete PATCH requests](#complete-patch-request-examples)</span></span>


<a name="append-examples"></a>

### <a name="append-child-elements"></a><span data-ttu-id="3342e-246">子要素の追加</span><span class="sxs-lookup"><span data-stu-id="3342e-246">Append child elements</span></span>
<span data-ttu-id="3342e-247">**append** アクションでは、**body**、**div** (div 内)、**ol**、**ul** 要素に子が追加されます。</span><span class="sxs-lookup"><span data-stu-id="3342e-247">The **append** action adds a child to a **body**, **div** (within a div), **ol**, or **ul** element.</span></span> <span data-ttu-id="3342e-248">**position** 属性により、ターゲットの前または後に子を追加することが決定されます。</span><span class="sxs-lookup"><span data-stu-id="3342e-248">The **position** attribute determines whether to append the child before or after the target.</span></span> <span data-ttu-id="3342e-249">既定の位置は**後**です。</span><span class="sxs-lookup"><span data-stu-id="3342e-249">The default position is **after**.</span></span>

#### <a name="append-to-a-div"></a><span data-ttu-id="3342e-250">div への追加</span><span class="sxs-lookup"><span data-stu-id="3342e-250">Append to a div</span></span>

<span data-ttu-id="3342e-251">次の例では、2 つの子ノードを **div1** 要素に追加します。</span><span class="sxs-lookup"><span data-stu-id="3342e-251">The following example adds two child nodes to the **div1** element.</span></span> <span data-ttu-id="3342e-252">最初の子として画像を追加し、最後の子として段落を追加します。</span><span class="sxs-lookup"><span data-stu-id="3342e-252">It adds an image as the first child and a paragraph as the last child.</span></span> 

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
 

#### <a name="append-to-the-body-element"></a><span data-ttu-id="3342e-253">*body* 要素への追加</span><span class="sxs-lookup"><span data-stu-id="3342e-253">Append to the *body* element</span></span>

<span data-ttu-id="3342e-254">**body** は、任意のページ上の最初の div 内に子要素を追加するためのショートカットとして使用できます。</span><span class="sxs-lookup"><span data-stu-id="3342e-254">You can use the **body** shortcut to append a child element inside the first div on any page.</span></span>

<span data-ttu-id="3342e-255">次の例では、ページの最初の div に 2 つの段落を最初の子と最後の子として追加しています。</span><span class="sxs-lookup"><span data-stu-id="3342e-255">The following example adds two paragraphs as the first child and the last child to the first div on the page.</span></span> <span data-ttu-id="3342e-256">**body** ターゲットと共に # を使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="3342e-256">Don't use a # with the **body** target.</span></span> <span data-ttu-id="3342e-257">この例では、**prepend** アクションを **append** + **before** として使用しています。</span><span class="sxs-lookup"><span data-stu-id="3342e-257">This example uses the **prepend** action as a shortcut for **append** + **before**.</span></span>

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
 

#### <a name="append-to-a-list"></a><span data-ttu-id="3342e-258">リストへの追加</span><span class="sxs-lookup"><span data-stu-id="3342e-258">Append to a list</span></span>

<span data-ttu-id="3342e-259">次の例では、リスト項目を最後の子として対象のリストに追加します。</span><span class="sxs-lookup"><span data-stu-id="3342e-259">The following example adds a list item as a last child to the target list.</span></span> <span data-ttu-id="3342e-260">項目は既定以外のリスト スタイルを使用するため、**list-style-type** プロパティが定義されます。</span><span class="sxs-lookup"><span data-stu-id="3342e-260">The **list-style-type** property is defined because the item uses a non-default list style.</span></span>

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

### <a name="insert-sibling-elements"></a><span data-ttu-id="3342e-261">兄弟要素の挿入</span><span class="sxs-lookup"><span data-stu-id="3342e-261">Insert sibling elements</span></span>
<span data-ttu-id="3342e-262">**insert** アクションでは、兄弟がターゲット要素に追加されます。</span><span class="sxs-lookup"><span data-stu-id="3342e-262">The **insert** action adds a sibling to the target element.</span></span> <span data-ttu-id="3342e-263">**position** 属性により、ターゲットの前または後に兄弟を挿入することが決定されます。</span><span class="sxs-lookup"><span data-stu-id="3342e-263">The **position** attribute determines whether to insert the sibling before or after the target.</span></span> <span data-ttu-id="3342e-264">既定の位置は**後**です。</span><span class="sxs-lookup"><span data-stu-id="3342e-264">The default position is **after**.</span></span> <span data-ttu-id="3342e-265">「[**insert** をサポートする要素](#supported-elements-and-actions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3342e-265">See [elements that support **insert**](#supported-elements-and-actions).</span></span>

<span data-ttu-id="3342e-266">**兄弟の挿入**</span><span class="sxs-lookup"><span data-stu-id="3342e-266">**Insert siblings**</span></span>

<span data-ttu-id="3342e-267">次の例では、2 つの兄弟ノードをページに追加します。</span><span class="sxs-lookup"><span data-stu-id="3342e-267">The following example adds two sibling nodes to the page.</span></span> <span data-ttu-id="3342e-268">**para1** 要素の上に画像を追加し、**para2** 要素の下に段落を追加します。</span><span class="sxs-lookup"><span data-stu-id="3342e-268">It adds an image above the **para1** element and a paragraph below the **para2** element.</span></span>

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

### <a name="replace-elements"></a><span data-ttu-id="3342e-269">要素の置換</span><span class="sxs-lookup"><span data-stu-id="3342e-269">Replace elements</span></span>

<span data-ttu-id="3342e-270">**data-id** と生成された **id** のいずれかをターゲット値として使用し、div 内にある **img** 要素および **object** 要素を置換できます。</span><span class="sxs-lookup"><span data-stu-id="3342e-270">You can use either the **data-id** or generated **id** as the target value to replace **img** and **object** elements that are within a div.</span></span> <span data-ttu-id="3342e-271">ページ タイトルを置換する場合は、**title** キーワードを使用します。</span><span class="sxs-lookup"><span data-stu-id="3342e-271">To replace the page title, use the **title** keyword.</span></span> <span data-ttu-id="3342e-272">[**replace** をサポートするその他すべての要素](#supported-elements-and-actions)については、生成されたこの ID を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3342e-272">For all other [elements that support **replace**](#supported-elements-and-actions), you must use the generated ID.</span></span>

#### <a name="replace-an-image"></a><span data-ttu-id="3342e-273">画像の置換</span><span class="sxs-lookup"><span data-stu-id="3342e-273">Replace an image</span></span>

<span data-ttu-id="3342e-274">次の例では、画像の **data-id** をターゲットとして使用して、div 内の画像が置換されます。</span><span class="sxs-lookup"><span data-stu-id="3342e-274">The following example replaces an image with a div by using the image's **data-id** as the target.</span></span> 

```json
[
  {
    'target':'#img1',
    'action':'replace',
    'content':'<div data-id="new-div"><p>This div replaces the image</p></div>'
  }
]
```
 

#### <a name="update-a-table"></a><span data-ttu-id="3342e-275">表の更新</span><span class="sxs-lookup"><span data-stu-id="3342e-275">Update a table</span></span> 

<span data-ttu-id="3342e-276">次の例では、生成された ID を使用して表を更新する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="3342e-276">This example shows how to update a table by using its generated ID.</span></span> <span data-ttu-id="3342e-277">**tr** 要素と **td** 要素の置換はサポートされていませんが、表全体を置換することはできます。</span><span class="sxs-lookup"><span data-stu-id="3342e-277">Replacing **tr** and **td** elements is not supported, but you can replace the entire table.</span></span>

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
 

#### <a name="change-the-title"></a><span data-ttu-id="3342e-278">タイトルの変更</span><span class="sxs-lookup"><span data-stu-id="3342e-278">Change the title</span></span> 

<span data-ttu-id="3342e-279">この例では、ページのタイトルを変更する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="3342e-279">This example shows how to change the title of a page.</span></span> <span data-ttu-id="3342e-280">タイトルを変更するには、ターゲット値として **title** キーワードを使用します。</span><span class="sxs-lookup"><span data-stu-id="3342e-280">To change the title, use the **title** keyword as the target value.</span></span> <span data-ttu-id="3342e-281">タイトル ターゲットで # を使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="3342e-281">Don't use a # with the title target.</span></span>

```json
[
  {
    'target':'title',
    'action':'replace',
    'content':'New title'
  }
]
```
 

#### <a name="update-a-to-do-item"></a><span data-ttu-id="3342e-282">To Do アイテムの更新</span><span class="sxs-lookup"><span data-stu-id="3342e-282">Update a to-do item</span></span>

<span data-ttu-id="3342e-283">次に示す例では、replace アクションを使用して、To Do チェック ボックス アイテムを完了状態に変更します。</span><span class="sxs-lookup"><span data-stu-id="3342e-283">The following example uses the replace action to change a to-do check box item to a completed state.</span></span>

```json
[
  {
    'target':'#task1',
    'action':'replace',
    'content':'<p data-tag="to-do:completed" data-id="task1">First task</p>'
  }
]
```

<span data-ttu-id="3342e-284">**data-tag** 属性の使用法の詳細については、「[ノート シールを使用する](onenote-note-tags.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3342e-284">See [Use note tags](onenote-note-tags.md) for more about using the **data-tag** attribute.</span></span>


<a name="complete-requests"></a>

### <a name="complete-patch-request-examples"></a><span data-ttu-id="3342e-285">完全な PATCH 要求の例</span><span class="sxs-lookup"><span data-stu-id="3342e-285">Complete PATCH request examples</span></span>

<span data-ttu-id="3342e-286">次の例に、完全な PATCH 要求を示します。</span><span class="sxs-lookup"><span data-stu-id="3342e-286">The following examples show complete PATCH requests.</span></span>

#### <a name="request-with-text-content-only"></a><span data-ttu-id="3342e-287">テキスト コンテンツのみの要求</span><span class="sxs-lookup"><span data-stu-id="3342e-287">Request with text content only</span></span>  
<span data-ttu-id="3342e-288">次の例では、PATCH 要求でコンテンツ タイプとして **application/json** が使用されています。</span><span class="sxs-lookup"><span data-stu-id="3342e-288">The following example shows a PATCH request that uses the **application/json** content type.</span></span> <span data-ttu-id="3342e-289">コンテンツにバイナリ データが含まれていない場合は、この形式を使用できます。</span><span class="sxs-lookup"><span data-stu-id="3342e-289">You can use this format when your content doesn't contain binary data.</span></span>

```
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

#### <a name="multipart-request-with-binary-content"></a><span data-ttu-id="3342e-290">バイナリ コンテンツを含むマルチパート要求</span><span class="sxs-lookup"><span data-stu-id="3342e-290">Multipart request with binary content</span></span> 

<span data-ttu-id="3342e-291">バイナリ データを含むマルチパート PATCH 要求を次の例で示します。</span><span class="sxs-lookup"><span data-stu-id="3342e-291">The following example shows a multipart PATCH request that includes binary data.</span></span> <span data-ttu-id="3342e-292">マルチパート要求には、**application/json** コンテンツ タイプを指定し、JSON 変更オブジェクトの配列を含める "Commands" 部分が必要になります。</span><span class="sxs-lookup"><span data-stu-id="3342e-292">Multipart requests require a "Commands" part that specifies the **application/json** content type and contains the array of JSON change objects.</span></span> <span data-ttu-id="3342e-293">その他のデータ部分に、バイナリ データを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="3342e-293">Other data parts can contain binary data.</span></span> <span data-ttu-id="3342e-294">部分の名前は、通常、ミリ秒単位での現在の時刻、またはランダムな GUID が付加された文字列になります。</span><span class="sxs-lookup"><span data-stu-id="3342e-294">Part names typically are strings appended with the current time in milliseconds or a random GUID.</span></span>

```
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

## <a name="request-and-response-information-for-patch-requests"></a><span data-ttu-id="3342e-295">PATCH 要求の要求情報と応答情報</span><span class="sxs-lookup"><span data-stu-id="3342e-295">Request and response information for PATCH requests</span></span>

| <span data-ttu-id="3342e-296">要求データ</span><span class="sxs-lookup"><span data-stu-id="3342e-296">Request data</span></span> | <span data-ttu-id="3342e-297">説明</span><span class="sxs-lookup"><span data-stu-id="3342e-297">Description</span></span> |  
|------|------|  
| <span data-ttu-id="3342e-298">プロトコル</span><span class="sxs-lookup"><span data-stu-id="3342e-298">Protocol</span></span> | <span data-ttu-id="3342e-299">すべての要求は SSL/TLS HTTPS プロトコルを使用します。</span><span class="sxs-lookup"><span data-stu-id="3342e-299">All requests use the SSL/TLS HTTPS protocol.</span></span> |  
| <span data-ttu-id="3342e-300">承認ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3342e-300">Authorization header</span></span> | <p><span data-ttu-id="3342e-301">`Bearer {token}`。*{token}* は、登録済みアプリの有効な OAuth 2.0 アクセス トークンになります。</span><span class="sxs-lookup"><span data-stu-id="3342e-301">`Bearer {token}`, where *{token}* is a valid OAuth 2.0 access token for your registered app.</span></span></p><p><span data-ttu-id="3342e-302">これがないか、無効の場合、要求は失敗し、401 ステータス コードが表示されます。</span><span class="sxs-lookup"><span data-stu-id="3342e-302">If missing or invalid, the request fails with a 401 status code.</span></span> <span data-ttu-id="3342e-303">「[認証とアクセス許可](permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3342e-303">See [Authentication and permissions](permissions_reference.md).</span></span></p> |  
| <span data-ttu-id="3342e-304">Content-Type ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3342e-304">Content-Type header</span></span> | <p><span data-ttu-id="3342e-305">JSON 変更オブジェクトの配列の `application/json`。メッセージ本文または[マルチパート要求](#multipart-request-with-binary-content)の必須の "Commands" パートで直接送信。</span><span class="sxs-lookup"><span data-stu-id="3342e-305">`application/json` for the array of JSON change objects, whether sent directly in the message body or in the required "Commands" part of [multipart requests](#multipart-request-with-binary-content).</span></span></p><p><span data-ttu-id="3342e-306">マルチパート要求はバイナリ データを送信するときに必須であり、コンテンツ タイプとして `multipart/form-data; boundary=part-boundary` を使用します。*{part-boundary}* は、各データ パートの開始と終了を伝える文字列です。</span><span class="sxs-lookup"><span data-stu-id="3342e-306">Multipart requests are required when sending binary data, and use the `multipart/form-data; boundary=part-boundary` content type, where *{part-boundary}* is a string that signals the start and end of each data part.</span></span></p> |  
 

| <span data-ttu-id="3342e-307">応答データ</span><span class="sxs-lookup"><span data-stu-id="3342e-307">Response data</span></span> | <span data-ttu-id="3342e-308">説明</span><span class="sxs-lookup"><span data-stu-id="3342e-308">Description</span></span> |  
|------|------|  
| <span data-ttu-id="3342e-309">成功コード</span><span class="sxs-lookup"><span data-stu-id="3342e-309">Success code</span></span> | <span data-ttu-id="3342e-p131">204 HTTP ステータス コード。PATCH 要求に対して JSON データは返されません。</span><span class="sxs-lookup"><span data-stu-id="3342e-p131">A 204 HTTP status code. No JSON data is returned for a PATCH request.</span></span> |  
| <span data-ttu-id="3342e-312">エラー</span><span class="sxs-lookup"><span data-stu-id="3342e-312">Errors</span></span> | <span data-ttu-id="3342e-313">Microsoft Graph から返されることのある OneNote エラーに関する詳細については、「[Microsoft Graph の OneNote API のエラー コード](onenote_error_codes.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="3342e-313">Read [Error codes for OneNote APIs in Microsoft Graph](onenote_error_codes.md) to learn about OneNote errors that Microsoft Graph can return.</span></span> |  
 
 

<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-service-root-url"></a><span data-ttu-id="3342e-314">Microsoft Graph サービスのルート URL の構築</span><span class="sxs-lookup"><span data-stu-id="3342e-314">Constructing the OneNote service root URL</span></span>

<a name="root-url"></a>

## <a name="root-url"></a><span data-ttu-id="3342e-315">ルート URL</span><span class="sxs-lookup"><span data-stu-id="3342e-315">URL Root</span></span>
<span data-ttu-id="3342e-316">OneNote サービスのルート URL は、OneNote API へのすべての呼び出しで次の形式を使用します。</span><span class="sxs-lookup"><span data-stu-id="3342e-316">The OneNote service root URL uses the following format for all calls to the OneNote API.</span></span>
`https://graph.microsoft.com/{version}/me/onenote/`

<span data-ttu-id="3342e-317">URL の `version` セグメントは、使用する Microsoft Graph のバージョンを示しています。</span><span class="sxs-lookup"><span data-stu-id="3342e-317">The `version` segment in the URL represents the version of the OneNote API that you want to use.</span></span>
- <span data-ttu-id="3342e-318">安定した運用コードには `v1.0` を使用します。</span><span class="sxs-lookup"><span data-stu-id="3342e-318">Use `v1.0` for stable production code.</span></span>
- <span data-ttu-id="3342e-319">開発中の機能を試すには `beta` を使用します。</span><span class="sxs-lookup"><span data-stu-id="3342e-319">Use `beta` to try out a feature that's in development.</span></span> <span data-ttu-id="3342e-320">ベータ版の機能は変更される可能性があるため、運用コードでは使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="3342e-320">Features and functionality in beta may change, so you shouldn't use it in your production code.</span></span>
- <span data-ttu-id="3342e-321">現在のユーザーがアクセスできる OneNote コンテンツには `me` を使用します (所有と共有)。</span><span class="sxs-lookup"><span data-stu-id="3342e-321">Use `me` for OneNote content that the current user can access (owned and shared).</span></span>
- <span data-ttu-id="3342e-322">指定されたユーザー (URL 内) が現在のユーザーと共有している OneNote コンテンツには `users/{id}` を使用します。</span><span class="sxs-lookup"><span data-stu-id="3342e-322">Use `users/{id}` for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="3342e-323">[Azure AD Graph API](https://msdn.microsoft.com/library/azure/ad/graph/api/api-catalog) の使用</span><span class="sxs-lookup"><span data-stu-id="3342e-323">Use the [Azure AD Graph API](https://msdn.microsoft.com/library/azure/ad/graph/api/api-catalog) to get group IDs.</span></span>


> <span data-ttu-id="3342e-324">**注:** `https://graph.microsoft.com/v1.0/users`で GET 要求を行うことにより、ユーザー ID を取得できます。</span><span class="sxs-lookup"><span data-stu-id="3342e-324">**Note:** You can get user ids by making a GET request on `https://graph.microsoft.com/v1.0/users`.</span></span>



<a name="permissions"></a>

## <a name="permissions"></a><span data-ttu-id="3342e-325">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3342e-325">Permissions</span></span>

<span data-ttu-id="3342e-p134">OneNote ページを更新するには、適切なアクセス許可を要求する必要があります。アプリの動作に必要な最低限のアクセス許可を選択してください。</span><span class="sxs-lookup"><span data-stu-id="3342e-p134">To update OneNote pages, you'll need to request appropriate permissions. Choose the lowest level of permissions that your app needs to do its work.</span></span>

- <span data-ttu-id="3342e-328">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3342e-328">Notes.ReadWrite</span></span>
- <span data-ttu-id="3342e-329">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3342e-329">Notes.ReadWrite.All</span></span>

<span data-ttu-id="3342e-330">アクセス許可のスコープと動作のしくみの詳細については、「[OneNote のアクセス許可のスコープ](permissions_reference.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="3342e-330">For more information about permission scopes and how they work, see [OneNote permission scopes](permissions_reference.md).</span></span>
   

<a name="see-also"></a>

## <a name="additional-resources"></a><span data-ttu-id="3342e-331">その他のリソース</span><span class="sxs-lookup"><span data-stu-id="3342e-331">Additional resources</span></span>

- [<span data-ttu-id="3342e-332">画像とファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="3342e-332">Add images and files</span></span>](onenote_images_files.md)
- [<span data-ttu-id="3342e-333">OneNote との統合</span><span class="sxs-lookup"><span data-stu-id="3342e-333">Integrate with OneNote</span></span>](integrate_with_onenote.md)
- [<span data-ttu-id="3342e-334">OneNote の開発者ブログ</span><span class="sxs-lookup"><span data-stu-id="3342e-334">OneNote Developer Blog</span></span>](http://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="3342e-335">Stack Overflow 掲載の OneNote の開発に関する質問</span><span class="sxs-lookup"><span data-stu-id="3342e-335">OneNote development questions on Stack Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="3342e-336">OneNote GitHub のリポジトリ</span><span class="sxs-lookup"><span data-stu-id="3342e-336">OneNote GitHub repos</span></span>](http://go.microsoft.com/fwlink/?LinkID=390178)  
