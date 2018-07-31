
# <a name="add-images-videos-and-files-to-onenote-pages"></a><span data-ttu-id="f4cb3-101">OneNote ページに画像、ビデオ、ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="f4cb3-101">Add images, videos, and files to OneNote pages</span></span>

<span data-ttu-id="f4cb3-102">**適用対象** OneDrive のコンシューマー ノートブック | Office 365 のエンタープライズ ノートブック</span><span class="sxs-lookup"><span data-stu-id="f4cb3-102">**Applies to:** Consumer notebooks on OneDrive | Enterprise notebooks on Office 365</span></span>

<span data-ttu-id="f4cb3-103">**img**、**object**、および **iframe** 要素を使用すると、OneNote ページの[作成](onenote-create-page.md)時や[更新](onenote_update_page.md)時に、画像、ビデオ、およびファイルをページに追加できます。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-103">You can use **img**, **object**, and **iframe** elements to add images, videos, and files to a OneNote page when you're [creating](onenote-create-page.md) or [updating](onenote_update_page.md) the page.</span></span> 

- <span data-ttu-id="f4cb3-104">**img** を使用して、ページに画像を表示します。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-104">Use **img** to render an image on the page.</span></span>
- <span data-ttu-id="f4cb3-105">**iframe** を使用して、ページにビデオを埋め込みます。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-105">Use **iframe** to embed a video on the page.</span></span>
- <span data-ttu-id="f4cb3-106">**object** を使用して、ページに添付ファイルを追加します。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-106">Use **object** to add a file attachment to the page.</span></span>


<a name="images"></a>

## <a name="adding-images"></a><span data-ttu-id="f4cb3-107">画像を追加する</span><span class="sxs-lookup"><span data-stu-id="f4cb3-107">Adding images</span></span>

<span data-ttu-id="f4cb3-108">URL の参照または生データの送信によって、画像を追加できます。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-108">Images can be added by URL reference or by sending raw data.</span></span> <span data-ttu-id="f4cb3-109">Microsoft Graph では、OneNote ページに画像、ロゴ、および写真を追加する次の方法がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-109">Microsoft Graph supports the following methods of adding images, logos, and photos to OneNote pages.</span></span> 

