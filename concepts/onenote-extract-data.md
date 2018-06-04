# <a name="use-onenote-api-div-tags-to-extract-data-from-captures"></a><span data-ttu-id="6a183-101">OneNote API div タグを使用してキャプチャからデータを抽出する</span><span class="sxs-lookup"><span data-stu-id="6a183-101">Use OneNote API div tags to extract data from captures</span></span> 

<span data-ttu-id="6a183-102">*__適用対象:__ OneDrive のコンシューマー ノートブック | Office 365 のエンタープライズ ノートブック*</span><span class="sxs-lookup"><span data-stu-id="6a183-102">*__Applies to:__ Consumer notebooks on OneDrive | Enterprise notebooks on Office 365*</span></span>

<span data-ttu-id="6a183-103">OneNote API を使用して、画像から名刺データを抽出したり、URL からレシピや製品データを抽出したりします。</span><span class="sxs-lookup"><span data-stu-id="6a183-103">Use the OneNote API to extract business card data from an image, or recipe and product data from a URL.</span></span>

<a name="attributes"></a>
## <a name="extraction-attributes"></a><span data-ttu-id="6a183-104">抽出の属性</span><span class="sxs-lookup"><span data-stu-id="6a183-104">Extraction attributes</span></span>

<span data-ttu-id="6a183-105">単に div を含めるだけで、データの抽出や変換ができます。div は [create-page](onenote-create-page.md) または [update-page](onenote_update_page.md) 要求で、ソース コンテンツ、抽出メソッド、およびフォールバックの動作を指定します。</span><span class="sxs-lookup"><span data-stu-id="6a183-105">To extract and transform data, simply include a div that specifies the source content, extraction method, and fallback behavior in your [create-page](onenote-create-page.md) or [update-page](onenote_update_page.md) request.</span></span> <span data-ttu-id="6a183-106">API は抽出したデータを、読みやすい形式でページに表示します。</span><span class="sxs-lookup"><span data-stu-id="6a183-106">The API renders extracted data on the page in an easy-to-read format.</span></span> 

```
<div
  data-render-src="image-or-url"
  data-render-method="extraction-method"
  data-render-fallback="fallback-action">
</div>
```

<span data-ttu-id="6a183-107">**data-render-src**</span><span class="sxs-lookup"><span data-stu-id="6a183-107">**data-render-src**</span></span>

<span data-ttu-id="6a183-p102">コンテンツ ソース。名刺の画像、または数多くの人気レシピや製品の Web サイトの絶対 URL にできます。必須。</span><span class="sxs-lookup"><span data-stu-id="6a183-p102">The content source. This can be an image of a business card or an absolute URL from many popular recipe or product websites. Required.</span></span>

<span data-ttu-id="6a183-p103">URL を指定するときに最適な結果を得るために、ソースの Web ページの HTML で定義された正規 URL を使用してください (定義されている場合)。たとえば、正規 URL はソースの Web ページで次のように定義されます。</span><span class="sxs-lookup"><span data-stu-id="6a183-p103">For best results when specifying a URL, use the canonical URL defined in the HTML of the source webpage, if one is defined. For example, a canonical URL might be defined in the source webpage like this:</span></span>

`<link rel="canonical" href="www.domainname.com/page/123/size12/type987" />` 


<span data-ttu-id="6a183-113">**data-render-method**</span><span class="sxs-lookup"><span data-stu-id="6a183-113">**data-render-method**</span></span>

<span data-ttu-id="6a183-p104">実行する抽出メソッド。必須。</span><span class="sxs-lookup"><span data-stu-id="6a183-p104">The extraction method to run. Required.</span></span>

