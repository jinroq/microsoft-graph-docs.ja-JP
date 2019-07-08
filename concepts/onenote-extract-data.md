---
title: 'OneNote API div タグを使用してキャプチャからデータを抽出する '
description: " Office 365 のエンタープライズ ノートブック"
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 8679f277cc893cd5903ff98adfa09f8285013792
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578850"
---
# <a name="use-onenote-api-div-tags-to-extract-data-from-captures"></a><span data-ttu-id="fbf5f-103">OneNote API div タグを使用してキャプチャからデータを抽出する</span><span class="sxs-lookup"><span data-stu-id="fbf5f-103">Use OneNote API div tags to extract data from captures</span></span> 

<span data-ttu-id="fbf5f-104">**適用対象** OneDrive のコンシューマー ノートブック | Office 365 のエンタープライズ ノートブック</span><span class="sxs-lookup"><span data-stu-id="fbf5f-104">**Applies to** Consumer notebooks on OneDrive | Enterprise notebooks on Office 365</span></span>

<span data-ttu-id="fbf5f-105">OneNote API を使用して、画像から名刺データを抽出したり、URL からレシピや製品データを抽出したりします。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-105">Use the OneNote API to extract business card data from an image, or recipe and product data from a URL.</span></span>

<a name="attributes"></a>

## <a name="extraction-attributes"></a><span data-ttu-id="fbf5f-106">抽出の属性</span><span class="sxs-lookup"><span data-stu-id="fbf5f-106">Extraction attributes</span></span>

<span data-ttu-id="fbf5f-p101">単に div を含めるだけで、データの抽出や変換ができます。div は [create-page](onenote-create-page.md) または [update-page](onenote-update-page.md) 要求で、ソース コンテンツ、抽出メソッド、およびフォールバックの動作を指定します。API は抽出したデータを、読みやすい形式でページに表示します。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-p101">To extract and transform data, simply include a div that specifies the source content, extraction method, and fallback behavior in your [create-page](onenote-create-page.md) or [update-page](onenote-update-page.md) request. The API renders extracted data on the page in an easy-to-read format.</span></span> 

```html
<div
  data-render-src="image-or-url"
  data-render-method="extraction-method"
  data-render-fallback="fallback-action">
</div>
```

### <a name="data-render-src"></a><span data-ttu-id="fbf5f-109">data-render-src</span><span class="sxs-lookup"><span data-stu-id="fbf5f-109">data-render-src</span></span>

<span data-ttu-id="fbf5f-p102">コンテンツ ソース。名刺の画像、または数多くの人気レシピや製品の Web サイトの絶対 URL にできます。必須。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-p102">The content source. This can be an image of a business card or an absolute URL from many popular recipe or product websites. Required.</span></span>

<span data-ttu-id="fbf5f-p103">URL を指定するときに最適な結果を得るために、ソースの Web ページの HTML で定義された正規 URL を使用してください (定義されている場合)。たとえば、正規 URL はソースの Web ページで次のように定義されます。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-p103">For best results when specifying a URL, use the canonical URL defined in the HTML of the source webpage, if one is defined. For example, a canonical URL might be defined in the source webpage like this:</span></span>

`<link rel="canonical" href="www.domainname.com/page/123/size12/type987" />` 


### <a name="data-render-method"></a><span data-ttu-id="fbf5f-115">data-render-method</span><span class="sxs-lookup"><span data-stu-id="fbf5f-115">data-render-method</span></span>

<span data-ttu-id="fbf5f-p104">実行する抽出メソッド。必須。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-p104">The extraction method to run. Required.</span></span>

