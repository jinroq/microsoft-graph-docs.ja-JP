# <a name="input-and-output-html-in-onenote-pages"></a><span data-ttu-id="1b84a-101">OneNote ページの入出力 HTML</span><span class="sxs-lookup"><span data-stu-id="1b84a-101">Input and output HTML for OneNote pages</span></span>

<span data-ttu-id="1b84a-102">OneNote ページを[作成](../api-reference/v1.0/api/section_post_pages.md)または[更新](../api-reference/v1.0/api/page_update.md)する際に、ページ コンテンツと構造を定義する HTML を*入力 HTML* と呼びます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-102">The HTML that defines the page content and structure when you [create](../api-reference/v1.0/api/section_post_pages.md) or [update](../api-reference/v1.0/api/page_update.md) a page is called *input HTML*.</span></span> 

<span data-ttu-id="1b84a-103">[ページ コンテンツを取得](../api-reference/v1.0/api/page_get.md)すると返される HTML を*出力 HTML* と呼びます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-103">The HTML that's returned when you [get page content](../api-reference/v1.0/api/page_get.md) is called *output HTML*.</span></span> <span data-ttu-id="1b84a-104">出力 HTML は入力 HTML と同じにはなりません。</span><span class="sxs-lookup"><span data-stu-id="1b84a-104">Output HTML won't be the same as input HTML.</span></span>