| <span data-ttu-id="6a183-116">値</span><span class="sxs-lookup"><span data-stu-id="6a183-116">Value</span></span> | <span data-ttu-id="6a183-117">説明</span><span class="sxs-lookup"><span data-stu-id="6a183-117">Description</span></span> |
|:------|:------|
| <span data-ttu-id="6a183-118">extract.businesscard</span><span class="sxs-lookup"><span data-stu-id="6a183-118">extract.businesscard</span></span> | <span data-ttu-id="6a183-119">名刺の抽出。</span><span class="sxs-lookup"><span data-stu-id="6a183-119">A business card extraction.</span></span> |
| <span data-ttu-id="6a183-120">extract.recipe</span><span class="sxs-lookup"><span data-stu-id="6a183-120">extract.recipe</span></span> | <span data-ttu-id="6a183-121">レシピの抽出。</span><span class="sxs-lookup"><span data-stu-id="6a183-121">A recipe extraction.</span></span> |
| <span data-ttu-id="6a183-122">extract.product</span><span class="sxs-lookup"><span data-stu-id="6a183-122">extract.product</span></span> | <span data-ttu-id="6a183-123">製品リストの抽出。</span><span class="sxs-lookup"><span data-stu-id="6a183-123">A product listing extraction.</span></span> |
| <span data-ttu-id="6a183-124">extract</span><span class="sxs-lookup"><span data-stu-id="6a183-124">extract</span></span> | <span data-ttu-id="6a183-125">不明な種類の抽出。</span><span class="sxs-lookup"><span data-stu-id="6a183-125">An unknown extraction type.</span></span> |

<span data-ttu-id="6a183-126">最適の結果を得るために、コンテンツの種類 (`extract.businesscard`、`extract.recipe`、または `extract.product`) を指定してください (種類がわかっている場合)。</span><span class="sxs-lookup"><span data-stu-id="6a183-126">For best results, specify the content type (`extract.businesscard`, `extract.recipe`, or `extract.product`) if you know it.</span></span> <span data-ttu-id="6a183-127">種類が不明の場合は、`extract` メソッドを使用してください。OneNote API は種類の自動検出を試行するようになります。</span><span class="sxs-lookup"><span data-stu-id="6a183-127">If the type is unknown, use the `extract` method and the OneNote API will try to auto-detect the type.</span></span>

<span data-ttu-id="6a183-128">**data-render-fallback**</span><span class="sxs-lookup"><span data-stu-id="6a183-128">**data-render-fallback**</span></span>

<span data-ttu-id="6a183-129">抽出できない場合のフォールバック動作。</span><span class="sxs-lookup"><span data-stu-id="6a183-129">The fallback behavior if the extraction fails.</span></span> <span data-ttu-id="6a183-130">省略すると、既定の **render** になります。</span><span class="sxs-lookup"><span data-stu-id="6a183-130">Defaults to **render** if omitted.</span></span> 

| <span data-ttu-id="6a183-131">値</span><span class="sxs-lookup"><span data-stu-id="6a183-131">Value</span></span> | <span data-ttu-id="6a183-132">説明</span><span class="sxs-lookup"><span data-stu-id="6a183-132">Description</span></span> |
|:------|:------|
| <span data-ttu-id="6a183-133">render</span><span class="sxs-lookup"><span data-stu-id="6a183-133">render</span></span> | <span data-ttu-id="6a183-134">レシピまたは製品の Web ページのソース画像またはスナップショットを表示します。</span><span class="sxs-lookup"><span data-stu-id="6a183-134">Renders the source image or a snapshot of the recipe or product webpage.</span></span> |
| <span data-ttu-id="6a183-135">none</span><span class="sxs-lookup"><span data-stu-id="6a183-135">none</span></span> | <span data-ttu-id="6a183-136">何も実行しません。</span><span class="sxs-lookup"><span data-stu-id="6a183-136">Does nothing.</span></span><br /><span data-ttu-id="6a183-137">このオプションは、抽出コンテンツに加えて、名刺または Web ページのスナップショットをページに必ず含める場合に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="6a183-137">This option is useful if you want to always include a snapshot of the business card or webpage on the page in addition to any extracted content.</span></span> <span data-ttu-id="6a183-138">例に示すように、要求には個別の `img` 要素を含めてください。</span><span class="sxs-lookup"><span data-stu-id="6a183-138">Be sure to send a separate `img` element in the request, as shown in the examples.</span></span> |

<a name="biz-card"></a>
## <a name="business-card-extractions"></a><span data-ttu-id="6a183-139">名刺の抽出</span><span class="sxs-lookup"><span data-stu-id="6a183-139">Business card extractions</span></span>

