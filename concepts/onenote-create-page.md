# <a name="create-onenote-pages"></a><span data-ttu-id="30330-101">OneNote ページの作成</span><span class="sxs-lookup"><span data-stu-id="30330-101">Create OneNote pages</span></span>

<span data-ttu-id="30330-102">**適用対象**: OneDrive のコンシューマー ノートブック | Office 365 のエンタープライズ ノートブック</span><span class="sxs-lookup"><span data-stu-id="30330-102">**Applies to**: Consumer notebooks on OneDrive | Enterprise notebooks on Office 365</span></span>

<span data-ttu-id="30330-p101">OneNote ページを作成する場合は、POST 要求を *pages* エンドポイントに送信します。次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="30330-p101">To create a OneNote page, you send a POST request to a *pages* endpoint. For example:</span></span>

`POST ../notes/sections/{id}/pages`

<br/>

<span data-ttu-id="30330-105">メッセージ本文でページを定義する HTML を送信します。</span><span class="sxs-lookup"><span data-stu-id="30330-105">Send the HTML that defines the page in the message body.</span></span> <span data-ttu-id="30330-106">要求が成功すると、Microsoft Graph は 201 HTTP 状態コードを返します。</span><span class="sxs-lookup"><span data-stu-id="30330-106">If the request is successful, Microsoft Graph returns a 201 HTTP status code.</span></span>