[<span data-ttu-id="f4cb3-110">Web からパブリック イメージを追加する</span><span class="sxs-lookup"><span data-stu-id="f4cb3-110">Add a public image from the web</span></span>](#add-a-public-image-from-the-web)

<span data-ttu-id="f4cb3-p102">`img` で `src="http://image-url"` を使用し、公開されていてアクセス可能な画像の URL を指定します。OneNote ページに画像を表示します。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-p102">Use `img` with `src="http://image-url"` and specify the URL of a publicly accessible image. Renders the image on the OneNote page.</span></span>

[<span data-ttu-id="f4cb3-113">バイナリ データを使用して画像を追加する</span><span class="sxs-lookup"><span data-stu-id="f4cb3-113">Add an image using binary data</span></span>](#add-an-image-using-binary-data)

<span data-ttu-id="f4cb3-p103">`img` で `src="name:image-block-name"` を使用し、マルチパート要求のデータ部分で画像ファイルを送信します。OneNote ページに画像を表示します。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-p103">Use `img` with `src="name:image-block-name"` and send the image file in a data part of a multipart request. Renders the image on the OneNote page.</span></span>

[<span data-ttu-id="f4cb3-116">Web ページのスナップショットを追加する</span><span class="sxs-lookup"><span data-stu-id="f4cb3-116">Add a webpage snapshot</span></span>](#add-a-webpage-snapshot)

<span data-ttu-id="f4cb3-p104">`img` で `data-render-src="http://webpage-url"` を使用し、Web ページの URL を指定します。OneNote ページに Web ページ全体のスナップショットを表示します。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-p104">Use `img` with `data-render-src="http://webpage-url"` and specify the URL of a webpage. Renders a snapshot of the whole webpage on the OneNote page.</span></span>

[<span data-ttu-id="f4cb3-119">HTML から表示される画像を追加する</span><span class="sxs-lookup"><span data-stu-id="f4cb3-119">Add an image rendered from HTML</span></span>](#add-an-image-rendered-from-html)

<span data-ttu-id="f4cb3-p105">`img` で `data-render-src="name:html-block-name"` を使用し、マルチパート要求のデータ部分で HTML を送信します。OneNote ページに HTML を画像として表示します。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-p105">Use `img` with `data-render-src="name:html-block-name"` and send HTML in the data part of a multipart request. Renders the HTML as an image on the OneNote page.</span></span>

[<span data-ttu-id="f4cb3-122">PDF ファイルのコンテンツの画像を追加する</span><span class="sxs-lookup"><span data-stu-id="f4cb3-122">Add images of PDF file contents</span></span>](#add-images-of-pdf-file-contents)

<span data-ttu-id="f4cb3-123">`<img data-render-src="name:part-name" />`を使用します。マルチパート要求のデータ部分で PDF ファイルを送信します。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-123">Use `<img data-render-src="name:part-name" />` and send the PDF file in the data part of a multipart request.</span></span> <span data-ttu-id="f4cb3-124">OneNote ページの個別の画像として、PDF の各ページを表示します。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-124">Renders each PDF page as a separate image on the OneNote page.</span></span>

[<span data-ttu-id="f4cb3-125">添付ファイルとして画像ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="f4cb3-125">Add an image file as a file attachment</span></span>](#add-an-image-file-as-an-attachment)

<span data-ttu-id="f4cb3-p107">`object` と `data="name:file-block-name" data-attachment="file-name.file-ext" type="media-type"` を使用します。マルチパート要求のデータ部分で画像ファイルを送信します。添付ファイルを OneNote ページに追加して、ファイルのアイコンを表示します。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-p107">Use `object` with `data="name:file-block-name" data-attachment="file-name.file-ext" type="media-type"` and send an image file in the data part of a multipart request. Adds a file attachment to the OneNote page and displays a file icon.</span></span>


> <span data-ttu-id="f4cb3-128">**注:** OneNote ページで画像を取得するには、最初に[ページのコンテンツの GET 要求](onenote-get-content.md#page-html-content)を送信します。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-128">**Note:** To get images on a OneNote page, first send a [GET request for the page content](onenote-get-content.md#page-html-content).</span></span> <span data-ttu-id="f4cb3-129">これにより、ページで画像リソースへの URL を返します。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-129">This returns the URLs to the image resources on the page.</span></span> <span data-ttu-id="f4cb3-130">次に、[画像リソースに対する GET 要求](onenote-get-content.md#image-or-other-file-resource)を分離します。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-130">Then you separate [GET requests to the image resources](onenote-get-content.md#image-or-other-file-resource).</span></span>


#### <a name="image-attributes"></a><span data-ttu-id="f4cb3-131">画像の属性</span><span class="sxs-lookup"><span data-stu-id="f4cb3-131">Image attributes</span></span> 

<span data-ttu-id="f4cb3-132">**img** 要素には、**alt**、**height**、**width** 属性をオプションで含めることができ、スタイル属性の **max-width** と **max-height** を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-132">An **img** element can optionally include **alt**, **height**, and **width** attributes, and the style attributes **max-width** and **max-height**.</span></span>

#### <a name="image-media-types"></a><span data-ttu-id="f4cb3-133">画像のメディア タイプ</span><span class="sxs-lookup"><span data-stu-id="f4cb3-133">Image media types</span></span>

<span data-ttu-id="f4cb3-134">Microsoft Graph では、TIFF、PNG、GIF、JPEG、BMP の画像タイプがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-134">Microsoft Graph supports TIFF, PNG, GIF, JPEG, and BMP image types.</span></span> <span data-ttu-id="f4cb3-135">変換を望まない別の形式を使用する画像をキャプチャするには、マルチパート要求で[バイナリ データを送信](#add-an-image-using-binary-data)します。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-135">To capture an image that uses a different format that you don't want to convert, [send the binary data](#add-an-image-using-binary-data) in a multipart request.</span></span> <span data-ttu-id="f4cb3-136">Base64 を使用する必要はなく、送信するバイナリ データをエンコードする必要もありません。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-136">You don't need to use Base64 or otherwise encode the binary data that you send.</span></span>

> <span data-ttu-id="f4cb3-137">**メモ:** API は元の入力画像の種類を検出し、それを[出力 HTML](onenote_input_output_html.md#output-html) の **data-fullres-src-type** 属性として返します。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-137">**Note:** The API detects the original input image type, and returns it as the **data-fullres-src-type** attribute in the [output HTML](onenote_input_output_html.md#output-html).</span></span> <span data-ttu-id="f4cb3-138">API は、**data-src-type** で最適化された画像の種類も返します。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-138">The API also returns the image type of the optimized image in **data-src-type**.</span></span>
 
<span data-ttu-id="f4cb3-139">メディアを含むページを作成する場合に適用する[制限](#size-limitations-for-post-pages-requests)を確認してください。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-139">See [limitations](#size-limitations-for-post-pages-requests) that apply when creating pages that contain media.</span></span>


<a name="image-img-url-src"></a>

### <a name="add-a-public-image-from-the-web"></a><span data-ttu-id="f4cb3-140">Web からパブリック イメージを追加する</span><span class="sxs-lookup"><span data-stu-id="f4cb3-140">Add a public image from the web</span></span>

<span data-ttu-id="f4cb3-141">要求の入力 HTML では、`<img src="http://..." />` を含め、**src** 属性に公開されていてアクセス可能な画像の URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-141">In the input HTML of your request, include  `<img src="http://..." />` and specify the URL of a publicly accessible image for the **src** attribute.</span></span>

```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: Public URL</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page displays an image from the web.</p>
    <img src="http://..." width="300"/>
  </body>
</html>

--MyAppPartBoundary--  
```

<a name="image-img-binary-src"></a>

### <a name="add-an-image-using-binary-data"></a><span data-ttu-id="f4cb3-142">バイナリ データを使用して画像を追加する</span><span class="sxs-lookup"><span data-stu-id="f4cb3-142">Add an image using binary data</span></span>

<span data-ttu-id="f4cb3-143">要求の **Presentation** 部分の入力 HTML に、`<img src="name:part-name" />` を含めます。ここで、*part-name* は、バイナリ画像データを含む[マルチパート要求](onenote-create-page.md#example-request)のデータ部分の一意識別子です。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-143">In the input HTML of your request's **Presentation** part, include  `<img src="name:part-name" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary image data.</span></span> <span data-ttu-id="f4cb3-144">バイナリ データのみを送信するようにし、Base64 を使用したりエンコードしたりしないでください。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-144">Just send the binary data, don't use Base64 or otherwise encode it.</span></span>

```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: Image binary data</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page displays the uploaded image.</p>
    <img src="name:image-block-name" alt="a cool image" width="500"/>
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="MyAppPictureId"
Content-Type: image/jpeg

... image binary data ...

--MyAppPartBoundary--  
```


<a name="image-img-url-data-render-src"></a>

### <a name="add-a-webpage-snapshot"></a><span data-ttu-id="f4cb3-145">Web ページのスナップショットを追加する</span><span class="sxs-lookup"><span data-stu-id="f4cb3-145">Add a webpage snapshot</span></span>

<span data-ttu-id="f4cb3-146">Microsoft Graph を使用して、Web ページ全体のスナップショットを作成し、新しいページに挿入できます。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-146">You can use Microsoft Graph to snapshot entire webpages and insert them into new pages.</span></span> <span data-ttu-id="f4cb3-147">この方法は、Web ページのアーカイブや、(一部の CSS など) OneNote がサポートしない機能を持つ複雑な Web ページをキャプチャする場合に便利です。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-147">This method is useful to archive webpages or capture complex webpages that have features that OneNote doesn't support (like some CSS).</span></span>  

<span data-ttu-id="f4cb3-148">要求の入力 HTML では、`<img src="http://..." />` を含め、挿入する Web ページの URL を **src** 属性に指定します。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-148">In the input HTML of your request, include  `<img src="http://..." />` and specify the URL of the webpage you want to insert for the **src** attribute.</span></span>

```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: Webpage capture</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page displays an image of the webpage.</p>
    <img data-render-src="http://www.onenote.com" width="200"/>
  </body>
</html>

--MyAppPartBoundary--  
```


<a name="image-img-binary-data-render-src"></a>

### <a name="add-an-image-rendered-from-html"></a><span data-ttu-id="f4cb3-149">HTML から表示される画像を追加する</span><span class="sxs-lookup"><span data-stu-id="f4cb3-149">Add an image rendered from HTML</span></span>

<span data-ttu-id="f4cb3-150">データ ブロックとして HTML を追加する場合は、ユーザーの資格情報、または事前に読み込まれたブラウザー プラグインが必要となるアクティブ コンテンツがないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-150">When you pass the HTML as a data-block, be sure there is no active content that would require user credentials, or a pre-loaded browser plug-in.</span></span> <span data-ttu-id="f4cb3-151">Microsoft Graph が HTML ページを画像にレンダリングするために使用するエンジンには、ユーザーがログインする機能がなく、Adobe Flash、Apple QuickTime のようなプラグインは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-151">The engine that Microsoft Graph uses to render the HTML page into an image has no ability to log in a user, and doesn't include plug-ins like Adobe Flash, Apple QuickTime, and so-on.</span></span> <span data-ttu-id="f4cb3-152">これはつまり、データの取得にユーザーのログイン資格情報または Cookie が必要な場合、AJAX スクリプトで使用されるような動的に読み込まれるコンテンツが表示されないということです。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-152">That also means that dynamically-loaded content, like might come with an AJAX script, won't appear if getting the data requires user login credentials or cookies.</span></span>

<span data-ttu-id="f4cb3-153">要求の **Presentation** 部分の入力 HTML に、`<img data-render-src="name:part-name" />` を含めます。ここで、*part-name* は、HTML を含む[マルチパート要求](onenote-create-page.md#example-request)のデータ部分の一意識別子です。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-153">In the input HTML of your request's **Presentation** part, include  `<img data-render-src="name:part-name" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the HTML.</span></span>


```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: HTML block</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page displays the block of HTML as an image.</p>
    <img data-render-src="name:html-block-name" alt="a cool image" width="500"/>
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="html-block-name"
Content-Type: text/html

<html>
<body>
<h1>This HTML will render as an image</h1>
<p><b>Don't</b> try to embed another <i>data-render-src</i> type-image inside the HTML part--
it won't work. Instead, use URL-based real images like this:</p>
<img src="http://cdn.onenote.net/1664161560_Images/OneNote.ico" />
</body>
</html>

--MyAppPartBoundary--  
```


<a name="image-object"></a>

### <a name="add-an-image-file-as-an-attachment"></a><span data-ttu-id="f4cb3-154">添付ファイルとして画像ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="f4cb3-154">Add an image file as an attachment</span></span>

<span data-ttu-id="f4cb3-155">要求の **Presentation** 部分の入力 HTML に、`<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />` を含めます。ここで、*part-name* は、バイナリ画像データを含む[マルチパート要求](onenote-create-page.md#example-request)のデータ部分の一意識別子です。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-155">In the input HTML of your request's **Presentation** part, include  `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary image data.</span></span> <span data-ttu-id="f4cb3-156">バイナリ データのみを送信するようにし、Base64 を使用したりエンコードしたりしないでください。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-156">Just send the binary data, don't use Base64 or otherwise encode it.</span></span>

```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: Binary image data as file attachment</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page contains the image as a file attachment.</p>
    <object data-attachment="image-file.jpg" data="name:image-block-name" type="image/jpeg" />
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="logo1-file"
Content-Type: image/jpeg

... binary file data ...

--MyAppPartBoundary--
```

<span data-ttu-id="f4cb3-157">[ファイルのメディア タイプ](#file-media-types)について説明します。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-157">Learn more about [file media types](#file-media-types).</span></span>



<a name="adding-videos"></a>

## <a name="adding-videos"></a><span data-ttu-id="f4cb3-158">ビデオを追加する</span><span class="sxs-lookup"><span data-stu-id="f4cb3-158">Adding videos</span></span>

<span data-ttu-id="f4cb3-159">入力 HTML の `<iframe data-original-src="http://..." />` を使用して、OneNote ページにビデオを埋め込むことができます。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-159">You can embed videos in OneNote pages using `<iframe data-original-src="http://..." />` in the input HTML.</span></span> 

### <a name="supported-video-sites"></a><span data-ttu-id="f4cb3-160">サポートされるビデオ サイト</span><span class="sxs-lookup"><span data-stu-id="f4cb3-160">Supported video sites</span></span>

- <span data-ttu-id="f4cb3-161">Dailymotion</span><span class="sxs-lookup"><span data-stu-id="f4cb3-161">Dailymotion</span></span>
- <span data-ttu-id="f4cb3-162">Office Mix</span><span class="sxs-lookup"><span data-stu-id="f4cb3-162">Office Mix</span></span>
- <span data-ttu-id="f4cb3-163">Sway</span><span class="sxs-lookup"><span data-stu-id="f4cb3-163">Sway</span></span>
- <span data-ttu-id="f4cb3-164">Sketchfab</span><span class="sxs-lookup"><span data-stu-id="f4cb3-164">Sketchfab</span></span>
- <span data-ttu-id="f4cb3-165">TED</span><span class="sxs-lookup"><span data-stu-id="f4cb3-165">TED</span></span>
- <span data-ttu-id="f4cb3-166">YouTube</span><span class="sxs-lookup"><span data-stu-id="f4cb3-166">YouTube</span></span>
- <span data-ttu-id="f4cb3-167">Vimeo</span><span class="sxs-lookup"><span data-stu-id="f4cb3-167">Vimeo</span></span>
- <span data-ttu-id="f4cb3-168">Vine</span><span class="sxs-lookup"><span data-stu-id="f4cb3-168">Vine</span></span>

### <a name="iframe-attributes"></a><span data-ttu-id="f4cb3-169">iframe の属性</span><span class="sxs-lookup"><span data-stu-id="f4cb3-169">iframe attributes</span></span>

#### <a name="data-original-src"></a><span data-ttu-id="f4cb3-170">data-original-src</span><span class="sxs-lookup"><span data-stu-id="f4cb3-170">data-original-src</span></span>

<span data-ttu-id="f4cb3-p115">必須です。ビデオの URL。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-p115">Required. The URL of the video.</span></span>

<span data-ttu-id="f4cb3-173">例: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span><span class="sxs-lookup"><span data-stu-id="f4cb3-173">Example: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span></span>

#### <a name="width"></a><span data-ttu-id="f4cb3-174">width</span><span class="sxs-lookup"><span data-stu-id="f4cb3-174">width</span></span>

<span data-ttu-id="f4cb3-p116">省略可能。ビデオを含む iframe の幅。既定値は 480 です。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-p116">Optional. The width of the iframe that contains the video. Default is 480.</span></span>

<span data-ttu-id="f4cb3-178">例: `width="300"`</span><span class="sxs-lookup"><span data-stu-id="f4cb3-178">Example: `width="300"`</span></span>

#### <a name="height"></a><span data-ttu-id="f4cb3-179">height</span><span class="sxs-lookup"><span data-stu-id="f4cb3-179">height</span></span>

<span data-ttu-id="f4cb3-p117">省略可能。ビデオを含む iframe の高さ。既定値は 360 です。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-p117">Optional. The height of the iframe that contains the video. Default is 360.</span></span>

<span data-ttu-id="f4cb3-183">例: `height="300"`</span><span class="sxs-lookup"><span data-stu-id="f4cb3-183">Example: `height="300"`</span></span>

### <a name="example"></a><span data-ttu-id="f4cb3-184">例</span><span class="sxs-lookup"><span data-stu-id="f4cb3-184">Example</span></span>

<span data-ttu-id="f4cb3-185">要求の入力 HTML では、`<iframe data-original-src="http://..." />` を含め、**data-original-src** 属性のビデオの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-185">In the input HTML of your request, include `<iframe data-original-src="http://..." />` and specify the URL of the video for the **data-original-src** attribute.</span></span>

```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
    <head>
        <title>A page with an embedded video</title>
    </head>
    <body>
        <iframe data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8" width="340" height="280"/>
    </body>
</html>

--MyAppPartBoundary--
```


<a name="adding-files"></a>

## <a name="adding-files"></a><span data-ttu-id="f4cb3-186">ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="f4cb3-186">Adding files</span></span>

<span data-ttu-id="f4cb3-p118">入力 HTML の **object** 要素を使用して、添付ファイルを OneNote ページに追加できます。PDF ファイルを追加している場合は、**img** 要素を使用して、PDF ページを画像として表示できます。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-p118">You can add file attachments to OneNote pages using an **object** element in the input HTML. If you're adding a PDF file, you can use an **img** element to render the PDF pages as images.</span></span> 

[<span data-ttu-id="f4cb3-189">添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="f4cb3-189">Add a file attachment</span></span>](#add-a-file-attachment)

<span data-ttu-id="f4cb3-190">`<object .../>`を使用します。マルチパート要求のデータ部分でファイルを送信します。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-190">Use `<object .../>` and send the file in a data part of a multipart request.</span></span> <span data-ttu-id="f4cb3-191">OneNote ページでファイル アイコンを表示する添付ファイルを追加します。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-191">Adds a file attachment that displays a file icon on the OneNote page.</span></span>

[<span data-ttu-id="f4cb3-192">PDF ファイルのコンテンツの画像を追加する</span><span class="sxs-lookup"><span data-stu-id="f4cb3-192">Add images of PDF file contents</span></span>](#add-images-of-pdf-file-contents)

<span data-ttu-id="f4cb3-193">`<img data-render-src="name:part-name" />`を使用します。マルチパート要求のデータ部分で PDF ファイルを送信します。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-193">Use `<img data-render-src="name:part-name" />` and send a PDF file in the data part of a multipart request.</span></span> <span data-ttu-id="f4cb3-194">OneNote ページの個別の画像として、PDF の各ページを表示します。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-194">Renders each PDF page as a separate image on the OneNote page.</span></span>

#### <a name="file-attributes"></a><span data-ttu-id="f4cb3-195">ファイルの属性</span><span class="sxs-lookup"><span data-stu-id="f4cb3-195">File attributes</span></span>

<span data-ttu-id="f4cb3-196">**object** 要素には、次の属性が必要です。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-196">The **object** element requires the following attributes.</span></span>

<span data-ttu-id="f4cb3-197">**data-attachment**</span><span class="sxs-lookup"><span data-stu-id="f4cb3-197">**data-attachment**</span></span>

<span data-ttu-id="f4cb3-198">OneNote ページで表示するファイル名と拡張子。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-198">The file name and extension to display on the OneNote page.</span></span>

<span data-ttu-id="f4cb3-199">例: `data-attachment="filename.docx"`</span><span class="sxs-lookup"><span data-stu-id="f4cb3-199">Example: `data-attachment="filename.docx"`</span></span>

<span data-ttu-id="f4cb3-200">**data**</span><span class="sxs-lookup"><span data-stu-id="f4cb3-200">**data**</span></span>

<span data-ttu-id="f4cb3-201">バイナリ ファイルのデータを含むマルチパート要求のボディ部の名前。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-201">The name of the body part in the multipart request that contains the binary file data.</span></span> <span data-ttu-id="f4cb3-202">Microsoft Graph は、ここでの URL 参照の受け渡しはサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-202">Microsoft Graph does not support passing a URL reference here.</span></span>

<span data-ttu-id="f4cb3-203">例: `data="name:part-name"`</span><span class="sxs-lookup"><span data-stu-id="f4cb3-203">Example: `data="name:part-name"`</span></span>

<span data-ttu-id="f4cb3-204">**type**</span><span class="sxs-lookup"><span data-stu-id="f4cb3-204">**type**</span></span>

<span data-ttu-id="f4cb3-205">ファイルのメディア タイプ。ページで利用するファイル アイコンの決定に使用されます。また、ユーザーが OneNote からデバイス上のファイルをアクティブ化する際に開始されるアプリケーションを決定します。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-205">The file media type, used to determine the file icon to use on the page, and which application starts when the user activates the file on the device from OneNote.</span></span>

<span data-ttu-id="f4cb3-206">例: `type="application/pdf"`</span><span class="sxs-lookup"><span data-stu-id="f4cb3-206">Example: `type="application/pdf"`</span></span>


<a name="file-media-types"></a>

#### <a name="file-media-types"></a><span data-ttu-id="f4cb3-207">ファイルのメディア タイプ</span><span class="sxs-lookup"><span data-stu-id="f4cb3-207">File media types</span></span>  

<span data-ttu-id="f4cb3-208">Microsoft Graph は、添付ファイルの定義済みのファイル タイプのアイコンを使用し、API がファイル タイプを認識しない場合は汎用のアイコンを使用します。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-208">Microsoft Graph uses predefined file-types icon for attached files, or a generic icon when the API doesn't recognize the file type.</span></span> <span data-ttu-id="f4cb3-209">API によって認識されている一般的なファイル タイプのいくつかを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-209">The following table shows some common file types that are recognized by the API.</span></span>

- <span data-ttu-id="f4cb3-210">application/pdf</span><span class="sxs-lookup"><span data-stu-id="f4cb3-210">application/pdf</span></span>  
- <span data-ttu-id="f4cb3-211">application/vnd.openxmlformats-officedocument.wordprocessingml.document</span><span class="sxs-lookup"><span data-stu-id="f4cb3-211">application/vnd.openxmlformats-officedocument.wordprocessingml.document</span></span>  
- <span data-ttu-id="f4cb3-212">application/vnd.openxmlformats-officedocument.presentationml.presentation</span><span class="sxs-lookup"><span data-stu-id="f4cb3-212">application/vnd.openxmlformats-officedocument.presentationml.presentation</span></span>
- <span data-ttu-id="f4cb3-213">application/vnd.openxmlformats-officedocument.spreadsheetml.sheet</span><span class="sxs-lookup"><span data-stu-id="f4cb3-213">application/vnd.openxmlformats-officedocument.spreadsheetml.sheet</span></span>
- <span data-ttu-id="f4cb3-214">image/png</span><span class="sxs-lookup"><span data-stu-id="f4cb3-214">image/png</span></span>
- <span data-ttu-id="f4cb3-215">image/jpeg</span><span class="sxs-lookup"><span data-stu-id="f4cb3-215">image/jpeg</span></span>
- <span data-ttu-id="f4cb3-216">image/gif</span><span class="sxs-lookup"><span data-stu-id="f4cb3-216">image/gif</span></span>
- <span data-ttu-id="f4cb3-217">audio/wav</span><span class="sxs-lookup"><span data-stu-id="f4cb3-217">audio/wav</span></span>
- <span data-ttu-id="f4cb3-218">video/mp4</span><span class="sxs-lookup"><span data-stu-id="f4cb3-218">video/mp4</span></span>
- <span data-ttu-id="f4cb3-219">application/msword</span><span class="sxs-lookup"><span data-stu-id="f4cb3-219">application/msword</span></span>
- <span data-ttu-id="f4cb3-220">application/mspowerpoint</span><span class="sxs-lookup"><span data-stu-id="f4cb3-220">application/mspowerpoint</span></span>
- <span data-ttu-id="f4cb3-221">application/excel</span><span class="sxs-lookup"><span data-stu-id="f4cb3-221">application/excel</span></span>

<span data-ttu-id="f4cb3-222">メディアを含むページを作成する場合に適用する[制限](#size-limitations-for-post-pages-requests)を確認してください。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-222">See [limitations](#size-limitations-for-post-pages-requests) that apply when creating pages that contain media.</span></span>


<a name="file-object"></a>

### <a name="add-a-file-attachment"></a><span data-ttu-id="f4cb3-223">添付ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="f4cb3-223">Add a file attachment</span></span>

<span data-ttu-id="f4cb3-224">要求の **Presentation** 部分の入力 HTML に、`<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />` を含めます。ここで、*part-name* は、バイナリ ファイルのデータを含む[マルチパート要求](onenote-create-page.md#example-request)のデータ部分の一意識別子です。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-224">In the input HTML of your request's **Presentation** part, include  `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary file data.</span></span> <span data-ttu-id="f4cb3-225">バイナリ データのみを送信するようにし、Base64 を使用したりエンコードしたりしないでください。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-225">Just send the binary data, don't use Base64 or otherwise encode it.</span></span>

```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image file attachment</title>
  </head>
  <body>
    <p>This is an image file attachment.</p>
    <object data-attachment="Logo.jpg" data="name:logo1-file" type="image/jpeg" />
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="logo1-file"
Content-Type: image/jpeg

... binary file data ...

--MyAppPartBoundary--
```


<a name="file-binary-data-render-src"></a>

### <a name="add-images-of-pdf-file-contents"></a><span data-ttu-id="f4cb3-226">PDF ファイルのコンテンツの画像を追加する</span><span class="sxs-lookup"><span data-stu-id="f4cb3-226">Add images of PDF file contents</span></span>

<span data-ttu-id="f4cb3-227">要求の **Presentation** 部分の入力 HTML に、`<img data-render-src="name:part-name" ... />` を含めます。ここで、*part-name* は、バイナリ ファイルのデータを含む[マルチパート要求](onenote-create-page.md#example-request)のデータ部分の一意識別子です。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-227">In the input HTML of your request's **Presentation** part, include  `<img data-render-src="name:part-name" ... />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary file data.</span></span> <span data-ttu-id="f4cb3-228">バイナリ データのみを送信するようにし、Base64 を使用したりエンコードしたりしないでください。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-228">Just send the binary data, don't use Base64 or otherwise encode it.</span></span>

```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with images of the pages of a PDF file</title>
  </head>
  <body>
    <p>The pages of this PDF file render as images.</p>
    <img data-render-src="name:file-part" alt="PDF file as images" width="500"/>
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="file-part"
Content-Type: application/pdf

... binary file data ...

--MyAppPartBoundary--  
```


<a name="size-limits"></a>

## <a name="size-limitations-for-post-pages-requests"></a><span data-ttu-id="f4cb3-229">POST pages 要求のサイズの上限</span><span class="sxs-lookup"><span data-stu-id="f4cb3-229">Size limitations for POST pages requests</span></span>

<span data-ttu-id="f4cb3-230">画像やファイルのデータを送信する場合は、これらの制限に注意してください: <!--TODO: check these--></span><span class="sxs-lookup"><span data-stu-id="f4cb3-230">When sending image and file data, be aware of these limitations: <!--TODO: check these--></span></span>

- <span data-ttu-id="f4cb3-p125">合計 POST サイズの上限は 70 MB までであり、画像、ファイル、その他のデータが含まれます。実際の上限はダウンストリームのエンコーディングに影響されるため、固定のバイト数の制限はありません。上限を超える要求は、信頼性の低い結果になる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-p125">The total POST size limit is ~70 MB, including images, files, and other data. The actual limit is affected by downstream encoding, so there's no fixed byte-count limit. Requests that exceed the limit may produce unreliable results.</span></span>

- <span data-ttu-id="f4cb3-234">各データ部分の上限は、part ヘッダーを含めて 25 MB です。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-234">The limit for each data part is 25 MB, including the part headers.</span></span> <span data-ttu-id="f4cb3-235">上限を超えるデータ部分は、Microsoft Graph によって拒否されます。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-235">Data parts that exceed the limit are rejected by Microsoft Graph.</span></span> 

- <span data-ttu-id="f4cb3-p127">1 ページあたりの画像の最大数は 150 です。`src="http://..."` 属性を使用する場合、API は上限を超えた **img** タグを無視します。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-p127">The maximum number of images per page is 150. When using the `src="http://..."` attribute, the API ignores **img** tags beyond the limit.</span></span>

- <span data-ttu-id="f4cb3-238">データ部分の最大数は、必須の **Presentation** パートを含めて 1 POST あたり 6 です。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-238">The maximum number of data parts is 6 per POST, including the required **Presentation** part.</span></span>

- <span data-ttu-id="f4cb3-239">各要求は、**data-render-src** を使用する **img** 要素を最大で 5 つ、**data-render-src** を使用する **object** 要素を 1 つ含めることができます。追加の画像とファイルの参照は無視されます。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-239">Each request can contain up to five **img** elements that use **data-render-src** and one **object** elements that uses **data-render-src**. Additional image and file references are ignored.</span></span>

- <span data-ttu-id="f4cb3-p128">API への送信に使用する方法に関係なく、単一の POST 内の画像の最大数は 30 です。追加の画像は無視されます。多数の画像を含む Web ページをキャプチャする場合は、[スナップショットとしてページ全体をキャプチャする](#add-a-webpage-snapshot)ことを検討してください。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-p128">The maximum number of images in a single POST is 30, no matter which method you use to send them to the API. Additional images are ignored. If you want to capture a webpage that contains a lot of images, consider [capturing the whole page as a snapshot](#add-a-webpage-snapshot).</span></span>


## <a name="when-to-use-html-versus-data-render-src"></a><span data-ttu-id="f4cb3-243">HTML を使用する場合と data-render-src を使用する場合</span><span class="sxs-lookup"><span data-stu-id="f4cb3-243">When to use HTML versus data-render-src</span></span> 

<span data-ttu-id="f4cb3-244">HTML を OneNote ページに直接配置するか、**data-render-src** 属性を使用するかを検討している場合、以下を考慮してください。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-244">When trying to decide between putting HTML directly onto the OneNote page instead of using the **data-render-src** attribute, consider the following:</span></span>

- <span data-ttu-id="f4cb3-245">複雑な HTML は、Microsoft Graph が受け入れることができるように HTML を変更するよりも、**data-render-src** を使用してレンダリング エンジンに送信する方がおそらく適しています。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-245">Complex HTML is probably best sent to the rendering engine via **data-render-src**, rather than attempting to modify the HTML to fit into what Microsoft Graph can accept.</span></span> <span data-ttu-id="f4cb3-246">これは、サポートされていないタグが HTML に含まれている場合にも当てはまります。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-246">This is also true when your HTML includes tags that aren't supported supported.</span></span>

- <span data-ttu-id="f4cb3-247">ページのレイアウトや外観を保持する正確なページ レンダリングは、**data-render-src** を使用してレンダリング エンジンを使用する方法が最適かもしれません。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-247">Accurate page rendering to preserve the layout and look of the page is probably best done with the rendering engine via **data-render-src**.</span></span>

- <span data-ttu-id="f4cb3-p130">直接編集可能なテキストは、多くの場合 HTML をページに直接挿入する方法が適しています。表示された画像は、光学式文字認識 (OCR) システムによってスキャンされますが、これは同じではありません。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-p130">Directly-editable text is often best done with inserting the HTML directly onto the page. The rendered images are scanned by an optical character recognition (OCR) system, but it's just not the same.</span></span>

- <span data-ttu-id="f4cb3-250">履歴またはアーカイブのためのスナップショット イン タイムには、通常 **data-render-src** メソッドが最も適しています。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-250">Snapshot-in-time for historical or archival purposes is usually best done with the data-render-src method.</span></span>

- <span data-ttu-id="f4cb3-p131">改訂するための Web ページ設計のマークアップは、**data-render-src** が真価を発揮する分野です。OneNote のインク機能を使用して、変更箇所を示すためイメージ上に描画したり、重要な場所をコールアウトすることができます。Web ページをイメージにすることにより、これらがより簡単になります。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-p131">Marking-up a web page design for revisions is one place the **data-render-src** truly shines. Using OneNote's inking capabilities, you can draw on the image to indicate changes or call out important areas. Having the web page as an image makes that a lot easier.</span></span>

- <span data-ttu-id="f4cb3-254">非常に大きい画像、または OneNote が直接受け入れない形式の画像は、**data-render-src** 属性を使用すると、独自のコードで行うよりも容易にサムネイル化し変換できる場合があります。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-254">Very large images, or images in formats that OneNote doesn't directly accept can sometimes be thumbnailed and converted with the **data-render-src** attribure more easily than by doing it in your own code.</span></span> <span data-ttu-id="f4cb3-255">画像がオンラインでも利用できる場合でも、POST にデータを埋め込むことで、OneNote ページの構築に必要なラウンドトリップの合計数を減らし、キャプチャしたページを OneNote ユーザーがすぐに利用できるようになる場合があります。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-255">Even if the image is also available onlinet, embedding the data in your POST can sometimes make the captured page available to OneNote user sooner, by reducing the total number of round-trips needed to build the OneNote page.</span></span>

<span data-ttu-id="f4cb3-256">ユーザーにどの方法が最適かを判断するのに、アプリを開発する際に両方の方法を試してみることが最善の場合があります。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-256">Sometimes, the best way to determine which method will work best for your users is to try it both ways as you develop your app.</span></span>


<a name="permissions"></a>

## <a name="permissions"></a><span data-ttu-id="f4cb3-257">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f4cb3-257">Permissions</span></span>

<span data-ttu-id="f4cb3-p133">OneNote ページを作成または更新するには、適切なアクセス許可を要求する必要があります。アプリの動作に必要な最低限のアクセス許可を選択してください。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-p133">To create or update OneNote pages, you'll need to request appropriate permissions. Choose the lowest level that your app needs to do its work.</span></span>

#### <a name="permissions-for-post-pages"></a><span data-ttu-id="f4cb3-260">POST ページのアクセス許可</span><span class="sxs-lookup"><span data-stu-id="f4cb3-260">Permissions for POST pages</span></span>

- <span data-ttu-id="f4cb3-261">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="f4cb3-261">Notes.Create</span></span>
- <span data-ttu-id="f4cb3-262">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f4cb3-262">Notes.ReadWrite</span></span>
- <span data-ttu-id="f4cb3-263">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4cb3-263">Notes.ReadWrite.All</span></span> 

#### <a name="permissions-for-patch-pages"></a><span data-ttu-id="f4cb3-264">PATCH ページのアクセス許可</span><span class="sxs-lookup"><span data-stu-id="f4cb3-264">Permissions for PATCH pages</span></span>

- <span data-ttu-id="f4cb3-265">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f4cb3-265">Notes.ReadWrite</span></span>
- <span data-ttu-id="f4cb3-266">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4cb3-266">Notes.ReadWrite.All</span></span>

<span data-ttu-id="f4cb3-267">アクセス許可のスコープと動作のしくみの詳細については、「[OneNote のアクセス許可のスコープ](permissions_reference.md#notes-permissions)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="f4cb3-267">For more information about permission scopes and how they work, see [OneNote permission scopes](permissions_reference.md#notes-permissions).</span></span>


<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="f4cb3-268">関連項目</span><span class="sxs-lookup"><span data-stu-id="f4cb3-268">See also</span></span>

- [<span data-ttu-id="f4cb3-269">OneNote との統合</span><span class="sxs-lookup"><span data-stu-id="f4cb3-269">Integrate with OneNote</span></span>](integrate_with_onenote.md)
- [<span data-ttu-id="f4cb3-270">OneNote の開発者ブログ</span><span class="sxs-lookup"><span data-stu-id="f4cb3-270">OneNote Developer Blog</span></span>](http://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="f4cb3-271">Stack Overflow 掲載の OneNote の開発に関する質問</span><span class="sxs-lookup"><span data-stu-id="f4cb3-271">OneNote development questions on Stack Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="f4cb3-272">OneNote GitHub のリポジトリ</span><span class="sxs-lookup"><span data-stu-id="f4cb3-272">OneNote GitHub repos</span></span>](http://go.microsoft.com/fwlink/?LinkID=390178)  