<span data-ttu-id="1b84a-105">Microsoft Graph の OneNote API は、入力 HTML の意味的コンテンツと基本的構造を保持しますが、その HTML を、[サポートされている HTML 要素および CSS プロパティ](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-create-page#supported-html)のセットに変換します。</span><span class="sxs-lookup"><span data-stu-id="1b84a-105">The OneNote API preserves the semantic content and basic structure of the input HTML, but converts it to a set of supported HTML elements and CSS properties. The API also adds custom attributes that support OneNote features.</span></span> <span data-ttu-id="1b84a-106">API はさらに、OneNote 機能をサポートするカスタム属性も追加します。</span><span class="sxs-lookup"><span data-stu-id="1b84a-106">The APIs also add custom attributes that support OneNote features.</span></span>
 
<span data-ttu-id="1b84a-p103">この資料では、入力 HTML と出力 HTML の主な要素と属性について説明します。ページ コンテンツを作成または更新する場合には入力 HTMLについて、返されるページ コンテンツを解析する場合には出力 HTML について理解することは役立ちます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-p103">This article describes the principal elements and attributes of input and output HTML. It can be helpful to understand input HTML when you're creating or updating page content, and output HTML when you're parsing returned page content.</span></span> 

## <a name="body-element"></a><span data-ttu-id="1b84a-109">body 要素</span><span class="sxs-lookup"><span data-stu-id="1b84a-109">Body element</span></span>
<span data-ttu-id="1b84a-110">ページ本文の HTML コンテンツは、画像やファイルのリソースなどを含むページのコンテンツと構造を表します。</span><span class="sxs-lookup"><span data-stu-id="1b84a-110">The HTML content in the page body represents the page content and structure, including image and file resources. The body element can contain the following attributes in the input and output HTML.</span></span> <span data-ttu-id="1b84a-111">入力および出力 HTML では、**body** 要素に次の属性を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-111">An **img** element can contain the following attributes in the input and output HTML.</span></span>

<span data-ttu-id="1b84a-112">**入力属性**</span><span class="sxs-lookup"><span data-stu-id="1b84a-112">**Input attributes**</span></span>

|<span data-ttu-id="1b84a-113">入力属性</span><span class="sxs-lookup"><span data-stu-id="1b84a-113">Input attribute</span></span>|<span data-ttu-id="1b84a-114">説明</span><span class="sxs-lookup"><span data-stu-id="1b84a-114">Description</span></span>|
|:------|:------|
| <span data-ttu-id="1b84a-115">data-absolute-enabled</span><span class="sxs-lookup"><span data-stu-id="1b84a-115">data-absolute-enabled</span></span> | <span data-ttu-id="1b84a-116">[絶対位置で配置](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos)された要素を入力本文でサポートするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1b84a-116">Indicates whether the input body supports [absolute positioned](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos) elements.</span></span> |
| <span data-ttu-id="1b84a-117">style</span><span class="sxs-lookup"><span data-stu-id="1b84a-117">style</span></span> | <p><span data-ttu-id="1b84a-118">本文の CSS の [style](#styles) プロパティ。</span><span class="sxs-lookup"><span data-stu-id="1b84a-118">The CSS [style](#styles) properties of the body.</span></span> <span data-ttu-id="1b84a-119">出力 HTML では、入力設定がインラインで、適切な子要素で返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="1b84a-119">In the output HTML, input settings may be returned inline on appropriate child elements.</span></span></p><p><span data-ttu-id="1b84a-120">現在、**body** 要素では背景色はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1b84a-120">Background color is not currently supported for the **body** element.</span></span></p> |
 

<span data-ttu-id="1b84a-121">**出力属性**</span><span class="sxs-lookup"><span data-stu-id="1b84a-121">**Output attributes**</span></span>

|<span data-ttu-id="1b84a-122">出力属性</span><span class="sxs-lookup"><span data-stu-id="1b84a-122">Output attribute</span></span>|<span data-ttu-id="1b84a-123">説明</span><span class="sxs-lookup"><span data-stu-id="1b84a-123">Description</span></span>|
|:------|:------|
| <span data-ttu-id="1b84a-124">data-absolute-enabled</span><span class="sxs-lookup"><span data-stu-id="1b84a-124">data-absolute-enabled</span></span> | <span data-ttu-id="1b84a-125">[絶対位置で配置](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos)された要素を本文でサポートするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1b84a-125">Indicates whether the body supports [absolute positioned](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos) elements.</span></span> <span data-ttu-id="1b84a-126">出力 HTML では常に **true** です。</span><span class="sxs-lookup"><span data-stu-id="1b84a-126">Always **true** in output HTML.</span></span> |
| <span data-ttu-id="1b84a-127">style</span><span class="sxs-lookup"><span data-stu-id="1b84a-127">style</span></span> | <span data-ttu-id="1b84a-128">本文の **font-family** および **font-size** プロパティ。</span><span class="sxs-lookup"><span data-stu-id="1b84a-128">The **font-family** and **font-size** properties of the body.</span></span> |


## <a name="div-elements"></a><span data-ttu-id="1b84a-129">div 要素</span><span class="sxs-lookup"><span data-stu-id="1b84a-129">Div elements</span></span>
<span data-ttu-id="1b84a-130">**div** 要素にはテキスト、画像、およびその他のコンテンツが含まれます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-130">Divs contain text, images, and other content.</span></span> <span data-ttu-id="1b84a-131">入力 HTML と出力 HTML では、**div** 要素に次の属性を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-131">A **div** element can contain the following attributes in the input and output HTML.</span></span>

<span data-ttu-id="1b84a-132">**入力属性**</span><span class="sxs-lookup"><span data-stu-id="1b84a-132">**Input attributes**</span></span>

|<span data-ttu-id="1b84a-133">入力属性</span><span class="sxs-lookup"><span data-stu-id="1b84a-133">Input attribute</span></span>|<span data-ttu-id="1b84a-134">説明</span><span class="sxs-lookup"><span data-stu-id="1b84a-134">Description</span></span>|
|:------|:------|
| <span data-ttu-id="1b84a-135">data-id</span><span class="sxs-lookup"><span data-stu-id="1b84a-135">data-id</span></span> | <span data-ttu-id="1b84a-136">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="1b84a-136">A reference for the element.</span></span> <span data-ttu-id="1b84a-137">[ページ コンテンツの更新](../api-reference/v1.0/api/page_update.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="1b84a-137">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="1b84a-138">data-render-fallback</span><span class="sxs-lookup"><span data-stu-id="1b84a-138">data-render-fallback</span></span> | <span data-ttu-id="1b84a-139">[抽出](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-extract-data)が失敗した場合のフォールバック操作。**render** (既定) または **none**。</span><span class="sxs-lookup"><span data-stu-id="1b84a-139">The fallback action if the [extraction](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-extract-data) fails: **render** (default) or **none**.</span></span> |
| <span data-ttu-id="1b84a-140">data-render-method</span><span class="sxs-lookup"><span data-stu-id="1b84a-140">data-render-method</span></span> | <span data-ttu-id="1b84a-141">[抽出](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-extract-data)を実行するメソッド。たとえば: `extract.businesscard` または `extract.recipe`。</span><span class="sxs-lookup"><span data-stu-id="1b84a-141">The [extraction](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-extract-data) method to perform, for example: `extract.businesscard` or `extract.recipe`.</span></span> |
| <span data-ttu-id="1b84a-142">data-render-src</span><span class="sxs-lookup"><span data-stu-id="1b84a-142">data-render-src</span></span> | <span data-ttu-id="1b84a-143">[抽出](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-extract-data)のコンテンツのソース。</span><span class="sxs-lookup"><span data-stu-id="1b84a-143">The content source for the [extraction](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-extract-data).</span></span> |
| <span data-ttu-id="1b84a-144">style</span><span class="sxs-lookup"><span data-stu-id="1b84a-144">style</span></span> | <p><span data-ttu-id="1b84a-145">div の位置、サイズ、フォント、および色のプロパティ:</span><span class="sxs-lookup"><span data-stu-id="1b84a-145">The position, size, font, and color properties for the div:</span></span></p><p> <span data-ttu-id="1b84a-146">- **position** (**absolute** のみ)、**left**、**top**、および **width**。</span><span class="sxs-lookup"><span data-stu-id="1b84a-146">- **position** (**absolute** only), **left**, **top**, and **width**.</span></span> <span data-ttu-id="1b84a-147">(div では height が自動構成されます。)</span><span class="sxs-lookup"><span data-stu-id="1b84a-147">(Height is auto-configured for divs.)</span></span><br /><span data-ttu-id="1b84a-148">本文が `data-absolute-enabled="true"` に設定されていて、div が本文の直接の子の場合にのみ、[絶対位置](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos)の div の作成に使用されます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-148">Used to create an [absolute positioned](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos) div, only if the div is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br /><span data-ttu-id="1b84a-149">例: `<div style="position:absolute;width:360px;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="1b84a-149">Example: `<div style="position:absolute;width:360px;top:350px;left:300px" ... />`</span></span></p><p> <span data-ttu-id="1b84a-150">- 要素の CSS の [style](#styles) プロパティ。</span><span class="sxs-lookup"><span data-stu-id="1b84a-150">- The CSS [style](#styles) properties of the element.</span></span> <span data-ttu-id="1b84a-151">出力 HTML では、これらの値が適切な子要素で、インラインで返されます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-151">In the output HTML, these values are returned inline on appropriate child elements.</span></span></p> |
 

<span data-ttu-id="1b84a-152">Microsoft Graph の OneNote API は、すべての本文のコンテンツを 1 つ以上の div でラップします。</span><span class="sxs-lookup"><span data-stu-id="1b84a-152">The OneNote APIs in Microsoft Graph wrap all body content in at least one div.</span></span> <span data-ttu-id="1b84a-153">次の場合に、API は既定の div (`data-id="_default"` の属性に設定) を作成して、本文のコンテンツを含めます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-153">The API creates a default div (attributed with `data-id="_default"`) to contain the body content if:</span></span>

- <span data-ttu-id="1b84a-154">本文の入力要素の **data-absolute-enabled** 属性は省略されるか、**false** に設定されます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-154">The input body element's data-absolute-enabled attribute is omitted or set to false. In this case, all body content is put in the default div.</span></span> <span data-ttu-id="1b84a-155">この例では、すべてのコンテンツは既定位置の div に配置されています。</span><span class="sxs-lookup"><span data-stu-id="1b84a-155">The input body element's data-absolute-enabled attribute is omitted or set to false. In this case, all body content is put in the default div.</span></span>

- <span data-ttu-id="1b84a-156">本文の入力要素の **data-absolute-enabled** 属性は** true** ですが、入力 HTML は、[絶対位置に配置された](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos)&nbsp;** div**、**img**、または **object** 要素ではない直接の子を含んでいます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-156">The input body element's **\`data-absolute-enabled** attribute is **true**, but the input HTML contains direct children that aren't [absolute positioned](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos)&nbsp;**div**, **img**, or **object** elements.</span></span> <span data-ttu-id="1b84a-157">この例では、[絶対位置に配置された](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos)&nbsp;** div**、**img**、または **object** 要素ではない直接の子が、既定位置の div に配置されています。</span><span class="sxs-lookup"><span data-stu-id="1b84a-157">In this case, direct children that aren't [absolute positioned](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos)&nbsp;**div**, **img**, or **object** elements are put in the default div.</span></span>


<span data-ttu-id="1b84a-158">**出力属性**</span><span class="sxs-lookup"><span data-stu-id="1b84a-158">**Output attributes**</span></span>

|<span data-ttu-id="1b84a-159">出力属性</span><span class="sxs-lookup"><span data-stu-id="1b84a-159">Output attribute</span></span>|<span data-ttu-id="1b84a-160">説明</span><span class="sxs-lookup"><span data-stu-id="1b84a-160">Description</span></span>|
|:------|:------|
| <span data-ttu-id="1b84a-161">data-id</span><span class="sxs-lookup"><span data-stu-id="1b84a-161">data-id</span></span> | <span data-ttu-id="1b84a-162">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="1b84a-162">A reference for the element.</span></span> <span data-ttu-id="1b84a-163">[ページ コンテンツの更新](../api-reference/v1.0/api/page_update.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="1b84a-163">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="1b84a-164">id</span><span class="sxs-lookup"><span data-stu-id="1b84a-164">id</span></span> | <span data-ttu-id="1b84a-165">要素の一意の生成された ID。</span><span class="sxs-lookup"><span data-stu-id="1b84a-165">A unique, generated ID for the element.</span></span> <span data-ttu-id="1b84a-166">`includeIDs=true` クエリ オプションを使用した場合に、[ページの *content* エンドポイントに対する GET 要求](../api-reference/v1.0/api/page_get.md)から返されます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-166">Returned by [GET requests to a page's *content* endpoint](../api-reference/v1.0/api/page_get.md) when the `includeIDs=true` query option is used.</span></span> <span data-ttu-id="1b84a-167">[ページ コンテンツの更新](../api-reference/v1.0/api/page_update.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="1b84a-167">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="1b84a-168">style</span><span class="sxs-lookup"><span data-stu-id="1b84a-168">style</span></span> | <span data-ttu-id="1b84a-169">div の位置とサイズのプロパティ。</span><span class="sxs-lookup"><span data-stu-id="1b84a-169">The position and size properties of the div.</span></span> |
 
### <a name="non-contributing-divs"></a><span data-ttu-id="1b84a-170">作用していない div</span><span class="sxs-lookup"><span data-stu-id="1b84a-170">Non-contributing divs</span></span>
<span data-ttu-id="1b84a-171">入力 HTML の **div** 要素がページ構造に作用しておらず、OneNote が使用する情報を含んでいない場合、API は div のコンテンツを親または既定の div に移動します。</span><span class="sxs-lookup"><span data-stu-id="1b84a-171">When a div element in the input HTML does not contribute to the page structure or carry information that onnvshort uses,  the API moves the div's content into the parent or default div.</span></span> <span data-ttu-id="1b84a-172">これを以下の例で説明します。</span><span class="sxs-lookup"><span data-stu-id="1b84a-172">This is illustrated in the following examples.</span></span>

<span data-ttu-id="1b84a-173">作用していない入れ子型の div を含む**入力 HTML**。</span><span class="sxs-lookup"><span data-stu-id="1b84a-173">**Input HTML** that contains a non-contributing, nested div.</span></span>

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

<span data-ttu-id="1b84a-174">**出力 HTML**</span><span class="sxs-lookup"><span data-stu-id="1b84a-174">**Output HTML**</span></span>

><span data-ttu-id="1b84a-175">**注:** div のコンテンツは親の div に移動し、入れ子状態の `<div>` タグが削除されました。</span><span class="sxs-lookup"><span data-stu-id="1b84a-175">Notice that the div's content was moved to the parent div and the nested  tags have been removed.</span></span> <span data-ttu-id="1b84a-176">**data-id** などの意味情報が div に定義されていた場合は、div は保持されています (例: `<div data-id="keep-me">`)。</span><span class="sxs-lookup"><span data-stu-id="1b84a-176">However, the div would have been preserved if it defined any semantic information, such as a **data-id** (example: `<div data-id="keep-me">`).</span></span>

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


## <a name="img-elements"></a><span data-ttu-id="1b84a-177">img 要素</span><span class="sxs-lookup"><span data-stu-id="1b84a-177">Img elements</span></span>
<span data-ttu-id="1b84a-178">OneNote ページの画像は **img** 要素で表されます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-178">Images on OneNote pages are represented by **img** elements.</span></span> <span data-ttu-id="1b84a-179">入力 HTML および出力 HTML では、**img** 要素に次の属性を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-179">An **img** element can contain the following attributes in the input and output HTML.</span></span>

<span data-ttu-id="1b84a-180">**入力属性**</span><span class="sxs-lookup"><span data-stu-id="1b84a-180">**Input attributes**</span></span>

|<span data-ttu-id="1b84a-181">入力属性</span><span class="sxs-lookup"><span data-stu-id="1b84a-181">Input attribute</span></span>|<span data-ttu-id="1b84a-182">説明</span><span class="sxs-lookup"><span data-stu-id="1b84a-182">Description</span></span>|
|:------|:------|
| <span data-ttu-id="1b84a-183">alt</span><span class="sxs-lookup"><span data-stu-id="1b84a-183">alt</span></span> | <span data-ttu-id="1b84a-184">画像に指定された代替テキスト。</span><span class="sxs-lookup"><span data-stu-id="1b84a-184">The supplied alt text for the image.</span></span> |
| <span data-ttu-id="1b84a-185">data-id</span><span class="sxs-lookup"><span data-stu-id="1b84a-185">data-id</span></span> | <span data-ttu-id="1b84a-186">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="1b84a-186">A reference for the element.</span></span> <span data-ttu-id="1b84a-187">[ページ コンテンツの更新](../api-reference/v1.0/api/page_update.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="1b84a-187">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="1b84a-188">data-render-src</span><span class="sxs-lookup"><span data-stu-id="1b84a-188">data-render-src</span></span> |<span data-ttu-id="1b84a-189">**data-render-src** か **src** のいずれかが必要です。</span><span class="sxs-lookup"><span data-stu-id="1b84a-189">Either **data-render-src** or **src** is required.</span></span><br/><br/><span data-ttu-id="1b84a-190">OneNote ページ上のビットマップ画像として表示する Web ページ。</span><span class="sxs-lookup"><span data-stu-id="1b84a-190">The webpage to render as a bit-mapped image on the OneNote page:</span></span><br /> <span data-ttu-id="1b84a-191">パブリック URL の場合は - `data-render-src="http://..."`。</span><span class="sxs-lookup"><span data-stu-id="1b84a-191">- `data-render-src="http://..."` for a public URL.</span></span><br /> <span data-ttu-id="1b84a-192">[マルチパート要求](../api-reference/v1.0/api/section_post_pages.md#example)の "Presentation" ブロックにある画像部分の場合は - `data-render-src="name:BlockName"`。</span><span class="sxs-lookup"><span data-stu-id="1b84a-192">- `data-render-src="name:BlockName"` for an image part in the "Presentation" block of a [multipart request](../api-reference/v1.0/api/section_post_pages.md#example).</span></span><br/><br/><span data-ttu-id="1b84a-193">このメソッドは、OneNote ページで忠実に表示できるものよりも複雑な Web ページの場合や、ページにログイン資格情報が必要な場合に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-193">This method is useful when the webpage is more complex than the OneNote page can faithfully render, or when the page requires login credentials.</span></span>|
| <span data-ttu-id="1b84a-194">data-tag</span><span class="sxs-lookup"><span data-stu-id="1b84a-194">data-tag</span></span> | <span data-ttu-id="1b84a-195">要素の[ノート シール](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags)。</span><span class="sxs-lookup"><span data-stu-id="1b84a-195">A [note tag](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) on the element.</span></span> |
| <span data-ttu-id="1b84a-196">style</span><span class="sxs-lookup"><span data-stu-id="1b84a-196">style</span></span> |<span data-ttu-id="1b84a-197">画像の位置とサイズのプロパティ: **position** (**absolute** のみ)、**left**、**top**、**width**、および **height**。</span><span class="sxs-lookup"><span data-stu-id="1b84a-197">The position and size properties for the image: **position** (**absolute** only), **left**, **top**, **width**, and **height**.</span></span><br/><br/><span data-ttu-id="1b84a-198">任意の画像のサイズを設定できます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-198">Size can be set on any image.</span></span> <span data-ttu-id="1b84a-199">位置プロパティは、本文が `data-absolute-enabled="true"` に設定されていて、画像が本文の直接の子である場合にのみ、[絶対位置](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos)の画像の作成に使用されます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-199">Position properties are used to create an [absolute positioned](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos) image, only if the image is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br /><span data-ttu-id="1b84a-200">例: `<img style="position:absolute;width:360px;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="1b84a-200">Example: `<img style="position:absolute;width:360px;top:350px;left:300px" ... />`</span></span><br/><br/><span data-ttu-id="1b84a-201">出力 HTML では、画像サイズは **width** 属性と **height** 属性で別々に返されます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-201">In the output HTML, the image size is returned separately in **width** and **height** attributes.</span></span> |
| <span data-ttu-id="1b84a-202">src</span><span class="sxs-lookup"><span data-stu-id="1b84a-202">src</span></span> |<span data-ttu-id="1b84a-203">**src** か **data-render-src** のいずれかが必要です。</span><span class="sxs-lookup"><span data-stu-id="1b84a-203">Either **src** or **data-render-src** is required.</span></span><br/><br/><span data-ttu-id="1b84a-204">OneNote ページに表示する画像。</span><span class="sxs-lookup"><span data-stu-id="1b84a-204">The image to render on the OneNote page:</span></span><br /> <span data-ttu-id="1b84a-205">インターネットで一般に使用可能な画像の URL の場合は - `src="http://..."`。</span><span class="sxs-lookup"><span data-stu-id="1b84a-205">- `src="http://..."` for a URL to a publicly available image on the internet.</span></span><br /> <span data-ttu-id="1b84a-206">画像を表すマルチパート要求の名前付き部分の場合は - `src="name:BlockName"`。</span><span class="sxs-lookup"><span data-stu-id="1b84a-206">- `src="name:BlockName"` for a named part in a multipart request that represents the image.</span></span>|
| <span data-ttu-id="1b84a-207">width、height</span><span class="sxs-lookup"><span data-stu-id="1b84a-207">width, height</span></span> | <span data-ttu-id="1b84a-208">画像の幅または高さ。ピクセル単位ですが px は付けません。</span><span class="sxs-lookup"><span data-stu-id="1b84a-208">The width or height of the image, in pixels but without the px.</span></span> <span data-ttu-id="1b84a-209">例: `width="400"`</span><span class="sxs-lookup"><span data-stu-id="1b84a-209">Example: `width="400"`</span></span> |
 
><span data-ttu-id="1b84a-210">**注:** OneNote API は入力画像の種類を自動的に検出し、それを **data-fullres-src-type** として出力 HTML に返します。</span><span class="sxs-lookup"><span data-stu-id="1b84a-210">The OneNote API automatically detects the input image type, and returns it as the **data-fullres-src-type** in the output HTML.</span></span> <span data-ttu-id="1b84a-211">API は、**data-src-type** で最適化された画像の種類も返します。</span><span class="sxs-lookup"><span data-stu-id="1b84a-211">The API also returns the image type of the optimized image in **data-src-type**.</span></span>
 

<span data-ttu-id="1b84a-212">**出力属性**</span><span class="sxs-lookup"><span data-stu-id="1b84a-212">**Output attributes**</span></span>

|<span data-ttu-id="1b84a-213">出力属性</span><span class="sxs-lookup"><span data-stu-id="1b84a-213">Output attribute</span></span>|<span data-ttu-id="1b84a-214">説明</span><span class="sxs-lookup"><span data-stu-id="1b84a-214">Description</span></span>|
|:------|:------|
| <span data-ttu-id="1b84a-215">alt</span><span class="sxs-lookup"><span data-stu-id="1b84a-215">alt</span></span> | <span data-ttu-id="1b84a-216">画像に指定された代替テキスト。</span><span class="sxs-lookup"><span data-stu-id="1b84a-216">The supplied alt text for the image.</span></span> |
| <span data-ttu-id="1b84a-217">data-id</span><span class="sxs-lookup"><span data-stu-id="1b84a-217">data-id</span></span> | <span data-ttu-id="1b84a-218">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="1b84a-218">A reference for the element.</span></span> <span data-ttu-id="1b84a-219">[ページ コンテンツの更新](../api-reference/v1.0/api/page_update.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="1b84a-219">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="1b84a-220">data-index</span><span class="sxs-lookup"><span data-stu-id="1b84a-220">data-index</span></span> | <span data-ttu-id="1b84a-221">画像の位置。</span><span class="sxs-lookup"><span data-stu-id="1b84a-221">The position of the image.</span></span> <span data-ttu-id="1b84a-222">[分割された画像](#split-images)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="1b84a-222">For [split image](#split-images) support.</span></span> |
| <span data-ttu-id="1b84a-223">data-fullres-src</span><span class="sxs-lookup"><span data-stu-id="1b84a-223">data-fullres-src</span></span> | <span data-ttu-id="1b84a-224">最初にページに埋め込まれていた画像リソースのバージョンのエンドポイント。</span><span class="sxs-lookup"><span data-stu-id="1b84a-224">The endpoint for the version of the image resource that was originally embedded in the page.</span></span> |
| <span data-ttu-id="1b84a-225">data-fullres-src-type</span><span class="sxs-lookup"><span data-stu-id="1b84a-225">data-fullres-src-type</span></span> | <span data-ttu-id="1b84a-226">**data-fullres-src** リソースのメディアの種類。たとえば、`image/png` または`image/jpeg`。</span><span class="sxs-lookup"><span data-stu-id="1b84a-226">The media type of the **data-fullres-src** resource, for example: `image/png` or `image/jpeg`.</span></span> |
| <span data-ttu-id="1b84a-227">data-options</span><span class="sxs-lookup"><span data-stu-id="1b84a-227">data-options</span></span> | <span data-ttu-id="1b84a-228">ソースの種類。PDF ファイルの場合は **printout**、その他のファイルはいずれも **splitimage**。</span><span class="sxs-lookup"><span data-stu-id="1b84a-228">The source type: **printout** for PDF files or **splitimage** for all others.</span></span> <span data-ttu-id="1b84a-229">**data-render-src** 属性で作成された、[分割された画像](#split-images)にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-229">Applies only to []split images](#split-images) created with the data-render-src attribute.</span></span> |
| <span data-ttu-id="1b84a-230">data-render-original-src</span><span class="sxs-lookup"><span data-stu-id="1b84a-230">data-render-original-src</span></span> | <span data-ttu-id="1b84a-231">ソース画像が公開されたインターネットの画像で、**data-render-src** 属性を付けて作成された場合の、画像の最初のソース URL。</span><span class="sxs-lookup"><span data-stu-id="1b84a-231">The original source URL of the image, if the source image is from the public internet and was created with the **data-render-src** attribute.</span></span> |
| <span data-ttu-id="1b84a-232">data-src-type</span><span class="sxs-lookup"><span data-stu-id="1b84a-232">data-src-type</span></span> | <span data-ttu-id="1b84a-233">**src** リソースのメディアの種類。たとえば、`image/png` または`image/jpeg`。</span><span class="sxs-lookup"><span data-stu-id="1b84a-233">The media type of the **src** resource, for example: `image/png` or `image/jpeg`.</span></span> |
| <span data-ttu-id="1b84a-234">data-tag</span><span class="sxs-lookup"><span data-stu-id="1b84a-234">data-tag</span></span> | <span data-ttu-id="1b84a-235">要素の[ノート シール](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags)。</span><span class="sxs-lookup"><span data-stu-id="1b84a-235">A [note tag](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) on the element.</span></span> |
| <span data-ttu-id="1b84a-236">id</span><span class="sxs-lookup"><span data-stu-id="1b84a-236">id</span></span> | <span data-ttu-id="1b84a-237">要素の一意の生成された ID。</span><span class="sxs-lookup"><span data-stu-id="1b84a-237">A unique, generated ID for the element.</span></span> <span data-ttu-id="1b84a-238">`includeIDs=true` クエリ オプションを使用した場合に、[ページの *content* エンドポイントに対する GET 要求](../api-reference/v1.0/api/page_get.md)から返されます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-238">Returned by [GET requests to a page's *content* endpoint](../api-reference/v1.0/api/page_get.md) when the `includeIDs=true` query option is used.</span></span> <span data-ttu-id="1b84a-239">[ページ コンテンツの更新](../api-reference/v1.0/api/page_update.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="1b84a-239">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="1b84a-240">src</span><span class="sxs-lookup"><span data-stu-id="1b84a-240">src</span></span> | <span data-ttu-id="1b84a-241">Web ブラウザー、モバイル、およびタブレットのフォーム ファクター向けに最適化された画像リソースのバージョンのエンドポイント。</span><span class="sxs-lookup"><span data-stu-id="1b84a-241">The endpoint for the version of the image resource that has been optimized for web browsers and mobile and tablet form factors.</span></span> |
| <span data-ttu-id="1b84a-242">style</span><span class="sxs-lookup"><span data-stu-id="1b84a-242">style</span></span> | <span data-ttu-id="1b84a-243">画像の位置のプロパティ。</span><span class="sxs-lookup"><span data-stu-id="1b84a-243">The position properties of the image.</span></span> |
| <span data-ttu-id="1b84a-244">width、height</span><span class="sxs-lookup"><span data-stu-id="1b84a-244">width, height</span></span> | <span data-ttu-id="1b84a-245">画像の幅または高さ (ピクセル単位)。</span><span class="sxs-lookup"><span data-stu-id="1b84a-245">The width or height of the image, in pixels.</span></span> |
 

### <a name="output-html-examples-for-images"></a><span data-ttu-id="1b84a-246">画像の出力 HTML の例</span><span class="sxs-lookup"><span data-stu-id="1b84a-246">Output HTML examples for images</span></span>
<span data-ttu-id="1b84a-247">出力 **img** 要素には、以下に示す画像ファイルのリソースと画像の種類のエンドポイントが含まれています。</span><span class="sxs-lookup"><span data-stu-id="1b84a-247">Output **img** elements contain endpoints for image file resources and the image type, as shown below. You can make separate GET requests to image resource endpoints to retrieve their binary contents.</span></span> <span data-ttu-id="1b84a-248">バイナリ コンテンツを取得するには、[画像リソースのエンドポイントに対して個別に GET 要求](../api-reference/v1.0/api/resource_get.md)を実行します。</span><span class="sxs-lookup"><span data-stu-id="1b84a-248">Output img elements contain endpoints for image file resources and the image type, as shown below. You can make separate [GET requests to image resource endpoints](../api-reference/v1.0/api/resource_get.md) to retrieve their binary contents.</span></span>

```http
<img 
    src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/$value"  
    data-src-type="image/png"
    data-fullres-src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/$value"  
    data-fullres-src-type="image/png" ... />
```

<span data-ttu-id="1b84a-249">既定では、画像は、ページ コンテンツの残りの部分と同様、それらを取得するために承認を必要とするため、ブラウザーで直接表示されることはありません。</span><span class="sxs-lookup"><span data-stu-id="1b84a-249">By default, images won't render directly in a browser because they are private and require authorization to retrieve them, like the rest of the page contents.</span></span> <span data-ttu-id="1b84a-250">ページにある画像リソースへの公開 URL を取得するには、ページ コンテンツを取得する際に、クエリ文字列に **preAuthenticated=true** を含めます (例: `GET ../pages/{page-id}/content?preAuthenticated=true`)。</span><span class="sxs-lookup"><span data-stu-id="1b84a-250">To get public URLs to the image resources on a page, include **preAuthenticated=true** in the query string when you retrieve the page content (example: `GET ../pages/{page-id}/content?preAuthenticated=true`).</span></span> <span data-ttu-id="1b84a-251">返される公開 URL は 1 時間有効です。</span><span class="sxs-lookup"><span data-stu-id="1b84a-251">The public URLs that are returned are valid for one hour.</span></span> 

<span data-ttu-id="1b84a-252">**要求に _preAuthenticated=true_ が含まれる場合の、パブリック URL を使用する画像**</span><span class="sxs-lookup"><span data-stu-id="1b84a-252">Image with public URL when _preAuthenticated=true_ is included in the request</span></span>

```html
<img 
    width="170" height="128" 
    src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/content?publicAuth=true&mimeType=image/jpeg" 
    data-src-type="image/{type}" 
    data-fullres-src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/content?publicAuth=true&mimeType=image/jpeg" 
    data-fullres-src-type="image/{type}" />
```

<span data-ttu-id="1b84a-253">次の例は、**img** 要素が出力 HTML に含む可能性がある情報を示しています。</span><span class="sxs-lookup"><span data-stu-id="1b84a-253">The following examples show the information an **img** element might contain in the output HTML.</span></span>

<span data-ttu-id="1b84a-254">**Web 対応の高解像度リソースがある画像**</span><span class="sxs-lookup"><span data-stu-id="1b84a-254">**Image with web-ready and high resolution resources**</span></span>

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

<span data-ttu-id="1b84a-255">***data-render-src* 属性を使用して作成された画像**</span><span class="sxs-lookup"><span data-stu-id="1b84a-255">**Image created by using the *data-render-src* attribute**</span></span>

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

### <a name="split-images"></a><span data-ttu-id="1b84a-256">分割された画像</span><span class="sxs-lookup"><span data-stu-id="1b84a-256">Split images</span></span>

<span data-ttu-id="1b84a-257">Web ページの URL または名前が付いた部分の **data-render-src** 属性を使用して作成された画像は、パフォーマンスと表示上の理由から、複数のコンポーネントの画像に分割されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1b84a-257">Images that are created using the **data-render-src** attribute (from a webpage URL or a named part) might be split into multiple component images for performance and rendering reasons. Component images are all assigned the same data-id value. Each component image has a zero-based data-index attribute that defines the original vertical layout.</span></span> <span data-ttu-id="1b84a-258">コンポーネントの画像には、すべて同じ **data-id** 値が割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-258">Component images are all assigned the same **data-id** value.</span></span> <span data-ttu-id="1b84a-259">各コンポーネントの画像には、元の垂直レイアウトを定義するゼロベースの data-index 属性があります。</span><span class="sxs-lookup"><span data-stu-id="1b84a-259">Each component image has a zero-based data-index attribute that defines the original vertical layout.</span></span>

<span data-ttu-id="1b84a-260">**画像を 3 つのコンポーネントの画像に分割する**</span><span class="sxs-lookup"><span data-stu-id="1b84a-260">**Split image with three component images**</span></span>

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

<span data-ttu-id="1b84a-p130">ユーザーはページ上の画像を移動できるため、返されるインデックスの順序が乱れている場合があります。順序は、y 軸方向の競合がある場合、y 軸方向の上から下に 、続いて x 軸方向の左から右に並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-p130">Because users can move the images on the page, the returned indexes might be out of order. Ordering should be in top to bottom y-order, then left to right x-order if there are y-order conflicts.</span></span>

## <a name="iframe-elements"></a><span data-ttu-id="1b84a-263">iframe 要素</span><span class="sxs-lookup"><span data-stu-id="1b84a-263">iframe elements</span></span>
<span data-ttu-id="1b84a-264">OneNote ページには、**iframe** 要素で表される埋め込みビデオを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-264">OneNote pages can contain embedded videos represented by **iframe** elements.</span></span> 

><span data-ttu-id="1b84a-265">**注:** [**object** 要素を使用してビデオ ファイルを添付](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-images-files#files)することもできます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-265">You can also [attach a video file using an **object** element](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-images-files#files).</span></span>

<span data-ttu-id="1b84a-266">**入力属性**</span><span class="sxs-lookup"><span data-stu-id="1b84a-266">**Input attributes**</span></span>

|<span data-ttu-id="1b84a-267">入力属性</span><span class="sxs-lookup"><span data-stu-id="1b84a-267">Input attribute</span></span>|<span data-ttu-id="1b84a-268">説明</span><span class="sxs-lookup"><span data-stu-id="1b84a-268">Description</span></span>|
|:------|:------|
| <span data-ttu-id="1b84a-269">data-original-src</span><span class="sxs-lookup"><span data-stu-id="1b84a-269">data-original-src</span></span> | <span data-ttu-id="1b84a-270">必須。</span><span class="sxs-lookup"><span data-stu-id="1b84a-270">Required.</span></span> <span data-ttu-id="1b84a-271">ビデオ ソースの URL。</span><span class="sxs-lookup"><span data-stu-id="1b84a-271">The URL of the video source.</span></span> <span data-ttu-id="1b84a-272">[サポートされるビデオ ソースの一覧](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-images-files#videos)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1b84a-272">See the [list of supported video sources](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-images-files#videos).</span></span> <span data-ttu-id="1b84a-273">例: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span><span class="sxs-lookup"><span data-stu-id="1b84a-273">Example: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span></span> |
| <span data-ttu-id="1b84a-274">width、height</span><span class="sxs-lookup"><span data-stu-id="1b84a-274">width, height</span></span> | <span data-ttu-id="1b84a-275">iframe の幅と高さ (ピクセル単位)。</span><span class="sxs-lookup"><span data-stu-id="1b84a-275">The width or height of the iframe, in pixels.</span></span> <span data-ttu-id="1b84a-276">例: `width=300`</span><span class="sxs-lookup"><span data-stu-id="1b84a-276">Example: `width=300`</span></span> |

<span data-ttu-id="1b84a-277">**出力属性**</span><span class="sxs-lookup"><span data-stu-id="1b84a-277">**Output attributes**</span></span>

|<span data-ttu-id="1b84a-278">出力属性</span><span class="sxs-lookup"><span data-stu-id="1b84a-278">Output attribute</span></span>|<span data-ttu-id="1b84a-279">説明</span><span class="sxs-lookup"><span data-stu-id="1b84a-279">Description</span></span>|
|:------|:------|
| <span data-ttu-id="1b84a-280">data-original-src</span><span class="sxs-lookup"><span data-stu-id="1b84a-280">data-original-src</span></span> | <span data-ttu-id="1b84a-281">ビデオ ソースの URL。</span><span class="sxs-lookup"><span data-stu-id="1b84a-281">The URL of the video source.</span></span> |
| <span data-ttu-id="1b84a-282">src</span><span class="sxs-lookup"><span data-stu-id="1b84a-282">src</span></span> | <span data-ttu-id="1b84a-283">OneNote ページに埋め込まれたビデオへのリンク。</span><span class="sxs-lookup"><span data-stu-id="1b84a-283">A link to the video that is embedded in the OneNote page.</span></span> |
| <span data-ttu-id="1b84a-284">width、height</span><span class="sxs-lookup"><span data-stu-id="1b84a-284">width, height</span></span> | <span data-ttu-id="1b84a-285">iframe の幅と高さ (ピクセル単位)。</span><span class="sxs-lookup"><span data-stu-id="1b84a-285">The width or height of the iframe, in pixels.</span></span> <span data-ttu-id="1b84a-286">例: `width=300`</span><span class="sxs-lookup"><span data-stu-id="1b84a-286">Example: `width=300`</span></span> |
 
<span data-ttu-id="1b84a-287">ビデオの**出力 HTML** の例</span><span class="sxs-lookup"><span data-stu-id="1b84a-287">**Output HTML** example for videos</span></span>

<span data-ttu-id="1b84a-288">次に示すように、出力 **iframe** 要素には、ソース ページとビデオに関連付けられたエンドポイントが含まれています。</span><span class="sxs-lookup"><span data-stu-id="1b84a-288">Output **iframe** elements contain endpoints that link to the source page and video, as shown below.</span></span> 

```html
<iframe 
    width="340" height="280" 
    data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8" 
    src="https://www.youtube.com/embed/3Ztr44aKmQ8?feature=oembed&autoplay=true" />
``` 

## <a name="object-elements"></a><span data-ttu-id="1b84a-289">object 要素</span><span class="sxs-lookup"><span data-stu-id="1b84a-289">Object elements</span></span>
<span data-ttu-id="1b84a-290">OneNote ページには、**object** 要素で表される添付ファイルを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-290">OneNote pages can contain file attachments represented by **object** elements. An object element can contain the following attributes in the input and output HTML.</span></span> <span data-ttu-id="1b84a-291">**object** 要素は、入力 HTML および出力 HTML に次の属性を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-291">An **img** element can contain the following attributes in the input and output HTML.</span></span>

><span data-ttu-id="1b84a-292">**注:** ファイルが画像として送信され、**data-render-src** 属性を使用する場合、OneNote API はファイルのコンテンツを画像としてページに表示できます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-292">The OneNote API can also render file content as images in a page when the file is sent as an image and uses the **data-render-src** attribute.</span></span> <span data-ttu-id="1b84a-293">例: `<img data-render-src="name:part-name" ... />`</span><span class="sxs-lookup"><span data-stu-id="1b84a-293">Example: `<img data-render-src="name:part-name" ... />`</span></span>
 

<span data-ttu-id="1b84a-294">**入力属性**</span><span class="sxs-lookup"><span data-stu-id="1b84a-294">**Input attributes**</span></span>

|<span data-ttu-id="1b84a-295">入力属性</span><span class="sxs-lookup"><span data-stu-id="1b84a-295">Input attribute</span></span>|<span data-ttu-id="1b84a-296">説明</span><span class="sxs-lookup"><span data-stu-id="1b84a-296">Description</span></span>|
|:------|:------|
| <span data-ttu-id="1b84a-297">data</span><span class="sxs-lookup"><span data-stu-id="1b84a-297">data</span></span> | <span data-ttu-id="1b84a-298">必須。</span><span class="sxs-lookup"><span data-stu-id="1b84a-298">Required.</span></span> <span data-ttu-id="1b84a-299">[マルチパート要求](../api-reference/v1.0/api/section_post_pages.md#example)のファイルを表す部分の名前。</span><span class="sxs-lookup"><span data-stu-id="1b84a-299">The name of the part that represents the file in the [multipart request](../api-reference/v1.0/api/section_post_pages.md#example).</span></span> |
| <span data-ttu-id="1b84a-300">data-attachment</span><span class="sxs-lookup"><span data-stu-id="1b84a-300">data-attachment</span></span> | <span data-ttu-id="1b84a-p137">必須。ファイル名。</span><span class="sxs-lookup"><span data-stu-id="1b84a-p137">Required. The file name.</span></span> |
| <span data-ttu-id="1b84a-303">data-id</span><span class="sxs-lookup"><span data-stu-id="1b84a-303">data-id</span></span> | <span data-ttu-id="1b84a-304">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="1b84a-304">A reference for the element.</span></span> <span data-ttu-id="1b84a-305">[ページ コンテンツの更新](../api-reference/v1.0/api/page_update.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="1b84a-305">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="1b84a-306">style</span><span class="sxs-lookup"><span data-stu-id="1b84a-306">style</span></span> | <p><span data-ttu-id="1b84a-307">オブジェクトの位置とサイズのプロパティ: **position** (**absolute** のみ)、**left**、**top**、および **width**。</span><span class="sxs-lookup"><span data-stu-id="1b84a-307">The position and size properties for the object: **position** (**absolute** only), **left**, **top**, and **width**.</span></span></p><p><span data-ttu-id="1b84a-308">本文が `data-absolute-enabled="true"` に設定されていて、オブジェクトが本文の直接の子の場合にのみ、[絶対位置](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos)のオブジェクトの作成に使用されます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-308">Used to create an [absolute positioned](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos) object, only if the object is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br /><span data-ttu-id="1b84a-309">例: `<object style="position:absolute;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="1b84a-309">Example: `<object style="position:absolute;top:350px;left:300px" ... />`</span></span></p> |
| <span data-ttu-id="1b84a-310">type</span><span class="sxs-lookup"><span data-stu-id="1b84a-310">type</span></span> | <span data-ttu-id="1b84a-p139">必須。標準のメディア ファイルの型。既知のファイルの型では、OneNote ページにファイルの種類と関連付けられたアイコンが表示されます。未知のファイルの型では、汎用のファイル アイコンが表示されます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-p139">Required. The standard media file type. Known file types display the icon associated with the file type on the OneNote page. Unknown file types display a generic file icon.</span></span> |
<!--todo: add link to known file types--> 

<span data-ttu-id="1b84a-315">**出力属性**</span><span class="sxs-lookup"><span data-stu-id="1b84a-315">**Output attributes**</span></span>

|<span data-ttu-id="1b84a-316">出力属性</span><span class="sxs-lookup"><span data-stu-id="1b84a-316">Output attribute</span></span>|<span data-ttu-id="1b84a-317">説明</span><span class="sxs-lookup"><span data-stu-id="1b84a-317">Description</span></span>|
|:------|:------|
| <span data-ttu-id="1b84a-318">data</span><span class="sxs-lookup"><span data-stu-id="1b84a-318">data</span></span> | <span data-ttu-id="1b84a-319">ファイルのリソースのエンドポイント。</span><span class="sxs-lookup"><span data-stu-id="1b84a-319">The endpoint for the file resource.</span></span> |
| <span data-ttu-id="1b84a-320">data-attachment</span><span class="sxs-lookup"><span data-stu-id="1b84a-320">data-attachment</span></span> | <span data-ttu-id="1b84a-321">ファイル名。</span><span class="sxs-lookup"><span data-stu-id="1b84a-321">The file name.</span></span> |
| <span data-ttu-id="1b84a-322">data-id</span><span class="sxs-lookup"><span data-stu-id="1b84a-322">data-id</span></span> | <span data-ttu-id="1b84a-323">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="1b84a-323">A reference for the element.</span></span> <span data-ttu-id="1b84a-324">[ページ コンテンツの更新](../api-reference/v1.0/api/page_update.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="1b84a-324">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="1b84a-325">id</span><span class="sxs-lookup"><span data-stu-id="1b84a-325">id</span></span> | <span data-ttu-id="1b84a-326">要素の一意の生成された ID。</span><span class="sxs-lookup"><span data-stu-id="1b84a-326">A unique, generated ID for the element.</span></span> <span data-ttu-id="1b84a-327">`includeIDs=true` クエリ オプションを使用した場合に、[ページの *content* エンドポイントに対する GET 要求](../api-reference/v1.0/api/page_get.md)から返されます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-327">Returned by [GET requests to a page's *content* endpoint](../api-reference/v1.0/api/page_get.md) when the `includeIDs=true` query option is used.</span></span> <span data-ttu-id="1b84a-328">[ページ コンテンツの更新](../api-reference/v1.0/api/page_update.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="1b84a-328">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="1b84a-329">style</span><span class="sxs-lookup"><span data-stu-id="1b84a-329">style</span></span> | <span data-ttu-id="1b84a-330">オブジェクトの位置のプロパティ。</span><span class="sxs-lookup"><span data-stu-id="1b84a-330">The position properties of the object.</span></span> |
| <span data-ttu-id="1b84a-331">type</span><span class="sxs-lookup"><span data-stu-id="1b84a-331">type</span></span> | <span data-ttu-id="1b84a-332">標準のメディア ファイルの種類。</span><span class="sxs-lookup"><span data-stu-id="1b84a-332">The standard media file type.</span></span> |
 

<span data-ttu-id="1b84a-333">オブジェクトの**出力 HTML** の例</span><span class="sxs-lookup"><span data-stu-id="1b84a-333">**Output HTML** example for objects</span></span>

<span data-ttu-id="1b84a-334">次に示すように、出力 **object** 要素には、ページ内のファイル リソースにリンクされたエンドポイントが含まれています。</span><span class="sxs-lookup"><span data-stu-id="1b84a-334">Output **object** elements contain endpoints that link to the file resources in the page, as shown below. You can make separate GET requests to file resource endpoints to retrieve their binary contents.</span></span> <span data-ttu-id="1b84a-335">バイナリ コンテンツを取得するには、これらの[ファイル リソースのエンドポイントに対して個別の GET 要求](../api-reference/v1.0/api/resource_get.md)を実行します。</span><span class="sxs-lookup"><span data-stu-id="1b84a-335">Output object elements contain endpoints that link to the file resources in the page, as shown below. You can make separate [GET requests to file resource endpoints](../api-reference/v1.0/api/resource_get.md) to retrieve their binary contents.</span></span>

```html
<object
    data="https://graph.microsoft.com/v1.0/me/onenote/resources/{file-id}/$value"
    data-attachment="fileName.pdf" 
    type="application/pdf" 
    [style="..."] />
``` 

## <a name="paragraphs-and-headings"></a><span data-ttu-id="1b84a-336">段落と見出し</span><span class="sxs-lookup"><span data-stu-id="1b84a-336">Paragraphs and headings</span></span>

<span data-ttu-id="1b84a-337">段落、見出し、その他のテキストのコンテナーには、入力 HTML と出力 HTML の次の属性を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-337">Paragraphs, headings, and other text containers can contain the following attributes in the input and output HTML.</span></span>

<span data-ttu-id="1b84a-338">**入力属性**</span><span class="sxs-lookup"><span data-stu-id="1b84a-338">**Input attributes**</span></span>

|<span data-ttu-id="1b84a-339">入力属性</span><span class="sxs-lookup"><span data-stu-id="1b84a-339">Input attribute</span></span>|<span data-ttu-id="1b84a-340">説明</span><span class="sxs-lookup"><span data-stu-id="1b84a-340">Description</span></span>|
|:------|:------|
| <span data-ttu-id="1b84a-341">data-id</span><span class="sxs-lookup"><span data-stu-id="1b84a-341">data-id</span></span> | <span data-ttu-id="1b84a-342">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="1b84a-342">A reference for the element.</span></span> <span data-ttu-id="1b84a-343">[ページ コンテンツの更新](../api-reference/v1.0/api/page_update.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="1b84a-343">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="1b84a-344">data-tag</span><span class="sxs-lookup"><span data-stu-id="1b84a-344">data-tag</span></span> | <span data-ttu-id="1b84a-345">**p** 要素または **h1** - **h6** 要素上の[ノート シール](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags)。</span><span class="sxs-lookup"><span data-stu-id="1b84a-345">A [note tag](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) on a **p** or **h1** - **h6** element.</span></span> |
| <span data-ttu-id="1b84a-346">style</span><span class="sxs-lookup"><span data-stu-id="1b84a-346">style</span></span> | <span data-ttu-id="1b84a-347">要素の CSS [style](#styles)のプロパティ。</span><span class="sxs-lookup"><span data-stu-id="1b84a-347">The CSS [style](#styles) properties of the element.</span></span> |
 

<span data-ttu-id="1b84a-348">**出力属性**</span><span class="sxs-lookup"><span data-stu-id="1b84a-348">**Output attributes**</span></span>

|<span data-ttu-id="1b84a-349">出力属性</span><span class="sxs-lookup"><span data-stu-id="1b84a-349">Output attribute</span></span>|<span data-ttu-id="1b84a-350">説明</span><span class="sxs-lookup"><span data-stu-id="1b84a-350">Description</span></span>|
|:------|:------|
| <span data-ttu-id="1b84a-351">data-id</span><span class="sxs-lookup"><span data-stu-id="1b84a-351">data-id</span></span> | <span data-ttu-id="1b84a-352">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="1b84a-352">A reference for the element.</span></span> <span data-ttu-id="1b84a-353">[ページ コンテンツの更新](../api-reference/v1.0/api/page_update.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="1b84a-353">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="1b84a-354">data-tag</span><span class="sxs-lookup"><span data-stu-id="1b84a-354">data-tag</span></span> | <span data-ttu-id="1b84a-355">**p** 要素または **h1** - **h6** 要素上の[ノート シール](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags)。</span><span class="sxs-lookup"><span data-stu-id="1b84a-355">A [note tag](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) on a **p** or **h1** - **h6** element.</span></span> |
| <span data-ttu-id="1b84a-356">id</span><span class="sxs-lookup"><span data-stu-id="1b84a-356">id</span></span> | <span data-ttu-id="1b84a-357">要素の一意の生成された ID。</span><span class="sxs-lookup"><span data-stu-id="1b84a-357">A unique, generated ID for the element.</span></span> <span data-ttu-id="1b84a-358">`includeIDs=true` クエリ オプションを使用した場合に、[ページの *content* エンドポイントに対する GET 要求](../api-reference/v1.0/api/page_get.md)から返されます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-358">Returned by [GET requests to a page's *content* endpoint](../api-reference/v1.0/api/page_get.md) when the `includeIDs=true` query option is used.</span></span> <span data-ttu-id="1b84a-359">[ページ コンテンツの更新](../api-reference/v1.0/api/page_update.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="1b84a-359">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="1b84a-360">style</span><span class="sxs-lookup"><span data-stu-id="1b84a-360">style</span></span> | <span data-ttu-id="1b84a-361">要素の CSS [style](#styles)のプロパティ。</span><span class="sxs-lookup"><span data-stu-id="1b84a-361">The CSS [style](#styles) properties of the element.</span></span> <span data-ttu-id="1b84a-362">出力 HTML では、これらの値は、適切な子要素または **span** 要素でインラインで返すことができます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-362">The CSS style properties of the element. In the output HTML, these values may be returned inline on appropriate child elements or on **span** elements.</span></span> |
 

<span data-ttu-id="1b84a-363">次の例では、テキストのコンテナーおよび返される出力 HTML にスタイルを定義するさまざまな方法を使用する入力 HTML を示しています。</span><span class="sxs-lookup"><span data-stu-id="1b84a-363">The following examples show input HTML that uses different ways to define styles on text containers and the output HTML that's returned.</span></span>

<span data-ttu-id="1b84a-364">開始タグ内、および **span** 要素内に、インライン文字スタイルを使用して定義されたスタイル付き **入力 HTML**。</span><span class="sxs-lookup"><span data-stu-id="1b84a-364">**Input HTML** with styles defined using inline character styles, in the start tag, and within a **span** element.</span></span>

```html
<h1>Heading <i>One</i> text</h1>
<p style="font-size:8pt;color:green;font-family:Courier;text-align:center">Some text</p>
<p>Some <span  style="font-size:16px;color:#ff0000;font-family:Segoe UI Black">more</span> text</p>
``` 

<span data-ttu-id="1b84a-365">**span** 要素でインライン CSS スタイルとして返される `<p>` 開始タグ内の `<i>` 文字スタイルとフォント設定を伴う**出力 HTML**。</span><span class="sxs-lookup"><span data-stu-id="1b84a-365">**Output HTML** with the `<i>` character style and the font settings in the `<p>` start tag returned as inline CSS styles on **span** elements.</span></span>

```html
<h1 style="font-size:16pt;color:#1e4e79;margin-top:11pt;margin-bottom:11pt">Heading <span style="font-style:italic">One</span> text</h1>
<p style="text-align:center"><span style="font-family:Courier;font-size:8pt;color:green">Some text</span></p>
<p>Some <span style="font-family:Segoe UI Black;font-size:12pt;color:red">more</span> text</p>
``` 


## <a name="lists"></a><span data-ttu-id="1b84a-366">リスト</span><span class="sxs-lookup"><span data-stu-id="1b84a-366">Lists</span></span>
<span data-ttu-id="1b84a-367">リストは、**li** 要素を含む **ol** 要素または **ul** 要素として表されます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-367">Lists are represented as **ol** or **ul** elements that contain list items represented as **li** elements.</span></span>

<span data-ttu-id="1b84a-368">入力 HTML および出力 HTML には、リストとリスト項目に次の属性を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-368">Lists and list items can contain the following attributes in the input and output HTML.</span></span>

<span data-ttu-id="1b84a-369">**入力属性**</span><span class="sxs-lookup"><span data-stu-id="1b84a-369">**Input attributes**</span></span>

|<span data-ttu-id="1b84a-370">入力属性</span><span class="sxs-lookup"><span data-stu-id="1b84a-370">Input attribute</span></span>|<span data-ttu-id="1b84a-371">説明</span><span class="sxs-lookup"><span data-stu-id="1b84a-371">Description</span></span>|
|:------|:------|
| <span data-ttu-id="1b84a-372">data-id</span><span class="sxs-lookup"><span data-stu-id="1b84a-372">data-id</span></span> | <span data-ttu-id="1b84a-373">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="1b84a-373">A reference for the element.</span></span> <span data-ttu-id="1b84a-374">[ページ コンテンツの更新](../api-reference/v1.0/api/page_update.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="1b84a-374">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="1b84a-375">data-tag</span><span class="sxs-lookup"><span data-stu-id="1b84a-375">data-tag</span></span> | <span data-ttu-id="1b84a-376">**ul**、**ol**、または **li** の各要素上の[ノート シール](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags)。</span><span class="sxs-lookup"><span data-stu-id="1b84a-376">A [note tag](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) on a **ul**, **ol**, or **li** element.</span></span> |
| <span data-ttu-id="1b84a-377">style</span><span class="sxs-lookup"><span data-stu-id="1b84a-377">style</span></span> | <span data-ttu-id="1b84a-378">リストまたはリスト項目の **list-style-type** および CSS [style](#styles) のプロパティ。</span><span class="sxs-lookup"><span data-stu-id="1b84a-378">The **list-style-type** and the CSS [style](#styles) properties for the list or list item.</span></span> |
 

<span data-ttu-id="1b84a-379">**出力属性**</span><span class="sxs-lookup"><span data-stu-id="1b84a-379">**Output attributes**</span></span>

|<span data-ttu-id="1b84a-380">出力属性</span><span class="sxs-lookup"><span data-stu-id="1b84a-380">Output attribute</span></span>|<span data-ttu-id="1b84a-381">説明</span><span class="sxs-lookup"><span data-stu-id="1b84a-381">Description</span></span>|
|:------|:------|
| <span data-ttu-id="1b84a-382">data-id</span><span class="sxs-lookup"><span data-stu-id="1b84a-382">data-id</span></span> | <span data-ttu-id="1b84a-383">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="1b84a-383">A reference for the element.</span></span> <span data-ttu-id="1b84a-384">[ページ コンテンツの更新](../api-reference/v1.0/api/page_update.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="1b84a-384">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="1b84a-385">data-tag</span><span class="sxs-lookup"><span data-stu-id="1b84a-385">data-tag</span></span> |  <span data-ttu-id="1b84a-386">**li** 要素内の span 上の[ノート シール](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags)。</span><span class="sxs-lookup"><span data-stu-id="1b84a-386">A [note tag](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) on a span in a **li** element.</span></span> |
| <span data-ttu-id="1b84a-387">id</span><span class="sxs-lookup"><span data-stu-id="1b84a-387">id</span></span> | <span data-ttu-id="1b84a-388">要素の一意の生成された ID。</span><span class="sxs-lookup"><span data-stu-id="1b84a-388">A unique, generated ID for the element.</span></span> <span data-ttu-id="1b84a-389">`includeIDs=true` クエリ オプションを使用した場合に、[ページの *content* エンドポイントに対する GET 要求](../api-reference/v1.0/api/page_get.md)から返されます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-389">Returned by [GET requests to a page's *content* endpoint](../api-reference/v1.0/api/page_get.md) when the `includeIDs=true` query option is used.</span></span> <span data-ttu-id="1b84a-390">[ページ コンテンツの更新](../api-reference/v1.0/api/page_update.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="1b84a-390">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="1b84a-391">style</span><span class="sxs-lookup"><span data-stu-id="1b84a-391">style</span></span> | <span data-ttu-id="1b84a-392">要素の **list-style-type** および CSS の [style](#styles) のプロパティ。</span><span class="sxs-lookup"><span data-stu-id="1b84a-392">The **list-style-type** and CSS [style](#styles) properties of the element.</span></span> <span data-ttu-id="1b84a-393">出力 HTML では、リストレベル設定がリスト項目で返されます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-393">The list-style-type and CSS style properties of the element. In the output HTML, list-level settings are returned on list items. Default properties are not returned.</span></span> <span data-ttu-id="1b84a-394">既定のプロパティは返されません。</span><span class="sxs-lookup"><span data-stu-id="1b84a-394">The following properties are not returned:</span></span> |
 

<span data-ttu-id="1b84a-395">Microsoft Graph の OneNote API では、次のリストのスタイルをサポートします。</span><span class="sxs-lookup"><span data-stu-id="1b84a-395">The OneNote APIs in Microsoft Graph support the following list styles:</span></span>

|<span data-ttu-id="1b84a-396">番号付きリスト</span><span class="sxs-lookup"><span data-stu-id="1b84a-396">Ordered list</span></span>|<span data-ttu-id="1b84a-397">記号付きリスト</span><span class="sxs-lookup"><span data-stu-id="1b84a-397">Unordered list</span></span>|
|:------|:------|
| <span data-ttu-id="1b84a-398">none</span><span class="sxs-lookup"><span data-stu-id="1b84a-398">none</span></span> | <span data-ttu-id="1b84a-399">none</span><span class="sxs-lookup"><span data-stu-id="1b84a-399">none</span></span> |
| <span data-ttu-id="1b84a-400">decimal (default)</span><span class="sxs-lookup"><span data-stu-id="1b84a-400">decimal (default)</span></span> | <span data-ttu-id="1b84a-401">disc (default)</span><span class="sxs-lookup"><span data-stu-id="1b84a-401">disc (default)</span></span> |
| <span data-ttu-id="1b84a-402">lower-alpha</span><span class="sxs-lookup"><span data-stu-id="1b84a-402">lower-alpha</span></span> | <span data-ttu-id="1b84a-403">Circle</span><span class="sxs-lookup"><span data-stu-id="1b84a-403">circle</span></span> |
| <span data-ttu-id="1b84a-404">lower-roman</span><span class="sxs-lookup"><span data-stu-id="1b84a-404">lower-roman</span></span> | <span data-ttu-id="1b84a-405">square</span><span class="sxs-lookup"><span data-stu-id="1b84a-405">square</span></span> |
| <span data-ttu-id="1b84a-406">upper-alpha</span><span class="sxs-lookup"><span data-stu-id="1b84a-406">upper-alpha</span></span> | &nbsp; |
| <span data-ttu-id="1b84a-407">upper-roman</span><span class="sxs-lookup"><span data-stu-id="1b84a-407">upper-roman</span></span> | &nbsp; |
 
<span data-ttu-id="1b84a-408">入力 HTML の **ol** 要素または **ul** 要素のリストにはグローバル スタイルを適用できますが、スタイルは **li** 要素で返されます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-408">You can apply global styles for a list on the **ol** or **ul** element in the input HTML, but styles are returned on the **li** elements.</span></span>

<span data-ttu-id="1b84a-409">**同種リスト スタイル**</span><span class="sxs-lookup"><span data-stu-id="1b84a-409">**Homogenous list style**</span></span>

<span data-ttu-id="1b84a-410">この例は、**ol** 要素のリスト スタイルの種類と個々のリスト項目の CSS スタイルを設定する入力 HTML を示しています。</span><span class="sxs-lookup"><span data-stu-id="1b84a-410">This example shows input HTML that sets the list style type on the **ol** element and CSS styles on individual list items.</span></span>

```html
<ol style="list-style-type:upper-roman;color:blue">
    <li style="font-weight:bold">Jacksonville</li>
    <li style="text-decoration:line-through">Orlando</li>
    <li style="font-family:Courier">Naples</li>
</ol>
``` 

<span data-ttu-id="1b84a-411">これは出力 HTML です。</span><span class="sxs-lookup"><span data-stu-id="1b84a-411">This is the output HTML.</span></span> <span data-ttu-id="1b84a-412">スタイルが個々の **li** 要素または **span** 要素で、インラインで返されることにご注意ください。</span><span class="sxs-lookup"><span data-stu-id="1b84a-412">Notice that styles are returned inline on the individual **li** or **span** elements.</span></span>

```html
<ol>
    <li style="list-style-type:upper-roman"><span style="color:blue;font-weight:bold">Jacksonville</span></li>
    <li style="list-style-type:upper-roman"><span style="color:blue;text-decoration:line-through">Orlando</span></li>
    <li style="list-style-type:upper-roman"><span style="font-family:Courier;color:blue">Naples</span></li>
</ol>
``` 

<span data-ttu-id="1b84a-413">**可変のリスト スタイル**</span><span class="sxs-lookup"><span data-stu-id="1b84a-413">**Variable list styles**</span></span>

<span data-ttu-id="1b84a-414">この例は、**li** 要素にさまざまなリスト スタイルの種類を設定する入力 HTML を示しています。</span><span class="sxs-lookup"><span data-stu-id="1b84a-414">This example shows input HTML that sets different list style types on the **li** elements.</span></span>

```html
<ul style="font-style:italic">
    <li style="list-style-type:square">square style</li>
    <li style="list-style-type:circle">circle style</li>
    <li style="list-style-type:disc">disc style (default)</li>
</ul>
``` 

<span data-ttu-id="1b84a-415">これは出力 HTML です。</span><span class="sxs-lookup"><span data-stu-id="1b84a-415">This is the output HTML.</span></span> <span data-ttu-id="1b84a-416">スタイルが個々の **li** 要素または **span** 要素で、インラインで返されることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="1b84a-416">Notice that styles are returned inline on the individual **li** or **span** elements.</span></span>

```html
<ul>
    <li style="list-style-type:square"><span style="font-style:italic">square style</span></li>
    <li style="list-style-type:circle"><span style="font-style:italic">circle style</span></li>
    <li><span style="font-style:italic">disc style (default)</span></li>
</ul>
``` 


## <a name="tables"></a><span data-ttu-id="1b84a-417">テーブル</span><span class="sxs-lookup"><span data-stu-id="1b84a-417">Tables</span></span>
<span data-ttu-id="1b84a-418">テーブルは、**tr** 要素と **td** 要素を含めることができる **table** 要素として表されます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-418">Tables are represented as **table** elements that can contain **tr** and **td** elements.</span></span> <span data-ttu-id="1b84a-419">入れ子のテーブルがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="1b84a-419">Nested tables are supported.</span></span>

<span data-ttu-id="1b84a-420">入力 HTML と出力 HTML では、テーブルに次の属性を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-420">Tables can contain the following attributes in the input and output HTML.</span></span> <span data-ttu-id="1b84a-421">OneNote API では、**rowspan** 属性または **colspan** 属性はサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="1b84a-421">The OneNote API does not support **rowspan** or **colspan** attributes.</span></span> 

<span data-ttu-id="1b84a-422">**入力属性**</span><span class="sxs-lookup"><span data-stu-id="1b84a-422">**Input attributes**</span></span>

|<span data-ttu-id="1b84a-423">入力属性</span><span class="sxs-lookup"><span data-stu-id="1b84a-423">Input attribute</span></span>|<span data-ttu-id="1b84a-424">説明</span><span class="sxs-lookup"><span data-stu-id="1b84a-424">Description</span></span>|
|:------|:------|
| <span data-ttu-id="1b84a-425">data-id</span><span class="sxs-lookup"><span data-stu-id="1b84a-425">data-id</span></span> | <span data-ttu-id="1b84a-426">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="1b84a-426">A reference for the element.</span></span> <span data-ttu-id="1b84a-427">[ページ コンテンツの更新](../api-reference/v1.0/api/page_update.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="1b84a-427">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="1b84a-428">style</span><span class="sxs-lookup"><span data-stu-id="1b84a-428">style</span></span> | <span data-ttu-id="1b84a-429">要素の CSS の [style](#styles)のプロパティ、および:</span><span class="sxs-lookup"><span data-stu-id="1b84a-429">The CSS [style](#styles) properties of the element, and also:</span></span><br/> <span data-ttu-id="1b84a-430">- **border**。</span><span class="sxs-lookup"><span data-stu-id="1b84a-430">- **border**.</span></span> <span data-ttu-id="1b84a-431">0px または 1px のいずれかにすることができます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-431">Can be either 0px or 1px.</span></span><br /> <span data-ttu-id="1b84a-432">- **width**。</span><span class="sxs-lookup"><span data-stu-id="1b84a-432">- **width**.</span></span> <span data-ttu-id="1b84a-433">**table** および **td** でサポートされます。ピクセル数またはページ幅のパーセンテージを使用します。</span><span class="sxs-lookup"><span data-stu-id="1b84a-433">Supported by **table** and **td** as pixels or percentage of page width.</span></span><br /><span data-ttu-id="1b84a-434">例: `width="100px"` または `width="60%"`</span><span class="sxs-lookup"><span data-stu-id="1b84a-434">Example: `width="100px"` or `width="60%"`</span></span> |
 

<span data-ttu-id="1b84a-435">**出力属性**</span><span class="sxs-lookup"><span data-stu-id="1b84a-435">**Output attributes**</span></span>

|<span data-ttu-id="1b84a-436">出力属性</span><span class="sxs-lookup"><span data-stu-id="1b84a-436">Output attribute</span></span>|<span data-ttu-id="1b84a-437">説明</span><span class="sxs-lookup"><span data-stu-id="1b84a-437">Description</span></span>|
|:------|:------|
| <span data-ttu-id="1b84a-438">data-id</span><span class="sxs-lookup"><span data-stu-id="1b84a-438">data-id</span></span> | <span data-ttu-id="1b84a-439">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="1b84a-439">A reference for the element.</span></span> <span data-ttu-id="1b84a-440">[ページ コンテンツの更新](../api-reference/v1.0/api/page_update.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="1b84a-440">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="1b84a-441">id</span><span class="sxs-lookup"><span data-stu-id="1b84a-441">id</span></span> | <span data-ttu-id="1b84a-442">要素の一意の生成された ID。</span><span class="sxs-lookup"><span data-stu-id="1b84a-442">A unique, generated ID for the element.</span></span> <span data-ttu-id="1b84a-443">`includeIDs=true` クエリ オプションを使用した場合に、[ページの *content* エンドポイントに対する GET 要求](../api-reference/v1.0/api/page_get.md)から返されます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-443">Returned by [GET requests to a page's *content* endpoint](../api-reference/v1.0/api/page_get.md) when the `includeIDs=true` query option is used.</span></span> <span data-ttu-id="1b84a-444">[ページ コンテンツの更新](../api-reference/v1.0/api/page_update.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="1b84a-444">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="1b84a-445">style</span><span class="sxs-lookup"><span data-stu-id="1b84a-445">style</span></span> | <span data-ttu-id="1b84a-446">要素の CSS [style](#styles)のプロパティ。</span><span class="sxs-lookup"><span data-stu-id="1b84a-446">The CSS [style](#styles) properties of the element.</span></span> |
 

<span data-ttu-id="1b84a-447">次の例では、さまざまな方法を使用してテーブルのスタイルと返される出力 HTML を定義する入力 HTML を示しています。</span><span class="sxs-lookup"><span data-stu-id="1b84a-447">The following examples show input HTML that uses different ways to define styles on tables and the output HTML that's returned.</span></span>

<span data-ttu-id="1b84a-448">さまざまなレベルのオプション設定を伴う**入力 HTML**。</span><span class="sxs-lookup"><span data-stu-id="1b84a-448">**Input HTML** with optional settings at different levels.</span></span>

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
 
<span data-ttu-id="1b84a-449">**td** 要素でインラインで返される CSS スタイルを伴う**出力 HTML**。</span><span class="sxs-lookup"><span data-stu-id="1b84a-449">**Output HTML** with CSS styles returned inline on the **td** elements.</span></span>

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


## <a name="styles"></a><span data-ttu-id="1b84a-450">Styles</span><span class="sxs-lookup"><span data-stu-id="1b84a-450">Styles</span></span>
<span data-ttu-id="1b84a-451">Microsoft Graph の OneNote API は、ページ本文の要素 (**body**、**div**、**p**、**li**、**span** など) として、次に示すインライン CSS の **style** プロパティをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="1b84a-451">The OneNote API supports the following inline CSS **style** properties for elements in the page body, such as **body**, **div**, **p**, **li**, and **span**.</span></span>

|<span data-ttu-id="1b84a-452">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1b84a-452">Property</span></span>|<span data-ttu-id="1b84a-453">例</span><span class="sxs-lookup"><span data-stu-id="1b84a-453">Example</span></span>|
|:------|:------|
| <span data-ttu-id="1b84a-454">background-color</span><span class="sxs-lookup"><span data-stu-id="1b84a-454">background-color</span></span> | <span data-ttu-id="1b84a-455">`style="background-color:#66cc66"` (既定は white)</span><span class="sxs-lookup"><span data-stu-id="1b84a-455">`style="background-color:#66cc66"` (defaults to white)</span></span><br /><span data-ttu-id="1b84a-456">16 進数形式と名前付きの色の両方がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="1b84a-456">Both hexadecimal format and named colors are supported.</span></span> |
| <span data-ttu-id="1b84a-457">color</span><span class="sxs-lookup"><span data-stu-id="1b84a-457">color</span></span> | <span data-ttu-id="1b84a-458">`style="color:#ffffff"` (既定は black)</span><span class="sxs-lookup"><span data-stu-id="1b84a-458">`style="color:#ffffff"` (defaults to black)</span></span> |
| <span data-ttu-id="1b84a-459">font-family</span><span class="sxs-lookup"><span data-stu-id="1b84a-459">font-family</span></span> | <span data-ttu-id="1b84a-460">`style="font-family:Courier"` (既定は Calibri)</span><span class="sxs-lookup"><span data-stu-id="1b84a-460">`style="font-family:Courier"` (defaults to Calibri)</span></span> |
| <span data-ttu-id="1b84a-461">font-size</span><span class="sxs-lookup"><span data-stu-id="1b84a-461">font-size</span></span> | <span data-ttu-id="1b84a-462">`style="font-size:10pt"` (既定は 11pt)</span><span class="sxs-lookup"><span data-stu-id="1b84a-462">`style="font-size:10pt"` (defaults to 11pt)</span></span><br /><span data-ttu-id="1b84a-463">API は *pt* または *px* のフォント サイズを受け入れますが、*px* は *pt* に変換します。</span><span class="sxs-lookup"><span data-stu-id="1b84a-463">The OneNote API accepts font size in *pt* or *px*, but converts *px* to *pt*.</span></span> <span data-ttu-id="1b84a-464">10 進数の値は、最も近い n.0pt または n.5pt に四捨五入されます。</span><span class="sxs-lookup"><span data-stu-id="1b84a-464">Decimal values are rounded to the nearest n.0pt or n.5pt.</span></span> |
| <span data-ttu-id="1b84a-465">font-style</span><span class="sxs-lookup"><span data-stu-id="1b84a-465">font-style</span></span> | <span data-ttu-id="1b84a-466">`style="font-style:italic"` (標準または斜体のみ)</span><span class="sxs-lookup"><span data-stu-id="1b84a-466">`style="font-style:italic"` (normal or italic only)</span></span> |
| <span data-ttu-id="1b84a-467">font-weight</span><span class="sxs-lookup"><span data-stu-id="1b84a-467">font-weight</span></span> | <span data-ttu-id="1b84a-468">`style="font-weight:bold"` (標準または太字のみ)</span><span class="sxs-lookup"><span data-stu-id="1b84a-468">`style="font-weight:bold"` (normal or bold only)</span></span> |
| <span data-ttu-id="1b84a-469">strike-through</span><span class="sxs-lookup"><span data-stu-id="1b84a-469">strike-through</span></span> | `style="text-decoration:line-through"` |
| <span data-ttu-id="1b84a-470">text-align</span><span class="sxs-lookup"><span data-stu-id="1b84a-470">text-align</span></span> | <span data-ttu-id="1b84a-471">`style="text-align:center"` (ブロック要素の場合のみ)</span><span class="sxs-lookup"><span data-stu-id="1b84a-471">`style="text-align:center"` (for block elements only)</span></span> |
| <span data-ttu-id="1b84a-472">text-decoration</span><span class="sxs-lookup"><span data-stu-id="1b84a-472">text-decoration</span></span> | <span data-ttu-id="1b84a-473">`style="text-decoration:underline"` (なし、または下線のみ)</span><span class="sxs-lookup"><span data-stu-id="1b84a-473">`style="text-decoration:underline"` (none or underline only)</span></span> |
 

<span data-ttu-id="1b84a-474">次のインライン文字スタイルもサポートされています。</span><span class="sxs-lookup"><span data-stu-id="1b84a-474">The following inline character styles and are also supported:</span></span>

<table id="simpletable">
<tr>
<td id="simplecell"><span data-ttu-id="1b84a-475">&lt;b&gt;</span><span class="sxs-lookup"><span data-stu-id="1b84a-475">&lt;b&gt;</span></span></td>
<td id="simplecell"><span data-ttu-id="1b84a-476">&lt;i&gt;</span><span class="sxs-lookup"><span data-stu-id="1b84a-476">&lt;I</span></span></td>
<td id="simplecell"><span data-ttu-id="1b84a-477">&lt;u&gt;</span><span class="sxs-lookup"><span data-stu-id="1b84a-477">&lt;U</span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="1b84a-478">&lt;em&gt;</span><span class="sxs-lookup"><span data-stu-id="1b84a-478">&lt;em&gt;</span></span></td>
<td id="simplecell"><span data-ttu-id="1b84a-479">&lt;strong&gt;</span><span class="sxs-lookup"><span data-stu-id="1b84a-479">&lt;strong&gt;</span></span></td>
<td id="simplecell"><span data-ttu-id="1b84a-480">&lt;strike&gt;</span><span class="sxs-lookup"><span data-stu-id="1b84a-480">&lt;strike&gt;</span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="1b84a-481">&lt;sup&gt;</span><span class="sxs-lookup"><span data-stu-id="1b84a-481">&lt;sup&gt;</span></span></td>
<td id="simplecell"><span data-ttu-id="1b84a-482">&lt;sub&gt;</span><span class="sxs-lookup"><span data-stu-id="1b84a-482">&lt;Sub&gt;</span></span></td>
<td id="simplecell"><span data-ttu-id="1b84a-483">&lt;del&gt;</span><span class="sxs-lookup"><span data-stu-id="1b84a-483">&lt;del&gt;</span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="1b84a-484">&lt;cite&gt;</span><span class="sxs-lookup"><span data-stu-id="1b84a-484">&lt;cite&gt;</span></span></td>
<td id="simplecell">&nbsp;</td>
<td id="simplecell">&nbsp;</td>
</tr>
</table>

 
## <a name="input-and-output-html-example"></a><span data-ttu-id="1b84a-485">入力 HTML と出力 HTML の例</span><span class="sxs-lookup"><span data-stu-id="1b84a-485">Input and output HTML</span></span>
<span data-ttu-id="1b84a-486">次の画像は、Microsoft Graph で作成された簡単なページを示しています。</span><span class="sxs-lookup"><span data-stu-id="1b84a-486">The following image shows a simple page that was created with the OneNote API.</span></span>

![Wikipedia によるコンテンツのスタディ ノートを付記した OneNote ページの画像](images/onenote-sample-image.png)

<span data-ttu-id="1b84a-488">これは、ページを作成するためにメッセージ本文で送信された入力 HTML です。</span><span class="sxs-lookup"><span data-stu-id="1b84a-488">This is the input HTML sent in the message body to create the page.</span></span>

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

<span data-ttu-id="1b84a-489">これは、[ページ コンテンツを取得](../api-reference/v1.0/api/page_get.md)するときに Microsoft Graph が返す出力 HTML です。</span><span class="sxs-lookup"><span data-stu-id="1b84a-489">This is the output HTML that the OneNote API returns when you [get page content](../api-reference/v1.0/api/page_get.md).</span></span>

><span data-ttu-id="1b84a-490">**注:** [ページを作成する](../api-reference/v1.0/api/section_post_pages.md)ときや、[ページのメタデータを取得する](../api-reference/v1.0/api/page_get.md)ときに、API は **contentUrl** プロパティのページの*コンテンツ* エンドポイント URL を返します。</span><span class="sxs-lookup"><span data-stu-id="1b84a-490">When you [create a page](../api-reference/v1.0/api/section_post_pages.md) or [get page metadata](../api-reference/v1.0/api/page_get.md), the API returns the *content* endpoint URL of the page in the **contentUrl** property.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="1b84a-491">関連項目</span><span class="sxs-lookup"><span data-stu-id="1b84a-491">See also</span></span>

- [<span data-ttu-id="1b84a-492">OneNote コンテンツと構造を取得する</span><span class="sxs-lookup"><span data-stu-id="1b84a-492">Get Onenote content and structure</span></span>](../api-reference/v1.0/api/page_get.md)
- [<span data-ttu-id="1b84a-493">OneNote ページの作成</span><span class="sxs-lookup"><span data-stu-id="1b84a-493">Create OneNote pages</span></span>](../api-reference/v1.0/api/section_post_pages.md)
- [<span data-ttu-id="1b84a-494">OneNote ページ コンテンツを更新する</span><span class="sxs-lookup"><span data-stu-id="1b84a-494">Update OneNote page content</span></span>](../api-reference/v1.0/api/page_update.md)
- [<span data-ttu-id="1b84a-495">画像とファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="1b84a-495">Add images and files</span></span>](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags)
