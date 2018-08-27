# <a name="input-and-output-html-in-onenote-pages"></a><span data-ttu-id="5810d-101">OneNote ページの入出力 HTML</span><span class="sxs-lookup"><span data-stu-id="5810d-101">Input and output HTML in OneNote pages</span></span>

<span data-ttu-id="5810d-102">OneNote ページを[作成](onenote-create-page.md)または[更新](onenote_update_page.md)する際に、ページ コンテンツと構造を定義する HTML を*入力 HTML* と呼びます。</span><span class="sxs-lookup"><span data-stu-id="5810d-102">The HTML that defines the page content and structure when you [create](onenote-create-page.md) or [update](onenote_update_page.md) a OneNote page is called *input HTML*.</span></span> 

<span data-ttu-id="5810d-p101">[ページ コンテンツを取得](onenote-get-content.md)すると返される HTML を*出力 HTML* と呼びます。出力 HTML は入力 HTML と同じにはなりません。</span><span class="sxs-lookup"><span data-stu-id="5810d-p101">The HTML that's returned when you [get page content](onenote-get-content.md) is called *output HTML*. Output HTML won't be the same as input HTML.</span></span>

<span data-ttu-id="5810d-105">Microsoft Graph の OneNote API は、入力 HTML の意味的コンテンツと基本的構造を保持しますが、その HTML を、[サポートされている HTML 要素および CSS プロパティ](onenote-create-page.md#supported-html-and-css-for-onenote-pages)のセットに変換します。</span><span class="sxs-lookup"><span data-stu-id="5810d-105">The OneNote APIs in Microsoft Graph preserve the semantic content and basic structure of the input HTML, but convert it to a set of [supported HTML elements and CSS properties](onenote-create-page.md#supported-html-and-css-for-onenote-pages).</span></span> <span data-ttu-id="5810d-106">API はさらに、OneNote 機能をサポートするカスタム属性も追加します。</span><span class="sxs-lookup"><span data-stu-id="5810d-106">The APIs also add custom attributes that support OneNote features.</span></span>
 
<span data-ttu-id="5810d-p103">この資料では、入力 HTML と出力 HTML の主な要素と属性について説明します。ページ コンテンツを作成または更新する場合には入力 HTML について、返されるページ コンテンツを解析する場合には出力 HTML について理解することは役立ちます。</span><span class="sxs-lookup"><span data-stu-id="5810d-p103">This article describes the principal elements and attributes of input and output HTML. It can be helpful to understand input HTML when you're creating or updating page content, and output HTML when you're parsing returned page content.</span></span> 

## <a name="body-element"></a><span data-ttu-id="5810d-109">body 要素</span><span class="sxs-lookup"><span data-stu-id="5810d-109">Body element</span></span>

<span data-ttu-id="5810d-p104">ページ本文の HTML コンテンツは、画像やファイルのリソースなどを含むページのコンテンツと構造を表します。入力および出力 HTML では、**body** 要素に次の属性を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="5810d-p104">The HTML content in the page body represents the page content and structure, including image and file resources. The **body** element can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="5810d-112">入力属性</span><span class="sxs-lookup"><span data-stu-id="5810d-112">Input attributes</span></span>

|<span data-ttu-id="5810d-113">入力属性</span><span class="sxs-lookup"><span data-stu-id="5810d-113">Input attribute</span></span>|<span data-ttu-id="5810d-114">説明</span><span class="sxs-lookup"><span data-stu-id="5810d-114">Description</span></span>|
|:------|:------|
| <span data-ttu-id="5810d-115">data-absolute-enabled</span><span class="sxs-lookup"><span data-stu-id="5810d-115">data-absolute-enabled</span></span> | <span data-ttu-id="5810d-116">[絶対位置で配置](onenote-abs-pos.md)された要素を入力本文でサポートするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5810d-116">Indicates whether the input body supports [absolute positioned](onenote-abs-pos.md) elements.</span></span> |
| <span data-ttu-id="5810d-117">style</span><span class="sxs-lookup"><span data-stu-id="5810d-117">style</span></span> | <p><span data-ttu-id="5810d-118">本文の CSS の [style](#styles) プロパティ。</span><span class="sxs-lookup"><span data-stu-id="5810d-118">The CSS [style](#styles) properties of the body.</span></span> <span data-ttu-id="5810d-119">出力 HTML では、入力設定がインラインで、適切な子要素で返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="5810d-119">In the output HTML, input settings might be returned inline on appropriate child elements.</span></span></p><p><span data-ttu-id="5810d-120">現在、**body** 要素では背景色はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5810d-120">Background color is not currently supported for the **body** element.</span></span></p> |
 

#### <a name="output-attributes"></a><span data-ttu-id="5810d-121">出力属性</span><span class="sxs-lookup"><span data-stu-id="5810d-121">Output attributes</span></span>

|<span data-ttu-id="5810d-122">出力属性</span><span class="sxs-lookup"><span data-stu-id="5810d-122">Output attribute</span></span>|<span data-ttu-id="5810d-123">説明</span><span class="sxs-lookup"><span data-stu-id="5810d-123">Description</span></span>|
|:------|:------|
| <span data-ttu-id="5810d-124">data-absolute-enabled</span><span class="sxs-lookup"><span data-stu-id="5810d-124">data-absolute-enabled</span></span> | <span data-ttu-id="5810d-p106">[絶対配置](onenote-abs-pos.md)要素を本文でサポートするかどうかを示します。出力 HTML では常に **true** です。</span><span class="sxs-lookup"><span data-stu-id="5810d-p106">Indicates whether the body supports [absolute positioned](onenote-abs-pos.md) elements. Always **true** in output HTML.</span></span> |
| <span data-ttu-id="5810d-127">style</span><span class="sxs-lookup"><span data-stu-id="5810d-127">style</span></span> | <span data-ttu-id="5810d-128">本文の **font-family** および **font-size** プロパティ。</span><span class="sxs-lookup"><span data-stu-id="5810d-128">The **font-family** and **font-size** properties of the body.</span></span> |


## <a name="div-elements"></a><span data-ttu-id="5810d-129">div 要素</span><span class="sxs-lookup"><span data-stu-id="5810d-129">Div elements</span></span>

<span data-ttu-id="5810d-130">**div** 要素にはテキスト、画像、およびその他のコンテンツが含まれます。</span><span class="sxs-lookup"><span data-stu-id="5810d-130">**Div** elements contain text, images, and other content.</span></span> <span data-ttu-id="5810d-131">入力 HTML と出力 HTML では、**div** 要素に次の属性を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="5810d-131">A **div** element can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="5810d-132">入力属性</span><span class="sxs-lookup"><span data-stu-id="5810d-132">Input attributes</span></span>

|<span data-ttu-id="5810d-133">入力属性</span><span class="sxs-lookup"><span data-stu-id="5810d-133">Input attribute</span></span>|<span data-ttu-id="5810d-134">説明</span><span class="sxs-lookup"><span data-stu-id="5810d-134">Description</span></span>|
|:------|:------|
| <span data-ttu-id="5810d-135">data-id</span><span class="sxs-lookup"><span data-stu-id="5810d-135">data-id</span></span> | <span data-ttu-id="5810d-136">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="5810d-136">A reference for the element.</span></span><br/><br/><span data-ttu-id="5810d-137">[ページ コンテンツの更新](onenote_update_page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="5810d-137">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="5810d-138">data-render-fallback</span><span class="sxs-lookup"><span data-stu-id="5810d-138">data-render-fallback</span></span> | <span data-ttu-id="5810d-139">[抽出](onenote-extract-data.md)が失敗した場合のフォールバック操作。**render** (既定値) または **none**。</span><span class="sxs-lookup"><span data-stu-id="5810d-139">The fallback action if the [extraction](onenote-extract-data.md) fails: **render** (default) or **none**.</span></span> |
| <span data-ttu-id="5810d-140">data-render-method</span><span class="sxs-lookup"><span data-stu-id="5810d-140">data-render-method</span></span> | <span data-ttu-id="5810d-141">[抽出](onenote-extract-data.md)を実行するメソッド。例:</span><span class="sxs-lookup"><span data-stu-id="5810d-141">The [extraction](onenote-extract-data.md) method to perform, for example:  or .</span></span><br/><span data-ttu-id="5810d-142">`extract.businesscard` または `extract.recipe`</span><span class="sxs-lookup"><span data-stu-id="5810d-142">`extract.businesscard` or `extract.recipe`</span></span> |
| <span data-ttu-id="5810d-143">data-render-src</span><span class="sxs-lookup"><span data-stu-id="5810d-143">data-render-src</span></span> | <span data-ttu-id="5810d-144">[抽出](onenote-extract-data.md)のコンテンツのソース。</span><span class="sxs-lookup"><span data-stu-id="5810d-144">The content source for the [extraction](onenote-extract-data.md).</span></span> |
| <span data-ttu-id="5810d-145">style</span><span class="sxs-lookup"><span data-stu-id="5810d-145">style</span></span> | <span data-ttu-id="5810d-146">div の位置、サイズ、フォント、および色のプロパティ:</span><span class="sxs-lookup"><span data-stu-id="5810d-146">The position, size, font, and color properties for the div:</span></span> <ul><li><span data-ttu-id="5810d-147">**position** (**absolute** のみ)、**left**、**top**、および **width**。(div では height が自動構成されます。)</span><span class="sxs-lookup"><span data-stu-id="5810d-147">**position** (**absolute** only), **left**, **top**, and **width**. (Height is auto-configured for divs.)</span></span><br/><br/><span data-ttu-id="5810d-148">本文が `data-absolute-enabled="true"` に設定されていて、div が本文の直接の子の場合にのみ、[絶対位置](onenote-abs-pos.md)の div の作成に使用されます。</span><span class="sxs-lookup"><span data-stu-id="5810d-148">Used to create an [absolute positioned](onenote-abs-pos.md) div, only if the div is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br/><br/><span data-ttu-id="5810d-149">例: `<div style="position:absolute;width:360px;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="5810d-149">Example: `<div style="position:absolute;width:360px;top:350px;left:300px" ... />`</span></span></li><li><span data-ttu-id="5810d-p108">要素の CSS の[スタイル](#styles)のプロパティ。出力 HTML では、これらの値は適切な子要素でインラインで返されます。</span><span class="sxs-lookup"><span data-stu-id="5810d-p108">The CSS [style](#styles) properties of the element. In the output HTML, these values are returned inline on appropriate child elements.</span></span></li></ul> |
 

<span data-ttu-id="5810d-152">Microsoft Graph の OneNote API は、すべての本文のコンテンツを 1 つ以上の div でラップします。</span><span class="sxs-lookup"><span data-stu-id="5810d-152">The OneNote APIs in Microsoft Graph wrap all body content in at least one div.</span></span> <span data-ttu-id="5810d-153">次の場合に、API は既定の div (`data-id="_default"` の属性に設定) を作成して、本文のコンテンツを含めます。</span><span class="sxs-lookup"><span data-stu-id="5810d-153">The API creates a default div (attributed with `data-id="_default"`) to contain the body content if:</span></span>

- <span data-ttu-id="5810d-p110">入力要素 body の **data-absolute-enabled** 属性が省略されたか、**false** に設定されている。この場合、すべての本文のコンテンツは既定の div に含められます。</span><span class="sxs-lookup"><span data-stu-id="5810d-p110">The input body element's **data-absolute-enabled** attribute is omitted or set to **false**. In this case, all body content is put in the default div.</span></span>

- <span data-ttu-id="5810d-156">本文の入力要素の **data-absolute-enabled** 属性は** true** ですが、入力 HTML は、[絶対位置に配置された](onenote-abs-pos.md)&nbsp;** div**、**img**、または **object** 要素ではない直接の子を含んでいます。</span><span class="sxs-lookup"><span data-stu-id="5810d-156">The input body element's **data-absolute-enabled** attribute is **true**, but the input HTML contains direct children that aren't [absolute positioned](onenote-abs-pos.md)&nbsp;**div**, **img**, or **object** elements.</span></span> <span data-ttu-id="5810d-157">この例では、[絶対位置に配置された](onenote-abs-pos.md)&nbsp;** div**、**img**、または **object** 要素ではない直接の子が、既定位置の div に配置されています。</span><span class="sxs-lookup"><span data-stu-id="5810d-157">In this case, direct children that aren't [absolute positioned](onenote-abs-pos.md)&nbsp;**div**, **img**, or **object** elements are put in the default div.</span></span>


#### <a name="output-attributes"></a><span data-ttu-id="5810d-158">出力属性</span><span class="sxs-lookup"><span data-stu-id="5810d-158">Output attributes</span></span>

|<span data-ttu-id="5810d-159">出力属性</span><span class="sxs-lookup"><span data-stu-id="5810d-159">Output attribute</span></span>|<span data-ttu-id="5810d-160">説明</span><span class="sxs-lookup"><span data-stu-id="5810d-160">Description</span></span>|
|:------|:------|
| <span data-ttu-id="5810d-161">data-id</span><span class="sxs-lookup"><span data-stu-id="5810d-161">data-id</span></span> | <span data-ttu-id="5810d-162">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="5810d-162">A reference for the element.</span></span><br/><br/><span data-ttu-id="5810d-163">[ページ コンテンツの更新](onenote_update_page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="5810d-163">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="5810d-164">id</span><span class="sxs-lookup"><span data-stu-id="5810d-164">id</span></span> | <span data-ttu-id="5810d-165">要素の一意の生成された ID。</span><span class="sxs-lookup"><span data-stu-id="5810d-165">A unique, generated ID for the element.</span></span> <span data-ttu-id="5810d-166">クエリ オプションを使用した場合に、[ページの *content* エンドポイントに対する GET 要求](../api-reference/v1.0/api/page_get.md)から返されます。`includeIDs=true`</span><span class="sxs-lookup"><span data-stu-id="5810d-166">Returned by [GET requests to a page's *content* endpoint](../api-reference/v1.0/api/page_get.md) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="5810d-167">[ページ コンテンツの更新](onenote_update_page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="5810d-167">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="5810d-168">style</span><span class="sxs-lookup"><span data-stu-id="5810d-168">style</span></span> | <span data-ttu-id="5810d-169">div の位置とサイズのプロパティ。</span><span class="sxs-lookup"><span data-stu-id="5810d-169">The position and size properties of the div.</span></span> |
 
### <a name="non-contributing-divs"></a><span data-ttu-id="5810d-170">作用していない div</span><span class="sxs-lookup"><span data-stu-id="5810d-170">Non-contributing divs</span></span>

<span data-ttu-id="5810d-p113">入力 HTML の **div** 要素がページ構造に作用しておらず、OneNote が使用する情報を含んでいない場合、API は div のコンテンツを親または既定の div に移動します。このことは次の例で示しています。</span><span class="sxs-lookup"><span data-stu-id="5810d-p113">When a **div** element in the input HTML does not contribute to the page structure or carry information that OneNote uses, the API moves the div's content into the parent or default div. This is illustrated in the following examples.</span></span>

#### <a name="input-html"></a><span data-ttu-id="5810d-173">入力 HTML</span><span class="sxs-lookup"><span data-stu-id="5810d-173">Input HTML</span></span>

<span data-ttu-id="5810d-174">作用していない入れ子型 div を含む。</span><span class="sxs-lookup"><span data-stu-id="5810d-174">Contains a non-contributing, nested div.</span></span>

```html
<html>
    <head>
        <title>Page Title</title>
    </head>
    <body>
        <div>
            <p>Some text</p>
            <div>
                <p>More text inside a div that doesn't define page structure</p>
            </div>
        </div>
    </body>
</html>
```

#### <a name="output-html"></a><span data-ttu-id="5810d-175">出力 HTML</span><span class="sxs-lookup"><span data-stu-id="5810d-175">Output HTML</span></span>

> <span data-ttu-id="5810d-176">**注:** div のコンテンツは親の div に移動し、入れ子状態の `<div>` タグが削除されました。</span><span class="sxs-lookup"><span data-stu-id="5810d-176">**Note:** The div's content was moved to the parent div and the nested `<div>` tags have been removed.</span></span> <span data-ttu-id="5810d-177">**data-id** などの意味情報が div に定義されていた場合は、div は保持されています (例: `<div data-id="keep-me">`)。</span><span class="sxs-lookup"><span data-stu-id="5810d-177">The div would have been preserved if it defined any semantic information, such as a **data-id** (example: `<div data-id="keep-me">`).</span></span>

```html
<html htmlns="http://www.w3.org/1999/xhtml" lang="en-US">
    <head>
        <title>Page Title</title>
    </head>
    <body data-absolute-enabled="true" style="font-family:Calibri;font-size:11px">
        <div data-id="_default" style="position:absolute;left:48px;top:120px;width:624px">
            <p>Some text</p>
            <p>More text inside a nested div</p>
        </div>
    </body>
</html>
```


## <a name="img-elements"></a><span data-ttu-id="5810d-178">img 要素</span><span class="sxs-lookup"><span data-stu-id="5810d-178">Img elements</span></span>

<span data-ttu-id="5810d-p115">OneNote ページの画像は **img** 要素で表されます。入力 HTML および出力 HTML では、**img** 要素に次の属性を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="5810d-p115">Images on OneNote pages are represented by **img** elements. An **img** element can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="5810d-181">入力属性</span><span class="sxs-lookup"><span data-stu-id="5810d-181">Input attributes</span></span>

|<span data-ttu-id="5810d-182">入力属性</span><span class="sxs-lookup"><span data-stu-id="5810d-182">Input attribute</span></span>|<span data-ttu-id="5810d-183">説明</span><span class="sxs-lookup"><span data-stu-id="5810d-183">Description</span></span>|
|:------|:------|
| <span data-ttu-id="5810d-184">alt</span><span class="sxs-lookup"><span data-stu-id="5810d-184">alt</span></span> | <span data-ttu-id="5810d-185">画像に指定された代替テキスト。</span><span class="sxs-lookup"><span data-stu-id="5810d-185">The supplied alt text for the image.</span></span> |
| <span data-ttu-id="5810d-186">data-id</span><span class="sxs-lookup"><span data-stu-id="5810d-186">data-id</span></span> | <span data-ttu-id="5810d-187">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="5810d-187">A reference for the element.</span></span><br/><br/><span data-ttu-id="5810d-188">[ページ コンテンツの更新](onenote_update_page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="5810d-188">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="5810d-189">data-render-src</span><span class="sxs-lookup"><span data-stu-id="5810d-189">data-render-src</span></span> |<span data-ttu-id="5810d-190">**data-render-src** か **src** のいずれかが必要です。</span><span class="sxs-lookup"><span data-stu-id="5810d-190">Either **data-render-src** or **src** is required.</span></span><br/><br/><span data-ttu-id="5810d-191">OneNote ページ上のビットマップ画像として表示する Web ページ。</span><span class="sxs-lookup"><span data-stu-id="5810d-191">The webpage to render as a bit-mapped image on the OneNote page:</span></span><br/><br/> <span data-ttu-id="5810d-192">- `data-render-src="http://..."` パブリック URL の場合は - `data-render-src="http://..."`。</span><span class="sxs-lookup"><span data-stu-id="5810d-192">- `data-render-src="http://..."` for a public URL.</span></span><br/><br/> <span data-ttu-id="5810d-193">- `data-render-src="name:BlockName"` [マルチパート要求](../api-reference/v1.0/api/section_post_pages.md#example)の "Presentation" ブロックにある画像部分の場合は `data-render-src="name:BlockName"`。</span><span class="sxs-lookup"><span data-stu-id="5810d-193">- `data-render-src="name:BlockName"` for an image part in the "Presentation" block of a [multipart request](../api-reference/v1.0/api/section_post_pages.md#example).</span></span><br/><br/><span data-ttu-id="5810d-194">このメソッドは、OneNote ページで忠実に表示できるものよりも複雑な Web ページの場合や、ページにログイン資格情報が必要な場合に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="5810d-194">This method is useful when the webpage is more complex than the OneNote page can faithfully render, or when the page requires login credentials.</span></span>|
| <span data-ttu-id="5810d-195">data-tag</span><span class="sxs-lookup"><span data-stu-id="5810d-195">data-tag</span></span> | <span data-ttu-id="5810d-196">要素の[ノート シール](onenote-note-tags.md)。</span><span class="sxs-lookup"><span data-stu-id="5810d-196">A [note tag](onenote-note-tags.md) on the element.</span></span> |
| <span data-ttu-id="5810d-197">style</span><span class="sxs-lookup"><span data-stu-id="5810d-197">style</span></span> |<span data-ttu-id="5810d-198">画像の位置とサイズのプロパティ: **position** (**absolute** のみ)、**left**、**top**、**width**、および **height**。</span><span class="sxs-lookup"><span data-stu-id="5810d-198">The position and size properties for the image: **position** (**absolute** only), **left**, **top**, **width**, and **height**.</span></span><br/><br/><span data-ttu-id="5810d-199">任意の画像のサイズを設定できます。</span><span class="sxs-lookup"><span data-stu-id="5810d-199">Size can be set on any image.</span></span><br/><br/><span data-ttu-id="5810d-200">位置プロパティは、本文が `data-absolute-enabled="true"` に設定されていて、画像が本文の直接の子である場合にのみ、[絶対位置](onenote-abs-pos.md)の画像の作成に使用されます。</span><span class="sxs-lookup"><span data-stu-id="5810d-200">Position properties are used to create an [absolute positioned](onenote-abs-pos.md) image, only if the image is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br/><br/><span data-ttu-id="5810d-201">例: `<img style="position:absolute;width:360px;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="5810d-201">Example: `<img style="position:absolute;width:360px;top:350px;left:300px" ... />`</span></span><br/><br/><span data-ttu-id="5810d-202">出力 HTML では、画像サイズは **width** 属性と **height** 属性で別々に返されます。</span><span class="sxs-lookup"><span data-stu-id="5810d-202">In the output HTML, the image size is returned separately in **width** and **height** attributes.</span></span> |
| <span data-ttu-id="5810d-203">src</span><span class="sxs-lookup"><span data-stu-id="5810d-203">src</span></span> |<span data-ttu-id="5810d-204">**src** か **data-render-src** のいずれかが必要です。</span><span class="sxs-lookup"><span data-stu-id="5810d-204">Either **src** or **data-render-src** is required.</span></span><br/><br/><span data-ttu-id="5810d-205">OneNote ページに表示する画像。</span><span class="sxs-lookup"><span data-stu-id="5810d-205">The image to render on the OneNote page:</span></span><br/><br/><span data-ttu-id="5810d-206">- `src="http://..."` インターネットで公開されている画像の URL</span><span class="sxs-lookup"><span data-stu-id="5810d-206">- `src="http://..."` for a URL to a publicly available image on the internet.</span></span><br/><br/> <span data-ttu-id="5810d-207">- `src="name:BlockName"` 画像を表すマルチパート要求の名前付き部分</span><span class="sxs-lookup"><span data-stu-id="5810d-207">- `src="name:BlockName"` for a named part in a multipart request that represents the image.</span></span>|
| <span data-ttu-id="5810d-208">width、height</span><span class="sxs-lookup"><span data-stu-id="5810d-208">width, height</span></span> | <span data-ttu-id="5810d-p116">画像の幅または高さ。ピクセル単位ですが px は付けません。例: `width="400"`</span><span class="sxs-lookup"><span data-stu-id="5810d-p116">The width or height of the image, in pixels but without the px. Example: `width="400"`</span></span> |
 
> <span data-ttu-id="5810d-211">**注:** OneNote API は入力画像の種類を自動的に検出し、それを **data-fullres-src-type** として出力 HTML に返します。</span><span class="sxs-lookup"><span data-stu-id="5810d-211">**Note:** The OneNote APIs automatically detect the input image type, and returns it as the **data-fullres-src-type** in the output HTML.</span></span> <span data-ttu-id="5810d-212">API は、**data-src-type** で最適化された画像の種類も返します。</span><span class="sxs-lookup"><span data-stu-id="5810d-212">The API also returns the image type of the optimized image in **data-src-type**.</span></span>
 

#### <a name="output-attributes"></a><span data-ttu-id="5810d-213">出力属性</span><span class="sxs-lookup"><span data-stu-id="5810d-213">Output attributes</span></span>

|<span data-ttu-id="5810d-214">出力属性</span><span class="sxs-lookup"><span data-stu-id="5810d-214">Output attribute</span></span>|<span data-ttu-id="5810d-215">説明</span><span class="sxs-lookup"><span data-stu-id="5810d-215">Description</span></span>|
|:------|:------|
| <span data-ttu-id="5810d-216">alt</span><span class="sxs-lookup"><span data-stu-id="5810d-216">alt</span></span> | <span data-ttu-id="5810d-217">画像に指定された代替テキスト。</span><span class="sxs-lookup"><span data-stu-id="5810d-217">The supplied alt text for the image.</span></span> |
| <span data-ttu-id="5810d-218">data-id</span><span class="sxs-lookup"><span data-stu-id="5810d-218">data-id</span></span> | <span data-ttu-id="5810d-219">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="5810d-219">A reference for the element.</span></span><br/><br/><span data-ttu-id="5810d-220">[ページ コンテンツの更新](onenote_update_page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="5810d-220">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="5810d-221">data-index</span><span class="sxs-lookup"><span data-stu-id="5810d-221">data-index</span></span> | <span data-ttu-id="5810d-p118">画像の位置。[分割された画像](#split-images)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5810d-p118">The position of the image. For [split image](#split-images) support.</span></span> |
| <span data-ttu-id="5810d-224">data-fullres-src</span><span class="sxs-lookup"><span data-stu-id="5810d-224">data-fullres-src</span></span> | <span data-ttu-id="5810d-225">最初にページに埋め込まれていた画像リソースのバージョンのエンドポイント。</span><span class="sxs-lookup"><span data-stu-id="5810d-225">The endpoint for the version of the image resource that was originally embedded in the page.</span></span> |
| <span data-ttu-id="5810d-226">data-fullres-src-type</span><span class="sxs-lookup"><span data-stu-id="5810d-226">data-fullres-src-type</span></span> | <span data-ttu-id="5810d-227">**data-fullres-src** リソースのメディアの種類。たとえば、`image/png` または`image/jpeg`。</span><span class="sxs-lookup"><span data-stu-id="5810d-227">The media type of the **data-fullres-src** resource, for example: `image/png` or `image/jpeg`.</span></span> |
| <span data-ttu-id="5810d-228">data-options</span><span class="sxs-lookup"><span data-stu-id="5810d-228">data-options</span></span> | <span data-ttu-id="5810d-229">ソースの種類。PDF ファイルの場合は **printout**、その他のファイルはいずれも **splitimage**。</span><span class="sxs-lookup"><span data-stu-id="5810d-229">The source type: **printout** for PDF files or **splitimage** for all others.</span></span> <span data-ttu-id="5810d-230">**data-render-src** 属性で作成された、[分割された画像](#split-images)にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="5810d-230">Applies only to [split images](#split-images) created with the **data-render-src** attribute.</span></span> |
| <span data-ttu-id="5810d-231">data-render-original-src</span><span class="sxs-lookup"><span data-stu-id="5810d-231">data-render-original-src</span></span> | <span data-ttu-id="5810d-232">ソース画像が公開されたインターネットの画像で、**data-render-src** 属性を付けて作成された場合の、画像の最初のソース URL。</span><span class="sxs-lookup"><span data-stu-id="5810d-232">The original source URL of the image, if the source image is from the public internet and was created with the **data-render-src** attribute.</span></span> |
| <span data-ttu-id="5810d-233">data-src-type</span><span class="sxs-lookup"><span data-stu-id="5810d-233">data-src-type</span></span> | <span data-ttu-id="5810d-234">**src** リソースのメディアの種類。たとえば、`image/png` または`image/jpeg`。</span><span class="sxs-lookup"><span data-stu-id="5810d-234">The media type of the **src** resource, for example: `image/png` or `image/jpeg`.</span></span> |
| <span data-ttu-id="5810d-235">data-tag</span><span class="sxs-lookup"><span data-stu-id="5810d-235">data-tag</span></span> | <span data-ttu-id="5810d-236">要素の[ノート シール](onenote-note-tags.md)。</span><span class="sxs-lookup"><span data-stu-id="5810d-236">A [note tag](onenote-note-tags.md) on the element.</span></span> |
| <span data-ttu-id="5810d-237">id</span><span class="sxs-lookup"><span data-stu-id="5810d-237">id</span></span> | <span data-ttu-id="5810d-238">要素の一意の生成された ID。</span><span class="sxs-lookup"><span data-stu-id="5810d-238">A unique, generated ID for the element.</span></span> <span data-ttu-id="5810d-239">クエリ オプションを使用した場合に、[ページの *content* エンドポイントに対する GET 要求](../api-reference/v1.0/api/page_get.md)から返されます。`includeIDs=true`</span><span class="sxs-lookup"><span data-stu-id="5810d-239">Returned by [GET requests to a page's *content* endpoint](../api-reference/v1.0/api/page_get.md) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="5810d-240">[ページ コンテンツの更新](onenote_update_page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="5810d-240">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="5810d-241">src</span><span class="sxs-lookup"><span data-stu-id="5810d-241">src</span></span> | <span data-ttu-id="5810d-242">Web ブラウザー、モバイル、およびタブレットのフォーム ファクター向けに最適化された画像リソースのバージョンのエンドポイント。</span><span class="sxs-lookup"><span data-stu-id="5810d-242">The endpoint for the version of the image resource that has been optimized for web browsers and mobile and tablet form factors.</span></span> |
| <span data-ttu-id="5810d-243">style</span><span class="sxs-lookup"><span data-stu-id="5810d-243">style</span></span> | <span data-ttu-id="5810d-244">画像の位置のプロパティ。</span><span class="sxs-lookup"><span data-stu-id="5810d-244">The position properties of the image.</span></span> |
| <span data-ttu-id="5810d-245">width、height</span><span class="sxs-lookup"><span data-stu-id="5810d-245">width, height</span></span> | <span data-ttu-id="5810d-246">画像の幅または高さ (ピクセル単位)。</span><span class="sxs-lookup"><span data-stu-id="5810d-246">The width or height of the image, in pixels.</span></span> |
 

### <a name="output-html-examples-for-images"></a><span data-ttu-id="5810d-247">画像の出力 HTML の例</span><span class="sxs-lookup"><span data-stu-id="5810d-247">Output HTML examples for images</span></span>

<span data-ttu-id="5810d-p121">出力 **img** 要素には、次に示すとおり、画像ファイルのリソースおよび画像の種類のためのエンドポイントが含まれています。バイナリ コンテンツを取得するには、[画像リソースのエンドポイントに対して個別に GET 要求を実行](../api-reference/v1.0/api/resource_get.md)します。</span><span class="sxs-lookup"><span data-stu-id="5810d-p121">Output **img** elements contain endpoints for image file resources and the image type, as shown below. You can make separate [GET requests to image resource endpoints](../api-reference/v1.0/api/resource_get.md) to retrieve their binary contents.</span></span>

```html
<img 
    src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/$value"  
    data-src-type="image/png"
    data-fullres-src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/$value"  
    data-fullres-src-type="image/png" ... />
```

<span data-ttu-id="5810d-p122">既定では、画像は、ページ コンテンツの残りの部分と同様、それらを取得するために承認を必要とするため、ブラウザーで直接表示されることはありません。ページにある画像リソースへの公開 URL を取得するには、ページ コンテンツを取得する際に、クエリ文字列に **preAuthenticated=true** を含めます (例: `GET ../pages/{page-id}/content?preAuthenticated=true`)。返される公開 URL は 1 時間有効です。</span><span class="sxs-lookup"><span data-stu-id="5810d-p122">By default, images won't render directly in a browser because they are private and require authorization to retrieve them, like the rest of the page contents. To get public URLs to the image resources on a page, include **preAuthenticated=true** in the query string when you retrieve the page content (example: `GET ../pages/{page-id}/content?preAuthenticated=true`). The public URLs that are returned are valid for one hour.</span></span> 

#### <a name="image-with-public-url-when-preauthenticatedtrue-is-included-in-the-request"></a><span data-ttu-id="5810d-253">要求に _preAuthenticated=true_ が含まれる場合の、パブリック URL を使用する画像</span><span class="sxs-lookup"><span data-stu-id="5810d-253">Image with public URL when _preAuthenticated=true_ is included in the request</span></span>

```html
<img 
    width="170" height="128" 
    src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/content?publicAuth=true&mimeType=image/jpeg" 
    data-src-type="image/{type}" 
    data-fullres-src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/content?publicAuth=true&mimeType=image/jpeg" 
    data-fullres-src-type="image/{type}"
/>
```

<span data-ttu-id="5810d-254">次の例は、**img** 要素が出力 HTML に含む可能性がある情報を示しています。</span><span class="sxs-lookup"><span data-stu-id="5810d-254">The following examples show the information an **img** element might contain in the output HTML.</span></span>

#### <a name="image-with-web-ready-and-high-resolution-resources"></a><span data-ttu-id="5810d-255">Web 対応の高解像度リソースがある画像</span><span class="sxs-lookup"><span data-stu-id="5810d-255">Image with web-ready and high resolution resources</span></span>

```html
<img
    src="{web-ready-image-resource-url}/$value"
    data-src-type="image/{type}"
    data-fullres-src="{high-resolution-image-resource-url}/$value"
    data-fullres-src-type="image/{type}"
    [data-render-original-src="{original-source-url-or-named-part}"]
    [data-id="{image-id}"]
    [alt="supplied alt text"]
    [width="345"] [height="180"]
    [style="..."] />
```

#### <a name="image-created-by-using-the-data-render-src-attribute"></a><span data-ttu-id="5810d-256">*data-render-src* 属性を使用して作成された画像</span><span class="sxs-lookup"><span data-stu-id="5810d-256">Image created by using the *data-render-src* attribute</span></span>

```html
<img
    src="{web-ready-image-resource-url}/$value"
    data-src-type="image/{type}"
    data-fullres-src="{high-resolution-image-resource-url}/$value"
    data-fullres-src-type="image/{type}"
    data-render-original-src="{original-source-url-or-named-part}"
    [data-id="{image-id}"]
    [data-index="{index-of-split-image}"]
    [data-options="{printout-or-splitimage}"]
    [alt="supplied alt text"]
    [width="1024"] [height="1900"]
    [style="..."] />
```

### <a name="split-images"></a><span data-ttu-id="5810d-257">分割された画像</span><span class="sxs-lookup"><span data-stu-id="5810d-257">Split images</span></span>

<span data-ttu-id="5810d-p123">**data-render-src** 属性 (Web ページの URL または名前が付いた部分のもの) を使用して作成された画像は、パフォーマンスと表示上の理由から複数のコンポーネントの画像に分割されることがあります。コンポーネント画像には、すべて同じ **data-id** 値が割り当てられます。各コンポーネントの画像には、元の垂直レイアウトを定義するゼロベースの data-index 属性があります。</span><span class="sxs-lookup"><span data-stu-id="5810d-p123">Images that are created using the **data-render-src** attribute (from a webpage URL or a named part) might be split into multiple component images for performance and rendering reasons. Component images are all assigned the same **data-id** value. Each component image has a zero-based data-index attribute that defines the original vertical layout.</span></span>

#### <a name="split-image-with-three-component-images"></a><span data-ttu-id="5810d-261">画像を 3 つのコンポーネントの画像に分割する</span><span class="sxs-lookup"><span data-stu-id="5810d-261">Split image with three component images</span></span>

```html
<div data-id="multi-component-image" style="position:absolute;left:48px;top:120px;width:624px">
    <img
        src="{image-resource0-url}/$value"
        data-src-type="image/{type}"
        data-fullres-src="{image-resource0-url}/$value" 
        data-fullres-src-type="image/{type}" 
        data-index="0" 
        data-render-original-src="{original-source-url-or-named-part}"
        data-id="{same-image-id}" ... />
    <img 
        src="{image-resource1-url}/$value" 
        data-src-type="image/{type}" 
        data-fullres-src="{image-resource1-url}/$value" 
        data-fullres-src-type="image/{type}" 
        data-index="1" 
        data-render-original-src="{original-source-url-or-named-part}"
        data-id="{same-image-id}" ... />
    <img 
        src="{image-resource2-url}/$value" 
        data-src-type="image/{type}" 
        data-fullres-src="{image-resource2-url}/$value" 
        data-fullres-src-type="image/{type}" 
        data-index="2" 
        data-render-original-src=""{original-source-url-or-named-part}"
        data-id="{same-image-id}" ... />
</div>
```

<span data-ttu-id="5810d-262">ユーザーはページ上の画像を移動することができるため、返されるインデックスが不適切である可能性があります。</span><span class="sxs-lookup"><span data-stu-id="5810d-262">Because users can move the images on the page, the returned indexes might be out of order. Ordering should be in top to bottom y-order, then left to right x-order if there are y-order conflicts.</span></span> <span data-ttu-id="5810d-263">順序は、y 軸方向の上から下に、続いて、y 軸方向の競合がある場合、x 軸方向の左から右にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="5810d-263">Because users can move the images on the page, the returned indexes might be out of order. Ordering should be in top to bottom y-order, then left to right x-order if there are y-order conflicts.</span></span>

## <a name="iframe-elements"></a><span data-ttu-id="5810d-264">iframe 要素</span><span class="sxs-lookup"><span data-stu-id="5810d-264">iframe elements</span></span>

<span data-ttu-id="5810d-265">OneNote ページには、**iframe** 要素で表される埋め込みビデオを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="5810d-265">OneNote pages can contain embedded videos represented by **iframe** elements.</span></span> 

> <span data-ttu-id="5810d-266">**注:** [**object** 要素を使用してビデオ ファイルを添付](onenote_images_files.md#adding-files)することもできます。</span><span class="sxs-lookup"><span data-stu-id="5810d-266">**Note:** You can also [attach a video file using an **object** element](onenote_images_files.md#adding-files).</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="5810d-267">入力属性</span><span class="sxs-lookup"><span data-stu-id="5810d-267">Input attributes</span></span>

|<span data-ttu-id="5810d-268">入力属性</span><span class="sxs-lookup"><span data-stu-id="5810d-268">Input attribute</span></span>|<span data-ttu-id="5810d-269">説明</span><span class="sxs-lookup"><span data-stu-id="5810d-269">Description</span></span>|
|:------|:------|
| <span data-ttu-id="5810d-270">data-original-src</span><span class="sxs-lookup"><span data-stu-id="5810d-270">data-original-src</span></span> | <span data-ttu-id="5810d-271">必須。</span><span class="sxs-lookup"><span data-stu-id="5810d-271">Required.</span></span> <span data-ttu-id="5810d-272">ビデオ ソースの URL。</span><span class="sxs-lookup"><span data-stu-id="5810d-272">The URL of the video source.</span></span> <span data-ttu-id="5810d-273">[サポートされるビデオ ソースの一覧](onenote_images_files.md#adding-videos)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5810d-273">See the [list of supported video sources](onenote_images_files.md#adding-videos).</span></span> <br/><br/><span data-ttu-id="5810d-274">例: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span><span class="sxs-lookup"><span data-stu-id="5810d-274">Example: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span></span> |
| <span data-ttu-id="5810d-275">width、height</span><span class="sxs-lookup"><span data-stu-id="5810d-275">width, height</span></span> | <span data-ttu-id="5810d-p126">iframe の幅と高さ (ピクセル単位)。例: `width=300`</span><span class="sxs-lookup"><span data-stu-id="5810d-p126">The width or height of the iframe, in pixels. Example: `width=300`</span></span> |

#### <a name="output-attributes"></a><span data-ttu-id="5810d-278">出力属性</span><span class="sxs-lookup"><span data-stu-id="5810d-278">Output attributes</span></span>

|<span data-ttu-id="5810d-279">出力属性</span><span class="sxs-lookup"><span data-stu-id="5810d-279">Output attribute</span></span>|<span data-ttu-id="5810d-280">説明</span><span class="sxs-lookup"><span data-stu-id="5810d-280">Description</span></span>|
|:------|:------|
| <span data-ttu-id="5810d-281">data-original-src</span><span class="sxs-lookup"><span data-stu-id="5810d-281">data-original-src</span></span> | <span data-ttu-id="5810d-282">ビデオ ソースの URL。</span><span class="sxs-lookup"><span data-stu-id="5810d-282">The URL of the video source.</span></span> |
| <span data-ttu-id="5810d-283">src</span><span class="sxs-lookup"><span data-stu-id="5810d-283">src</span></span> | <span data-ttu-id="5810d-284">OneNote ページに埋め込まれたビデオへのリンク。</span><span class="sxs-lookup"><span data-stu-id="5810d-284">A link to the video that is embedded in the OneNote page.</span></span> |
| <span data-ttu-id="5810d-285">width、height</span><span class="sxs-lookup"><span data-stu-id="5810d-285">width, height</span></span> | <span data-ttu-id="5810d-286">iframe の幅と高さ (ピクセル単位)。</span><span class="sxs-lookup"><span data-stu-id="5810d-286">The width or height of the iframe, in pixels.</span></span><br/><br/><span data-ttu-id="5810d-287">例: `width=300`</span><span class="sxs-lookup"><span data-stu-id="5810d-287">Example: `width=300`</span></span> |
 
### <a name="output-html-example-for-videos"></a><span data-ttu-id="5810d-288">ビデオの出力 HTML の例</span><span class="sxs-lookup"><span data-stu-id="5810d-288">Output HTML example for videos</span></span>

<span data-ttu-id="5810d-289">次に示すように、出力 **iframe** 要素には、ソース ページとビデオに関連付けられたエンドポイントが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5810d-289">Output **iframe** elements contain endpoints that link to the source page and video, as shown.</span></span> 

```html
<iframe 
    width="340" height="280" 
    data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8" 
    src="https://www.youtube.com/embed/3Ztr44aKmQ8?feature=oembed&autoplay=true" />
``` 

## <a name="object-elements"></a><span data-ttu-id="5810d-290">object 要素</span><span class="sxs-lookup"><span data-stu-id="5810d-290">Object elements</span></span>

<span data-ttu-id="5810d-p127">OneNote ページには、**object** 要素で表される添付ファイルを含めることができます。**object** 要素は、入力 HTML および出力 HTML に次の属性を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="5810d-p127">OneNote pages can contain file attachments represented by **object** elements. An **object** element can contain the following attributes in the input and output HTML.</span></span>

> <span data-ttu-id="5810d-293">**注:** ファイルが画像として送信され、**data-render-src** 属性を使用する場合、OneNote API はファイルのコンテンツを画像としてページに表示できます。</span><span class="sxs-lookup"><span data-stu-id="5810d-293">**Note:** The OneNote APIs can also render file content as images in a page when the file is sent as an image and uses the **data-render-src** attribute.</span></span>
> <span data-ttu-id="5810d-294">例: `<img data-render-src="name:part-name" ... />`</span><span class="sxs-lookup"><span data-stu-id="5810d-294">Example: `<img data-render-src="name:part-name" ... />`</span></span>
 

#### <a name="input-attributes"></a><span data-ttu-id="5810d-295">入力属性</span><span class="sxs-lookup"><span data-stu-id="5810d-295">Input attributes</span></span>

|<span data-ttu-id="5810d-296">入力属性</span><span class="sxs-lookup"><span data-stu-id="5810d-296">Input attribute</span></span>|<span data-ttu-id="5810d-297">説明</span><span class="sxs-lookup"><span data-stu-id="5810d-297">Description</span></span>|
|:------|:------|
| <span data-ttu-id="5810d-298">data</span><span class="sxs-lookup"><span data-stu-id="5810d-298">data</span></span> | <span data-ttu-id="5810d-p129">必須。[マルチパート要求](../api-reference/v1.0/api/section_post_pages.md#example)のファイルを表す部分の名前。</span><span class="sxs-lookup"><span data-stu-id="5810d-p129">Required. The name of the part that represents the file in the [multipart request](../api-reference/v1.0/api/section_post_pages.md#example).</span></span> |
| <span data-ttu-id="5810d-301">data-attachment</span><span class="sxs-lookup"><span data-stu-id="5810d-301">data-attachment</span></span> | <span data-ttu-id="5810d-p130">必須。ファイル名。</span><span class="sxs-lookup"><span data-stu-id="5810d-p130">Required. The file name.</span></span> |
| <span data-ttu-id="5810d-304">data-id</span><span class="sxs-lookup"><span data-stu-id="5810d-304">data-id</span></span> | <span data-ttu-id="5810d-305">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="5810d-305">A reference for the element.</span></span><br/><br/><span data-ttu-id="5810d-306">[ページ コンテンツの更新](onenote_update_page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="5810d-306">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="5810d-307">style</span><span class="sxs-lookup"><span data-stu-id="5810d-307">style</span></span> | <span data-ttu-id="5810d-308">オブジェクトの位置とサイズのプロパティ: **position** (**absolute** のみ)、**left**、**top**、および **width**。</span><span class="sxs-lookup"><span data-stu-id="5810d-308">The position and size properties for the object: **position** (**absolute** only), **left**, **top**, and **width**.</span></span><br/><br/><span data-ttu-id="5810d-309">本文が `data-absolute-enabled="true"` に設定されていて、オブジェクトが本文の直接の子の場合にのみ、[絶対位置](onenote-abs-pos.md)のオブジェクトの作成に使用されます。</span><span class="sxs-lookup"><span data-stu-id="5810d-309">Used to create an [absolute positioned](onenote-abs-pos.md) object, only if the object is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br/><br/><span data-ttu-id="5810d-310">例: `<object style="position:absolute;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="5810d-310">Example: `<object style="position:absolute;top:350px;left:300px" ... />`</span></span> |
| <span data-ttu-id="5810d-311">type</span><span class="sxs-lookup"><span data-stu-id="5810d-311">type</span></span> | <span data-ttu-id="5810d-312">必須。</span><span class="sxs-lookup"><span data-stu-id="5810d-312">Required.</span></span><br/><br/><span data-ttu-id="5810d-313">標準のメディア ファイルの種類。</span><span class="sxs-lookup"><span data-stu-id="5810d-313">The standard media file type.</span></span> <span data-ttu-id="5810d-314">既知のファイルの型では、OneNote ページにファイルの種類と関連付けられたアイコンが表示されます。</span><span class="sxs-lookup"><span data-stu-id="5810d-314">Required. The standard media file type. Known file types display the icon associated with the file type on the OneNote page. Unknown file types display a generic file icon.</span></span> <span data-ttu-id="5810d-315">未知のファイルの型では、汎用のファイル アイコンが表示されます。</span><span class="sxs-lookup"><span data-stu-id="5810d-315">Unknown file types display a generic file icon.</span></span> |
<!--todo: add link to known file types--> 

#### <a name="output-attributes"></a><span data-ttu-id="5810d-316">出力属性</span><span class="sxs-lookup"><span data-stu-id="5810d-316">Output attributes</span></span>

|<span data-ttu-id="5810d-317">出力属性</span><span class="sxs-lookup"><span data-stu-id="5810d-317">Output attribute</span></span>|<span data-ttu-id="5810d-318">説明</span><span class="sxs-lookup"><span data-stu-id="5810d-318">Description</span></span>|
|:------|:------|
| <span data-ttu-id="5810d-319">data</span><span class="sxs-lookup"><span data-stu-id="5810d-319">data</span></span> | <span data-ttu-id="5810d-320">ファイルのリソースのエンドポイント。</span><span class="sxs-lookup"><span data-stu-id="5810d-320">The endpoint for the file resource.</span></span> |
| <span data-ttu-id="5810d-321">data-attachment</span><span class="sxs-lookup"><span data-stu-id="5810d-321">data-attachment</span></span> | <span data-ttu-id="5810d-322">ファイル名。</span><span class="sxs-lookup"><span data-stu-id="5810d-322">The file name.</span></span> |
| <span data-ttu-id="5810d-323">data-id</span><span class="sxs-lookup"><span data-stu-id="5810d-323">data-id</span></span> | <span data-ttu-id="5810d-324">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="5810d-324">A reference for the element.</span></span><br/><br/><span data-ttu-id="5810d-325">[ページ コンテンツの更新](onenote_update_page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="5810d-325">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="5810d-326">id</span><span class="sxs-lookup"><span data-stu-id="5810d-326">id</span></span> | <span data-ttu-id="5810d-327">要素の一意の生成された ID。</span><span class="sxs-lookup"><span data-stu-id="5810d-327">A unique, generated ID for the element.</span></span> <span data-ttu-id="5810d-328">クエリ オプションを使用した場合に、[ページの *content* エンドポイントに対する GET 要求](../api-reference/v1.0/api/page_get.md)から返されます。`includeIDs=true`</span><span class="sxs-lookup"><span data-stu-id="5810d-328">Returned by [GET requests to a page's *content* endpoint](../api-reference/v1.0/api/page_get.md) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="5810d-329">[ページ コンテンツの更新](onenote_update_page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="5810d-329">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="5810d-330">style</span><span class="sxs-lookup"><span data-stu-id="5810d-330">style</span></span> | <span data-ttu-id="5810d-331">オブジェクトの位置のプロパティ。</span><span class="sxs-lookup"><span data-stu-id="5810d-331">The position properties of the object.</span></span> |
| <span data-ttu-id="5810d-332">type</span><span class="sxs-lookup"><span data-stu-id="5810d-332">type</span></span> | <span data-ttu-id="5810d-333">標準のメディア ファイルの種類。</span><span class="sxs-lookup"><span data-stu-id="5810d-333">The standard media file type.</span></span> |
 

#### <a name="output-html-example-for-objects"></a><span data-ttu-id="5810d-334">オブジェクトの出力 HTML の例</span><span class="sxs-lookup"><span data-stu-id="5810d-334">Output HTML example for objects</span></span>

<span data-ttu-id="5810d-335">次に示すように、出力 **object** 要素には、ページ内のファイル リソースにリンクされたエンドポイントが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5810d-335">Output **object** elements contain endpoints that link to the file resources in the page, as shown.</span></span> <span data-ttu-id="5810d-336">バイナリ コンテンツを取得するには、これらの[ファイル リソースのエンドポイントに対して個別の GET 要求](../api-reference/v1.0/api/resource_get.md)を実行します。</span><span class="sxs-lookup"><span data-stu-id="5810d-336">You can make separate [GET requests to file resource endpoints](../api-reference/v1.0/api/resource_get.md) to retrieve their binary contents.</span></span>

```html
<object
    data="https://graph.microsoft.com/v1.0/me/onenote/resources/{file-id}/$value"
    data-attachment="fileName.pdf" 
    type="application/pdf" 
    [style="..."] />
``` 

## <a name="paragraphs-and-headings"></a><span data-ttu-id="5810d-337">段落と見出し</span><span class="sxs-lookup"><span data-stu-id="5810d-337">Paragraphs and headings</span></span>

<span data-ttu-id="5810d-338">段落、見出し、その他のテキストのコンテナーには、入力 HTML と出力 HTML の次の属性を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="5810d-338">Paragraphs, headings, and other text containers can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="5810d-339">入力属性</span><span class="sxs-lookup"><span data-stu-id="5810d-339">Input attributes</span></span>

|<span data-ttu-id="5810d-340">入力属性</span><span class="sxs-lookup"><span data-stu-id="5810d-340">Input attribute</span></span>|<span data-ttu-id="5810d-341">説明</span><span class="sxs-lookup"><span data-stu-id="5810d-341">Description</span></span>|
|:------|:------|
| <span data-ttu-id="5810d-342">data-id</span><span class="sxs-lookup"><span data-stu-id="5810d-342">data-id</span></span> | <span data-ttu-id="5810d-343">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="5810d-343">A reference for the element.</span></span><br/><br/><span data-ttu-id="5810d-344">[ページ コンテンツの更新](onenote_update_page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="5810d-344">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="5810d-345">data-tag</span><span class="sxs-lookup"><span data-stu-id="5810d-345">data-tag</span></span> | <span data-ttu-id="5810d-346">**p** 要素または **h1** - **h6** 要素上の[ノート シール](onenote-note-tags.md)。</span><span class="sxs-lookup"><span data-stu-id="5810d-346">A [note tag](onenote-note-tags.md) on a **p** or **h1** - **h6** element.</span></span> |
| <span data-ttu-id="5810d-347">style</span><span class="sxs-lookup"><span data-stu-id="5810d-347">style</span></span> | <span data-ttu-id="5810d-348">要素の CSS [style](#styles)のプロパティ。</span><span class="sxs-lookup"><span data-stu-id="5810d-348">The CSS [style](#styles) properties of the element.</span></span> |
 

#### <a name="output-attributes"></a><span data-ttu-id="5810d-349">出力属性</span><span class="sxs-lookup"><span data-stu-id="5810d-349">Output attributes</span></span>

|<span data-ttu-id="5810d-350">出力属性</span><span class="sxs-lookup"><span data-stu-id="5810d-350">Output attribute</span></span>|<span data-ttu-id="5810d-351">説明</span><span class="sxs-lookup"><span data-stu-id="5810d-351">Description</span></span>|
|:------|:------|
| <span data-ttu-id="5810d-352">data-id</span><span class="sxs-lookup"><span data-stu-id="5810d-352">data-id</span></span> | <span data-ttu-id="5810d-353">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="5810d-353">A reference for the element.</span></span><br/><br/><span data-ttu-id="5810d-354">[ページ コンテンツの更新](onenote_update_page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="5810d-354">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="5810d-355">data-tag</span><span class="sxs-lookup"><span data-stu-id="5810d-355">data-tag</span></span> | <span data-ttu-id="5810d-356">**p** 要素または **h1** - **h6** 要素上の[ノート シール](onenote-note-tags.md)。</span><span class="sxs-lookup"><span data-stu-id="5810d-356">A [note tag](onenote-note-tags.md) on a **p** or **h1** - **h6** element.</span></span> |
| <span data-ttu-id="5810d-357">id</span><span class="sxs-lookup"><span data-stu-id="5810d-357">id</span></span> | <span data-ttu-id="5810d-358">要素の一意の生成された ID。</span><span class="sxs-lookup"><span data-stu-id="5810d-358">A unique, generated ID for the element.</span></span> <span data-ttu-id="5810d-359">クエリ オプションを使用した場合に、[ページの *content* エンドポイントに対する GET 要求](../api-reference/v1.0/api/page_get.md)から返されます。`includeIDs=true`</span><span class="sxs-lookup"><span data-stu-id="5810d-359">Returned by [GET requests to a page's *content* endpoint](../api-reference/v1.0/api/page_get.md) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="5810d-360">[ページ コンテンツの更新](onenote_update_page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="5810d-360">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="5810d-361">style</span><span class="sxs-lookup"><span data-stu-id="5810d-361">style</span></span> | <span data-ttu-id="5810d-p135">要素の CSS [style](#styles)のプロパティ。出力 HTML では、これらの値は、適切な子要素または **span** 要素でインラインで返すことができます。</span><span class="sxs-lookup"><span data-stu-id="5810d-p135">The CSS [style](#styles) properties of the element. In the output HTML, these values may be returned inline on appropriate child elements or on **span** elements.</span></span> |
 

<span data-ttu-id="5810d-364">次の例では、テキストのコンテナーおよび返される出力 HTML にスタイルを定義するさまざまな方法を使用する入力 HTML を示しています。</span><span class="sxs-lookup"><span data-stu-id="5810d-364">The following examples show input HTML that uses different ways to define styles on text containers and the output HTML that's returned.</span></span>

#### <a name="input-html-with-styles-defined-using-inline-character-styles-in-the-start-tag-and-within-a-span-element"></a><span data-ttu-id="5810d-365">開始タグ内、および span 要素内に、インライン文字スタイルを使用して定義されたスタイル付き 入力 HTML。</span><span class="sxs-lookup"><span data-stu-id="5810d-365">Input HTML with styles defined using inline character styles, in the start tag, and within a span element.</span></span>

```html
<h1>Heading <i>One</i> text</h1>
<p style="font-size:8pt;color:green;font-family:Courier;text-align:center">Some text</p>
<p>Some <span  style="font-size:16px;color:#ff0000;font-family:Segoe UI Black">more</span> text</p>
``` 

#### <a name="output-html-with-the-i-character-style-and-the-font-settings-in-the-p-start-tag-returned-as-inline-css-styles-on-span-elements"></a><span data-ttu-id="5810d-366">span 要素でインライン CSS スタイルとして返される `<p>` 開始タグ内の `<i>` 文字スタイルとフォント設定を伴う出力 HTML。</span><span class="sxs-lookup"><span data-stu-id="5810d-366">Output HTML with the `<i>` character style and the font settings in the `<p>` start tag returned as inline CSS styles on span elements.</span></span>

```html
<h1 style="font-size:16pt;color:#1e4e79;margin-top:11pt;margin-bottom:11pt">Heading <span style="font-style:italic">One</span> text</h1>
<p style="text-align:center"><span style="font-family:Courier;font-size:8pt;color:green">Some text</span></p>
<p>Some <span style="font-family:Segoe UI Black;font-size:12pt;color:red">more</span> text</p>
``` 


## <a name="lists"></a><span data-ttu-id="5810d-367">リスト</span><span class="sxs-lookup"><span data-stu-id="5810d-367">Lists</span></span>

<span data-ttu-id="5810d-368">リストは、**li** 要素を含む **ol** 要素または **ul** 要素として表されます。</span><span class="sxs-lookup"><span data-stu-id="5810d-368">Lists are represented as **ol** or **ul** elements that contain list items represented as **li** elements.</span></span>

<span data-ttu-id="5810d-369">入力 HTML および出力 HTML には、リストとリスト項目に次の属性を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="5810d-369">Lists and list items can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="5810d-370">入力属性</span><span class="sxs-lookup"><span data-stu-id="5810d-370">Input attributes</span></span>

|<span data-ttu-id="5810d-371">入力属性</span><span class="sxs-lookup"><span data-stu-id="5810d-371">Input attribute</span></span>|<span data-ttu-id="5810d-372">説明</span><span class="sxs-lookup"><span data-stu-id="5810d-372">Description</span></span>|
|:------|:------|
| <span data-ttu-id="5810d-373">data-id</span><span class="sxs-lookup"><span data-stu-id="5810d-373">data-id</span></span> | <span data-ttu-id="5810d-374">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="5810d-374">A reference for the element.</span></span><br/><br/><span data-ttu-id="5810d-375">[ページ コンテンツの更新](onenote_update_page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="5810d-375">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="5810d-376">data-tag</span><span class="sxs-lookup"><span data-stu-id="5810d-376">data-tag</span></span> | <span data-ttu-id="5810d-377">**ul**、**ol**、または **li** の各要素上の[ノート シール](onenote-note-tags.md)。</span><span class="sxs-lookup"><span data-stu-id="5810d-377">A [note tag](onenote-note-tags.md) on a **ul**, **ol**, or **li** element.</span></span> |
| <span data-ttu-id="5810d-378">style</span><span class="sxs-lookup"><span data-stu-id="5810d-378">style</span></span> | <span data-ttu-id="5810d-379">リストまたはリスト項目の **list-style-type** および CSS [style](#styles) のプロパティ。</span><span class="sxs-lookup"><span data-stu-id="5810d-379">The **list-style-type** and the CSS [style](#styles) properties for the list or list item.</span></span> |
 

#### <a name="output-attributes"></a><span data-ttu-id="5810d-380">出力属性</span><span class="sxs-lookup"><span data-stu-id="5810d-380">Output attributes</span></span>

|<span data-ttu-id="5810d-381">出力属性</span><span class="sxs-lookup"><span data-stu-id="5810d-381">Output attribute</span></span>|<span data-ttu-id="5810d-382">説明</span><span class="sxs-lookup"><span data-stu-id="5810d-382">Description</span></span>|
|:------|:------|
| <span data-ttu-id="5810d-383">data-id</span><span class="sxs-lookup"><span data-stu-id="5810d-383">data-id</span></span> | <span data-ttu-id="5810d-384">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="5810d-384">A reference for the element.</span></span><br/><br/><span data-ttu-id="5810d-385">[ページ コンテンツの更新](onenote_update_page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="5810d-385">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="5810d-386">data-tag</span><span class="sxs-lookup"><span data-stu-id="5810d-386">data-tag</span></span> |  <span data-ttu-id="5810d-387">**li** 要素内の span 上の[ノート シール](onenote-note-tags.md)。</span><span class="sxs-lookup"><span data-stu-id="5810d-387">A [note tag](onenote-note-tags.md) on a span in a **li** element.</span></span> |
| <span data-ttu-id="5810d-388">id</span><span class="sxs-lookup"><span data-stu-id="5810d-388">id</span></span> | <span data-ttu-id="5810d-389">要素の一意の生成された ID。</span><span class="sxs-lookup"><span data-stu-id="5810d-389">A unique, generated ID for the element.</span></span> <span data-ttu-id="5810d-390">クエリ オプションを使用した場合に、[ページの *content* エンドポイントに対する GET 要求](../api-reference/v1.0/api/page_get.md)から返されます。`includeIDs=true`</span><span class="sxs-lookup"><span data-stu-id="5810d-390">Returned by [GET requests to a page's *content* endpoint](../api-reference/v1.0/api/page_get.md) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="5810d-391">[ページ コンテンツの更新](onenote_update_page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="5810d-391">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="5810d-392">style</span><span class="sxs-lookup"><span data-stu-id="5810d-392">style</span></span> | <span data-ttu-id="5810d-p137">要素の **list-style-type** および CSS [style](#styles)のプロパティ。出力 HTML では、リストレベル設定はリスト項目で返されます。既定のプロパティは返されません。</span><span class="sxs-lookup"><span data-stu-id="5810d-p137">The **list-style-type** and CSS [style](#styles) properties of the element. In the output HTML, list-level settings are returned on list items. Default properties are not returned.</span></span> |
 
### <a name="list-styles"></a><span data-ttu-id="5810d-396">リストのスタイル</span><span class="sxs-lookup"><span data-stu-id="5810d-396">List styles</span></span>

<span data-ttu-id="5810d-397">Microsoft Graph の OneNote API では、次のリストのスタイルをサポートします。</span><span class="sxs-lookup"><span data-stu-id="5810d-397">The OneNote APIs in Microsoft Graph support the following list styles:</span></span>

|<span data-ttu-id="5810d-398">番号付きリスト</span><span class="sxs-lookup"><span data-stu-id="5810d-398">Ordered list</span></span>|<span data-ttu-id="5810d-399">記号付きリスト</span><span class="sxs-lookup"><span data-stu-id="5810d-399">Unordered list</span></span>|
|:------|:------|
| <span data-ttu-id="5810d-400">none</span><span class="sxs-lookup"><span data-stu-id="5810d-400">none</span></span> | <span data-ttu-id="5810d-401">none</span><span class="sxs-lookup"><span data-stu-id="5810d-401">none</span></span> |
| <span data-ttu-id="5810d-402">decimal (default)</span><span class="sxs-lookup"><span data-stu-id="5810d-402">decimal (default)</span></span> | <span data-ttu-id="5810d-403">disc (default)</span><span class="sxs-lookup"><span data-stu-id="5810d-403">disc (default)</span></span> |
| <span data-ttu-id="5810d-404">lower-alpha</span><span class="sxs-lookup"><span data-stu-id="5810d-404">lower-alpha</span></span> | <span data-ttu-id="5810d-405">Circle</span><span class="sxs-lookup"><span data-stu-id="5810d-405">circle</span></span> |
| <span data-ttu-id="5810d-406">lower-roman</span><span class="sxs-lookup"><span data-stu-id="5810d-406">lower-roman</span></span> | <span data-ttu-id="5810d-407">square</span><span class="sxs-lookup"><span data-stu-id="5810d-407">square</span></span> |
| <span data-ttu-id="5810d-408">upper-alpha</span><span class="sxs-lookup"><span data-stu-id="5810d-408">upper-alpha</span></span> | &nbsp; |
| <span data-ttu-id="5810d-409">upper-roman</span><span class="sxs-lookup"><span data-stu-id="5810d-409">upper-roman</span></span> | &nbsp; |
 
<span data-ttu-id="5810d-410">入力 HTML の **ol** 要素または **ul** 要素のリストにはグローバル スタイルを適用できますが、スタイルは **li** 要素で返されます。</span><span class="sxs-lookup"><span data-stu-id="5810d-410">You can apply global styles for a list on the **ol** or **ul** element in the input HTML, but styles are returned on the **li** elements.</span></span>

#### <a name="homogenous-list-style"></a><span data-ttu-id="5810d-411">同種リスト スタイル</span><span class="sxs-lookup"><span data-stu-id="5810d-411">Homogenous list style</span></span>

<span data-ttu-id="5810d-412">この例は、**ol** 要素のリスト スタイルの種類と個々のリスト項目の CSS スタイルを設定する入力 HTML を示しています。</span><span class="sxs-lookup"><span data-stu-id="5810d-412">This example shows input HTML that sets the list style type on the **ol** element and CSS styles on individual list items.</span></span>

```html
<ol style="list-style-type:upper-roman;color:blue">
    <li style="font-weight:bold">Jacksonville</li>
    <li style="text-decoration:line-through">Orlando</li>
    <li style="font-family:Courier">Naples</li>
</ol>
``` 

<span data-ttu-id="5810d-p138">これは出力 HTML です。スタイルが個々の **li** 要素または **span** 要素で、インラインで返されることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="5810d-p138">This is the output HTML. Notice that styles are returned inline on the individual **li** or **span** elements.</span></span>

```html
<ol>
    <li style="list-style-type:upper-roman"><span style="color:blue;font-weight:bold">Jacksonville</span></li>
    <li style="list-style-type:upper-roman"><span style="color:blue;text-decoration:line-through">Orlando</span></li>
    <li style="list-style-type:upper-roman"><span style="font-family:Courier;color:blue">Naples</span></li>
</ol>
``` 

#### <a name="variable-list-styles"></a><span data-ttu-id="5810d-415">可変のリスト スタイル</span><span class="sxs-lookup"><span data-stu-id="5810d-415">Variable list styles</span></span>

<span data-ttu-id="5810d-416">この例は、**li** 要素にさまざまなリスト スタイルの種類を設定する入力 HTML を示しています。</span><span class="sxs-lookup"><span data-stu-id="5810d-416">This example shows input HTML that sets different list style types on the **li** elements.</span></span>

```html
<ul style="font-style:italic">
    <li style="list-style-type:square">square style</li>
    <li style="list-style-type:circle">circle style</li>
    <li style="list-style-type:disc">disc style (default)</li>
</ul>
``` 

<span data-ttu-id="5810d-p139">これは出力 HTML です。スタイルが個々の **li** 要素または **span** 要素で、インラインで返されることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="5810d-p139">This is the output HTML. Notice that styles are returned inline on the individual **li** or **span** elements.</span></span>

```html
<ul>
    <li style="list-style-type:square"><span style="font-style:italic">square style</span></li>
    <li style="list-style-type:circle"><span style="font-style:italic">circle style</span></li>
    <li><span style="font-style:italic">disc style (default)</span></li>
</ul>
``` 


## <a name="tables"></a><span data-ttu-id="5810d-419">テーブル</span><span class="sxs-lookup"><span data-stu-id="5810d-419">Tables</span></span>

<span data-ttu-id="5810d-p140">テーブルは、**tr** 要素と **td** 要素を含めることができる **table** 要素として表されます。入れ子のテーブルがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="5810d-p140">Tables are represented as **table** elements that can contain **tr** and **td** elements. Nested tables are supported.</span></span>

<span data-ttu-id="5810d-422">入力 HTML と出力 HTML では、テーブルに次の属性を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="5810d-422">Tables can contain the following attributes in the input and output HTML.</span></span> <span data-ttu-id="5810d-423">OneNote API では、**rowspan** 属性または **colspan** 属性はサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="5810d-423">The OneNote APIs do not support **rowspan** or **colspan** attributes.</span></span> 

#### <a name="input-attributes"></a><span data-ttu-id="5810d-424">入力属性</span><span class="sxs-lookup"><span data-stu-id="5810d-424">Input attributes</span></span>

|<span data-ttu-id="5810d-425">入力属性</span><span class="sxs-lookup"><span data-stu-id="5810d-425">Input attribute</span></span>|<span data-ttu-id="5810d-426">説明</span><span class="sxs-lookup"><span data-stu-id="5810d-426">Description</span></span>|
|:------|:------|
| <span data-ttu-id="5810d-427">data-id</span><span class="sxs-lookup"><span data-stu-id="5810d-427">data-id</span></span> | <span data-ttu-id="5810d-428">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="5810d-428">A reference for the element.</span></span><br/><br/><span data-ttu-id="5810d-429">[ページ コンテンツの更新](onenote_update_page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="5810d-429">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="5810d-430">style</span><span class="sxs-lookup"><span data-stu-id="5810d-430">style</span></span> | <span data-ttu-id="5810d-431">要素の CSS の [style](#styles)のプロパティ、および:</span><span class="sxs-lookup"><span data-stu-id="5810d-431">The CSS [style](#styles) properties of the element, and also:</span></span><br/> <span data-ttu-id="5810d-p142">- **border**。0px または 1px のいずれかにすることができます。</span><span class="sxs-lookup"><span data-stu-id="5810d-p142">- **border**. Can be either 0px or 1px.</span></span><br/> <span data-ttu-id="5810d-p143">- **width**。**table** および **td** でサポートされます。ピクセル数またはページ幅のパーセンテージを使用します。</span><span class="sxs-lookup"><span data-stu-id="5810d-p143">- **width**. Supported by **table** and **td** as pixels or percentage of page width.</span></span><br/><br/><span data-ttu-id="5810d-436">例: `width="100px"` または `width="60%"`</span><span class="sxs-lookup"><span data-stu-id="5810d-436">Example: `width="100px"` or `width="60%"`</span></span> |
 

#### <a name="output-attributes"></a><span data-ttu-id="5810d-437">出力属性</span><span class="sxs-lookup"><span data-stu-id="5810d-437">Output attributes</span></span>

|<span data-ttu-id="5810d-438">出力属性</span><span class="sxs-lookup"><span data-stu-id="5810d-438">Output attribute</span></span>|<span data-ttu-id="5810d-439">説明</span><span class="sxs-lookup"><span data-stu-id="5810d-439">Description</span></span>|
|:------|:------|
| <span data-ttu-id="5810d-440">data-id</span><span class="sxs-lookup"><span data-stu-id="5810d-440">data-id</span></span> | <span data-ttu-id="5810d-441">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="5810d-441">A reference for the element.</span></span><br/><br/><span data-ttu-id="5810d-442">[ページ コンテンツの更新](onenote_update_page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="5810d-442">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="5810d-443">id</span><span class="sxs-lookup"><span data-stu-id="5810d-443">id</span></span> | <span data-ttu-id="5810d-444">要素の一意の生成された ID。</span><span class="sxs-lookup"><span data-stu-id="5810d-444">A unique, generated ID for the element.</span></span> <span data-ttu-id="5810d-445">クエリ オプションを使用した場合に、[ページの *content* エンドポイントに対する GET 要求](../api-reference/v1.0/api/page_get.md)から返されます。`includeIDs=true`</span><span class="sxs-lookup"><span data-stu-id="5810d-445">Returned by [GET requests to a page's *content* endpoint](../api-reference/v1.0/api/page_get.md) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="5810d-446">[ページ コンテンツの更新](onenote_update_page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="5810d-446">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="5810d-447">style</span><span class="sxs-lookup"><span data-stu-id="5810d-447">style</span></span> | <span data-ttu-id="5810d-448">要素の CSS [style](#styles)のプロパティ。</span><span class="sxs-lookup"><span data-stu-id="5810d-448">The CSS [style](#styles) properties of the element.</span></span> |
 

<span data-ttu-id="5810d-449">次の例では、さまざまな方法を使用してテーブルのスタイルと返される出力 HTML を定義する入力 HTML を示しています。</span><span class="sxs-lookup"><span data-stu-id="5810d-449">The following examples show input HTML that uses different ways to define styles on tables and the output HTML that's returned.</span></span>

#### <a name="input-html-with-optional-settings-at-different-levels"></a><span data-ttu-id="5810d-450">さまざまなレベルのオプション設定を伴う入力 HTML</span><span class="sxs-lookup"><span data-stu-id="5810d-450">Input HTML with optional settings at different levels.</span></span>

```html
<table style="border:0px;width:500px;background-color:green">
    <tr> 
        <td>Cell 1</td> 
        <td>Cell 2</td> 
        <td>Cell 3</td> 
    </tr> 
    <tr style="background-color:blue"> 
        <td style="text-align:right;background-color:red">Left</td> 
        <td style="text-align:center">Middle</td> 
        <td>Right</td> 
    </tr> 
</table>
```
 
#### <a name="output-html-with-css-styles-returned-inline-on-the-td-elements"></a><span data-ttu-id="5810d-451">td 要素でインラインで返される CSS スタイルを伴う出力 HTML</span><span class="sxs-lookup"><span data-stu-id="5810d-451">Output HTML with CSS styles returned inline on the td elements.</span></span>

```html
<table style="border:0px">
    <tr>
        <td style="background-color:green;width:166;border:0px">Cell 1</td>
        <td style="background-color:green;width:166;border:0px">Cell 2</td>
        <td style="background-color:green;width:166;border:0px">Cell 3</td>
    </tr>
    <tr>
        <td style="background-color:red;width:166;border:0px;text-align:right">Left</td>
        <td style="background-color:blue;width:166;border:0px;text-align:center">Middle</td>
        <td style="background-color:blue;width:166;border:0px">Right</td>
    </tr>
</table>
``` 


## <a name="styles"></a><span data-ttu-id="5810d-452">スタイル</span><span class="sxs-lookup"><span data-stu-id="5810d-452">Styles</span></span>

<span data-ttu-id="5810d-453">Microsoft Graph の OneNote API は、ページ本文の要素 (**body**、**div**、**p**、**li**、**span** など) として、次に示すインライン CSS の **style** プロパティをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="5810d-453">OneNote APIs in Microsoft Graph support the following inline CSS **style** properties for elements in the page body, such as **body**, **div**, **p**, **li**, and **span**.</span></span>

|<span data-ttu-id="5810d-454">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5810d-454">Property</span></span>|<span data-ttu-id="5810d-455">例</span><span class="sxs-lookup"><span data-stu-id="5810d-455">Example</span></span>|
|:------|:------|
| <span data-ttu-id="5810d-456">background-color</span><span class="sxs-lookup"><span data-stu-id="5810d-456">background-color</span></span> | <span data-ttu-id="5810d-457">`style="background-color:#66cc66"` (既定は white)</span><span class="sxs-lookup"><span data-stu-id="5810d-457">`style="background-color:#66cc66"` (defaults to white)</span></span><br/><br/><span data-ttu-id="5810d-458">16 進数形式と名前付きの色の両方がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="5810d-458">Both hexadecimal format and named colors are supported.</span></span> |
| <span data-ttu-id="5810d-459">color</span><span class="sxs-lookup"><span data-stu-id="5810d-459">color</span></span> | <span data-ttu-id="5810d-460">`style="color:#ffffff"` (既定は black)</span><span class="sxs-lookup"><span data-stu-id="5810d-460">`style="color:#ffffff"` (defaults to black)</span></span> |
| <span data-ttu-id="5810d-461">font-family</span><span class="sxs-lookup"><span data-stu-id="5810d-461">font-family</span></span> | <span data-ttu-id="5810d-462">`style="font-family:Courier"` (既定は Calibri)</span><span class="sxs-lookup"><span data-stu-id="5810d-462">`style="font-family:Courier"` (defaults to Calibri)</span></span> |
| <span data-ttu-id="5810d-463">font-size</span><span class="sxs-lookup"><span data-stu-id="5810d-463">font-size</span></span> | <span data-ttu-id="5810d-464">`style="font-size:10pt"` (既定は 11pt)</span><span class="sxs-lookup"><span data-stu-id="5810d-464">`style="font-size:10pt"` (defaults to 11pt)</span></span><br/><br/><span data-ttu-id="5810d-465">API は *pt* または *px* のフォント サイズを受け入れますが、*px* は *pt* に変換します。</span><span class="sxs-lookup"><span data-stu-id="5810d-465">The APIs accept font size in *pt* or *px*, but converts *px* to *pt*.</span></span> <span data-ttu-id="5810d-466">10 進数の値は、最も近い n.0pt または n.5pt に四捨五入されます。</span><span class="sxs-lookup"><span data-stu-id="5810d-466">Decimal values are rounded to the nearest n.0pt or n.5pt.</span></span> |
| <span data-ttu-id="5810d-467">font-style</span><span class="sxs-lookup"><span data-stu-id="5810d-467">font-style</span></span> | <span data-ttu-id="5810d-468">`style="font-style:italic"` (標準または斜体のみ)</span><span class="sxs-lookup"><span data-stu-id="5810d-468">`style="font-style:italic"` (normal or italic only)</span></span> |
| <span data-ttu-id="5810d-469">font-weight</span><span class="sxs-lookup"><span data-stu-id="5810d-469">font-weight</span></span> | <span data-ttu-id="5810d-470">`style="font-weight:bold"` (標準または太字のみ)</span><span class="sxs-lookup"><span data-stu-id="5810d-470">`style="font-weight:bold"` (normal or bold only)</span></span> |
| <span data-ttu-id="5810d-471">strike-through</span><span class="sxs-lookup"><span data-stu-id="5810d-471">strike-through</span></span> | `style="text-decoration:line-through"` |
| <span data-ttu-id="5810d-472">text-align</span><span class="sxs-lookup"><span data-stu-id="5810d-472">text-align</span></span> | <span data-ttu-id="5810d-473">`style="text-align:center"` (ブロック要素の場合のみ)</span><span class="sxs-lookup"><span data-stu-id="5810d-473">`style="text-align:center"` (for block elements only)</span></span> |
| <span data-ttu-id="5810d-474">text-decoration</span><span class="sxs-lookup"><span data-stu-id="5810d-474">text-decoration</span></span> | <span data-ttu-id="5810d-475">`style="text-decoration:underline"` (なし、または下線のみ)</span><span class="sxs-lookup"><span data-stu-id="5810d-475">`style="text-decoration:underline"` (none or underline only)</span></span> |
 

<span data-ttu-id="5810d-476">次のインライン文字スタイルもサポートされています。</span><span class="sxs-lookup"><span data-stu-id="5810d-476">The following inline character styles and are also supported:</span></span>

<table id="simpletable">
<tr>
<td id="simplecell"><span data-ttu-id="5810d-477">&lt;b&gt;</span><span class="sxs-lookup"><span data-stu-id="5810d-477">&lt;b&gt;</span></span></td>
<td id="simplecell"><span data-ttu-id="5810d-478">&lt;i&gt;</span><span class="sxs-lookup"><span data-stu-id="5810d-478">&lt;i&gt;</span></span></td>
<td id="simplecell"><span data-ttu-id="5810d-479">&lt;u&gt;</span><span class="sxs-lookup"><span data-stu-id="5810d-479">&lt;u&gt;</span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="5810d-480">&lt;em&gt;</span><span class="sxs-lookup"><span data-stu-id="5810d-480">&lt;em&gt;</span></span></td>
<td id="simplecell"><span data-ttu-id="5810d-481">&lt;strong&gt;</span><span class="sxs-lookup"><span data-stu-id="5810d-481">&lt;strong&gt;</span></span></td>
<td id="simplecell"><span data-ttu-id="5810d-482">&lt;strike&gt;</span><span class="sxs-lookup"><span data-stu-id="5810d-482">&lt;strike&gt;</span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="5810d-483">&lt;sup&gt;</span><span class="sxs-lookup"><span data-stu-id="5810d-483">&lt;sup&gt;</span></span></td>
<td id="simplecell"><span data-ttu-id="5810d-484">&lt;sub&gt;</span><span class="sxs-lookup"><span data-stu-id="5810d-484">&lt;sub&gt;</span></span></td>
<td id="simplecell"><span data-ttu-id="5810d-485">&lt;del&gt;</span><span class="sxs-lookup"><span data-stu-id="5810d-485">&lt;del&gt;</span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="5810d-486">&lt;cite&gt;</span><span class="sxs-lookup"><span data-stu-id="5810d-486">&lt;cite&gt;</span></span></td>
<td id="simplecell">&nbsp;</td>
<td id="simplecell">&nbsp;</td>
</tr>
</table>

 
## <a name="input-and-output-html-example"></a><span data-ttu-id="5810d-487">入力 HTML と出力 HTML の例</span><span class="sxs-lookup"><span data-stu-id="5810d-487">Input and output HTML example</span></span>

<span data-ttu-id="5810d-488">次の画像は、Microsoft Graph で作成された簡単なページを示しています。</span><span class="sxs-lookup"><span data-stu-id="5810d-488">The following image shows a simple page that was created with Microsoft Graph.</span></span>

![Wikipedia によるコンテンツのスタディ ノートを付記した OneNote ページの画像](images/onenote-sample-image.png)

<span data-ttu-id="5810d-490">これは、ページを作成するためにメッセージ本文で送信された入力 HTML です。</span><span class="sxs-lookup"><span data-stu-id="5810d-490">This is the input HTML sent in the message body to create the page.</span></span>

```html
<html lang="en-US">
    <head>
        <title>Sample Study Notes</title>
        <meta name="created" content="2015-01-01T01:01"/>
    </head>
    <body>
        <h1>Aurora Borealis</h1>
        <p>Dancing lights in the sky. Also called <i>Northern Lights</i>. Caused by solar radiation.</p>
        <br />
        <p><b>Intersting facts</b></p>
        <table>
            <tr>
                <td>Neil Armstrong</td>
                <td>Commander</td>
            </tr>
            <tr>
                <td>Buzz Aldrin</td>
                <td>LM Pilot</td>
            </tr>
            <tr>
                <td>Michael Collins</td>
                <td>Command Module Pilot</td>
            </tr>
        </table>
        <img alt="Apollo 11 commemorative stamp." src="http://upload.wikimedia.org/wikipedia/commons/a/a4/First_Man_on_Moon_1969_Issue-10c.jpg"  width="400"/>
        <p>References:</p>
        <p><a href="http://en.wikipedia.org/wiki/Apollo_11">http://en.wikipedia.org/wiki/Apollo_11</a></p>
        <p><a href="http://www.nasa.gov/mission_pages/apollo/missions/apollo11.html">http://www.nasa.gov/mission_pages/apollo/missions/apollo11.html</a></p>
    </body>
</html>
``` 

<br/>

<span data-ttu-id="5810d-491">これは、[ページ コンテンツを取得](onenote-get-content.md)するときに Microsoft Graph が返す出力 HTML です。</span><span class="sxs-lookup"><span data-stu-id="5810d-491">This is the output HTML that Microsoft Graph returns when you [get page content](onenote-get-content.md).</span></span>

> <span data-ttu-id="5810d-492">**注:** [ページを作成する](onenote-create-page.md)ときや、[ページのメタデータを取得する](../api-reference/v1.0/api/page_get.md)ときに、API は **contentUrl** プロパティのページの*コンテンツ* エンドポイント URL を返します。</span><span class="sxs-lookup"><span data-stu-id="5810d-492">**Note:** When you [create a page](onenote-create-page.md) or [get page metadata](../api-reference/v1.0/api/page_get.md), the API returns the *content* endpoint URL of the page in the **contentUrl** property.</span></span>

```html
<html htmlns="http://www.w3.org/1999/xhtml" lang="en-US">
    <head>
        <title>Sample Study Notes</title>
    </head>
    <body data-absolute-enabled="true" style="font-family:Calibri;font-size:11pt">
        <div data-id="_default" style="position:absolute;left:48px;top:120px;width:624px">
            <h1 style="font-size:16pt;color:#1e4e79;margin-top:11pt;margin-bottom:11pt">American History 101: Moon Landing</h1>
            <p>First moon landing - July 20, 1969 with Apollo 11 (Eagle)</p>
            <br />
            <p><span style="font-weight:bold">Apollo 11 Astronauts</span></p>
            <table style="border:0px">
                <tr>
                    <td style="border:0px">Neil Armstrong</td>
                    <td style="border:0px">Commander</td>
                </tr>
                <tr>
                    <td style="border:0px">Buzz Aldrin</td>
                    <td style="border:0px">LM Pilot</td>
                </tr>
                <tr>
                    <td style="border:0px">Michael Collins</td>
                    <td style="border:0px">Command Module Pilot</td>
                </tr>
            </table>
            <br />
            <img alt="Apollo 11 commemorative stamp." width="400" height="248" src="https://graph.microsoft.com/v1.0/me/onenote/resources/0-f717b5fa5eaa454da7ecdf72a8c137fe!1-73DBAF9B7E5C4B4C!10456/$value"
                 data-src-type="image/jpeg" data-fullres-src="https://graph.microsoft.com/v1.0/me/onenote/resources/0-f717b5fa5eaa454da7ecdf72a8c137fe!1-73DBAF9B7E5C4B4C!10456/$value" data-fullres-src-type="image/jpeg" />
            <p>References:</p>
            <p><a href="http://en.wikipedia.org/wiki/Apollo_11">http://en.wikipedia.org/wiki/Apollo_11</a></p>
            <p><a href="http://www.nasa.gov/mission_pages/apollo/missions/apollo11.html">http://www.nasa.gov/mission_pages/apollo/missions/apollo11.html</a></p>
        </div>
    </body>
</html>
``` 

## <a name="see-also"></a><span data-ttu-id="5810d-493">関連項目</span><span class="sxs-lookup"><span data-stu-id="5810d-493">See also</span></span>

- [<span data-ttu-id="5810d-494">OneNote コンテンツと構造を取得する</span><span class="sxs-lookup"><span data-stu-id="5810d-494">Get OneNote content and structure</span></span>](onenote-get-content.md)
- [<span data-ttu-id="5810d-495">OneNote ページの作成</span><span class="sxs-lookup"><span data-stu-id="5810d-495">Create OneNote pages</span></span>](onenote-create-page.md)
- [<span data-ttu-id="5810d-496">OneNote ページ コンテンツを更新する</span><span class="sxs-lookup"><span data-stu-id="5810d-496">Update OneNote page content</span></span>](onenote_update_page.md)
- [<span data-ttu-id="5810d-497">画像、ビデオ、ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="5810d-497">Add images, videos, and files</span></span>](onenote_images_files.md)
