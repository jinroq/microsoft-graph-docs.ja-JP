---
title: OneNote ページの入出力 HTML
description: 'OneNote ページを作成または更新する際に、ページ コンテンツと構造を定義する HTML を*入力 HTML* と呼びます。 '
ms.openlocfilehash: f75601771437e359626ef9ffbb474b9a29f07033
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092513"
---
# <a name="input-and-output-html-in-onenote-pages"></a><span data-ttu-id="99894-103">OneNote ページの入出力 HTML</span><span class="sxs-lookup"><span data-stu-id="99894-103">Input and output HTML in OneNote pages</span></span>

<span data-ttu-id="99894-104">OneNote ページを[作成](onenote-create-page.md)または[更新](onenote-update-page.md)する際に、ページ コンテンツと構造を定義する HTML を*入力 HTML* と呼びます。</span><span class="sxs-lookup"><span data-stu-id="99894-104">The HTML that defines the page content and structure when you [create](onenote-create-page.md) or [update](onenote-update-page.md) a OneNote page is called *input HTML*.</span></span> 

<span data-ttu-id="99894-p101">[ページ コンテンツを取得](onenote-get-content.md)すると返される HTML を *出力 HTML* と呼びます。出力 HTML は入力 HTML と同じにはなりません。</span><span class="sxs-lookup"><span data-stu-id="99894-p101">The HTML that's returned when you [get page content](onenote-get-content.md) is called *output HTML*. Output HTML won't be the same as input HTML.</span></span>