| <span data-ttu-id="fbf5f-118">値</span><span class="sxs-lookup"><span data-stu-id="fbf5f-118">Value</span></span> | <span data-ttu-id="fbf5f-119">説明</span><span class="sxs-lookup"><span data-stu-id="fbf5f-119">Description</span></span> |
|:------|:------|
| <span data-ttu-id="fbf5f-120">extract.businesscard</span><span class="sxs-lookup"><span data-stu-id="fbf5f-120">extract.businesscard</span></span> | <span data-ttu-id="fbf5f-121">名刺の抽出。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-121">A business card extraction.</span></span> |
| <span data-ttu-id="fbf5f-122">extract.recipe</span><span class="sxs-lookup"><span data-stu-id="fbf5f-122">extract.recipe</span></span> | <span data-ttu-id="fbf5f-123">レシピの抽出。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-123">A recipe extraction.</span></span> |
| <span data-ttu-id="fbf5f-124">extract.product</span><span class="sxs-lookup"><span data-stu-id="fbf5f-124">extract.product</span></span> | <span data-ttu-id="fbf5f-125">製品リストの抽出。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-125">A product listing extraction.</span></span> |
| <span data-ttu-id="fbf5f-126">extract</span><span class="sxs-lookup"><span data-stu-id="fbf5f-126">extract</span></span> | <span data-ttu-id="fbf5f-127">不明な種類の抽出。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-127">An unknown extraction type.</span></span> |

<span data-ttu-id="fbf5f-128">最適の結果を得るために、コンテンツの種類 (`extract.businesscard`、`extract.recipe`、または `extract.product`) を指定してください (種類がわかっている場合)。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-128">For best results, specify the content type (`extract.businesscard`, `extract.recipe`, or `extract.product`) if you know it.</span></span> <span data-ttu-id="fbf5f-129">種類が不明の場合は、`extract` メソッドを使用してください。OneNote API が種類の自動検出を試行します。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-129">If the type is unknown, use the `extract` method, and the OneNote API will try to auto-detect the type.</span></span>

### <a name="data-render-fallback"></a><span data-ttu-id="fbf5f-130">data-render-fallback</span><span class="sxs-lookup"><span data-stu-id="fbf5f-130">data-render-fallback</span></span>

<span data-ttu-id="fbf5f-p106">抽出できない場合のフォールバック動作。省略すると、既定の **render** になります。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-p106">The fallback behavior if the extraction fails. Defaults to **render** if omitted.</span></span> 

| <span data-ttu-id="fbf5f-133">値</span><span class="sxs-lookup"><span data-stu-id="fbf5f-133">Value</span></span> | <span data-ttu-id="fbf5f-134">説明</span><span class="sxs-lookup"><span data-stu-id="fbf5f-134">Description</span></span> |
|:------|:------|
| <span data-ttu-id="fbf5f-135">render</span><span class="sxs-lookup"><span data-stu-id="fbf5f-135">render</span></span> | <span data-ttu-id="fbf5f-136">レシピまたは製品の Web ページのソース画像またはスナップショットを表示します。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-136">Renders the source image or a snapshot of the recipe or product webpage.</span></span> |
| <span data-ttu-id="fbf5f-137">none</span><span class="sxs-lookup"><span data-stu-id="fbf5f-137">none</span></span> | <span data-ttu-id="fbf5f-138">何も実行しません。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-138">Does nothing.</span></span><br /><br /><span data-ttu-id="fbf5f-p107">このオプションは、抽出コンテンツに加えて、名刺または Web ページのスナップショットをページに必ず含める場合に役立ちます。例に示すように、要求には個別の `img` 要素を含めてください。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-p107">This option is useful if you want to always include a snapshot of the business card or webpage on the page in addition to any extracted content. Be sure to send a separate `img` element in the request, as shown in the examples.</span></span> |

<a name="biz-card"></a>

## <a name="business-card-extractions"></a><span data-ttu-id="fbf5f-141">名刺の抽出</span><span class="sxs-lookup"><span data-stu-id="fbf5f-141">Business card extractions</span></span>

<span data-ttu-id="fbf5f-142">OneNote API は、個人または会社の名刺の画像に基づいて、次の連絡先情報の検索および表示を試行します。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-142">The OneNote API tries to find and render the following contact information based on an image of a person's or company's business card.</span></span>