> <span data-ttu-id="30330-107">**注:** セクション、セクション グループ、ノートブックを作成するために送信できる POST 要求の詳細については、[対話型 REST リファレンス](http://dev.onenote.com/docs)</span><span class="sxs-lookup"><span data-stu-id="30330-107">**Note:** To learn about the POST requests you can send to create sections, section groups, and notebooks, see our [interactive REST reference](http://dev.onenote.com/docs).</span></span>


<a name="request-uri"></a>

## <a name="construct-the-request-uri"></a><span data-ttu-id="30330-108">要求 URI の構築</span><span class="sxs-lookup"><span data-stu-id="30330-108">Construct the request URI</span></span>

<span data-ttu-id="30330-109">POST 要求 URI を構築するには、サービス ルート URL から開始します。</span><span class="sxs-lookup"><span data-stu-id="30330-109">To construct the POST request URI, start with the service root URL:</span></span>

`https://graph.microsoft.com/v1.0/me/onenote`

<br/>

<span data-ttu-id="30330-110">次に、*pages* エンドポイントを追加します。</span><span class="sxs-lookup"><span data-stu-id="30330-110">Then append the *pages* endpoint:</span></span>

- <span data-ttu-id="30330-111">**任意のセクション (セクション名で指定) にページを作成する**</span><span class="sxs-lookup"><span data-stu-id="30330-111">**Create a page in any section (specified by section name)**</span></span><br/><br/>`.../pages?sectionName=DefaultSection`

- <span data-ttu-id="30330-112">**任意のセクション (ID で指定) にページを作成する**</span><span class="sxs-lookup"><span data-stu-id="30330-112">**Create a page in any section (specified by ID)**</span></span><br/><br/>`.../sections/{section-id}/pages` 

<span data-ttu-id="30330-113">ユーザーの個人用ノートブックにページを作成する場合は、Microsoft Graph が提供する、既定のノートブックにページを作成するためのエンドポイントを使用することもできます。</span><span class="sxs-lookup"><span data-stu-id="30330-113">If you're creating pages in the user's personal notebook, Microsoft Graph also provides endpoints you can use to create pages in the default notebook:</span></span>

- <span data-ttu-id="30330-114">**既定のノートブックの既定のセクションにページを作成する**</span><span class="sxs-lookup"><span data-stu-id="30330-114">**Create a page in the default section of the default notebook**</span></span><br/><br/>`../pages` 



<span data-ttu-id="30330-115">完全な要求 URI は、次に示す例のいずれかのようになります。</span><span class="sxs-lookup"><span data-stu-id="30330-115">Your full request URI will look like one of these examples:</span></span>

- `https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/pages`
- `https://graph.microsoft.com/v1.0/me/onenote/pages?sectionName=Homework`

<span data-ttu-id="30330-116">[サービス ルート URL](../api-reference/v1.0/resources/onenote-api-overview.md#root-url) の詳細についてはリンク先を参照してください。</span><span class="sxs-lookup"><span data-stu-id="30330-116">Learn more about the [service root URL](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span></span>

<a name="post-pages-section-name"></a>

### <a name="using-the-sectionname-url-parameter"></a><span data-ttu-id="30330-117">*sectionName* URL パラメーターの使用</span><span class="sxs-lookup"><span data-stu-id="30330-117">Using the *sectionName* URL parameter</span></span>

<span data-ttu-id="30330-118">次に示すルールは、*sectionName* パラメーターを使用して、既定のノートブックの指名したセクションにページを作成するときに適用されます。</span><span class="sxs-lookup"><span data-stu-id="30330-118">The following rules apply when using the *sectionName* parameter to create a page in a named section in the default notebook:</span></span>

- <span data-ttu-id="30330-119">最上位のセクションのみを参照できます (セクション グループ内のセクションは参照できません)。</span><span class="sxs-lookup"><span data-stu-id="30330-119">Only top-level sections can be referenced (not sections within section groups).</span></span>

- <span data-ttu-id="30330-120">指定した名前のセクションが既定のノートブックに存在しない場合、そのセクションは API によって作成されます。</span><span class="sxs-lookup"><span data-stu-id="30330-120">If a section with the specified name doesn't exist in the default notebook, the API creates it.</span></span> <span data-ttu-id="30330-121">セクション名に使用できない文字は、「`? * \ / : < > | & # " % ~`」です。 `? * \ / : < > | & # " % ~`</span><span class="sxs-lookup"><span data-stu-id="30330-121">These characters are not allowed for section names: `? * \ / : < > | & # " % ~`</span></span>

- <span data-ttu-id="30330-p104">セクション名の照合では、大文字と小文字が区別されませんが、セクションが作成されるときには大文字と小文字が維持されます。そのため、"My New Section" はこのとおりに表示されますが、これ以降の POST では "my new section" も一致します。</span><span class="sxs-lookup"><span data-stu-id="30330-p104">Section names are case-insensitive for matching, but case is preserved when sections are created. So "My New Section" will display like that, but "my new section" would also match on subsequent posts.</span></span>

- <span data-ttu-id="30330-p105">セクション名は、URL エンコードされている必要があります。たとえば、スペースは *%20* とエンコードされなければなりません。</span><span class="sxs-lookup"><span data-stu-id="30330-p105">Section names must be URL-encoded. For example, spaces must be encoded as *%20*.</span></span>

- <span data-ttu-id="30330-126">*sectionName* パラメーターは、`../notes/pages` のルートでのみ有効になります (`../notes/sections/{id}/pages` では無効です)。</span><span class="sxs-lookup"><span data-stu-id="30330-126">The *sectionName* parameter is valid only with the `../notes/pages` route (not `../notes/sections/{id}/pages`).</span></span>

<span data-ttu-id="30330-127">セクションは存在しない場合に作成されるため、この呼び出しはアプリで作成するすべてのページに使用しても問題ありません。</span><span class="sxs-lookup"><span data-stu-id="30330-127">Because sections are created if they don't exist, it's safe to use this call with every page your app creates.</span></span> <span data-ttu-id="30330-128">セクションの名前はユーザーが変更する可能性もありますが、API は指定されたセクション名で新しいセクションを作成します。</span><span class="sxs-lookup"><span data-stu-id="30330-128">Users might rename sections, but the API will create a new section with the section name that you supply.</span></span> 

> <span data-ttu-id="30330-129">**注:** API から返された、名前を変更したセクション内のページへのリンクは、引き続き元のページに到達します。</span><span class="sxs-lookup"><span data-stu-id="30330-129">**Note:** The links returned by the API for pages in a renamed section will still reach those older pages.</span></span> 


<a name="message-body"></a>

## <a name="construct-the-message-body"></a><span data-ttu-id="30330-130">メッセージ本文の構築</span><span class="sxs-lookup"><span data-stu-id="30330-130">Construct the message body</span></span>

<span data-ttu-id="30330-p107">ページのコンテンツを定義する HTML は、*入力 HTML* と呼ばれます。入力 HTML は、[標準の HTML および CSS のサブセット](#supported-html-and-css-for-onenote-pages)と、追加のカスタム属性をサポートしています。(**data-id** や **data-render-src** のようなカスタム属性は[入力および出力 HTML](onenote_input_output_html.md) で記述されます)。</span><span class="sxs-lookup"><span data-stu-id="30330-p107">The HTML that defines page content is called *input HTML*. Input HTML supports a [subset of standard HTML and CSS](#supported-html-and-css-for-onenote-pages), with the addition of custom attributes. (Custom attributes, like **data-id** and **data-render-src**, are described in [Input and output HTML](onenote_input_output_html.md).)</span></span> 

<span data-ttu-id="30330-p108">入力 HTML は、POST 要求のメッセージ本文で送信します。入力 HTML は、`application/xhtml+xml` または `text/html` コンテンツ タイプを使用して、メッセージ本文に直接含めて送信することも、マルチパート要求の "Presentation" 部分に含めて送信することもできます。</span><span class="sxs-lookup"><span data-stu-id="30330-p108">Send the input HTML in the message body of the POST request. You can send the input HTML directly in the message body using the  `application/xhtml+xml` or `text/html` content type, or you can send it in the "Presentation" part of a multipart request.</span></span> 

<span data-ttu-id="30330-136">次に示す例では、入力 HTML をメッセージ本文に直接含めて送信しています。</span><span class="sxs-lookup"><span data-stu-id="30330-136">The following example sends the input HTML directly in the message body.</span></span>

```html
POST https://graph.microsoft.com/v1.0/me/onenote/pages
Authorization: Bearer {token}
Content-Type: application/xhtml+xml

<!DOCTYPE html>
<html>
  <head>
    <title>A page with a block of HTML</title>
    <meta name="created" content="2015-07-22T09:00:00-08:00" />
  </head>
  <body>
    <p>This page contains some <i>formatted</i> <b>text</b> and an image.</p>
    <img src="http://..." alt="an image on the page" width="500" />
  </body>
</html>
```

<br/>

<span data-ttu-id="30330-137">バイナリ データを送信する場合は、[マルチパート要求](#example-request)を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="30330-137">If you're sending binary data, you must use a [multipart request](#example-request).</span></span> 

> <span data-ttu-id="30330-138">**注:** プログラミングを簡単にして、アプリでの一貫性を保つために、すべてのページの作成にマルチパート要求を使用できます。</span><span class="sxs-lookup"><span data-stu-id="30330-138">**Note:** To simplify programming and consistency in your app, you can use multipart requests to create all pages.</span></span> <span data-ttu-id="30330-139">マルチパート メッセージを作成するライブラリの使用をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="30330-139">It's a good idea to use a library to construct multipart messages.</span></span> <span data-ttu-id="30330-140">これにより、無効な形式のペイロードを作成してしまう危険性が少なくなります。</span><span class="sxs-lookup"><span data-stu-id="30330-140">This reduces the risk of creating malformed payloads.</span></span>


<a name="input-html-rules"></a>

### <a name="requirements-and-limitations-for-input-html-in-post-pages-requests"></a><span data-ttu-id="30330-141">POST pages 要求の入力 HTML に対する要件と制限事項</span><span class="sxs-lookup"><span data-stu-id="30330-141">Requirements and limitations for input HTML in POST pages requests</span></span>

<span data-ttu-id="30330-142">入力 HTML を送信するときには、次に示す一般的な要件と制限事項に注意してください。</span><span class="sxs-lookup"><span data-stu-id="30330-142">When sending input HTML, be aware of these general requirements and limitations:</span></span>  

- <span data-ttu-id="30330-p110">入力 HTML は、UTF-8 でエンコードされた整形式の XHTML である必要があります。すべてのコンテナーの開始タグは、終了タグと一致する必要があります。すべての属性値は、二重引用符または一重引用符で囲む必要があります。  <!--docs say MUST be encoded--></span><span class="sxs-lookup"><span data-stu-id="30330-p110">Input HTML should be UTF-8 encoded and well-formed XHTML. All container start tags require matching closing tags. All attribute values must be surrounded by double- or single-quote marks.  <!--docs say MUST be encoded--></span></span>

- <span data-ttu-id="30330-146">JavaScript コード (ファイルを含む) および CSS は削除されます。</span><span class="sxs-lookup"><span data-stu-id="30330-146">JavaScript code, included files, and CSS are removed.</span></span> 

- <span data-ttu-id="30330-147">HTML フォームは全体が削除されます。</span><span class="sxs-lookup"><span data-stu-id="30330-147">HTML forms are removed in their entirety.</span></span>  

- <span data-ttu-id="30330-148">Microsoft Graph は [HTML 要素のサブセット](#supported-html-and-css-for-onenote-pages)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="30330-148">Microsoft Graph supports a [subset of HTML elements](#supported-html-and-css-for-onenote-pages).</span></span> 

- <span data-ttu-id="30330-149">Microsoft Graph は一般的な HTML 属性のサブセットとカスタム属性のセットをサポートします (ページの更新に使用される **data-id** 属性など)。</span><span class="sxs-lookup"><span data-stu-id="30330-149">Microsoft Graph supports a subset of common HTML attributes and a set of custom attributes, such as the **data-id** attribute used for updating pages.</span></span> <span data-ttu-id="30330-150">サポートされる属性については、「[入出力 HTML](onenote_input_output_html.md)</span><span class="sxs-lookup"><span data-stu-id="30330-150">For supported attributes, see [Input and output HTML](onenote_input_output_html.md).</span></span>


<a name="supported-html"></a>

### <a name="supported-html-and-css-for-onenote-pages"></a><span data-ttu-id="30330-151">OneNote ページでサポートされる HTML と CSS</span><span class="sxs-lookup"><span data-stu-id="30330-151">Supported HTML and CSS for OneNote pages</span></span>

<span data-ttu-id="30330-152">すべての要素、属性、およびプロパティがサポートされるわけではありません (HTML4、XHTML、CSS、HTML5 などについて)。</span><span class="sxs-lookup"><span data-stu-id="30330-152">Not all elements, attributes, and properties are supported (in HTML4, XHTML, CSS, HTML5, etc.).</span></span> <span data-ttu-id="30330-153">Microsoft Graph は、ユーザーの OneNote の使用方法に適した、限定的な HTML のセットを受け入れます。</span><span class="sxs-lookup"><span data-stu-id="30330-153">Instead, Microsoft Graph accepts a limited set of HTML that better fits how people use OneNote.</span></span> <span data-ttu-id="30330-154">詳細については、「[ページでサポートされる HTML タグ](http://dev.onenote.com/docs#/introduction/html-tag-support-for-pages)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="30330-154">For more information, see [HTML tag support for pages](http://dev.onenote.com/docs#/introduction/html-tag-support-for-pages).</span></span> <span data-ttu-id="30330-155">この参照先に示されていないタグは、無視されることがあります。</span><span class="sxs-lookup"><span data-stu-id="30330-155">If a tag's not listed there, it'll probably be ignored.</span></span>

<!--Microsoft Graph only accepts UTF-8 data. Be sure that all requests are encoded that way, and your content-type headers indicate that as well. xx our examples don't show this-->

<span data-ttu-id="30330-156">次に、Microsoft Graph でサポートされる基本的な要素の種類の一覧を示します。</span><span class="sxs-lookup"><span data-stu-id="30330-156">The following list shows the basic element types that Microsoft Graph supports:</span></span>

- <span data-ttu-id="30330-157">`<head>` と `<body>`</span><span class="sxs-lookup"><span data-stu-id="30330-157">`<head>` and `<body>`</span></span></p>
- <span data-ttu-id="30330-158">`<title>` と `<meta>` (ページのタイトルと作成日を設定する)</span><span class="sxs-lookup"><span data-stu-id="30330-158">`<title>` and `<meta>` that set the page title and creation date</span></span></p>
- <span data-ttu-id="30330-159">`<h1>` から `<h6>` (セクションの見出し用)</span><span class="sxs-lookup"><span data-stu-id="30330-159">`<h1>` through `<h6>` for section headings</span></span></p>
- <span data-ttu-id="30330-160">`<p>` (段落用)</span><span class="sxs-lookup"><span data-stu-id="30330-160">`<p>` for paragraphs</span></span></p>
- <span data-ttu-id="30330-161">`<ul>`、`<ol>`、および `<li>` (リストおよびリスト アイテム用)</span><span class="sxs-lookup"><span data-stu-id="30330-161">`<ul>`, `<ol>`, and `<li>` for lists and list items</span></span></p>
- <span data-ttu-id="30330-162">`<table>`、`<tr>`、および `<td>` (入れ子になったテーブルを含む)</span><span class="sxs-lookup"><span data-stu-id="30330-162">`<table>`, `<tr>` and `<td>`, including nested tables</span></span></p>
- <span data-ttu-id="30330-163">`<pre>` (書式設定済みのテキスト用であり、空白と改行が維持される)</span><span class="sxs-lookup"><span data-stu-id="30330-163">`<pre>` for preformatted text (preserves white space and line breaks)</span></span></p>
- <span data-ttu-id="30330-164">`<b>` と `<i>` (太字および斜体文字スタイル用)</span><span class="sxs-lookup"><span data-stu-id="30330-164">`<b>` and `<i>` for bold and italic character styles</span></span></p>

<span data-ttu-id="30330-165">Microsoft Graph は、ページの作成時に入力 HTML の意味内容と基本的構造を維持しますが、サポートされている HTML および CSS のセットを使用するように入力 HTML を変換します。</span><span class="sxs-lookup"><span data-stu-id="30330-165">Microsoft Graph preserves the semantic content and basic structure of the input HTML when it creates pages, but it converts the input HTML to use the supported set of HTML and CSS.</span></span> <span data-ttu-id="30330-166">OneNote に存在しない機能は変換されないため、ソース HTML では認識されない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="30330-166">Features that don't exist in OneNote have nothing to be translated to, so they might not be recognized in the source HTML.</span></span> 


<a name="example"></a>

## <a name="example-request"></a><span data-ttu-id="30330-167">要求の例</span><span class="sxs-lookup"><span data-stu-id="30330-167">Example request</span></span>

<span data-ttu-id="30330-168">ここに示すマルチパート要求の例では、イメージと埋め込みファイルが含まれたページを作成します。</span><span class="sxs-lookup"><span data-stu-id="30330-168">This example multipart request creates a page that contains images and an embedded file.</span></span> <span data-ttu-id="30330-169">必須の **Presentation** パーツには、ページを定義する入力 HTML が含まれています。</span><span class="sxs-lookup"><span data-stu-id="30330-169">The required **Presentation** part contains the input HTML that defines the page.</span></span> <span data-ttu-id="30330-170">**imageBlock1** パーツにはバイナリ イメージ データが含まれ、**fileBlock1** にはバイナリ ファイル データが含まれています。</span><span class="sxs-lookup"><span data-stu-id="30330-170">The **imageBlock1** part contains the binary image data, and **fileBlock1** contains the binary file data.</span></span> <span data-ttu-id="30330-171">データ パーツには、Microsoft Graph が OneNote ページに[画像として HTML をレンダリングする](onenote_images_files.md#add-an-image-using-binary-data)場合の HTML を含めることもできます。</span><span class="sxs-lookup"><span data-stu-id="30330-171">Data parts can also contain HTML, in which case Microsoft Graph [renders the HTML as an image](onenote_images_files.md#add-an-image-using-binary-data) on the OneNote page.</span></span> 

```html
POST https://graph.microsoft.com/v1.0/me/onenote/pages
Authorization: Bearer {token}
Content-Type: multipart/form-data; boundary=MyPartBoundary198374

--MyPartBoundary198374
Content-Disposition:form-data; name="Presentation"
Content-Type:text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with rendered images and an attached file</title>
    <meta name="created" content="2015-07-22T09:00:00-08:00" />
  </head>
  <body>
    <p>Here's an image from an <i>online source</i>:</p>
    <img src="http://..." alt="an image on the page" width="500" />
    <p>Here's an image uploaded as <b>binary data</b>:</p>
    <img src="name:imageBlock1" alt="an image on the page" width="300" />
    <p>Here's a file attachment:</p>
    <object data-attachment="FileName.pdf" data="name:fileBlock1" type="application/pdf" />
  </body>
</html>

--MyPartBoundary198374
Content-Disposition:form-data; name="imageBlock1"
Content-Type:image/jpeg

... binary image data ...

--MyPartBoundary198374
Content-Disposition:form-data; name="fileBlock1"
Content-Type:application/pdf

... binary file data ...

--MyPartBoundary198374--
```

<span data-ttu-id="30330-p115">複数イメージやその他のファイルを含むページの作成方法を示す例については、「[画像とファイルを追加する](onenote_images_files.md)」、および[チュートリアル](https://docs.microsoft.com/en-us/previous-versions/office/office-365-api/how-to/onenote-tutorial)と[サンプル](https://github.com/onenotedev)を参照してください。また、[絶対配置要素の作成](onenote-abs-pos.md)方法、[ノート シールの使用](onenote-note-tags.md)方法と、名刺キャプチャ、オンラインのレシピ一覧およびオンラインの製品一覧の[データ抽出](onenote-extract-data.md)方法について調べてください。</span><span class="sxs-lookup"><span data-stu-id="30330-p115">For more examples that show how to create pages that contain images and other files, see [Add images and files](onenote_images_files.md), our [tutorials](https://docs.microsoft.com/en-us/previous-versions/office/office-365-api/how-to/onenote-tutorial), and our [samples](https://github.com/onenotedev). Also, learn how to [create absolute positioned elements](onenote-abs-pos.md), [use note tags](onenote-note-tags.md), and [extract data](onenote-extract-data.md) for business card captures and online recipe and product listings.</span></span>

<span data-ttu-id="30330-174">Microsoft Graph は、マルチパート メッセージ本文の CRLF 改行など、一部の書式設定については厳密です。</span><span class="sxs-lookup"><span data-stu-id="30330-174">Microsoft Graph is strict about some formats, such as CRLF newlines in a multipart message body.</span></span> <span data-ttu-id="30330-175">無効な形式のペイロードを作成してしまう危険性を少なくするために、マルチパート メッセージはライブラリを使用して作成してください。</span><span class="sxs-lookup"><span data-stu-id="30330-175">To reduce the risk of creating malformed payloads, you should use a library to construct multipart messages.</span></span> 

<span data-ttu-id="30330-176">無効な形式のペイロードに関する 400 状態を受信した場合は、改行と空白の書式を確認し、エンコーディングの問題について調べます。</span><span class="sxs-lookup"><span data-stu-id="30330-176">If you do receive a 400 status for a malformed payload, check the formatting of newlines and whitespaces, and check for encoding issues.</span></span> <span data-ttu-id="30330-177">たとえば、`charset=utf-8` を使用してみてください (例: `Content-Type: text/html; charset=utf-8`)。</span><span class="sxs-lookup"><span data-stu-id="30330-177">For example, try using `charset=utf-8` (example: `Content-Type: text/html; charset=utf-8`).</span></span>

<span data-ttu-id="30330-178">[入力 HTML に対する要件と制限事項](#requirements-and-limitations-for-input-html-in-post-pages-requests) および [POST 要求のサイズ制限](onenote_images_files.md#size-limitations-for-post-pages-requests)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="30330-178">See [requirements and limitations for input HTML](#requirements-and-limitations-for-input-html-in-post-pages-requests) and [size limits for POST requests](onenote_images_files.md#size-limitations-for-post-pages-requests).</span></span>


<a name="request-response-info"></a>

## <a name="request-and-response-information-for-post-pages-requests"></a><span data-ttu-id="30330-179">*POST pages* 要求の要求情報と応答情報</span><span class="sxs-lookup"><span data-stu-id="30330-179">Request and response information for *POST pages* requests</span></span>

| <span data-ttu-id="30330-180">要求データ</span><span class="sxs-lookup"><span data-stu-id="30330-180">Request data</span></span> | <span data-ttu-id="30330-181">説明</span><span class="sxs-lookup"><span data-stu-id="30330-181">Description</span></span> |  
|------|------|  
| <span data-ttu-id="30330-182">プロトコル</span><span class="sxs-lookup"><span data-stu-id="30330-182">Protocol</span></span> | <span data-ttu-id="30330-183">すべての要求は SSL/TLS HTTPS プロトコルを使用します。</span><span class="sxs-lookup"><span data-stu-id="30330-183">All requests use the SSL/TLS HTTPS protocol.</span></span> |  
| <span data-ttu-id="30330-184">承認ヘッダー</span><span class="sxs-lookup"><span data-stu-id="30330-184">Authorization header</span></span> | <p><span data-ttu-id="30330-185">`Bearer {token}`。`{token}` は、登録済みアプリの有効な OAuth 2.0 アクセス トークンです。</span><span class="sxs-lookup"><span data-stu-id="30330-185">`Bearer {token}`, where `{token}` is a valid OAuth 2.0 access token for your registered app.</span></span></p><p><span data-ttu-id="30330-p118">これがないか、無効の場合、401 ステータス コードで要求は失敗します。「[認証とアクセス許可](permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="30330-p118">If missing or invalid, the request fails with a 401 status code. See [Authentication and permissions](permissions_reference.md).</span></span></p> |  
| <span data-ttu-id="30330-188">Content-Type ヘッダー</span><span class="sxs-lookup"><span data-stu-id="30330-188">Content-Type header</span></span> | <p><span data-ttu-id="30330-189">`text/html` HTML コンテンツの `text/html` または `application/xhtml+xml`。メッセージ本文またはマルチパート要求の必須の "Presentation" パートで直接送信します。</span><span class="sxs-lookup"><span data-stu-id="30330-189">`text/html` or `application/xhtml+xml` for the HTML content, whether it's sent directly in the message body or in the required "Presentation" part of multipart requests.</span></span></p><p><span data-ttu-id="30330-190">マルチパート要求はバイナリ データを送信するときに必須であり、コンテンツ タイプとして `multipart/form-data; boundary=part-boundary` を使用します。`{part-boundary}` は、各データ パートの開始と終了を伝える文字列です。</span><span class="sxs-lookup"><span data-stu-id="30330-190">Multipart requests are required when sending binary data, and use the `multipart/form-data; boundary=part-boundary` content type, where `{part-boundary}` is a string that signals the start and end of each data part.</span></span></p> |  
| <span data-ttu-id="30330-191">Accept ヘッダー</span><span class="sxs-lookup"><span data-stu-id="30330-191">Accept header</span></span> | `application/json` | 

<br/>

| <span data-ttu-id="30330-192">応答データ</span><span class="sxs-lookup"><span data-stu-id="30330-192">Response data</span></span> | <span data-ttu-id="30330-193">説明</span><span class="sxs-lookup"><span data-stu-id="30330-193">Description</span></span> |  
|------|------|  
| <span data-ttu-id="30330-194">成功コード</span><span class="sxs-lookup"><span data-stu-id="30330-194">Success code</span></span> | <span data-ttu-id="30330-195">201 HTTP ステータス コード。</span><span class="sxs-lookup"><span data-stu-id="30330-195">A 201 HTTP status code.</span></span> |  
| <span data-ttu-id="30330-196">応答本文</span><span class="sxs-lookup"><span data-stu-id="30330-196">Response body</span></span> | <span data-ttu-id="30330-197">JSON 形式での新しいページの OData 表現。</span><span class="sxs-lookup"><span data-stu-id="30330-197">A OData representation of the new page in JSON format.</span></span> |  
| <span data-ttu-id="30330-198">エラー</span><span class="sxs-lookup"><span data-stu-id="30330-198">Errors</span></span> | <span data-ttu-id="30330-199">要求が失敗すると、API は応答本文の **@api.diagnostics** オブジェクトでエラーを返します。</span><span class="sxs-lookup"><span data-stu-id="30330-199">If the request fails, the API returns errors in the **@api.diagnostics** object in the response body.</span></span> |  
| <span data-ttu-id="30330-200">Location ヘッダー</span><span class="sxs-lookup"><span data-stu-id="30330-200">Location header</span></span> | <span data-ttu-id="30330-201">新しいページのリソース URL。</span><span class="sxs-lookup"><span data-stu-id="30330-201">The resource URL for the new page.</span></span> |  
| <span data-ttu-id="30330-202">X-CorrelationId ヘッダー</span><span class="sxs-lookup"><span data-stu-id="30330-202">X-CorrelationId header</span></span> | <span data-ttu-id="30330-p119">要求を一意に識別する GUID。Microsoft サポートと問題のトラブルシューティングを行う際に、この値を Date ヘッダーの値とともに使用できます。</span><span class="sxs-lookup"><span data-stu-id="30330-p119">A GUID that uniquely identifies the request. You can use this value along with the value of the Date header when working with Microsoft support to troubleshoot issues.</span></span> |  


<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-service-root-url"></a><span data-ttu-id="30330-205">Microsoft Graph サービスのルート URL の構築</span><span class="sxs-lookup"><span data-stu-id="30330-205">Constructing the Microsoft Graph service root URL</span></span>

<span data-ttu-id="30330-206">Microsoft Graph サービスのルート URL は、Microsoft Graph へのすべての呼び出しで次の形式を使用します。</span><span class="sxs-lookup"><span data-stu-id="30330-206">The Microsoft Graph service root URL uses the following format for all calls to Microsoft Graph:</span></span>

`https://graph.microsoft.com/{version}/me/onenote/`  

<span data-ttu-id="30330-207">URL の `version` セグメントは、使用する Microsoft Graph のバージョンを示しています。</span><span class="sxs-lookup"><span data-stu-id="30330-207">The `version` segment in the URL represents the version of Microsoft Graph that you want to use.</span></span> <span data-ttu-id="30330-208">安定した運用コードには `v1.0` を使用します。</span><span class="sxs-lookup"><span data-stu-id="30330-208">Use `v1.0` for stable production code.</span></span> <span data-ttu-id="30330-209">開発中の機能を試すには `beta` を使用します。</span><span class="sxs-lookup"><span data-stu-id="30330-209">Use `beta` to try out a feature that's in development.</span></span> <span data-ttu-id="30330-210">ベータ版の機能は変更される可能性があるため、運用コードでは使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="30330-210">Features and functionality in beta may change, so you shouldn't use it in your production code.</span></span> 

<span data-ttu-id="30330-211">現在のユーザーがアクセスできる OneNote コンテンツには `me` を使用します (所有と共有)。</span><span class="sxs-lookup"><span data-stu-id="30330-211">Use `me` for OneNote content that the current user can access (owned and shared).</span></span> <span data-ttu-id="30330-212">指定されたユーザー (URL 内) が現在のユーザーと共有している OneNote コンテンツには `users/{id}` を使用します。</span><span class="sxs-lookup"><span data-stu-id="30330-212">Use `users/{id}` for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="30330-213">ユーザー ID を取得するには [Microsoft Graph](https://graph.microsoft.com/v1.0/users) を使用します。</span><span class="sxs-lookup"><span data-stu-id="30330-213">Use [Microsoft Graph](https://graph.microsoft.com/v1.0/users) to get user IDs.</span></span> 


<a name="permissions"></a>

## <a name="permissions"></a><span data-ttu-id="30330-214">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="30330-214">Permissions</span></span>

<span data-ttu-id="30330-p122">OneNote ページを作成するには、適切なアクセス許可を要求する必要があります。アプリの動作に必要な最低限のアクセス許可を選択してください。</span><span class="sxs-lookup"><span data-stu-id="30330-p122">To create OneNote pages, you'll need to request appropriate permissions. Choose the lowest level of permissions that your app needs to do its work.</span></span>

<span data-ttu-id="30330-217">次から選択します。</span><span class="sxs-lookup"><span data-stu-id="30330-217">Choose from:</span></span>

- <span data-ttu-id="30330-218">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="30330-218">Notes.Create</span></span>
- <span data-ttu-id="30330-219">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="30330-219">Notes.ReadWrite</span></span>
- <span data-ttu-id="30330-220">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30330-220">Notes.ReadWrite.All</span></span>

<span data-ttu-id="30330-221">アクセス許可の範囲とその動作方法の詳細については、「[Microsoft Graph のアクセス許可のリファレンス](permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="30330-221">For more information about permission scopes and how they work, see [Microsoft Graph permissions reference](permissions_reference.md).</span></span>




<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="30330-222">関連項目</span><span class="sxs-lookup"><span data-stu-id="30330-222">See also</span></span>

- [<span data-ttu-id="30330-223">画像とファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="30330-223">Add images and files</span></span>](onenote_images_files.md)
- [<span data-ttu-id="30330-224">絶対配置要素を作成する</span><span class="sxs-lookup"><span data-stu-id="30330-224">Create absolute positioned elements</span></span>](onenote-abs-pos.md)  
- [<span data-ttu-id="30330-225">データを抽出する</span><span class="sxs-lookup"><span data-stu-id="30330-225">Extract data</span></span>](onenote-extract-data.md)
- [<span data-ttu-id="30330-226">ノート シールを使用する</span><span class="sxs-lookup"><span data-stu-id="30330-226">Use note tags</span></span>](onenote-note-tags.md)
- [<span data-ttu-id="30330-227">OneNote との統合</span><span class="sxs-lookup"><span data-stu-id="30330-227">Integrate with OneNote</span></span>](integrate_with_onenote.md)
- [<span data-ttu-id="30330-228">OneNote の開発者ブログ</span><span class="sxs-lookup"><span data-stu-id="30330-228">OneNote Developer Blog</span></span>](http://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="30330-229">Stack Overflow 掲載の OneNote の開発に関する質問</span><span class="sxs-lookup"><span data-stu-id="30330-229">OneNote development questions on Stack Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="30330-230">OneNote GitHub のリポジトリ</span><span class="sxs-lookup"><span data-stu-id="30330-230">OneNote GitHub repos</span></span>](http://go.microsoft.com/fwlink/?LinkID=390178)  