<span data-ttu-id="99894-107">Microsoft Graph の OneNote API は、入力 HTML の意味的コンテンツと基本的構造を保持しますが、その HTML を、[サポートされている HTML 要素および CSS プロパティ](onenote-create-page.md#supported-html-and-css-for-onenote-pages)のセットに変換します。</span><span class="sxs-lookup"><span data-stu-id="99894-107">The OneNote APIs in Microsoft Graph preserve the semantic content and basic structure of the input HTML, but convert it to a set of [supported HTML elements and CSS properties](onenote-create-page.md#supported-html-and-css-for-onenote-pages).</span></span> <span data-ttu-id="99894-108">API はさらに、OneNote 機能をサポートするカスタム属性も追加します。</span><span class="sxs-lookup"><span data-stu-id="99894-108">The APIs also add custom attributes that support OneNote features.</span></span>
 
<span data-ttu-id="99894-p103">この資料では、入力 HTML と出力 HTML の主な要素と属性について説明します。ページ コンテンツを作成または更新する場合には入力 HTMLについて、返されるページ コンテンツを解析する場合には出力 HTML について理解することは役立ちます。</span><span class="sxs-lookup"><span data-stu-id="99894-p103">This article describes the principal elements and attributes of input and output HTML. It can be helpful to understand input HTML when you're creating or updating page content, and output HTML when you're parsing returned page content.</span></span> 

## <a name="body-element"></a><span data-ttu-id="99894-111">body 要素</span><span class="sxs-lookup"><span data-stu-id="99894-111">Body element</span></span>

<span data-ttu-id="99894-p104">ページ本文の HTML コンテンツは、画像やファイルのリソースなどを含むページのコンテンツと構造を表します。入力および出力 HTML では、**body** 要素に次の属性を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="99894-p104">The HTML content in the page body represents the page content and structure, including image and file resources. The **body** element can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="99894-114">入力属性</span><span class="sxs-lookup"><span data-stu-id="99894-114">Input attributes</span></span>

|<span data-ttu-id="99894-115">入力属性</span><span class="sxs-lookup"><span data-stu-id="99894-115">Input attribute</span></span>|<span data-ttu-id="99894-116">説明</span><span class="sxs-lookup"><span data-stu-id="99894-116">Description</span></span>|
|:------|:------|
| <span data-ttu-id="99894-117">data-absolute-enabled</span><span class="sxs-lookup"><span data-stu-id="99894-117">data-absolute-enabled</span></span> | <span data-ttu-id="99894-118">[絶対位置で配置](onenote-abs-pos.md)された要素を入力本文でサポートするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="99894-118">Indicates whether the input body supports [absolute positioned](onenote-abs-pos.md) elements.</span></span> |
| <span data-ttu-id="99894-119">style</span><span class="sxs-lookup"><span data-stu-id="99894-119">style</span></span> | <p><span data-ttu-id="99894-120">本文の CSS の [style](#styles) プロパティ。</span><span class="sxs-lookup"><span data-stu-id="99894-120">The CSS [style](#styles) properties of the body.</span></span> <span data-ttu-id="99894-121">出力 HTML では、入力設定がインラインで、適切な子要素で返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="99894-121">In the output HTML, input settings might be returned inline on appropriate child elements.</span></span></p><p><span data-ttu-id="99894-122">現在、**body** 要素では背景色はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="99894-122">Background color is not currently supported for the **body** element.</span></span></p> |
 

#### <a name="output-attributes"></a><span data-ttu-id="99894-123">出力属性</span><span class="sxs-lookup"><span data-stu-id="99894-123">Output attributes</span></span>

|<span data-ttu-id="99894-124">出力属性</span><span class="sxs-lookup"><span data-stu-id="99894-124">Output attribute</span></span>|<span data-ttu-id="99894-125">説明</span><span class="sxs-lookup"><span data-stu-id="99894-125">Description</span></span>|
|:------|:------|
| <span data-ttu-id="99894-126">data-absolute-enabled</span><span class="sxs-lookup"><span data-stu-id="99894-126">data-absolute-enabled</span></span> | <span data-ttu-id="99894-p106">[絶対位置で配置](onenote-abs-pos.md)された要素を本文でサポートするかどうかを示します。出力 HTML では常に **true** です。</span><span class="sxs-lookup"><span data-stu-id="99894-p106">Indicates whether the body supports [absolute positioned](onenote-abs-pos.md) elements. Always **true** in output HTML.</span></span> |
| <span data-ttu-id="99894-129">style</span><span class="sxs-lookup"><span data-stu-id="99894-129">style</span></span> | <span data-ttu-id="99894-130">本文の **font-family** および **font-size** プロパティ。</span><span class="sxs-lookup"><span data-stu-id="99894-130">The **font-family** and **font-size** properties of the body.</span></span> |


## <a name="div-elements"></a><span data-ttu-id="99894-131">div 要素</span><span class="sxs-lookup"><span data-stu-id="99894-131">Div elements</span></span>

<span data-ttu-id="99894-132">**div** 要素にはテキスト、画像、およびその他のコンテンツが含まれます。</span><span class="sxs-lookup"><span data-stu-id="99894-132">**Div** elements contain text, images, and other content.</span></span> <span data-ttu-id="99894-133">入力 HTML と出力 HTML では、**div** 要素に次の属性を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="99894-133">A **div** element can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="99894-134">入力属性</span><span class="sxs-lookup"><span data-stu-id="99894-134">Input attributes</span></span>

|<span data-ttu-id="99894-135">入力属性</span><span class="sxs-lookup"><span data-stu-id="99894-135">Input attribute</span></span>|<span data-ttu-id="99894-136">説明</span><span class="sxs-lookup"><span data-stu-id="99894-136">Description</span></span>|
|:------|:------|
| <span data-ttu-id="99894-137">data-id</span><span class="sxs-lookup"><span data-stu-id="99894-137">data-id</span></span> | <span data-ttu-id="99894-138">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="99894-138">A reference for the element.</span></span><br/><br/><span data-ttu-id="99894-139">[ページ コンテンツの更新](onenote-update-page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="99894-139">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="99894-140">data-render-fallback</span><span class="sxs-lookup"><span data-stu-id="99894-140">data-render-fallback</span></span> | <span data-ttu-id="99894-141">[抽出](onenote-extract-data.md)が失敗した場合のフォールバック操作。**render** (既定) または **none**</span><span class="sxs-lookup"><span data-stu-id="99894-141">The fallback action if the [extraction](onenote-extract-data.md) fails: **render** (default) or **none**.</span></span> |
| <span data-ttu-id="99894-142">data-render-method</span><span class="sxs-lookup"><span data-stu-id="99894-142">data-render-method</span></span> | <span data-ttu-id="99894-143">[抽出](onenote-extract-data.md)を実行するメソッド。たとえば:</span><span class="sxs-lookup"><span data-stu-id="99894-143">The [extraction](onenote-extract-data.md) method to perform, for example:  or .</span></span><br/><span data-ttu-id="99894-144">`extract.businesscard` または `extract.recipe`</span><span class="sxs-lookup"><span data-stu-id="99894-144">`extract.businesscard` or `extract.recipe`</span></span> |
| <span data-ttu-id="99894-145">data-render-src</span><span class="sxs-lookup"><span data-stu-id="99894-145">data-render-src</span></span> | <span data-ttu-id="99894-146">[抽出](onenote-extract-data.md)のコンテンツのソース。</span><span class="sxs-lookup"><span data-stu-id="99894-146">The content source for the [extraction](onenote-extract-data.md).</span></span> |
| <span data-ttu-id="99894-147">style</span><span class="sxs-lookup"><span data-stu-id="99894-147">style</span></span> | <span data-ttu-id="99894-148">div の位置、サイズ、フォント、および色のプロパティ:</span><span class="sxs-lookup"><span data-stu-id="99894-148">The position, size, font, and color properties for the div:</span></span> <ul><li><span data-ttu-id="99894-149">**position** (**absolute** のみ)、**left**、**top**、および **width** (div では height が自動構成されます)</span><span class="sxs-lookup"><span data-stu-id="99894-149">**position** (**absolute** only), **left**, **top**, and **width**. (Height is auto-configured for divs.)</span></span><br/><br/><span data-ttu-id="99894-150">本文が `data-absolute-enabled="true"` に設定されていて、div が本文の直接の子の場合にのみ、[絶対位置](onenote-abs-pos.md)の div の作成に使用されます。</span><span class="sxs-lookup"><span data-stu-id="99894-150">Used to create an [absolute positioned](onenote-abs-pos.md) div, only if the div is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br/><br/><span data-ttu-id="99894-151">例: `<div style="position:absolute;width:360px;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="99894-151">Example: `<div style="position:absolute;width:360px;top:350px;left:300px" ... />`</span></span></li><li><span data-ttu-id="99894-p108">要素の CSS [スタイル](#styles) プロパティ。出力 HTML では、これらの値は適切な子要素でインラインで返されます。</span><span class="sxs-lookup"><span data-stu-id="99894-p108">The CSS [style](#styles) properties of the element. In the output HTML, these values are returned inline on appropriate child elements.</span></span></li></ul> |
 

<span data-ttu-id="99894-154">Microsoft Graph の OneNote API は、すべての本文のコンテンツを 1 つ以上の div でラップします。</span><span class="sxs-lookup"><span data-stu-id="99894-154">The OneNote APIs in Microsoft Graph wrap all body content in at least one div.</span></span> <span data-ttu-id="99894-155">次の場合に、API は既定の div (`data-id="_default"` の属性に設定) を作成して、本文のコンテンツを含めます。</span><span class="sxs-lookup"><span data-stu-id="99894-155">The API creates a default div (attributed with `data-id="_default"`) to contain the body content if:</span></span>

- <span data-ttu-id="99894-p110">入力要素 body の **data-absolute-enabled** 属性が省略されたか、**false** に設定されている。この場合、すべての本文のコンテンツは既定の div に含められます。</span><span class="sxs-lookup"><span data-stu-id="99894-p110">The input body element's **data-absolute-enabled** attribute is omitted or set to **false**. In this case, all body content is put in the default div.</span></span>

- <span data-ttu-id="99894-158">本文の入力要素の **data-absolute-enabled** 属性は\*\* true\*\* ですが、入力 HTML は、[絶対位置に配置された](onenote-abs-pos.md)&nbsp;\*\* div**、**img\*\*、または **object** 要素ではない直接の子を含んでいます。</span><span class="sxs-lookup"><span data-stu-id="99894-158">The input body element's **data-absolute-enabled** attribute is **true**, but the input HTML contains direct children that aren't [absolute positioned](onenote-abs-pos.md)&nbsp;**div**, **img**, or **object** elements.</span></span> <span data-ttu-id="99894-159">この例では、[絶対位置に配置された](onenote-abs-pos.md)&nbsp;\*\* div**、**img\*\*、または **object** 要素ではない直接の子が、既定位置の div に配置されています。</span><span class="sxs-lookup"><span data-stu-id="99894-159">In this case, direct children that aren't [absolute positioned](onenote-abs-pos.md)&nbsp;**div**, **img**, or **object** elements are put in the default div.</span></span>


#### <a name="output-attributes"></a><span data-ttu-id="99894-160">出力属性</span><span class="sxs-lookup"><span data-stu-id="99894-160">Output attributes</span></span>

|<span data-ttu-id="99894-161">出力属性</span><span class="sxs-lookup"><span data-stu-id="99894-161">Output attribute</span></span>|<span data-ttu-id="99894-162">説明</span><span class="sxs-lookup"><span data-stu-id="99894-162">Description</span></span>|
|:------|:------|
| <span data-ttu-id="99894-163">data-id</span><span class="sxs-lookup"><span data-stu-id="99894-163">data-id</span></span> | <span data-ttu-id="99894-164">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="99894-164">A reference for the element.</span></span><br/><br/><span data-ttu-id="99894-165">[ページ コンテンツの更新](onenote-update-page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="99894-165">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="99894-166">id</span><span class="sxs-lookup"><span data-stu-id="99894-166">id</span></span> | <span data-ttu-id="99894-167">要素の一意の生成された ID。</span><span class="sxs-lookup"><span data-stu-id="99894-167">A unique, generated ID for the element.</span></span> <span data-ttu-id="99894-168">`includeIDs=true` クエリ オプションを使用した場合に、[ページの *content* エンドポイントに対する GET 要求](/graph/api/page-get?view=graph-rest-1.0)から返されます。</span><span class="sxs-lookup"><span data-stu-id="99894-168">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="99894-169">[ページ コンテンツの更新](onenote-update-page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="99894-169">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="99894-170">style</span><span class="sxs-lookup"><span data-stu-id="99894-170">style</span></span> | <span data-ttu-id="99894-171">div の位置とサイズのプロパティ。</span><span class="sxs-lookup"><span data-stu-id="99894-171">The position and size properties of the div.</span></span> |
 
### <a name="non-contributing-divs"></a><span data-ttu-id="99894-172">作用していない div</span><span class="sxs-lookup"><span data-stu-id="99894-172">Non-contributing divs</span></span>

<span data-ttu-id="99894-p113">入力 HTML の **div** 要素がページ構造に作用しておらず、OneNote が使用する情報を含んでいない場合、API は div のコンテンツを親または既定の div に移動します。このことは次の例で示しています。</span><span class="sxs-lookup"><span data-stu-id="99894-p113">When a **div** element in the input HTML does not contribute to the page structure or carry information that OneNote uses, the API moves the div's content into the parent or default div. This is illustrated in the following examples.</span></span>

#### <a name="input-html"></a><span data-ttu-id="99894-175">入力 HTML</span><span class="sxs-lookup"><span data-stu-id="99894-175">Input HTML</span></span>

<span data-ttu-id="99894-176">作用していない入れ子型の div を含んでいます。</span><span class="sxs-lookup"><span data-stu-id="99894-176">Contains a non-contributing, nested div.</span></span>

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

#### <a name="output-html"></a><span data-ttu-id="99894-177">出力 HTML</span><span class="sxs-lookup"><span data-stu-id="99894-177">Output HTML</span></span>

> <span data-ttu-id="99894-178">**注:** div のコンテンツは親の div に移動し、入れ子状態の `<div>` タグが削除されました。</span><span class="sxs-lookup"><span data-stu-id="99894-178">**Note:** The div's content was moved to the parent div and the nested `<div>` tags have been removed.</span></span> <span data-ttu-id="99894-179">**data-id** などの意味情報が div に定義されていた場合は、div は保持されています (例: `<div data-id="keep-me">`)。</span><span class="sxs-lookup"><span data-stu-id="99894-179">The div would have been preserved if it defined any semantic information, such as a **data-id** (example: `<div data-id="keep-me">`).</span></span>

```html
<html htmlns="https://www.w3.org/1999/xhtml" lang="en-US">
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


## <a name="img-elements"></a><span data-ttu-id="99894-180">img 要素</span><span class="sxs-lookup"><span data-stu-id="99894-180">Img elements</span></span>

<span data-ttu-id="99894-p115">OneNote ページの画像は **img** 要素で表されます。入力 HTML および出力 HTML では、**img** 要素に次の属性を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="99894-p115">Images on OneNote pages are represented by **img** elements. An **img** element can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="99894-183">入力属性</span><span class="sxs-lookup"><span data-stu-id="99894-183">Input attributes</span></span>

|<span data-ttu-id="99894-184">入力属性</span><span class="sxs-lookup"><span data-stu-id="99894-184">Input attribute</span></span>|<span data-ttu-id="99894-185">説明</span><span class="sxs-lookup"><span data-stu-id="99894-185">Description</span></span>|
|:------|:------|
| <span data-ttu-id="99894-186">alt</span><span class="sxs-lookup"><span data-stu-id="99894-186">alt</span></span> | <span data-ttu-id="99894-187">画像に指定された代替テキスト。</span><span class="sxs-lookup"><span data-stu-id="99894-187">The supplied alt text for the image.</span></span> |
| <span data-ttu-id="99894-188">data-id</span><span class="sxs-lookup"><span data-stu-id="99894-188">data-id</span></span> | <span data-ttu-id="99894-189">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="99894-189">A reference for the element.</span></span><br/><br/><span data-ttu-id="99894-190">[ページ コンテンツの更新](onenote-update-page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="99894-190">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="99894-191">data-render-src</span><span class="sxs-lookup"><span data-stu-id="99894-191">data-render-src</span></span> |<span data-ttu-id="99894-192">**data-render-src** か **src** のいずれかが必要です。</span><span class="sxs-lookup"><span data-stu-id="99894-192">Either **data-render-src** or **src** is required.</span></span><br/><br/><span data-ttu-id="99894-193">OneNote ページ上のビットマップ画像として表示する Web ページ。</span><span class="sxs-lookup"><span data-stu-id="99894-193">The webpage to render as a bit-mapped image on the OneNote page:</span></span><br/><br/> <span data-ttu-id="99894-194">パブリック URL の場合は - `data-render-src="https://..."`。</span><span class="sxs-lookup"><span data-stu-id="99894-194">- `data-render-src="https://..."` for a public URL.</span></span><br/><br/> <span data-ttu-id="99894-195">[マルチパート要求](/graph/api/section-post-pages?view=graph-rest-1.0#example)の "Presentation" ブロックにある画像部分の場合は - `data-render-src="name:BlockName"`。</span><span class="sxs-lookup"><span data-stu-id="99894-195">- `data-render-src="name:BlockName"` for an image part in the "Presentation" block of a [multipart request](/graph/api/section-post-pages?view=graph-rest-1.0#example).</span></span><br/><br/><span data-ttu-id="99894-196">このメソッドは、OneNote ページで忠実に表示できるものよりも複雑な Web ページの場合や、ページにログイン資格情報が必要な場合に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="99894-196">This method is useful when the webpage is more complex than the OneNote page can faithfully render, or when the page requires login credentials.</span></span>|
| <span data-ttu-id="99894-197">data-tag</span><span class="sxs-lookup"><span data-stu-id="99894-197">data-tag</span></span> | <span data-ttu-id="99894-198">要素の[ノート シール](onenote-note-tags.md)。</span><span class="sxs-lookup"><span data-stu-id="99894-198">A [note tag](onenote-note-tags.md) on the element.</span></span> |
| <span data-ttu-id="99894-199">style</span><span class="sxs-lookup"><span data-stu-id="99894-199">style</span></span> |<span data-ttu-id="99894-200">画像の位置とサイズのプロパティ: **position** (**absolute** のみ)、**left**、**top**、**width**、および **height**。</span><span class="sxs-lookup"><span data-stu-id="99894-200">The position and size properties for the image: **position** (**absolute** only), **left**, **top**, **width**, and **height**.</span></span><br/><br/><span data-ttu-id="99894-201">任意の画像のサイズを設定できます。</span><span class="sxs-lookup"><span data-stu-id="99894-201">Size can be set on any image.</span></span><br/><br/><span data-ttu-id="99894-202">位置プロパティは、本文が `data-absolute-enabled="true"` に設定されていて、画像が本文の直接の子である場合にのみ、[絶対位置](onenote-abs-pos.md)の画像の作成に使用されます。</span><span class="sxs-lookup"><span data-stu-id="99894-202">Position properties are used to create an [absolute positioned](onenote-abs-pos.md) image, only if the image is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br/><br/><span data-ttu-id="99894-203">例: `<img style="position:absolute;width:360px;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="99894-203">Example: `<img style="position:absolute;width:360px;top:350px;left:300px" ... />`</span></span><br/><br/><span data-ttu-id="99894-204">出力 HTML では、画像サイズは **width** 属性と **height** 属性で別々に返されます。</span><span class="sxs-lookup"><span data-stu-id="99894-204">In the output HTML, the image size is returned separately in **width** and **height** attributes.</span></span> |
| <span data-ttu-id="99894-205">src</span><span class="sxs-lookup"><span data-stu-id="99894-205">src</span></span> |<span data-ttu-id="99894-206">**src** か **data-render-src** のいずれかが必要です。</span><span class="sxs-lookup"><span data-stu-id="99894-206">Either **src** or **data-render-src** is required.</span></span><br/><br/><span data-ttu-id="99894-207">OneNote ページに表示する画像。</span><span class="sxs-lookup"><span data-stu-id="99894-207">The image to render on the OneNote page:</span></span><br/><br/><span data-ttu-id="99894-208">インターネットで一般に使用可能な画像の URL の場合は - `src="https://..."`。</span><span class="sxs-lookup"><span data-stu-id="99894-208">- `src="https://..."` for a URL to a publicly available image on the internet.</span></span><br/><br/> <span data-ttu-id="99894-209">画像を表すマルチパート要求の名前付き部分の場合は - `src="name:BlockName"`。</span><span class="sxs-lookup"><span data-stu-id="99894-209">- `src="name:BlockName"` for a named part in a multipart request that represents the image.</span></span>|
| <span data-ttu-id="99894-210">width、height</span><span class="sxs-lookup"><span data-stu-id="99894-210">width, height</span></span> | <span data-ttu-id="99894-p116">画像の幅または高さ。ピクセル単位ですが px は付けません。例: `width="400"`</span><span class="sxs-lookup"><span data-stu-id="99894-p116">The width or height of the image, in pixels but without the px. Example: `width="400"`</span></span> |
 
> <span data-ttu-id="99894-213">**注:** OneNote API は入力画像の種類を自動的に検出し、それを **data-fullres-src-type** として出力 HTML に返します。</span><span class="sxs-lookup"><span data-stu-id="99894-213">**Note:** The OneNote APIs automatically detect the input image type, and returns it as the **data-fullres-src-type** in the output HTML.</span></span> <span data-ttu-id="99894-214">API は、**data-src-type** で最適化された画像の種類も返します。</span><span class="sxs-lookup"><span data-stu-id="99894-214">The API also returns the image type of the optimized image in **data-src-type**.</span></span>
 

#### <a name="output-attributes"></a><span data-ttu-id="99894-215">出力属性</span><span class="sxs-lookup"><span data-stu-id="99894-215">Output attributes</span></span>

|<span data-ttu-id="99894-216">出力属性</span><span class="sxs-lookup"><span data-stu-id="99894-216">Output attribute</span></span>|<span data-ttu-id="99894-217">説明</span><span class="sxs-lookup"><span data-stu-id="99894-217">Description</span></span>|
|:------|:------|
| <span data-ttu-id="99894-218">alt</span><span class="sxs-lookup"><span data-stu-id="99894-218">alt</span></span> | <span data-ttu-id="99894-219">画像に指定された代替テキスト。</span><span class="sxs-lookup"><span data-stu-id="99894-219">The supplied alt text for the image.</span></span> |
| <span data-ttu-id="99894-220">data-id</span><span class="sxs-lookup"><span data-stu-id="99894-220">data-id</span></span> | <span data-ttu-id="99894-221">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="99894-221">A reference for the element.</span></span><br/><br/><span data-ttu-id="99894-222">[ページ コンテンツの更新](onenote-update-page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="99894-222">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="99894-223">data-index</span><span class="sxs-lookup"><span data-stu-id="99894-223">data-index</span></span> | <span data-ttu-id="99894-p118">画像の位置。[分割された画像](#split-images)のサポート向け。</span><span class="sxs-lookup"><span data-stu-id="99894-p118">The position of the image. For [split image](#split-images) support.</span></span> |
| <span data-ttu-id="99894-226">data-fullres-src</span><span class="sxs-lookup"><span data-stu-id="99894-226">data-fullres-src</span></span> | <span data-ttu-id="99894-227">最初にページに埋め込まれていた画像リソースのバージョンのエンドポイント。</span><span class="sxs-lookup"><span data-stu-id="99894-227">The endpoint for the version of the image resource that was originally embedded in the page.</span></span> |
| <span data-ttu-id="99894-228">data-fullres-src-type</span><span class="sxs-lookup"><span data-stu-id="99894-228">data-fullres-src-type</span></span> | <span data-ttu-id="99894-229">**data-fullres-src** リソースのメディアの種類。たとえば、`image/png` または`image/jpeg`。</span><span class="sxs-lookup"><span data-stu-id="99894-229">The media type of the **data-fullres-src** resource, for example: `image/png` or `image/jpeg`.</span></span> |
| <span data-ttu-id="99894-230">data-options</span><span class="sxs-lookup"><span data-stu-id="99894-230">data-options</span></span> | <span data-ttu-id="99894-231">ソースの種類。PDF ファイルの場合は **printout**、その他のファイルはいずれも **splitimage**。</span><span class="sxs-lookup"><span data-stu-id="99894-231">The source type: **printout** for PDF files or **splitimage** for all others.</span></span> <span data-ttu-id="99894-232">**data-render-src** 属性で作成された、[分割された画像](#split-images)にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="99894-232">Applies only to [split images](#split-images) created with the **data-render-src** attribute.</span></span> |
| <span data-ttu-id="99894-233">data-render-original-src</span><span class="sxs-lookup"><span data-stu-id="99894-233">data-render-original-src</span></span> | <span data-ttu-id="99894-234">ソース画像が公開されたインターネットの画像で、**data-render-src** 属性を付けて作成された場合の、画像の最初のソース URL。</span><span class="sxs-lookup"><span data-stu-id="99894-234">The original source URL of the image, if the source image is from the public internet and was created with the **data-render-src** attribute.</span></span> |
| <span data-ttu-id="99894-235">data-src-type</span><span class="sxs-lookup"><span data-stu-id="99894-235">data-src-type</span></span> | <span data-ttu-id="99894-236">**src** リソースのメディアの種類。たとえば、`image/png` または`image/jpeg`。</span><span class="sxs-lookup"><span data-stu-id="99894-236">The media type of the **src** resource, for example: `image/png` or `image/jpeg`.</span></span> |
| <span data-ttu-id="99894-237">data-tag</span><span class="sxs-lookup"><span data-stu-id="99894-237">data-tag</span></span> | <span data-ttu-id="99894-238">要素の[ノート シール](onenote-note-tags.md)。</span><span class="sxs-lookup"><span data-stu-id="99894-238">A [note tag](onenote-note-tags.md) on the element.</span></span> |
| <span data-ttu-id="99894-239">id</span><span class="sxs-lookup"><span data-stu-id="99894-239">id</span></span> | <span data-ttu-id="99894-240">要素の一意の生成された ID。</span><span class="sxs-lookup"><span data-stu-id="99894-240">A unique, generated ID for the element.</span></span> <span data-ttu-id="99894-241">`includeIDs=true` クエリ オプションを使用した場合に、[ページの *content* エンドポイントに対する GET 要求](/graph/api/page-get?view=graph-rest-1.0)から返されます。</span><span class="sxs-lookup"><span data-stu-id="99894-241">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="99894-242">[ページ コンテンツの更新](onenote-update-page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="99894-242">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="99894-243">src</span><span class="sxs-lookup"><span data-stu-id="99894-243">src</span></span> | <span data-ttu-id="99894-244">Web ブラウザー、モバイル、およびタブレットのフォーム ファクター向けに最適化された画像リソースのバージョンのエンドポイント。</span><span class="sxs-lookup"><span data-stu-id="99894-244">The endpoint for the version of the image resource that has been optimized for web browsers and mobile and tablet form factors.</span></span> |
| <span data-ttu-id="99894-245">style</span><span class="sxs-lookup"><span data-stu-id="99894-245">style</span></span> | <span data-ttu-id="99894-246">画像の位置のプロパティ。</span><span class="sxs-lookup"><span data-stu-id="99894-246">The position properties of the image.</span></span> |
| <span data-ttu-id="99894-247">width、height</span><span class="sxs-lookup"><span data-stu-id="99894-247">width, height</span></span> | <span data-ttu-id="99894-248">画像の幅または高さ (ピクセル単位)。</span><span class="sxs-lookup"><span data-stu-id="99894-248">The width or height of the image, in pixels.</span></span> |
 

### <a name="output-html-examples-for-images"></a><span data-ttu-id="99894-249">画像の出力 HTML の例</span><span class="sxs-lookup"><span data-stu-id="99894-249">Output HTML examples for images</span></span>

<span data-ttu-id="99894-p121">出力 **img** 要素には、次に示すとおり、画像ファイルのリソースおよび画像の種類のためのエンドポイントが含まれています。バイナリ コンテンツを取得するには、[画像リソースのエンドポイントに対して個別に GET 要求を実行](/graph/api/resource-get?view=graph-rest-1.0)します。</span><span class="sxs-lookup"><span data-stu-id="99894-p121">Output **img** elements contain endpoints for image file resources and the image type, as shown below. You can make separate [GET requests to image resource endpoints](/graph/api/resource-get?view=graph-rest-1.0) to retrieve their binary contents.</span></span>

```html
<img 
    src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/$value"  
    data-src-type="image/png"
    data-fullres-src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/$value"  
    data-fullres-src-type="image/png" ... />
```

<span data-ttu-id="99894-p122">既定では、画像は、ページ コンテンツの残りの部分と同様、それらを取得するために承認を必要とするため、ブラウザーで直接表示されることはありません。ページにある画像リソースへの公開 URL を取得するには、ページ コンテンツを取得する際に、クエリ文字列に **preAuthenticated=true** を含めます (例: `GET ../pages/{page-id}/content?preAuthenticated=true`)。返される公開 URL は 1 時間有効です。</span><span class="sxs-lookup"><span data-stu-id="99894-p122">By default, images won't render directly in a browser because they are private and require authorization to retrieve them, like the rest of the page contents. To get public URLs to the image resources on a page, include **preAuthenticated=true** in the query string when you retrieve the page content (example: `GET ../pages/{page-id}/content?preAuthenticated=true`). The public URLs that are returned are valid for one hour.</span></span> 

#### <a name="image-with-public-url-when-preauthenticatedtrue-is-included-in-the-request"></a><span data-ttu-id="99894-255">要求に _preAuthenticated=true_ が含まれる場合の、パブリック URL を使用する画像</span><span class="sxs-lookup"><span data-stu-id="99894-255">Image with public URL when _preAuthenticated=true_ is included in the request</span></span>

```html
<img 
    width="170" height="128" 
    src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/content?publicAuth=true&mimeType=image/jpeg" 
    data-src-type="image/{type}" 
    data-fullres-src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/content?publicAuth=true&mimeType=image/jpeg" 
    data-fullres-src-type="image/{type}"
/>
```

<span data-ttu-id="99894-256">次の例は、**img** 要素が出力 HTML に含む可能性がある情報を示しています。</span><span class="sxs-lookup"><span data-stu-id="99894-256">The following examples show the information an **img** element might contain in the output HTML.</span></span>

#### <a name="image-with-web-ready-and-high-resolution-resources"></a><span data-ttu-id="99894-257">Web 対応の高解像度リソースがある画像</span><span class="sxs-lookup"><span data-stu-id="99894-257">Image with web-ready and high resolution resources</span></span>

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

#### <a name="image-created-by-using-the-data-render-src-attribute"></a><span data-ttu-id="99894-258">*data-render-src* 属性を使用して作成された画像</span><span class="sxs-lookup"><span data-stu-id="99894-258">Image created by using the *data-render-src* attribute</span></span>

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

### <a name="split-images"></a><span data-ttu-id="99894-259">分割された画像</span><span class="sxs-lookup"><span data-stu-id="99894-259">Split images</span></span>

<span data-ttu-id="99894-p123">**data-render-src** 属性 (Web ページの URL または名前が付いた部分のもの) を使用して作成された画像は、パフォーマンスと表示上の理由から複数のコンポーネントの画像に分割されることがあります。コンポーネント画像には、すべて同じ **data-id** 値が割り当てられます。各コンポーネントの画像には、元の垂直レイアウトを定義するゼロベースの data-index 属性があります。</span><span class="sxs-lookup"><span data-stu-id="99894-p123">Images that are created using the **data-render-src** attribute (from a webpage URL or a named part) might be split into multiple component images for performance and rendering reasons. Component images are all assigned the same **data-id** value. Each component image has a zero-based data-index attribute that defines the original vertical layout.</span></span>

#### <a name="split-image-with-three-component-images"></a><span data-ttu-id="99894-263">画像を 3 つのコンポーネントの画像に分割する</span><span class="sxs-lookup"><span data-stu-id="99894-263">Split image with three component images</span></span>

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

<span data-ttu-id="99894-264">ユーザーがページ上で画像を移動することができるため、返されるインデックスが適切な順序になっていない場合があります。</span><span class="sxs-lookup"><span data-stu-id="99894-264">Because users can move the images on the page, the returned indexes might be out of order. Ordering should be in top to bottom y-order, then left to right x-order if there are y-order conflicts.</span></span> <span data-ttu-id="99894-265">順序は、y 方向に上から下へ、そしてもし y 方向で競合があれば x 方向に左から右へとなっていなければなりません。</span><span class="sxs-lookup"><span data-stu-id="99894-265">Because users can move the images on the page, the returned indexes might be out of order. Ordering should be in top to bottom y-order, then left to right x-order if there are y-order conflicts.</span></span>

## <a name="iframe-elements"></a><span data-ttu-id="99894-266">iframe 要素</span><span class="sxs-lookup"><span data-stu-id="99894-266">iframe elements</span></span>

<span data-ttu-id="99894-267">OneNote ページには、**iframe** 要素で表される埋め込みビデオを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="99894-267">OneNote pages can contain embedded videos represented by **iframe** elements.</span></span> 

> <span data-ttu-id="99894-268">**注:** [**object** 要素を使用してビデオ ファイルを添付する](onenote-images-files.md#adding-files)こともできます。</span><span class="sxs-lookup"><span data-stu-id="99894-268">**Note:** You can also [attach a video file using an **object** element](onenote-images-files.md#adding-files).</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="99894-269">入力属性</span><span class="sxs-lookup"><span data-stu-id="99894-269">Input attributes</span></span>

|<span data-ttu-id="99894-270">入力属性</span><span class="sxs-lookup"><span data-stu-id="99894-270">Input attribute</span></span>|<span data-ttu-id="99894-271">説明</span><span class="sxs-lookup"><span data-stu-id="99894-271">Description</span></span>|
|:------|:------|
| <span data-ttu-id="99894-272">data-original-src</span><span class="sxs-lookup"><span data-stu-id="99894-272">data-original-src</span></span> | <span data-ttu-id="99894-273">必須。</span><span class="sxs-lookup"><span data-stu-id="99894-273">Required.</span></span> <span data-ttu-id="99894-274">ビデオ ソースの URL。</span><span class="sxs-lookup"><span data-stu-id="99894-274">The URL of the video source.</span></span> <span data-ttu-id="99894-275">[サポートされるビデオ ソースの一覧](onenote-images-files.md#adding-videos)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="99894-275">See the [list of supported video sources](onenote-images-files.md#adding-videos).</span></span> <br/><br/><span data-ttu-id="99894-276">例: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span><span class="sxs-lookup"><span data-stu-id="99894-276">Example: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span></span> |
| <span data-ttu-id="99894-277">width、height</span><span class="sxs-lookup"><span data-stu-id="99894-277">width, height</span></span> | <span data-ttu-id="99894-p126">iframe の幅と高さ (ピクセル単位)。例: `width=300`</span><span class="sxs-lookup"><span data-stu-id="99894-p126">The width or height of the iframe, in pixels. Example: `width=300`</span></span> |

#### <a name="output-attributes"></a><span data-ttu-id="99894-280">出力属性</span><span class="sxs-lookup"><span data-stu-id="99894-280">Output attributes</span></span>

|<span data-ttu-id="99894-281">出力属性</span><span class="sxs-lookup"><span data-stu-id="99894-281">Output attribute</span></span>|<span data-ttu-id="99894-282">説明</span><span class="sxs-lookup"><span data-stu-id="99894-282">Description</span></span>|
|:------|:------|
| <span data-ttu-id="99894-283">data-original-src</span><span class="sxs-lookup"><span data-stu-id="99894-283">data-original-src</span></span> | <span data-ttu-id="99894-284">ビデオ ソースの URL。</span><span class="sxs-lookup"><span data-stu-id="99894-284">The URL of the video source.</span></span> |
| <span data-ttu-id="99894-285">src</span><span class="sxs-lookup"><span data-stu-id="99894-285">src</span></span> | <span data-ttu-id="99894-286">OneNote ページに埋め込まれたビデオへのリンク。</span><span class="sxs-lookup"><span data-stu-id="99894-286">A link to the video that is embedded in the OneNote page.</span></span> |
| <span data-ttu-id="99894-287">width、height</span><span class="sxs-lookup"><span data-stu-id="99894-287">width, height</span></span> | <span data-ttu-id="99894-288">iframe の幅と高さ (ピクセル単位)。</span><span class="sxs-lookup"><span data-stu-id="99894-288">The width or height of the iframe, in pixels.</span></span><br/><br/><span data-ttu-id="99894-289">例: `width=300`</span><span class="sxs-lookup"><span data-stu-id="99894-289">Example: `width=300`</span></span> |
 
### <a name="output-html-example-for-videos"></a><span data-ttu-id="99894-290">ビデオの出力 HTML の例</span><span class="sxs-lookup"><span data-stu-id="99894-290">Output HTML example for videos</span></span>

<span data-ttu-id="99894-291">次に示すように、出力 **iframe** 要素には、ソース ページとビデオに関連付けられたエンドポイントが含まれています。</span><span class="sxs-lookup"><span data-stu-id="99894-291">Output **iframe** elements contain endpoints that link to the source page and video, as shown.</span></span> 

```html
<iframe 
    width="340" height="280" 
    data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8" 
    src="https://www.youtube.com/embed/3Ztr44aKmQ8?feature=oembed&autoplay=true" />
``` 

## <a name="object-elements"></a><span data-ttu-id="99894-292">object 要素</span><span class="sxs-lookup"><span data-stu-id="99894-292">Object elements</span></span>

<span data-ttu-id="99894-p127">OneNote ページには、**object** 要素で表される添付ファイルを含めることができます。**object** 要素は、入力 HTML および出力 HTML に次の属性を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="99894-p127">OneNote pages can contain file attachments represented by **object** elements. An **object** element can contain the following attributes in the input and output HTML.</span></span>

> <span data-ttu-id="99894-295">**注:** ファイルが画像として送信され、**data-render-src** 属性を使用する場合、OneNote API はファイルのコンテンツを画像としてページに表示できます。</span><span class="sxs-lookup"><span data-stu-id="99894-295">**Note:** The OneNote APIs can also render file content as images in a page when the file is sent as an image and uses the **data-render-src** attribute.</span></span>
> <span data-ttu-id="99894-296">例: `<img data-render-src="name:part-name" ... />`</span><span class="sxs-lookup"><span data-stu-id="99894-296">Example: `<img data-render-src="name:part-name" ... />`</span></span>
 

#### <a name="input-attributes"></a><span data-ttu-id="99894-297">入力属性</span><span class="sxs-lookup"><span data-stu-id="99894-297">Input attributes</span></span>

|<span data-ttu-id="99894-298">入力属性</span><span class="sxs-lookup"><span data-stu-id="99894-298">Input attribute</span></span>|<span data-ttu-id="99894-299">説明</span><span class="sxs-lookup"><span data-stu-id="99894-299">Description</span></span>|
|:------|:------|
| <span data-ttu-id="99894-300">data</span><span class="sxs-lookup"><span data-stu-id="99894-300">data</span></span> | <span data-ttu-id="99894-p129">必須。[マルチパート要求](/graph/api/section-post-pages?view=graph-rest-1.0#example)のファイルを表す部分の名前。</span><span class="sxs-lookup"><span data-stu-id="99894-p129">Required. The name of the part that represents the file in the [multipart request](/graph/api/section-post-pages?view=graph-rest-1.0#example).</span></span> |
| <span data-ttu-id="99894-303">data-attachment</span><span class="sxs-lookup"><span data-stu-id="99894-303">data-attachment</span></span> | <span data-ttu-id="99894-p130">必須。ファイル名。</span><span class="sxs-lookup"><span data-stu-id="99894-p130">Required. The file name.</span></span> |
| <span data-ttu-id="99894-306">data-id</span><span class="sxs-lookup"><span data-stu-id="99894-306">data-id</span></span> | <span data-ttu-id="99894-307">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="99894-307">A reference for the element.</span></span><br/><br/><span data-ttu-id="99894-308">[ページ コンテンツの更新](onenote-update-page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="99894-308">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="99894-309">style</span><span class="sxs-lookup"><span data-stu-id="99894-309">style</span></span> | <span data-ttu-id="99894-310">オブジェクトの位置とサイズのプロパティ: **position** (**absolute** のみ)、**left**、**top**、および **width**。</span><span class="sxs-lookup"><span data-stu-id="99894-310">The position and size properties for the object: **position** (**absolute** only), **left**, **top**, and **width**.</span></span><br/><br/><span data-ttu-id="99894-311">本文が `data-absolute-enabled="true"` に設定されていて、オブジェクトが本文の直接の子の場合にのみ、[絶対位置](onenote-abs-pos.md)のオブジェクトの作成に使用されます。</span><span class="sxs-lookup"><span data-stu-id="99894-311">Used to create an [absolute positioned](onenote-abs-pos.md) object, only if the object is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br/><br/><span data-ttu-id="99894-312">例: `<object style="position:absolute;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="99894-312">Example: `<object style="position:absolute;top:350px;left:300px" ... />`</span></span> |
| <span data-ttu-id="99894-313">type</span><span class="sxs-lookup"><span data-stu-id="99894-313">type</span></span> | <span data-ttu-id="99894-314">必須。</span><span class="sxs-lookup"><span data-stu-id="99894-314">Required.</span></span><br/><br/><span data-ttu-id="99894-315">標準のメディア ファイルの種類。</span><span class="sxs-lookup"><span data-stu-id="99894-315">The standard media file type.</span></span> <span data-ttu-id="99894-316">ファイルの種類が既知の場合は、OneNote ページ上でそのファイルの種類に関連付けられているアイコンが表示されます。</span><span class="sxs-lookup"><span data-stu-id="99894-316">Required. The standard media file type. Known file types display the icon associated with the file type on the OneNote page. Unknown file types display a generic file icon.</span></span> <span data-ttu-id="99894-317">ファイルの種類が不明の場合は、一般的なファイル アイコンが表示されます。</span><span class="sxs-lookup"><span data-stu-id="99894-317">Unknown file types display a generic file icon.</span></span> |
<!--todo: add link to known file types--> 

#### <a name="output-attributes"></a><span data-ttu-id="99894-318">出力属性</span><span class="sxs-lookup"><span data-stu-id="99894-318">Output attributes</span></span>

|<span data-ttu-id="99894-319">出力属性</span><span class="sxs-lookup"><span data-stu-id="99894-319">Output attribute</span></span>|<span data-ttu-id="99894-320">説明</span><span class="sxs-lookup"><span data-stu-id="99894-320">Description</span></span>|
|:------|:------|
| <span data-ttu-id="99894-321">data</span><span class="sxs-lookup"><span data-stu-id="99894-321">data</span></span> | <span data-ttu-id="99894-322">ファイルのリソースのエンドポイント。</span><span class="sxs-lookup"><span data-stu-id="99894-322">The endpoint for the file resource.</span></span> |
| <span data-ttu-id="99894-323">data-attachment</span><span class="sxs-lookup"><span data-stu-id="99894-323">data-attachment</span></span> | <span data-ttu-id="99894-324">ファイル名。</span><span class="sxs-lookup"><span data-stu-id="99894-324">The file name.</span></span> |
| <span data-ttu-id="99894-325">data-id</span><span class="sxs-lookup"><span data-stu-id="99894-325">data-id</span></span> | <span data-ttu-id="99894-326">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="99894-326">A reference for the element.</span></span><br/><br/><span data-ttu-id="99894-327">[ページ コンテンツの更新](onenote-update-page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="99894-327">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="99894-328">id</span><span class="sxs-lookup"><span data-stu-id="99894-328">id</span></span> | <span data-ttu-id="99894-329">要素の一意の生成された ID。</span><span class="sxs-lookup"><span data-stu-id="99894-329">A unique, generated ID for the element.</span></span> <span data-ttu-id="99894-330">`includeIDs=true` クエリ オプションを使用した場合に、[ページの *content* エンドポイントに対する GET 要求](/graph/api/page-get?view=graph-rest-1.0)から返されます。</span><span class="sxs-lookup"><span data-stu-id="99894-330">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="99894-331">[ページ コンテンツの更新](onenote-update-page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="99894-331">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="99894-332">style</span><span class="sxs-lookup"><span data-stu-id="99894-332">style</span></span> | <span data-ttu-id="99894-333">オブジェクトの位置のプロパティ。</span><span class="sxs-lookup"><span data-stu-id="99894-333">The position properties of the object.</span></span> |
| <span data-ttu-id="99894-334">type</span><span class="sxs-lookup"><span data-stu-id="99894-334">type</span></span> | <span data-ttu-id="99894-335">標準のメディア ファイルの種類。</span><span class="sxs-lookup"><span data-stu-id="99894-335">The standard media file type.</span></span> |
 

#### <a name="output-html-example-for-objects"></a><span data-ttu-id="99894-336">オブジェクトの出力 HTML の例</span><span class="sxs-lookup"><span data-stu-id="99894-336">Output HTML example for objects</span></span>

<span data-ttu-id="99894-337">次に示すように、出力 **object** 要素には、ページ内のファイル リソースにリンクされたエンドポイントが含まれています。</span><span class="sxs-lookup"><span data-stu-id="99894-337">Output **object** elements contain endpoints that link to the file resources in the page, as shown.</span></span> <span data-ttu-id="99894-338">バイナリ コンテンツを取得するには、これらの[ファイル リソースのエンドポイントに対して個別の GET 要求](/graph/api/resource-get?view=graph-rest-1.0)を実行します。</span><span class="sxs-lookup"><span data-stu-id="99894-338">You can make separate [GET requests to file resource endpoints](/graph/api/resource-get?view=graph-rest-1.0) to retrieve their binary contents.</span></span>

```html
<object
    data="https://graph.microsoft.com/v1.0/me/onenote/resources/{file-id}/$value"
    data-attachment="fileName.pdf" 
    type="application/pdf" 
    [style="..."] />
``` 

## <a name="paragraphs-and-headings"></a><span data-ttu-id="99894-339">段落と見出し</span><span class="sxs-lookup"><span data-stu-id="99894-339">Paragraphs and headings</span></span>

<span data-ttu-id="99894-340">段落、見出し、その他のテキストのコンテナーには、入力 HTML と出力 HTML の次の属性を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="99894-340">Paragraphs, headings, and other text containers can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="99894-341">入力属性</span><span class="sxs-lookup"><span data-stu-id="99894-341">Input attributes</span></span>

|<span data-ttu-id="99894-342">入力属性</span><span class="sxs-lookup"><span data-stu-id="99894-342">Input attribute</span></span>|<span data-ttu-id="99894-343">説明</span><span class="sxs-lookup"><span data-stu-id="99894-343">Description</span></span>|
|:------|:------|
| <span data-ttu-id="99894-344">data-id</span><span class="sxs-lookup"><span data-stu-id="99894-344">data-id</span></span> | <span data-ttu-id="99894-345">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="99894-345">A reference for the element.</span></span><br/><br/><span data-ttu-id="99894-346">[ページ コンテンツの更新](onenote-update-page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="99894-346">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="99894-347">data-tag</span><span class="sxs-lookup"><span data-stu-id="99894-347">data-tag</span></span> | <span data-ttu-id="99894-348">**p** 要素または **h1** - **h6** 要素上の[ノート シール](onenote-note-tags.md)。</span><span class="sxs-lookup"><span data-stu-id="99894-348">A [note tag](onenote-note-tags.md) on a **p** or **h1** - **h6** element.</span></span> |
| <span data-ttu-id="99894-349">style</span><span class="sxs-lookup"><span data-stu-id="99894-349">style</span></span> | <span data-ttu-id="99894-350">要素の CSS [スタイル](#styles)のプロパティ。</span><span class="sxs-lookup"><span data-stu-id="99894-350">The CSS [style](#styles) properties of the element.</span></span> |
 

#### <a name="output-attributes"></a><span data-ttu-id="99894-351">出力属性</span><span class="sxs-lookup"><span data-stu-id="99894-351">Output attributes</span></span>

|<span data-ttu-id="99894-352">出力属性</span><span class="sxs-lookup"><span data-stu-id="99894-352">Output attribute</span></span>|<span data-ttu-id="99894-353">説明</span><span class="sxs-lookup"><span data-stu-id="99894-353">Description</span></span>|
|:------|:------|
| <span data-ttu-id="99894-354">data-id</span><span class="sxs-lookup"><span data-stu-id="99894-354">data-id</span></span> | <span data-ttu-id="99894-355">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="99894-355">A reference for the element.</span></span><br/><br/><span data-ttu-id="99894-356">[ページ コンテンツの更新](onenote-update-page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="99894-356">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="99894-357">data-tag</span><span class="sxs-lookup"><span data-stu-id="99894-357">data-tag</span></span> | <span data-ttu-id="99894-358">**p** 要素または **h1** - **h6** 要素上の[ノート シール](onenote-note-tags.md)。</span><span class="sxs-lookup"><span data-stu-id="99894-358">A [note tag](onenote-note-tags.md) on a **p** or **h1** - **h6** element.</span></span> |
| <span data-ttu-id="99894-359">id</span><span class="sxs-lookup"><span data-stu-id="99894-359">id</span></span> | <span data-ttu-id="99894-360">要素の一意の生成された ID。</span><span class="sxs-lookup"><span data-stu-id="99894-360">A unique, generated ID for the element.</span></span> <span data-ttu-id="99894-361">`includeIDs=true` クエリ オプションを使用した場合に、[ページの *content* エンドポイントに対する GET 要求](/graph/api/page-get?view=graph-rest-1.0)から返されます。</span><span class="sxs-lookup"><span data-stu-id="99894-361">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="99894-362">[ページ コンテンツの更新](onenote-update-page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="99894-362">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="99894-363">style</span><span class="sxs-lookup"><span data-stu-id="99894-363">style</span></span> | <span data-ttu-id="99894-p135">要素の CSS [style](#styles)のプロパティ。出力 HTML では、これらの値は、適切な子要素または **span** 要素でインラインで返すことができます。</span><span class="sxs-lookup"><span data-stu-id="99894-p135">The CSS [style](#styles) properties of the element. In the output HTML, these values may be returned inline on appropriate child elements or on **span** elements.</span></span> |
 

<span data-ttu-id="99894-366">次の例では、テキストのコンテナーおよび返される出力 HTML にスタイルを定義するさまざまな方法を使用する入力 HTML を示しています。</span><span class="sxs-lookup"><span data-stu-id="99894-366">The following examples show input HTML that uses different ways to define styles on text containers and the output HTML that's returned.</span></span>

#### <a name="input-html-with-styles-defined-using-inline-character-styles-in-the-start-tag-and-within-a-span-element"></a><span data-ttu-id="99894-367">開始タグ内、および span 要素内に、インライン文字スタイルを使用して定義されたスタイル付き入力 HTML。</span><span class="sxs-lookup"><span data-stu-id="99894-367">Input HTML with styles defined using inline character styles, in the start tag, and within a span element.</span></span>

```html
<h1>Heading <i>One</i> text</h1>
<p style="font-size:8pt;color:green;font-family:Courier;text-align:center">Some text</p>
<p>Some <span  style="font-size:16px;color:#ff0000;font-family:Segoe UI Black">more</span> text</p>
``` 

#### <a name="output-html-with-the-i-character-style-and-the-font-settings-in-the-p-start-tag-returned-as-inline-css-styles-on-span-elements"></a><span data-ttu-id="99894-368">`<i>` 文字スタイルと `<p>` 開始タグ内のフォント設定が span 要素のインライン CSS スタイルとして返された出力 HTML。</span><span class="sxs-lookup"><span data-stu-id="99894-368">Output HTML with the `<i>` character style and the font settings in the `<p>` start tag returned as inline CSS styles on span elements.</span></span>

```html
<h1 style="font-size:16pt;color:#1e4e79;margin-top:11pt;margin-bottom:11pt">Heading <span style="font-style:italic">One</span> text</h1>
<p style="text-align:center"><span style="font-family:Courier;font-size:8pt;color:green">Some text</span></p>
<p>Some <span style="font-family:Segoe UI Black;font-size:12pt;color:red">more</span> text</p>
``` 


## <a name="lists"></a><span data-ttu-id="99894-369">リスト</span><span class="sxs-lookup"><span data-stu-id="99894-369">Lists</span></span>

<span data-ttu-id="99894-370">リストは、**li** 要素を含む **ol** 要素または **ul** 要素として表されます。</span><span class="sxs-lookup"><span data-stu-id="99894-370">Lists are represented as **ol** or **ul** elements that contain list items represented as **li** elements.</span></span>

<span data-ttu-id="99894-371">入力 HTML および出力 HTML には、リストとリスト項目に次の属性を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="99894-371">Lists and list items can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="99894-372">入力属性</span><span class="sxs-lookup"><span data-stu-id="99894-372">Input attributes</span></span>

|<span data-ttu-id="99894-373">入力属性</span><span class="sxs-lookup"><span data-stu-id="99894-373">Input attribute</span></span>|<span data-ttu-id="99894-374">説明</span><span class="sxs-lookup"><span data-stu-id="99894-374">Description</span></span>|
|:------|:------|
| <span data-ttu-id="99894-375">data-id</span><span class="sxs-lookup"><span data-stu-id="99894-375">data-id</span></span> | <span data-ttu-id="99894-376">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="99894-376">A reference for the element.</span></span><br/><br/><span data-ttu-id="99894-377">[ページ コンテンツの更新](onenote-update-page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="99894-377">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="99894-378">data-tag</span><span class="sxs-lookup"><span data-stu-id="99894-378">data-tag</span></span> | <span data-ttu-id="99894-379">**ul**、**ol**、または **li** の各要素上の[ノート シール](onenote-note-tags.md)。</span><span class="sxs-lookup"><span data-stu-id="99894-379">A [note tag](onenote-note-tags.md) on a **ul**, **ol**, or **li** element.</span></span> |
| <span data-ttu-id="99894-380">style</span><span class="sxs-lookup"><span data-stu-id="99894-380">style</span></span> | <span data-ttu-id="99894-381">リストまたはリスト項目の **list-style-type** および CSS [style](#styles) のプロパティ。</span><span class="sxs-lookup"><span data-stu-id="99894-381">The **list-style-type** and the CSS [style](#styles) properties for the list or list item.</span></span> |
 

#### <a name="output-attributes"></a><span data-ttu-id="99894-382">出力属性</span><span class="sxs-lookup"><span data-stu-id="99894-382">Output attributes</span></span>

|<span data-ttu-id="99894-383">出力属性</span><span class="sxs-lookup"><span data-stu-id="99894-383">Output attribute</span></span>|<span data-ttu-id="99894-384">説明</span><span class="sxs-lookup"><span data-stu-id="99894-384">Description</span></span>|
|:------|:------|
| <span data-ttu-id="99894-385">data-id</span><span class="sxs-lookup"><span data-stu-id="99894-385">data-id</span></span> | <span data-ttu-id="99894-386">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="99894-386">A reference for the element.</span></span><br/><br/><span data-ttu-id="99894-387">[ページ コンテンツの更新](onenote-update-page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="99894-387">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="99894-388">data-tag</span><span class="sxs-lookup"><span data-stu-id="99894-388">data-tag</span></span> |  <span data-ttu-id="99894-389">**li** 要素内の span 上の[ノート シール](onenote-note-tags.md)。</span><span class="sxs-lookup"><span data-stu-id="99894-389">A [note tag](onenote-note-tags.md) on a span in a **li** element.</span></span> |
| <span data-ttu-id="99894-390">ID</span><span class="sxs-lookup"><span data-stu-id="99894-390">id</span></span> | <span data-ttu-id="99894-391">要素の一意の生成された ID。</span><span class="sxs-lookup"><span data-stu-id="99894-391">A unique, generated ID for the element.</span></span> <span data-ttu-id="99894-392">`includeIDs=true` クエリ オプションを使用した場合に、[ページの *content* エンドポイントに対する GET 要求](/graph/api/page-get?view=graph-rest-1.0)から返されます。</span><span class="sxs-lookup"><span data-stu-id="99894-392">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="99894-393">[ページ コンテンツの更新](onenote-update-page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="99894-393">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="99894-394">style</span><span class="sxs-lookup"><span data-stu-id="99894-394">style</span></span> | <span data-ttu-id="99894-p137">要素の **list-style-type** および CSS [style](#styles)のプロパティ。出力 HTML では、リストレベル設定はリスト項目で返されます。既定のプロパティは返されません。</span><span class="sxs-lookup"><span data-stu-id="99894-p137">The **list-style-type** and CSS [style](#styles) properties of the element. In the output HTML, list-level settings are returned on list items. Default properties are not returned.</span></span> |
 
### <a name="list-styles"></a><span data-ttu-id="99894-398">リストのスタイル</span><span class="sxs-lookup"><span data-stu-id="99894-398">List styles</span></span>

<span data-ttu-id="99894-399">Microsoft Graph の OneNote API では、次のリストのスタイルをサポートします。</span><span class="sxs-lookup"><span data-stu-id="99894-399">The OneNote APIs in Microsoft Graph support the following list styles:</span></span>

|<span data-ttu-id="99894-400">番号付きリスト</span><span class="sxs-lookup"><span data-stu-id="99894-400">Ordered list</span></span>|<span data-ttu-id="99894-401">記号付きリスト</span><span class="sxs-lookup"><span data-stu-id="99894-401">Unordered list</span></span>|
|:------|:------|
| <span data-ttu-id="99894-402">none</span><span class="sxs-lookup"><span data-stu-id="99894-402">none</span></span> | <span data-ttu-id="99894-403">none</span><span class="sxs-lookup"><span data-stu-id="99894-403">none</span></span> |
| <span data-ttu-id="99894-404">decimal (default)</span><span class="sxs-lookup"><span data-stu-id="99894-404">decimal (default)</span></span> | <span data-ttu-id="99894-405">disc (default)</span><span class="sxs-lookup"><span data-stu-id="99894-405">disc (default)</span></span> |
| <span data-ttu-id="99894-406">lower-alpha</span><span class="sxs-lookup"><span data-stu-id="99894-406">lower-alpha</span></span> | <span data-ttu-id="99894-407">Circle</span><span class="sxs-lookup"><span data-stu-id="99894-407">circle</span></span> |
| <span data-ttu-id="99894-408">lower-roman</span><span class="sxs-lookup"><span data-stu-id="99894-408">lower-roman</span></span> | <span data-ttu-id="99894-409">square</span><span class="sxs-lookup"><span data-stu-id="99894-409">square</span></span> |
| <span data-ttu-id="99894-410">upper-alpha</span><span class="sxs-lookup"><span data-stu-id="99894-410">upper-alpha</span></span> | &nbsp; |
| <span data-ttu-id="99894-411">upper-roman</span><span class="sxs-lookup"><span data-stu-id="99894-411">upper-roman</span></span> | &nbsp; |
 
<span data-ttu-id="99894-412">入力 HTML の **ol** 要素または **ul** 要素のリストにはグローバル スタイルを適用できますが、スタイルは **li** 要素で返されます。</span><span class="sxs-lookup"><span data-stu-id="99894-412">You can apply global styles for a list on the **ol** or **ul** element in the input HTML, but styles are returned on the **li** elements.</span></span>

#### <a name="homogenous-list-style"></a><span data-ttu-id="99894-413">同種リスト スタイル</span><span class="sxs-lookup"><span data-stu-id="99894-413">Homogenous list style</span></span>

<span data-ttu-id="99894-414">この例は、**ol** 要素のリスト スタイルの種類と個々のリスト項目の CSS スタイルを設定する入力 HTML を示しています。</span><span class="sxs-lookup"><span data-stu-id="99894-414">This example shows input HTML that sets the list style type on the **ol** element and CSS styles on individual list items.</span></span>

```html
<ol style="list-style-type:upper-roman;color:blue">
    <li style="font-weight:bold">Jacksonville</li>
    <li style="text-decoration:line-through">Orlando</li>
    <li style="font-family:Courier">Naples</li>
</ol>
``` 

<span data-ttu-id="99894-p138">これは出力 HTML です。スタイルが個々の **li** 要素または **span** 要素でインラインで返されることに注目してください。</span><span class="sxs-lookup"><span data-stu-id="99894-p138">This is the output HTML. Notice that styles are returned inline on the individual **li** or **span** elements.</span></span>

```html
<ol>
    <li style="list-style-type:upper-roman"><span style="color:blue;font-weight:bold">Jacksonville</span></li>
    <li style="list-style-type:upper-roman"><span style="color:blue;text-decoration:line-through">Orlando</span></li>
    <li style="list-style-type:upper-roman"><span style="font-family:Courier;color:blue">Naples</span></li>
</ol>
``` 

#### <a name="variable-list-styles"></a><span data-ttu-id="99894-417">可変のリスト スタイル</span><span class="sxs-lookup"><span data-stu-id="99894-417">Variable list styles</span></span>

<span data-ttu-id="99894-418">この例は、**li** 要素にさまざまなリスト スタイルの種類を設定する入力 HTML を示しています。</span><span class="sxs-lookup"><span data-stu-id="99894-418">This example shows input HTML that sets different list style types on the **li** elements.</span></span>

```html
<ul style="font-style:italic">
    <li style="list-style-type:square">square style</li>
    <li style="list-style-type:circle">circle style</li>
    <li style="list-style-type:disc">disc style (default)</li>
</ul>
``` 

<span data-ttu-id="99894-p139">これは出力 HTML です。スタイルが個々の **li** 要素または **span** 要素でインラインで返されることに注目してください。</span><span class="sxs-lookup"><span data-stu-id="99894-p139">This is the output HTML. Notice that styles are returned inline on the individual **li** or **span** elements.</span></span>

```html
<ul>
    <li style="list-style-type:square"><span style="font-style:italic">square style</span></li>
    <li style="list-style-type:circle"><span style="font-style:italic">circle style</span></li>
    <li><span style="font-style:italic">disc style (default)</span></li>
</ul>
``` 


## <a name="tables"></a><span data-ttu-id="99894-421">テーブル</span><span class="sxs-lookup"><span data-stu-id="99894-421">Tables</span></span>

<span data-ttu-id="99894-p140">テーブルは、**tr** 要素および **td** 要素を含めることができる **table** 要素として表されます。入れ子型のテーブルがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="99894-p140">Tables are represented as **table** elements that can contain **tr** and **td** elements. Nested tables are supported.</span></span>

<span data-ttu-id="99894-424">入力 HTML と出力 HTML では、テーブルに次の属性を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="99894-424">Tables can contain the following attributes in the input and output HTML.</span></span> <span data-ttu-id="99894-425">OneNote API では、**rowspan** 属性または **colspan** 属性はサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="99894-425">The OneNote APIs do not support **rowspan** or **colspan** attributes.</span></span> 

#### <a name="input-attributes"></a><span data-ttu-id="99894-426">入力属性</span><span class="sxs-lookup"><span data-stu-id="99894-426">Input attributes</span></span>

|<span data-ttu-id="99894-427">入力属性</span><span class="sxs-lookup"><span data-stu-id="99894-427">Input attribute</span></span>|<span data-ttu-id="99894-428">説明</span><span class="sxs-lookup"><span data-stu-id="99894-428">Description</span></span>|
|:------|:------|
| <span data-ttu-id="99894-429">data-id</span><span class="sxs-lookup"><span data-stu-id="99894-429">data-id</span></span> | <span data-ttu-id="99894-430">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="99894-430">A reference for the element.</span></span><br/><br/><span data-ttu-id="99894-431">[ページ コンテンツの更新](onenote-update-page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="99894-431">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="99894-432">style</span><span class="sxs-lookup"><span data-stu-id="99894-432">style</span></span> | <span data-ttu-id="99894-433">要素の CSS の [style](#styles)のプロパティ、および:</span><span class="sxs-lookup"><span data-stu-id="99894-433">The CSS [style](#styles) properties of the element, and also:</span></span><br/> <span data-ttu-id="99894-p142">- **border**。0px または 1px のいずれか。</span><span class="sxs-lookup"><span data-stu-id="99894-p142">- **border**. Can be either 0px or 1px.</span></span><br/> <span data-ttu-id="99894-p143">- **width**。**table** および **td** でサポートされます。ピクセル数またはページ幅のパーセンテージを使用します。</span><span class="sxs-lookup"><span data-stu-id="99894-p143">- **width**. Supported by **table** and **td** as pixels or percentage of page width.</span></span><br/><br/><span data-ttu-id="99894-438">例: `width="100px"` または `width="60%"`</span><span class="sxs-lookup"><span data-stu-id="99894-438">Example: `width="100px"` or `width="60%"`</span></span> |
 

#### <a name="output-attributes"></a><span data-ttu-id="99894-439">出力属性</span><span class="sxs-lookup"><span data-stu-id="99894-439">Output attributes</span></span>

|<span data-ttu-id="99894-440">出力属性</span><span class="sxs-lookup"><span data-stu-id="99894-440">Output attribute</span></span>|<span data-ttu-id="99894-441">説明</span><span class="sxs-lookup"><span data-stu-id="99894-441">Description</span></span>|
|:------|:------|
| <span data-ttu-id="99894-442">data-id</span><span class="sxs-lookup"><span data-stu-id="99894-442">data-id</span></span> | <span data-ttu-id="99894-443">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="99894-443">A reference for the element.</span></span><br/><br/><span data-ttu-id="99894-444">[ページ コンテンツの更新](onenote-update-page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="99894-444">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="99894-445">id</span><span class="sxs-lookup"><span data-stu-id="99894-445">id</span></span> | <span data-ttu-id="99894-446">要素の一意の生成された ID。</span><span class="sxs-lookup"><span data-stu-id="99894-446">A unique, generated ID for the element.</span></span> <span data-ttu-id="99894-447">`includeIDs=true` クエリ オプションを使用した場合に、[ページの *content* エンドポイントに対する GET 要求](/graph/api/page-get?view=graph-rest-1.0)から返されます。</span><span class="sxs-lookup"><span data-stu-id="99894-447">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="99894-448">[ページ コンテンツの更新](onenote-update-page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="99894-448">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="99894-449">style</span><span class="sxs-lookup"><span data-stu-id="99894-449">style</span></span> | <span data-ttu-id="99894-450">要素の CSS [style](#styles)のプロパティ。</span><span class="sxs-lookup"><span data-stu-id="99894-450">The CSS [style](#styles) properties of the element.</span></span> |
 

<span data-ttu-id="99894-451">次の例では、さまざまな方法を使用してテーブルのスタイルと返される出力 HTML を定義する入力 HTML を示しています。</span><span class="sxs-lookup"><span data-stu-id="99894-451">The following examples show input HTML that uses different ways to define styles on tables and the output HTML that's returned.</span></span>

#### <a name="input-html-with-optional-settings-at-different-levels"></a><span data-ttu-id="99894-452">さまざまなレベルのオプション設定を伴う入力 HTML</span><span class="sxs-lookup"><span data-stu-id="99894-452">Input HTML with optional settings at different levels.</span></span>

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
 
#### <a name="output-html-with-css-styles-returned-inline-on-the-td-elements"></a><span data-ttu-id="99894-453">td 要素でインラインで返される CSS スタイルを伴う出力 HTML</span><span class="sxs-lookup"><span data-stu-id="99894-453">Output HTML with CSS styles returned inline on the td elements.</span></span>

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


## <a name="styles"></a><span data-ttu-id="99894-454">スタイル</span><span class="sxs-lookup"><span data-stu-id="99894-454">Styles</span></span>

<span data-ttu-id="99894-455">Microsoft Graph の OneNote API は、ページ本文の要素 (**body**、**div**、**p**、**li**、**span** など) として、次に示すインライン CSS の **style** プロパティをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="99894-455">OneNote APIs in Microsoft Graph support the following inline CSS **style** properties for elements in the page body, such as **body**, **div**, **p**, **li**, and **span**.</span></span>

|<span data-ttu-id="99894-456">プロパティ</span><span class="sxs-lookup"><span data-stu-id="99894-456">Property</span></span>|<span data-ttu-id="99894-457">例</span><span class="sxs-lookup"><span data-stu-id="99894-457">Example</span></span>|
|:------|:------|
| <span data-ttu-id="99894-458">background-color</span><span class="sxs-lookup"><span data-stu-id="99894-458">background-color</span></span> | <span data-ttu-id="99894-459">`style="background-color:#66cc66"` (既定は white)</span><span class="sxs-lookup"><span data-stu-id="99894-459">`style="background-color:#66cc66"` (defaults to white)</span></span><br/><br/><span data-ttu-id="99894-460">16 進数形式と名前付きの色の両方がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="99894-460">Both hexadecimal format and named colors are supported.</span></span> |
| <span data-ttu-id="99894-461">color</span><span class="sxs-lookup"><span data-stu-id="99894-461">color</span></span> | <span data-ttu-id="99894-462">`style="color:#ffffff"` (既定は black)</span><span class="sxs-lookup"><span data-stu-id="99894-462">`style="color:#ffffff"` (defaults to black)</span></span> |
| <span data-ttu-id="99894-463">font-family</span><span class="sxs-lookup"><span data-stu-id="99894-463">font-family</span></span> | <span data-ttu-id="99894-464">`style="font-family:Courier"` (既定は Calibri)</span><span class="sxs-lookup"><span data-stu-id="99894-464">`style="font-family:Courier"` (defaults to Calibri)</span></span> |
| <span data-ttu-id="99894-465">font-size</span><span class="sxs-lookup"><span data-stu-id="99894-465">font-size</span></span> | <span data-ttu-id="99894-466">`style="font-size:10pt"` (既定は 11pt)</span><span class="sxs-lookup"><span data-stu-id="99894-466">`style="font-size:10pt"` (defaults to 11pt)</span></span><br/><br/><span data-ttu-id="99894-467">API は *pt* または *px* のフォント サイズを受け入れますが、*px* は *pt* に変換します。</span><span class="sxs-lookup"><span data-stu-id="99894-467">The APIs accept font size in *pt* or *px*, but converts *px* to *pt*.</span></span> <span data-ttu-id="99894-468">10 進数の値は、最も近い n.0pt または n.5pt に四捨五入されます。</span><span class="sxs-lookup"><span data-stu-id="99894-468">Decimal values are rounded to the nearest n.0pt or n.5pt.</span></span> |
| <span data-ttu-id="99894-469">font-style</span><span class="sxs-lookup"><span data-stu-id="99894-469">font-style</span></span> | <span data-ttu-id="99894-470">`style="font-style:italic"` (標準または斜体のみ)</span><span class="sxs-lookup"><span data-stu-id="99894-470">`style="font-style:italic"` (normal or italic only)</span></span> |
| <span data-ttu-id="99894-471">font-weight</span><span class="sxs-lookup"><span data-stu-id="99894-471">font-weight</span></span> | <span data-ttu-id="99894-472">`style="font-weight:bold"` (標準または太字のみ)</span><span class="sxs-lookup"><span data-stu-id="99894-472">`style="font-weight:bold"` (normal or bold only)</span></span> |
| <span data-ttu-id="99894-473">strike-through</span><span class="sxs-lookup"><span data-stu-id="99894-473">strike-through</span></span> | `style="text-decoration:line-through"` |
| <span data-ttu-id="99894-474">text-align</span><span class="sxs-lookup"><span data-stu-id="99894-474">text-align</span></span> | <span data-ttu-id="99894-475">`style="text-align:center"` (ブロック要素の場合のみ)</span><span class="sxs-lookup"><span data-stu-id="99894-475">`style="text-align:center"` (for block elements only)</span></span> |
| <span data-ttu-id="99894-476">text-decoration</span><span class="sxs-lookup"><span data-stu-id="99894-476">text-decoration</span></span> | <span data-ttu-id="99894-477">`style="text-decoration:underline"` (なし、または下線のみ)</span><span class="sxs-lookup"><span data-stu-id="99894-477">`style="text-decoration:underline"` (none or underline only)</span></span> |
 

<span data-ttu-id="99894-478">次のインライン文字スタイルもサポートされています:</span><span class="sxs-lookup"><span data-stu-id="99894-478">The following inline character styles and are also supported:</span></span>

<table id="simpletable">
<tr>
<td id="simplecell"><span data-ttu-id="99894-479"><b></span><span class="sxs-lookup"><span data-stu-id="99894-479"><b></span></span></td>
<td id="simplecell"><span data-ttu-id="99894-480"><i></span><span class="sxs-lookup"><span data-stu-id="99894-480"><i></span></span></td>
<td id="simplecell"><span data-ttu-id="99894-481"><u></span><span class="sxs-lookup"><span data-stu-id="99894-481"><u></span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="99894-482"><em></span><span class="sxs-lookup"><span data-stu-id="99894-482"><em></span></span></td>
<td id="simplecell"><span data-ttu-id="99894-483"><strong></span><span class="sxs-lookup"><span data-stu-id="99894-483"><strong></span></span></td>
<td id="simplecell"><span data-ttu-id="99894-484"><strike></span><span class="sxs-lookup"><span data-stu-id="99894-484"><strike></span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="99894-485"><sup></span><span class="sxs-lookup"><span data-stu-id="99894-485"><sup></span></span></td>
<td id="simplecell"><span data-ttu-id="99894-486"><sub></span><span class="sxs-lookup"><span data-stu-id="99894-486"><sub></span></span></td>
<td id="simplecell"><span data-ttu-id="99894-487"><del></span><span class="sxs-lookup"><span data-stu-id="99894-487"><del></span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="99894-488"><cite></span><span class="sxs-lookup"><span data-stu-id="99894-488"><cite></span></span></td>
<td id="simplecell">&nbsp;</td>
<td id="simplecell">&nbsp;</td>
</tr>
</table>

 
## <a name="input-and-output-html-example"></a><span data-ttu-id="99894-489">入力 HTML と出力 HTML の例</span><span class="sxs-lookup"><span data-stu-id="99894-489">Input and output HTML example</span></span>

<span data-ttu-id="99894-490">次の画像は、Microsoft Graph で作成された簡単なページを示しています。</span><span class="sxs-lookup"><span data-stu-id="99894-490">The following image shows a simple page that was created with Microsoft Graph.</span></span>

![Wikipedia によるコンテンツのスタディ ノートを付記した OneNote ページの画像](images/onenote-sample-image.png)

<span data-ttu-id="99894-492">これは、ページを作成するためにメッセージ本文で送信された入力 HTML です。</span><span class="sxs-lookup"><span data-stu-id="99894-492">This is the input HTML sent in the message body to create the page.</span></span>

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
        <img alt="Apollo 11 commemorative stamp." src="https://upload.wikimedia.org/wikipedia/commons/a/a4/First_Man_on_Moon_1969_Issue-10c.jpg"  width="400"/>
        <p>References:</p>
        <p><a href="https://en.wikipedia.org/wiki/Apollo_11">https://en.wikipedia.org/wiki/Apollo_11</a></p>
        <p><a href="https://www.nasa.gov/mission_pages/apollo/missions/apollo11.html">https://www.nasa.gov/mission_pages/apollo/missions/apollo11.html</a></p>
    </body>
</html>
``` 

<br/>

<span data-ttu-id="99894-493">これは、[ページ コンテンツを取得](onenote-get-content.md)するときに Microsoft Graph が返す出力 HTML です。</span><span class="sxs-lookup"><span data-stu-id="99894-493">This is the output HTML that Microsoft Graph returns when you [get page content](onenote-get-content.md).</span></span>

> <span data-ttu-id="99894-494">**注:** [ページを作成する](onenote-create-page.md)ときや、[ページのメタデータを取得する](/graph/api/page-get?view=graph-rest-1.0)ときに、API は **contentUrl** プロパティのページの*コンテンツ* エンドポイント URL を返します。</span><span class="sxs-lookup"><span data-stu-id="99894-494">**Note:** When you [create a page](onenote-create-page.md) or [get page metadata](/graph/api/page-get?view=graph-rest-1.0), the API returns the *content* endpoint URL of the page in the **contentUrl** property.</span></span>

```html
<html htmlns="https://www.w3.org/1999/xhtml" lang="en-US">
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
            <p><a href="https://en.wikipedia.org/wiki/Apollo_11">https://en.wikipedia.org/wiki/Apollo_11</a></p>
            <p><a href="https://www.nasa.gov/mission_pages/apollo/missions/apollo11.html">https://www.nasa.gov/mission_pages/apollo/missions/apollo11.html</a></p>
        </div>
    </body>
</html>
``` 

## <a name="see-also"></a><span data-ttu-id="99894-495">関連項目</span><span class="sxs-lookup"><span data-stu-id="99894-495">See also</span></span>

- [<span data-ttu-id="99894-496">OneNote コンテンツと構造を取得する</span><span class="sxs-lookup"><span data-stu-id="99894-496">Get OneNote content and structure</span></span>](onenote-get-content.md)
- [<span data-ttu-id="99894-497">OneNote ページを作成する</span><span class="sxs-lookup"><span data-stu-id="99894-497">Create OneNote pages</span></span>](onenote-create-page.md)
- [<span data-ttu-id="99894-498">OneNote ページ コンテンツを更新する</span><span class="sxs-lookup"><span data-stu-id="99894-498">Update OneNote page content</span></span>](onenote-update-page.md)
- [<span data-ttu-id="99894-499">画像、ビデオ、ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="99894-499">Add images, videos, and files</span></span>](onenote-images-files.md)