<span data-ttu-id="6a183-140">OneNote API は、個人または会社の名刺の画像に基づいて、次の連絡先情報の検索および表示を試行します。</span><span class="sxs-lookup"><span data-stu-id="6a183-140">The OneNote API tries to find and render the following contact information based on an image of a person's or company's business card.</span></span>


- <span data-ttu-id="6a183-141">名前</span><span class="sxs-lookup"><span data-stu-id="6a183-141">Name</span></span>
- <span data-ttu-id="6a183-142">タイトル</span><span class="sxs-lookup"><span data-stu-id="6a183-142">Title</span></span>
- <span data-ttu-id="6a183-143">組織</span><span class="sxs-lookup"><span data-stu-id="6a183-143">Organization</span></span>
- <span data-ttu-id="6a183-144">電話および FAX 番号</span><span class="sxs-lookup"><span data-stu-id="6a183-144">Phone and fax numbers</span></span>
- <span data-ttu-id="6a183-145">郵送先および実際の住所</span><span class="sxs-lookup"><span data-stu-id="6a183-145">Mailing and physical addresses</span></span>
- <span data-ttu-id="6a183-146">電子メール アドレス</span><span class="sxs-lookup"><span data-stu-id="6a183-146">Email addresses</span></span>
- <span data-ttu-id="6a183-147">Web サイト</span><span class="sxs-lookup"><span data-stu-id="6a183-147">Websites</span></span>
   
  ![名刺抽出の例。](images/biz-card-extraction.png)

<span data-ttu-id="6a183-p108">ページには、抽出された連絡先情報が含まれる vCard (.VCF ファイル) も組み込まれます。この vCard は、ページの HTML コンテンツを取得するときに連絡先情報を入手するのに便利な方法です。</span><span class="sxs-lookup"><span data-stu-id="6a183-p108">A vCard (.VCF file) with the extracted contact information is also embedded in the page. The vCard is a convenient way to get the contact information when retrieving page HTML content.</span></span>

### <a name="common-scenarios-for-business-card-extractions"></a><span data-ttu-id="6a183-151">名刺抽出の一般的なシナリオ</span><span class="sxs-lookup"><span data-stu-id="6a183-151">Common scenarios for business card extractions</span></span>

<span data-ttu-id="6a183-152">**名刺情報を抽出して、名刺の画像を表示する**</span><span class="sxs-lookup"><span data-stu-id="6a183-152">**Extract business card information, and also render the business card image**</span></span>

<span data-ttu-id="6a183-153">`extract.businesscard` メソッドと `none` フォールバックを指定します。</span><span class="sxs-lookup"><span data-stu-id="6a183-153">Specify the `extract.businesscard` method and the `none` fallback.</span></span> <span data-ttu-id="6a183-154">また、画像を参照する `src` 属性を含む `img` 要素も送信します。</span><span class="sxs-lookup"><span data-stu-id="6a183-154">Also send an `img` element with the `src` attribute that also references the image.</span></span> <span data-ttu-id="6a183-155">API ではコンテンツを抽出できない場合は、名刺の画像のみが表示されます。</span><span class="sxs-lookup"><span data-stu-id="6a183-155">If the API is unable to extract any content, it renders the business card image only.</span></span>

```html 
<div
    data-render-src="name:scanned-card-image"
    data-render-method="extract.businesscard"
    data-render-fallback="none">
</div>
<img src="name:scanned-card-image" />
```


<span data-ttu-id="6a183-156">**名刺情報を抽出して、抽出に失敗した場合のみ名刺の画像を表示する**</span><span class="sxs-lookup"><span data-stu-id="6a183-156">**Extract business card information, and render the business card image only if the extraction fails**</span></span>

<span data-ttu-id="6a183-157">`extract.businesscard` メソッドを指定して、既定の `render` フォールバックを使用します。</span><span class="sxs-lookup"><span data-stu-id="6a183-157">Specify the `extract.businesscard` method and use the default `render` fallback.</span></span> <span data-ttu-id="6a183-158">API ではコンテンツを抽出できない場合は、その代わりに名刺の画像が表示されます。</span><span class="sxs-lookup"><span data-stu-id="6a183-158">If the API is unable to extract any content, it renders the business card image instead.</span></span>

```html
<div
    data-render-src="name:scanned-card-image"
    data-render-method="extract.businesscard">
</div>
```
 