- <span data-ttu-id="fbf5f-143">名前</span><span class="sxs-lookup"><span data-stu-id="fbf5f-143">Name</span></span>
- <span data-ttu-id="fbf5f-144">タイトル</span><span class="sxs-lookup"><span data-stu-id="fbf5f-144">Title</span></span>
- <span data-ttu-id="fbf5f-145">組織</span><span class="sxs-lookup"><span data-stu-id="fbf5f-145">Organization</span></span>
- <span data-ttu-id="fbf5f-146">電話および FAX 番号</span><span class="sxs-lookup"><span data-stu-id="fbf5f-146">Phone and fax numbers</span></span>
- <span data-ttu-id="fbf5f-147">郵送先および実際の住所</span><span class="sxs-lookup"><span data-stu-id="fbf5f-147">Mailing and physical addresses</span></span>
- <span data-ttu-id="fbf5f-148">電子メール アドレス</span><span class="sxs-lookup"><span data-stu-id="fbf5f-148">Email addresses</span></span>
- <span data-ttu-id="fbf5f-149">Web サイト</span><span class="sxs-lookup"><span data-stu-id="fbf5f-149">Websites</span></span>



<img alt="An example business card extraction" src="images/biz-card-extraction.png" width="200">

<span data-ttu-id="fbf5f-p108">ページには、抽出された連絡先情報が含まれる vCard (.VCF ファイル) も組み込まれます。この vCard は、ページの HTML コンテンツを取得するときに連絡先情報を入手するのに便利な方法です。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-p108">A vCard (.VCF file) with the extracted contact information is also embedded in the page. The vCard is a convenient way to get the contact information when retrieving page HTML content.</span></span>

### <a name="common-scenarios-for-business-card-extractions"></a><span data-ttu-id="fbf5f-152">名刺抽出の一般的なシナリオ</span><span class="sxs-lookup"><span data-stu-id="fbf5f-152">Common scenarios for business card extractions</span></span>

#### <a name="extract-business-card-information-and-also-render-the-business-card-image"></a><span data-ttu-id="fbf5f-153">名刺情報を抽出して、名刺の画像を表示する</span><span class="sxs-lookup"><span data-stu-id="fbf5f-153">Extract business card information, and also render the business card image</span></span>

<span data-ttu-id="fbf5f-p109">`extract.businesscard` メソッドと `none` フォールバックを指定します。また、画像を参照する `src` 属性を含む `img` 要素も送信します。API ではコンテンツを抽出できない場合は、名刺の画像のみが表示されます。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-p109">Specify the `extract.businesscard` method and the `none` fallback. Also send an `img` element with the `src` attribute that also references the image. If the API is unable to extract any content, it renders the business card image only.</span></span>

```html 
<div
    data-render-src="name:scanned-card-image"
    data-render-method="extract.businesscard"
    data-render-fallback="none">
</div>
<img src="name:scanned-card-image" />
```


#### <a name="extract-business-card-information-and-render-the-business-card-image-only-if-the-extraction-fails"></a><span data-ttu-id="fbf5f-157">名刺情報を抽出する。抽出に失敗した場合のみ名刺の画像を表示する</span><span class="sxs-lookup"><span data-stu-id="fbf5f-157">Extract business card information, and render the business card image only if the extraction fails</span></span>

<span data-ttu-id="fbf5f-p110">`extract.businesscard` メソッドを指定して、既定の `render` フォールバックを使用します。API ではコンテンツを抽出できない場合は、その代わりに名刺の画像が表示されます。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-p110">Specify the `extract.businesscard` method and use the default `render` fallback. If the API is unable to extract any content, it renders the business card image instead.</span></span>

```html
<div
    data-render-src="name:scanned-card-image"
    data-render-method="extract.businesscard">
</div>
```
 