<span data-ttu-id="6a183-159">名刺の抽出では、画像はマルチパートの要求の名前付きパートとして送信されます。</span><span class="sxs-lookup"><span data-stu-id="6a183-159">For business card extractions, the image is sent as a named part in a multipart request.</span></span> <span data-ttu-id="6a183-160">要求で画像を送信する例については、「[画像とファイルの追加](onenote_images_files.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6a183-160">See [Add images and files](onenote_images_files.md) for examples that show how to send an image in a request.</span></span>


<a name="recipe"></a>
## <a name="recipe-extractions"></a><span data-ttu-id="6a183-161">レシピの抽出</span><span class="sxs-lookup"><span data-stu-id="6a183-161">Recipe extractions</span></span>

<span data-ttu-id="6a183-162">OneNote API は、レシピの URL に基づいて、次の情報の検索および表示を試行します。</span><span class="sxs-lookup"><span data-stu-id="6a183-162">The OneNote API tries to find and render the following information based on a recipe's URL.</span></span>

- <span data-ttu-id="6a183-163">完成例の画像</span><span class="sxs-lookup"><span data-stu-id="6a183-163">Hero image</span></span>
- <span data-ttu-id="6a183-164">評価</span><span class="sxs-lookup"><span data-stu-id="6a183-164">Rating</span></span>
- <span data-ttu-id="6a183-165">材料</span><span class="sxs-lookup"><span data-stu-id="6a183-165">Ingredients</span></span>
- <span data-ttu-id="6a183-166">手順</span><span class="sxs-lookup"><span data-stu-id="6a183-166">Instructions</span></span>
- <span data-ttu-id="6a183-167">準備、調理、および合計の時間</span><span class="sxs-lookup"><span data-stu-id="6a183-167">Prep, cook, and total times</span></span>
- <span data-ttu-id="6a183-168">分量</span><span class="sxs-lookup"><span data-stu-id="6a183-168">Servings</span></span>

   ![レシピの抽出例](images/recipe-extraction.png)

<span data-ttu-id="6a183-170">この API は、*Allrecipes.com*、*FoodNetwork.com*、および *SeriousEats.com* など、数多くの人気サイトのレシピ用に最適化されています。</span><span class="sxs-lookup"><span data-stu-id="6a183-170">The API is optimized for recipes from many popular sites such as *Allrecipes.com*, *FoodNetwork.com*, and *SeriousEats.com*.</span></span>

### <a name="common-scenarios-for-recipe-extractions"></a><span data-ttu-id="6a183-171">レシピ抽出の一般的なシナリオ</span><span class="sxs-lookup"><span data-stu-id="6a183-171">Common scenarios for recipe extractions</span></span>

<span data-ttu-id="6a183-172">**レシピ情報を抽出して、レシピの Web ページのスナップショットも表示する**</span><span class="sxs-lookup"><span data-stu-id="6a183-172">**Extract recipe information, and also render a snapshot of the recipe webpage**</span></span>

<span data-ttu-id="6a183-173">`extract.recipe` メソッドと `none` フォールバックを指定します。</span><span class="sxs-lookup"><span data-stu-id="6a183-173">Specify the `extract.recipe` method and the `none` fallback.</span></span> <span data-ttu-id="6a183-174">また、レシピの URL に設定した `data-render-src` 属性を含む `img` 要素も送信します。</span><span class="sxs-lookup"><span data-stu-id="6a183-174">Also send an `img` element with the `data-render-src` attribute set to the recipe URL.</span></span> <span data-ttu-id="6a183-175">API ではコンテンツを抽出できない場合は、レシピの Web ページのスナップショットのみが表示されます。</span><span class="sxs-lookup"><span data-stu-id="6a183-175">If the API is unable to extract any content, it renders a snapshot of the recipe webpage only.</span></span>

<span data-ttu-id="6a183-176">おそらく、このシナリオが最も多くの情報を提供することになります。Web ページには、お客様のレビューや提案などの追加情報が含まれている場合があるためです。</span><span class="sxs-lookup"><span data-stu-id="6a183-176">This scenario potentially provides the most information because the webpage may include additional information, such as customer reviews and suggestions.</span></span>

```html 
<div
    data-render-src="http://allrecipes.com/recipe/guacamole/"
    data-render-method="extract.recipe"
    data-render-fallback="none">
</div>
<img data-render-src="http://allrecipes.com/recipe/guacamole/" />
```
 

<span data-ttu-id="6a183-177">**レシピ情報を抽出して、抽出に失敗した場合にのみレシピの Web ページのスナップショットを表示する**</span><span class="sxs-lookup"><span data-stu-id="6a183-177">**Extract recipe information, and render a snapshot of the recipe webpage only if the extraction fails**</span></span>

<span data-ttu-id="6a183-178">`extract.recipe` メソッドを指定して、既定の render フォールバックを使用します。</span><span class="sxs-lookup"><span data-stu-id="6a183-178">Specify the `extract.recipe` method and use the default render fallback.</span></span> <span data-ttu-id="6a183-179">API ではコンテンツを抽出できない場合は、その代わりにレシピの Web ページのスナップショットが表示されます。</span><span class="sxs-lookup"><span data-stu-id="6a183-179">If the API is unable to extract any content, it renders a snapshot of the recipe webpage instead.</span></span>

```html  
<div
    data-render-src="http://www.foodnetwork.com/recipes/alton-brown/creme-brulee-recipe.html"
    data-render-method="extract.recipe">
</div>
```


<span data-ttu-id="6a183-180">**レシピ情報を抽出して、そのレシピへのリンクも表示する**</span><span class="sxs-lookup"><span data-stu-id="6a183-180">**Extract recipe information, and also render a link to the recipe**</span></span>

<span data-ttu-id="6a183-181">`extract.recipe` メソッドと `none` フォールバックを指定します。</span><span class="sxs-lookup"><span data-stu-id="6a183-181">Specify the `extract.recipe` method and the `none` fallback.</span></span> <span data-ttu-id="6a183-182">レシピの URL に設定された `src` 属性を含む `a` 要素も送信します (または、ページに追加するその他の情報を送信することもできます)。</span><span class="sxs-lookup"><span data-stu-id="6a183-182">Also send an `a` element with the `src` attribute set to the recipe URL (or you can send any other information you want to add to the page).</span></span> <span data-ttu-id="6a183-183">API ではコンテンツを抽出できない場合は、レシピのリンクのみが表示されます。</span><span class="sxs-lookup"><span data-stu-id="6a183-183">If the API is unable to extract any content, only the recipe link is rendered.</span></span>

```html  
<div
    data-render-src="http://www.seriouseats.com/recipes/2014/09/diy-spicy-kimchi-beef-instant-noodles-recipe.html"
    data-render-method="extract.recipe"
    data-render-fallback="none">
</div>
<a href="http://www.seriouseats.com/recipes/2014/09/diy-spicy-kimchi-beef-instant-noodles-recipe.html">Recipe URL</a>
``` 


<a name="product"></a>
## <a name="product-listing-extractions"></a><span data-ttu-id="6a183-184">製品リストの抽出</span><span class="sxs-lookup"><span data-stu-id="6a183-184">Product listing extractions</span></span>

- <span data-ttu-id="6a183-185">タイトル</span><span class="sxs-lookup"><span data-stu-id="6a183-185">Title</span></span>
- <span data-ttu-id="6a183-186">評価</span><span class="sxs-lookup"><span data-stu-id="6a183-186">Rating</span></span>
- <span data-ttu-id="6a183-187">主要画像</span><span class="sxs-lookup"><span data-stu-id="6a183-187">Primary image</span></span>
- <span data-ttu-id="6a183-188">説明</span><span class="sxs-lookup"><span data-stu-id="6a183-188">Description</span></span>
- <span data-ttu-id="6a183-189">機能</span><span class="sxs-lookup"><span data-stu-id="6a183-189">Features</span></span>
- <span data-ttu-id="6a183-190">仕様</span><span class="sxs-lookup"><span data-stu-id="6a183-190">Specifications</span></span></td>

  ![製品リスト抽出の例。](images/product-extraction.png)

<span data-ttu-id="6a183-192">この API は、*Amazon.com* や *HomeDepot.com* など、数多くの人気サイトの製品用に最適化されています。</span><span class="sxs-lookup"><span data-stu-id="6a183-192">The API is optimized for products from many popular sites such as *Amazon.com* and *HomeDepot.com*.</span></span>

### <a name="common-scenarios-for-recipe-extractions"></a><span data-ttu-id="6a183-193">レシピ抽出の一般的なシナリオ</span><span class="sxs-lookup"><span data-stu-id="6a183-193">Common scenarios for recipe extractions</span></span>

<span data-ttu-id="6a183-194">**製品情報を抽出して、製品の Web ページのスナップショットも表示する**</span><span class="sxs-lookup"><span data-stu-id="6a183-194">**Extract product information, and also render a snapshot of the product webpage**</span></span>

<span data-ttu-id="6a183-195">`extract.product` メソッドと `none` フォールバックを指定します。</span><span class="sxs-lookup"><span data-stu-id="6a183-195">Specify the `extract.product` method and the `none` fallback.</span></span> <span data-ttu-id="6a183-196">また、製品の URL に設定した `data-render-src` 属性を含む `img` 要素も送信します。</span><span class="sxs-lookup"><span data-stu-id="6a183-196">Also send an `img` element with the `data-render-src` attribute set to the product URL.</span></span> <span data-ttu-id="6a183-197">API ではコンテンツを抽出できない場合は、製品の Web ページのスナップショットのみが表示されます。</span><span class="sxs-lookup"><span data-stu-id="6a183-197">If the API is unable to extract any content, it renders a snapshot of the product webpage only.</span></span>

<span data-ttu-id="6a183-198">おそらく、このシナリオが最も多くの情報を提供することになります。Web ページには、お客様のレビューや提案などの追加情報が含まれている場合があるためです。</span><span class="sxs-lookup"><span data-stu-id="6a183-198">This scenario potentially provides the most information because the webpage may include additional information, such as customer reviews and suggestions.</span></span>

```html 
<div
    data-render-src="http://www.amazon.com/Microsoft-Band-Small/dp/B00P2T2WVO"
    data-render-method="extract.product"
    data-render-fallback="none">
</div>
<img data-render-src="http://www.amazon.com/Microsoft-Band-Small/dp/B00P2T2WVO" />
```


<span data-ttu-id="6a183-199">**製品情報を抽出して、抽出に失敗した場合のみ製品の Web ページのスナップショットも表示する**</span><span class="sxs-lookup"><span data-stu-id="6a183-199">**Extract product information, and render a snapshot of the product webpage only if the extraction fails**</span></span>

<span data-ttu-id="6a183-200">`extract.product` メソッドを指定して、既定の render フォールバックを使用します。</span><span class="sxs-lookup"><span data-stu-id="6a183-200">Specify the `extract.product` method and use the default render fallback.</span></span> <span data-ttu-id="6a183-201">API ではコンテンツを抽出できない場合は、その代わりに製品の Web ページのスナップショットが表示されます。</span><span class="sxs-lookup"><span data-stu-id="6a183-201">If the API is unable to extract any content, it renders a snapshot of the product webpage instead.</span></span>

```html 
<div
    data-render-src="http://www.sears.com/craftsman-19hp-42-8221-turn-tight-174-hydrostatic-yard-tractor/p-07120381000P"
    data-render-method="extract.product">
</div>
```
 

<span data-ttu-id="6a183-202">**製品情報を抽出して、その製品へのリンクも表示する**</span><span class="sxs-lookup"><span data-stu-id="6a183-202">**Extract product information, and also render a link to the product**</span></span>

<span data-ttu-id="6a183-203">`extract.product` メソッドと `none` フォールバックを指定します。</span><span class="sxs-lookup"><span data-stu-id="6a183-203">Specify the `extract.product` method and the `none` fallback.</span></span> <span data-ttu-id="6a183-204">製品の URL に設定された `src` 属性を含む `a` 要素も送信します (または、ページに追加するその他の情報を送信することもできます)。</span><span class="sxs-lookup"><span data-stu-id="6a183-204">Also send an `a` element with the `src` attribute set to the product URL (or you can send any other information you want to add to the page).</span></span> <span data-ttu-id="6a183-205">API ではコンテンツを抽出できない場合は、ページのリンクのみが表示されます。</span><span class="sxs-lookup"><span data-stu-id="6a183-205">If the API is unable to extract any content, only the page link is rendered.</span></span>

```html 
<div
    data-render-src="http://www.homedepot.com/p/Active-Ventilation-5-Watt-Solar-Powered-Exhaust-Attic-Fan-RBSF-8-WT/204203001"
    data-render-method="extract.product"
    data-render-fallback="none">
</div>
<a href="http://www.homedepot.com/p/Active-Ventilation-5-Watt-Solar-Powered-Exhaust-Attic-Fan-RBSF-8-WT/204203001">Product URL</a>
```


<a name="unknown"></a> 
## <a name="unknown-content-type-extractions"></a><span data-ttu-id="6a183-206">不明な種類のコンテンツの抽出</span><span class="sxs-lookup"><span data-stu-id="6a183-206">Unknown content type extractions</span></span>

<span data-ttu-id="6a183-207">送信するコンテンツの種類 (名刺、レシピ、製品) がわからない場合、修飾されていない `extract` メソッドを使用して、OneNote API が対象種類を自動検出するようにできます。</span><span class="sxs-lookup"><span data-stu-id="6a183-207">If you don't know the content type (business card, recipe, or product) that you're sending, you can use the unqualified `extract` method and let the OneNote API automatically detect the type.</span></span> <span data-ttu-id="6a183-208">この方法は、目的のアプリが各種のキャプチャを送信する場合に使用できます。</span><span class="sxs-lookup"><span data-stu-id="6a183-208">You might want to do this if your app sends different capture types.</span></span>

> <span data-ttu-id="6a183-209">**注:** 送信するコンテンツの種類がわかっている場合は、`extract.businesscard`、`extract.recipe`、または `extract.product` のメソッドを使用してください。</span><span class="sxs-lookup"><span data-stu-id="6a183-209">If you do know the content type that you're sending, you should use the , `extract.businesscard`, or `extract.recipe` method.</span></span> <span data-ttu-id="6a183-210">これにより、最適な抽出結果が得られるようになることがあります。</span><span class="sxs-lookup"><span data-stu-id="6a183-210">In some cases, this can help to optimize the extraction results.</span></span>
 
### <a name="common-scenarios-for-unknown-extractions"></a><span data-ttu-id="6a183-211">不明な抽出の一般的なシナリオ</span><span class="sxs-lookup"><span data-stu-id="6a183-211">Common scenarios for unknown extractions</span></span>

<span data-ttu-id="6a183-212">**画像または URL を送信して、抽出に失敗した場合は指定された画像または Web ページのスナップショットを表示する**</span><span class="sxs-lookup"><span data-stu-id="6a183-212">**Send an image or a URL, and render the supplied image or a snapshot of the webpage if the extraction fails**</span></span>

<span data-ttu-id="6a183-213">API が自動的にコンテンツの種類を検出するように `extract` メソッドを指定して、既定の render フォールバックを使用します。</span><span class="sxs-lookup"><span data-stu-id="6a183-213">Specify the `extract` method so the API automatically detects the content type, and use the default render fallback.</span></span> <span data-ttu-id="6a183-214">API ではコンテンツを抽出できない場合は、その代わりに指定された画像または Web ページのスナップショットが表示されます。</span><span class="sxs-lookup"><span data-stu-id="6a183-214">If the API is unable to extract any content, it renders the supplied image or snapshot of the webpage instead.</span></span>

```html 
<div
    data-render-src="some image or url"
    data-render-method="extract">
</div>
```


<a name="request-response-info"></a>
## <a name="response-information"></a><span data-ttu-id="6a183-215">応答情報</span><span class="sxs-lookup"><span data-stu-id="6a183-215">Response information</span></span>

| <span data-ttu-id="6a183-216">応答データ</span><span class="sxs-lookup"><span data-stu-id="6a183-216">Response data</span></span> | <span data-ttu-id="6a183-217">説明</span><span class="sxs-lookup"><span data-stu-id="6a183-217">Description</span></span> |  
|------|------|  
| <span data-ttu-id="6a183-218">成功コード</span><span class="sxs-lookup"><span data-stu-id="6a183-218">Success code</span></span> | <span data-ttu-id="6a183-219">成功した POST 要求に対しては 201 HTTP ステータス コード、成功した PATCH 要求に対しては 204 HTTP ステータス コードが戻ります。</span><span class="sxs-lookup"><span data-stu-id="6a183-219">A 201 HTTP status code for a successful POST request, and a 204 HTTP status code for a successful PATCH request.</span></span> |  
| <span data-ttu-id="6a183-220">エラー</span><span class="sxs-lookup"><span data-stu-id="6a183-220">Errors</span></span>| <span data-ttu-id="6a183-221">Microsoft Graph から返されることのある OneNote エラーに関する詳細については、「[Microsoft Graph の OneNote API のエラー コード](onenote_error_codes.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="6a183-221">Read [Error codes for OneNote APIs in Microsoft Graph](onenote_error_codes.md) to learn about OneNote errors that Microsoft Graph can return.</span></span> |  


<a name="permissions"></a>
## <a name="permissions"></a><span data-ttu-id="6a183-222">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6a183-222">Permissions</span></span>

<span data-ttu-id="6a183-p121">OneNote ページを作成または更新するには、適切なアクセス許可を要求する必要があります。アプリの動作に必要な最低限のアクセス許可を選択してください。</span><span class="sxs-lookup"><span data-stu-id="6a183-p121">To create or update OneNote pages, you'll need to request appropriate permissions. Choose the lowest level of permissions that your app needs to do its work.</span></span>

<span data-ttu-id="6a183-225">**_POST pages_ のアクセス許可**</span><span class="sxs-lookup"><span data-stu-id="6a183-225">**Permissions for _POST pages_**</span></span>

- <span data-ttu-id="6a183-226">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="6a183-226">Notes.Create</span></span>
- <span data-ttu-id="6a183-227">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6a183-227">Notes.ReadWrite</span></span>
- <span data-ttu-id="6a183-228">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a183-228">Notes.ReadWrite.All</span></span>  

<span data-ttu-id="6a183-229">**_PATCH pages_ のアクセス許可**</span><span class="sxs-lookup"><span data-stu-id="6a183-229">**Permissions for _PATCH pages_**</span></span>

- <span data-ttu-id="6a183-230">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6a183-230">Notes.ReadWrite</span></span>
- <span data-ttu-id="6a183-231">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a183-231">Notes.ReadWrite.All</span></span>

<span data-ttu-id="6a183-232">アクセス許可の範囲とその動作方法の詳細については、「[Microsoft Graph のアクセス許可のリファレンス](permissions_reference.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="6a183-232">For more information about permission scopes and how they work, see [OneNote permission scopes](permissions_reference.md).</span></span>


<a name="see-also"></a>
## <a name="additional-resources"></a><span data-ttu-id="6a183-233">その他のリソース</span><span class="sxs-lookup"><span data-stu-id="6a183-233">Additional resources</span></span>

- [<span data-ttu-id="6a183-234">OneNote ページの作成</span><span class="sxs-lookup"><span data-stu-id="6a183-234">Create OneNote pages</span></span>](onenote-create-page.md)
- [<span data-ttu-id="6a183-235">OneNote ページ コンテンツを更新する</span><span class="sxs-lookup"><span data-stu-id="6a183-235">Update OneNote page content</span></span>](onenote_update_page.md)
- [<span data-ttu-id="6a183-236">画像とファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="6a183-236">Add images and files</span></span>](onenote_images_files.md)
- [<span data-ttu-id="6a183-237">OneNote との統合</span><span class="sxs-lookup"><span data-stu-id="6a183-237">Integrate with OneNote</span></span>](integrate_with_onenote.md)
- [<span data-ttu-id="6a183-238">OneNote の開発者ブログ</span><span class="sxs-lookup"><span data-stu-id="6a183-238">OneNote Developer Blog</span></span>](http://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="6a183-239">Stack Overflow 掲載の OneNote の開発に関する質問</span><span class="sxs-lookup"><span data-stu-id="6a183-239">OneNote development questions on Stack Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="6a183-240">OneNote GitHub のリポジトリ</span><span class="sxs-lookup"><span data-stu-id="6a183-240">OneNote GitHub repos</span></span>](http://go.microsoft.com/fwlink/?LinkID=390178)  