<span data-ttu-id="fbf5f-p111">名刺の抽出では、画像はマルチパートの要求の名前付きパートとして送信されます。要求で画像を送信する例については、「[画像とファイルの追加](onenote-images-files.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-p111">For business card extractions, the image is sent as a named part in a multipart request. See [Add images and files](onenote-images-files.md) for examples that show how to send an image in a request.</span></span>


<a name="recipe"></a>

## <a name="recipe-extractions"></a><span data-ttu-id="fbf5f-162">レシピの抽出</span><span class="sxs-lookup"><span data-stu-id="fbf5f-162">Recipe extractions</span></span>

<span data-ttu-id="fbf5f-163">OneNote API は、レシピの URL に基づいて、次の情報の検索および表示を試行します。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-163">The OneNote API tries to find and render the following information based on a recipe's URL.</span></span>

- <span data-ttu-id="fbf5f-164">完成例の画像</span><span class="sxs-lookup"><span data-stu-id="fbf5f-164">Hero image</span></span>
- <span data-ttu-id="fbf5f-165">評価</span><span class="sxs-lookup"><span data-stu-id="fbf5f-165">Rating</span></span>
- <span data-ttu-id="fbf5f-166">材料</span><span class="sxs-lookup"><span data-stu-id="fbf5f-166">Ingredients</span></span>
- <span data-ttu-id="fbf5f-167">手順</span><span class="sxs-lookup"><span data-stu-id="fbf5f-167">Instructions</span></span>
- <span data-ttu-id="fbf5f-168">準備、調理、および合計の時間</span><span class="sxs-lookup"><span data-stu-id="fbf5f-168">Prep, cook, and total times</span></span>
- <span data-ttu-id="fbf5f-169">分量</span><span class="sxs-lookup"><span data-stu-id="fbf5f-169">Servings</span></span>


<img alt="An example recipe extraction" src="images/recipe-extraction.png" width="200">

<span data-ttu-id="fbf5f-170">この API は、*Allrecipes.com*、*FoodNetwork.com*、および *SeriousEats.com* など、数多くの人気サイトのレシピ用に最適化されています。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-170">The API is optimized for recipes from many popular sites such as *Allrecipes.com*, *FoodNetwork.com*, and *SeriousEats.com*.</span></span>

### <a name="common-scenarios-for-recipe-extractions"></a><span data-ttu-id="fbf5f-171">レシピ抽出の一般的なシナリオ</span><span class="sxs-lookup"><span data-stu-id="fbf5f-171">Common scenarios for recipe extractions</span></span>

#### <a name="extract-recipe-information-and-also-render-a-snapshot-of-the-recipe-webpage"></a><span data-ttu-id="fbf5f-172">レシピ情報を抽出して、レシピの Web ページのスナップショットも表示する</span><span class="sxs-lookup"><span data-stu-id="fbf5f-172">Extract recipe information, and also render a snapshot of the recipe webpage</span></span>

<span data-ttu-id="fbf5f-p112">`extract.recipe` メソッドと `none` フォールバックを指定します。また、レシピの URL に設定した `data-render-src` 属性を含む `img` 要素も送信します。API ではコンテンツを抽出できない場合は、レシピの Web ページのスナップショットのみが表示されます。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-p112">Specify the `extract.recipe` method and the `none` fallback. Also send an `img` element with the `data-render-src` attribute set to the recipe URL. If the API is unable to extract any content, it renders a snapshot of the recipe webpage only.</span></span>

<span data-ttu-id="fbf5f-176">おそらく、このシナリオが最も多くの情報を提供することになります。Web ページには、お客様のレビューや提案などの追加情報が含まれている場合があるためです。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-176">This scenario potentially provides the most information because the webpage may include additional information, such as customer reviews and suggestions.</span></span>

```html 
<div
    data-render-src="https://allrecipes.com/recipe/guacamole/"
    data-render-method="extract.recipe"
    data-render-fallback="none">
</div>
<img data-render-src="https://allrecipes.com/recipe/guacamole/" />
```
 

#### <a name="extract-recipe-information-and-render-a-snapshot-of-the-recipe-webpage-only-if-the-extraction-fails"></a><span data-ttu-id="fbf5f-177">レシピ情報を抽出する。抽出に失敗した場合のみレシピの Web ページのスナップショットも表示する</span><span class="sxs-lookup"><span data-stu-id="fbf5f-177">Extract recipe information, and render a snapshot of the recipe webpage only if the extraction fails</span></span>

<span data-ttu-id="fbf5f-p113">`extract.recipe` メソッドを指定して、既定の render フォールバックを使用します。API ではコンテンツを抽出できない場合は、その代わりにレシピの Web ページのスナップショットが表示されます。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-p113">Specify the `extract.recipe` method and use the default render fallback. If the API is unable to extract any content, it renders a snapshot of the recipe webpage instead.</span></span>

```html  
<div
    data-render-src="https://www.foodnetwork.com/recipes/alton-brown/creme-brulee-recipe.html"
    data-render-method="extract.recipe">
</div>
```


#### <a name="extract-recipe-information-and-also-render-a-link-to-the-recipe"></a><span data-ttu-id="fbf5f-180">レシピ情報を抽出し、そのレシピへのリンクも表示する</span><span class="sxs-lookup"><span data-stu-id="fbf5f-180">Extract recipe information, and also render a link to the recipe</span></span>

<span data-ttu-id="fbf5f-p114">`extract.recipe` メソッドと `none` フォールバックを指定します。レシピの URL に設定された `src` 属性を含む `a` 要素も送信します (または、ページに追加するその他の情報を送信することもできます)。API ではコンテンツを抽出できない場合は、レシピのリンクのみが表示されます。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-p114">Specify the `extract.recipe` method and the `none` fallback. Also send an `a` element with the `src` attribute set to the recipe URL (or you can send any other information you want to add to the page). If the API is unable to extract any content, only the recipe link is rendered.</span></span>

```html  
<div
    data-render-src="https://www.seriouseats.com/recipes/2014/09/diy-spicy-kimchi-beef-instant-noodles-recipe.html"
    data-render-method="extract.recipe"
    data-render-fallback="none">
</div>
<a href="https://www.seriouseats.com/recipes/2014/09/diy-spicy-kimchi-beef-instant-noodles-recipe.html">Recipe URL</a>
``` 


<a name="product"></a>

## <a name="product-listing-extractions"></a><span data-ttu-id="fbf5f-184">製品リストの抽出</span><span class="sxs-lookup"><span data-stu-id="fbf5f-184">Product listing extractions</span></span>

- <span data-ttu-id="fbf5f-185">タイトル</span><span class="sxs-lookup"><span data-stu-id="fbf5f-185">Title</span></span>
- <span data-ttu-id="fbf5f-186">評価</span><span class="sxs-lookup"><span data-stu-id="fbf5f-186">Rating</span></span>
- <span data-ttu-id="fbf5f-187">主要画像</span><span class="sxs-lookup"><span data-stu-id="fbf5f-187">Primary image</span></span>
- <span data-ttu-id="fbf5f-188">説明</span><span class="sxs-lookup"><span data-stu-id="fbf5f-188">Description</span></span>
- <span data-ttu-id="fbf5f-189">機能</span><span class="sxs-lookup"><span data-stu-id="fbf5f-189">Features</span></span>
- <span data-ttu-id="fbf5f-190">仕様</span><span class="sxs-lookup"><span data-stu-id="fbf5f-190">Specifications</span></span>



<img alt="An example product listing extraction" src="images/product-extraction.png" width="200">

<span data-ttu-id="fbf5f-191">この API は、*Amazon.com* や *HomeDepot.com* など、数多くの人気サイトの製品用に最適化されています。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-191">The API is optimized for products from many popular sites such as *Amazon.com* and *HomeDepot.com*.</span></span>

### <a name="common-scenarios-for-recipe-extractions"></a><span data-ttu-id="fbf5f-192">レシピ抽出の一般的なシナリオ</span><span class="sxs-lookup"><span data-stu-id="fbf5f-192">Common scenarios for recipe extractions</span></span>

#### <a name="extract-product-information-and-also-render-a-snapshot-of-the-product-webpage"></a><span data-ttu-id="fbf5f-193">製品情報を抽出して、製品の Web のスナップショットも表示する</span><span class="sxs-lookup"><span data-stu-id="fbf5f-193">Extract product information, and also render a snapshot of the product webpage</span></span>

<span data-ttu-id="fbf5f-p115">`extract.product` メソッドと `none` フォールバックを指定します。また、製品の URL に設定した `data-render-src` 属性を含む `img` 要素も送信します。API ではコンテンツを抽出できない場合は、製品の Web ページのスナップショットのみが表示されます。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-p115">Specify the `extract.product` method and the `none` fallback. Also send an `img` element with the `data-render-src` attribute set to the product URL. If the API is unable to extract any content, it renders a snapshot of the product webpage only.</span></span>

<span data-ttu-id="fbf5f-197">おそらく、このシナリオが最も多くの情報を提供することになります。Web ページには、お客様のレビューや提案などの追加情報が含まれている場合があるためです。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-197">This scenario potentially provides the most information because the webpage may include additional information, such as customer reviews and suggestions.</span></span>

```html 
<div
    data-render-src="https://www.amazon.com/Microsoft-Band-Small/dp/B00P2T2WVO"
    data-render-method="extract.product"
    data-render-fallback="none">
</div>
<img data-render-src="https://www.amazon.com/Microsoft-Band-Small/dp/B00P2T2WVO" />
```


#### <a name="extract-product-information-and-render-a-snapshot-of-the-product-webpage-only-if-the-extraction-fails"></a><span data-ttu-id="fbf5f-198">製品情報を抽出する。抽出に失敗した場合のみ製品の Web ページのスナップショットも表示する</span><span class="sxs-lookup"><span data-stu-id="fbf5f-198">Extract product information, and render a snapshot of the product webpage only if the extraction fails</span></span>

<span data-ttu-id="fbf5f-p116">`extract.product` メソッドを指定して、既定の render フォールバックを使用します。API ではコンテンツを抽出できない場合は、その代わりに製品の Web ページのスナップショットが表示されます。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-p116">Specify the `extract.product` method and use the default render fallback. If the API is unable to extract any content, it renders a snapshot of the product webpage instead.</span></span>

```html 
<div
    data-render-src="https://www.sears.com/craftsman-19hp-42-8221-turn-tight-174-hydrostatic-yard-tractor/p-07120381000P"
    data-render-method="extract.product">
</div>
```
 

#### <a name="extract-product-information-and-also-render-a-link-to-the-product"></a><span data-ttu-id="fbf5f-201">製品情報を抽出し、その製品へのリンクも表示する</span><span class="sxs-lookup"><span data-stu-id="fbf5f-201">Extract product information, and also render a link to the product</span></span>

<span data-ttu-id="fbf5f-p117">`extract.product` メソッドと `none` フォールバックを指定します。製品の URL に設定された `src` 属性を含む `a` 要素も送信します (または、ページに追加するその他の情報を送信することもできます)。API ではコンテンツを抽出できない場合は、ページのリンクのみが表示されます。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-p117">Specify the `extract.product` method and the `none` fallback. Also send an `a` element with the `src` attribute set to the product URL (or you can send any other information you want to add to the page). If the API is unable to extract any content, only the page link is rendered.</span></span>

```html 
<div
    data-render-src="https://www.homedepot.com/p/Active-Ventilation-5-Watt-Solar-Powered-Exhaust-Attic-Fan-RBSF-8-WT/204203001"
    data-render-method="extract.product"
    data-render-fallback="none">
</div>
<a href="https://www.homedepot.com/p/Active-Ventilation-5-Watt-Solar-Powered-Exhaust-Attic-Fan-RBSF-8-WT/204203001">Product URL</a>
```


<a name="unknown"></a> 

## <a name="unknown-content-type-extractions"></a><span data-ttu-id="fbf5f-205">不明な種類のコンテンツの抽出</span><span class="sxs-lookup"><span data-stu-id="fbf5f-205">Unknown content type extractions</span></span>

<span data-ttu-id="fbf5f-p118">送信するコンテンツの種類 (名刺、レシピ、製品) がわからない場合、修飾されていない `extract` メソッドを使用して、OneNote API が対象種類を自動検出するようにできます。この方法は、目的のアプリが各種のキャプチャを送信する場合に使用できます。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-p118">If you don't know the content type (business card, recipe, or product) that you're sending, you can use the unqualified `extract` method and let the OneNote API automatically detect the type. You might want to do this if your app sends different capture types.</span></span>

> <span data-ttu-id="fbf5f-208">**注:** 送信するコンテンツの種類がわかっている場合は、`extract.businesscard`、`extract.recipe`、または `extract.product` のメソッドを使用してください。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-208">**Note:** If you do know the content type that you're sending, you should use the `extract.businesscard`, `extract.recipe`, or `extract.product` method.</span></span> <span data-ttu-id="fbf5f-209">これにより、最適な抽出結果が得られるようになることがあります。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-209">In some cases, this can help to optimize the extraction results.</span></span>
 
### <a name="common-scenarios-for-unknown-extractions"></a><span data-ttu-id="fbf5f-210">不明な抽出の一般的なシナリオ</span><span class="sxs-lookup"><span data-stu-id="fbf5f-210">Common scenarios for unknown extractions</span></span>

#### <a name="send-an-image-or-a-url-and-render-the-supplied-image-or-a-snapshot-of-the-webpage-if-the-extraction-fails"></a><span data-ttu-id="fbf5f-211">画像または URL を送信して、抽出に失敗した場合は指定された画像または Web ページのスナップショットを表示する</span><span class="sxs-lookup"><span data-stu-id="fbf5f-211">Send an image or a URL, and render the supplied image or a snapshot of the webpage if the extraction fails</span></span>

<span data-ttu-id="fbf5f-p120">API が自動的にコンテンツの種類を検出するように `extract` メソッドを指定して、既定の render フォールバックを使用します。API ではコンテンツを抽出できない場合は、その代わりに指定された画像または Web ページのスナップショットが表示されます。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-p120">Specify the `extract` method so the API automatically detects the content type, and use the default render fallback. If the API is unable to extract any content, it renders the supplied image or snapshot of the webpage instead.</span></span>

```html 
<div
    data-render-src="some image or url"
    data-render-method="extract">
</div>
```


<a name="request-response-info"></a>

## <a name="response-information"></a><span data-ttu-id="fbf5f-214">応答情報</span><span class="sxs-lookup"><span data-stu-id="fbf5f-214">Response information</span></span>

| <span data-ttu-id="fbf5f-215">応答データ</span><span class="sxs-lookup"><span data-stu-id="fbf5f-215">Response data</span></span> | <span data-ttu-id="fbf5f-216">説明</span><span class="sxs-lookup"><span data-stu-id="fbf5f-216">Description</span></span> |  
|------|------|  
| <span data-ttu-id="fbf5f-217">成功コード</span><span class="sxs-lookup"><span data-stu-id="fbf5f-217">Success code</span></span> | <span data-ttu-id="fbf5f-218">成功した POST 要求に対しては 201 HTTP ステータス コード、成功した PATCH 要求に対しては 204 HTTP ステータス コードが戻ります。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-218">A 201 HTTP status code for a successful POST request, and a 204 HTTP status code for a successful PATCH request.</span></span> |  
| <span data-ttu-id="fbf5f-219">エラー</span><span class="sxs-lookup"><span data-stu-id="fbf5f-219">Errors</span></span>| <span data-ttu-id="fbf5f-220">Microsoft Graph から返されることのある OneNote エラーに関する詳細については、「[Microsoft Graph の OneNote API のエラー コード](onenote-error-codes.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-220">Read [Error codes for OneNote APIs in Microsoft Graph](onenote-error-codes.md) to learn about OneNote errors that Microsoft Graph can return.</span></span> |  


<a name="permissions"></a>

## <a name="permissions"></a><span data-ttu-id="fbf5f-221">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fbf5f-221">Permissions</span></span>

<span data-ttu-id="fbf5f-p121">OneNote ページを作成または更新するには、適切なアクセス許可を要求する必要があります。アプリの動作に必要な最低限のアクセス許可を選択してください。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-p121">To create or update OneNote pages, you'll need to request appropriate permissions. Choose the lowest level of permissions that your app needs to do its work.</span></span>

#### <a name="permissions-for-post-pages"></a><span data-ttu-id="fbf5f-224">POST ページのアクセス許可</span><span class="sxs-lookup"><span data-stu-id="fbf5f-224">Permissions for POST pages</span></span>

- <span data-ttu-id="fbf5f-225">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="fbf5f-225">Notes.Create</span></span>
- <span data-ttu-id="fbf5f-226">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fbf5f-226">Notes.ReadWrite</span></span>
- <span data-ttu-id="fbf5f-227">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbf5f-227">Notes.ReadWrite.All</span></span>  

#### <a name="permissions-for-patch-pages"></a><span data-ttu-id="fbf5f-228">PATCH ページのアクセス許可</span><span class="sxs-lookup"><span data-stu-id="fbf5f-228">Permissions for PATCH pages</span></span>

- <span data-ttu-id="fbf5f-229">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fbf5f-229">Notes.ReadWrite</span></span>
- <span data-ttu-id="fbf5f-230">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbf5f-230">Notes.ReadWrite.All</span></span>

<span data-ttu-id="fbf5f-231">アクセス許可の範囲とその動作方法の詳細については、「[Microsoft Graph のアクセス許可のリファレンス](permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fbf5f-231">For more information about permission scopes and how they work, see [Microsoft Graph permissions reference](permissions-reference.md).</span></span>


<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="fbf5f-232">関連項目</span><span class="sxs-lookup"><span data-stu-id="fbf5f-232">See also</span></span>

- [<span data-ttu-id="fbf5f-233">OneNote ページを作成する</span><span class="sxs-lookup"><span data-stu-id="fbf5f-233">Create OneNote pages</span></span>](onenote-create-page.md)
- [<span data-ttu-id="fbf5f-234">OneNote ページ コンテンツを更新する</span><span class="sxs-lookup"><span data-stu-id="fbf5f-234">Update OneNote page content</span></span>](onenote-update-page.md)
- [<span data-ttu-id="fbf5f-235">画像とファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="fbf5f-235">Add images and files</span></span>](onenote-images-files.md)
- [<span data-ttu-id="fbf5f-236">OneNote との統合</span><span class="sxs-lookup"><span data-stu-id="fbf5f-236">Integrate with OneNote</span></span>](integrate-with-onenote.md)
- [<span data-ttu-id="fbf5f-237">OneNote の開発者ブログ</span><span class="sxs-lookup"><span data-stu-id="fbf5f-237">OneNote Developer Blog</span></span>](https://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="fbf5f-238">Stack Overflow 掲載の OneNote の開発に関する質問</span><span class="sxs-lookup"><span data-stu-id="fbf5f-238">OneNote development questions on Stack Overflow</span></span>](https://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="fbf5f-239">OneNote GitHub のリポジトリ</span><span class="sxs-lookup"><span data-stu-id="fbf5f-239">OneNote GitHub repos</span></span>](https://go.microsoft.com/fwlink/?LinkID=390178)  

