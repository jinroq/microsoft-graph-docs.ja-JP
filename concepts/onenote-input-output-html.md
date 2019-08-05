---
title: OneNote ページの入出力 HTML
description: 'OneNote ページを作成または更新する際に、ページ コンテンツと構造を定義する HTML を*入力 HTML* と呼びます。 '
author: jewan-microsoft
localization_priority: Priority
ms.prod: onenote
ms.openlocfilehash: fcb4a8127b633ba309212a7160c9e5548836466c
ms.sourcegitcommit: 6720736406f21e40914b27ba28387adedf97fa56
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/12/2019
ms.locfileid: "35639221"
---
# <a name="input-and-output-html-in-onenote-pages"></a><span data-ttu-id="57e34-103">OneNote ページの入出力 HTML</span><span class="sxs-lookup"><span data-stu-id="57e34-103">Input and output HTML in OneNote pages</span></span>

<span data-ttu-id="57e34-104">OneNote ページを[作成](onenote-create-page.md)または[更新](onenote-update-page.md)する際に、ページ コンテンツと構造を定義する HTML を*入力 HTML* と呼びます。</span><span class="sxs-lookup"><span data-stu-id="57e34-104">The HTML that defines the page content and structure when you [create](onenote-create-page.md) or [update](onenote-update-page.md) a OneNote page is called *input HTML*.</span></span> 

<span data-ttu-id="57e34-p101">[ページ コンテンツを取得](onenote-get-content.md)すると返される HTML を *出力 HTML* と呼びます。出力 HTML は入力 HTML と同じにはなりません。</span><span class="sxs-lookup"><span data-stu-id="57e34-p101">The HTML that's returned when you [get page content](onenote-get-content.md) is called *output HTML*. Output HTML won't be the same as input HTML.</span></span>

<span data-ttu-id="57e34-107">Microsoft Graph の OneNote API は、入力 HTML の意味的コンテンツと基本的構造を保持しますが、その HTML を、[サポートされている HTML 要素および CSS プロパティ](onenote-create-page.md#supported-html-and-css-for-onenote-pages)のセットに変換します。</span><span class="sxs-lookup"><span data-stu-id="57e34-107">The OneNote APIs in Microsoft Graph preserve the semantic content and basic structure of the input HTML, but convert it to a set of [supported HTML elements and CSS properties](onenote-create-page.md#supported-html-and-css-for-onenote-pages).</span></span> <span data-ttu-id="57e34-108">API はさらに、OneNote 機能をサポートするカスタム属性も追加します。</span><span class="sxs-lookup"><span data-stu-id="57e34-108">The APIs also add custom attributes that support OneNote features.</span></span>
 
<span data-ttu-id="57e34-p103">この資料では、入力 HTML と出力 HTML の主な要素と属性について説明します。ページ コンテンツを作成または更新する場合には入力 HTMLについて、返されるページ コンテンツを解析する場合には出力 HTML について理解することは役立ちます。</span><span class="sxs-lookup"><span data-stu-id="57e34-p103">This article describes the principal elements and attributes of input and output HTML. It can be helpful to understand input HTML when you're creating or updating page content, and output HTML when you're parsing returned page content.</span></span> 

## <a name="body-element"></a><span data-ttu-id="57e34-111">body 要素</span><span class="sxs-lookup"><span data-stu-id="57e34-111">body element</span></span>

<span data-ttu-id="57e34-p104">ページ本文の HTML コンテンツは、画像やファイルのリソースなどを含むページのコンテンツと構造を表します。入力および出力 HTML では、**body** 要素に次の属性を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="57e34-p104">The HTML content in the page body represents the page content and structure, including image and file resources. The **body** element can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="57e34-114">入力属性</span><span class="sxs-lookup"><span data-stu-id="57e34-114">Input attributes</span></span>

|<span data-ttu-id="57e34-115">入力属性</span><span class="sxs-lookup"><span data-stu-id="57e34-115">Input attribute</span></span>|<span data-ttu-id="57e34-116">説明</span><span class="sxs-lookup"><span data-stu-id="57e34-116">Description</span></span>|
|:------|:------|
| <span data-ttu-id="57e34-117">data-absolute-enabled</span><span class="sxs-lookup"><span data-stu-id="57e34-117">data-absolute-enabled</span></span> | <span data-ttu-id="57e34-118">[絶対位置で配置](onenote-abs-pos.md)された要素を入力本文でサポートするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="57e34-118">Indicates whether the input body supports [absolute positioned](onenote-abs-pos.md) elements.</span></span> |
| <span data-ttu-id="57e34-119">style</span><span class="sxs-lookup"><span data-stu-id="57e34-119">style</span></span> | <p><span data-ttu-id="57e34-120">本文の CSS の [style](#styles) プロパティ。</span><span class="sxs-lookup"><span data-stu-id="57e34-120">The CSS [style](#styles) properties of the body.</span></span> <span data-ttu-id="57e34-121">出力 HTML では、入力設定がインラインで、適切な子要素で返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="57e34-121">In the output HTML, input settings might be returned inline on appropriate child elements.</span></span></p><p><span data-ttu-id="57e34-122">現在、**body** 要素では背景色はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="57e34-122">Background color is not currently supported for the **body** element.</span></span></p> |
 

#### <a name="output-attributes"></a><span data-ttu-id="57e34-123">出力属性</span><span class="sxs-lookup"><span data-stu-id="57e34-123">Output attributes</span></span>

|<span data-ttu-id="57e34-124">出力属性</span><span class="sxs-lookup"><span data-stu-id="57e34-124">Output attribute</span></span>|<span data-ttu-id="57e34-125">説明</span><span class="sxs-lookup"><span data-stu-id="57e34-125">Description</span></span>|
|:------|:------|
| <span data-ttu-id="57e34-126">data-absolute-enabled</span><span class="sxs-lookup"><span data-stu-id="57e34-126">data-absolute-enabled</span></span> | <span data-ttu-id="57e34-p106">[絶対位置で配置](onenote-abs-pos.md)された要素を本文でサポートするかどうかを示します。出力 HTML では常に **true** です。</span><span class="sxs-lookup"><span data-stu-id="57e34-p106">Indicates whether the body supports [absolute positioned](onenote-abs-pos.md) elements. Always **true** in output HTML.</span></span> |
| <span data-ttu-id="57e34-129">style</span><span class="sxs-lookup"><span data-stu-id="57e34-129">style</span></span> | <span data-ttu-id="57e34-130">本文の **font-family** および **font-size** プロパティ。</span><span class="sxs-lookup"><span data-stu-id="57e34-130">The **font-family** and **font-size** properties of the body.</span></span> |


## <a name="div-elements"></a><span data-ttu-id="57e34-131">div 要素</span><span class="sxs-lookup"><span data-stu-id="57e34-131">div elements</span></span>

<span data-ttu-id="57e34-132">**div** 要素にはテキスト、画像、およびその他のコンテンツが含まれます。</span><span class="sxs-lookup"><span data-stu-id="57e34-132">**Div** elements contain text, images, and other content.</span></span> <span data-ttu-id="57e34-133">入力 HTML と出力 HTML では、**div** 要素に次の属性を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="57e34-133">A **div** element can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="57e34-134">入力属性</span><span class="sxs-lookup"><span data-stu-id="57e34-134">Input attributes</span></span>

|<span data-ttu-id="57e34-135">入力属性</span><span class="sxs-lookup"><span data-stu-id="57e34-135">Input attribute</span></span>|<span data-ttu-id="57e34-136">説明</span><span class="sxs-lookup"><span data-stu-id="57e34-136">Description</span></span>|
|:------|:------|
| <span data-ttu-id="57e34-137">data-id</span><span class="sxs-lookup"><span data-stu-id="57e34-137">data-id</span></span> | <span data-ttu-id="57e34-138">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="57e34-138">A reference for the element.</span></span><br/><br/><span data-ttu-id="57e34-139">[ページ コンテンツの更新](onenote-update-page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="57e34-139">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="57e34-140">data-render-fallback</span><span class="sxs-lookup"><span data-stu-id="57e34-140">data-render-fallback</span></span> | <span data-ttu-id="57e34-141">[抽出](onenote-extract-data.md)が失敗した場合のフォールバック操作。**render** (既定) または **none**</span><span class="sxs-lookup"><span data-stu-id="57e34-141">The fallback action if the [extraction](onenote-extract-data.md) fails: **render** (default) or **none**</span></span> |
| <span data-ttu-id="57e34-142">data-render-method</span><span class="sxs-lookup"><span data-stu-id="57e34-142">data-render-method</span></span> | <span data-ttu-id="57e34-143">[抽出](onenote-extract-data.md)を実行するメソッド。たとえば:</span><span class="sxs-lookup"><span data-stu-id="57e34-143">The [extraction](onenote-extract-data.md) method to perform, for example:</span></span><br/><span data-ttu-id="57e34-144">`extract.businesscard` または `extract.recipe`</span><span class="sxs-lookup"><span data-stu-id="57e34-144">`extract.businesscard` or `extract.recipe`</span></span> |
| <span data-ttu-id="57e34-145">data-render-src</span><span class="sxs-lookup"><span data-stu-id="57e34-145">data-render-src</span></span> | <span data-ttu-id="57e34-146">[抽出](onenote-extract-data.md)のコンテンツのソース。</span><span class="sxs-lookup"><span data-stu-id="57e34-146">The content source for the [extraction](onenote-extract-data.md).</span></span> |
| <span data-ttu-id="57e34-147">style</span><span class="sxs-lookup"><span data-stu-id="57e34-147">style</span></span> | <span data-ttu-id="57e34-148">div の位置、サイズ、フォント、および色のプロパティ:</span><span class="sxs-lookup"><span data-stu-id="57e34-148">The position, size, font, and color properties for the div:</span></span> <ul><li><span data-ttu-id="57e34-149">**position** (**absolute** のみ)、**left**、**top**、および **width** (div では height が自動構成されます)</span><span class="sxs-lookup"><span data-stu-id="57e34-149">**position** (**absolute** only), **left**, **top**, and **width** (height is auto-configured for divs)</span></span><br/><br/><span data-ttu-id="57e34-150">本文が `data-absolute-enabled="true"` に設定されていて、div が本文の直接の子の場合にのみ、[絶対位置](onenote-abs-pos.md)の div の作成に使用されます。</span><span class="sxs-lookup"><span data-stu-id="57e34-150">Used to create an [absolute positioned](onenote-abs-pos.md) div, only if the div is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br/><br/><span data-ttu-id="57e34-151">例: `<div style="position:absolute;width:360px;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="57e34-151">Example: `<div style="position:absolute;width:360px;top:350px;left:300px" ... />`</span></span></li><li><span data-ttu-id="57e34-p108">要素の CSS [スタイル](#styles) プロパティ。出力 HTML では、これらの値は適切な子要素でインラインで返されます。</span><span class="sxs-lookup"><span data-stu-id="57e34-p108">The CSS [style](#styles) properties of the element. In the output HTML, these values are returned inline on appropriate child elements.</span></span></li></ul> |
 

<span data-ttu-id="57e34-154">Microsoft Graph の OneNote API は、すべての本文のコンテンツを 1 つ以上の div でラップします。</span><span class="sxs-lookup"><span data-stu-id="57e34-154">The OneNote APIs in Microsoft Graph wrap all body content in at least one div.</span></span> <span data-ttu-id="57e34-155">次の場合に、API は既定の div (`data-id="_default"` の属性に設定) を作成して、本文のコンテンツを含めます。</span><span class="sxs-lookup"><span data-stu-id="57e34-155">The API creates a default div (attributed with `data-id="_default"`) to contain the body content if:</span></span>

- <span data-ttu-id="57e34-p110">入力要素 body の **data-absolute-enabled** 属性が省略されたか、**false** に設定されている。この場合、すべての本文のコンテンツは既定の div に含められます。</span><span class="sxs-lookup"><span data-stu-id="57e34-p110">The input body element's **data-absolute-enabled** attribute is omitted or set to **false**. In this case, all body content is put in the default div.</span></span>

- <span data-ttu-id="57e34-158">本文の入力要素の **data-absolute-enabled** 属性は\*\* true\*\* ですが、入力 HTML は、[絶対位置に配置された](onenote-abs-pos.md)&nbsp;\*\* div**、**img\*\*、または **object** 要素ではない直接の子を含んでいます。</span><span class="sxs-lookup"><span data-stu-id="57e34-158">The input body element's **data-absolute-enabled** attribute is **true**, but the input HTML contains direct children that aren't [absolute positioned](onenote-abs-pos.md)&nbsp;**div**, **img**, or **object** elements.</span></span> <span data-ttu-id="57e34-159">この例では、[絶対位置に配置された](onenote-abs-pos.md)&nbsp;\*\* div**、**img\*\*、または **object** 要素ではない直接の子が、既定位置の div に配置されています。</span><span class="sxs-lookup"><span data-stu-id="57e34-159">In this case, direct children that aren't [absolute positioned](onenote-abs-pos.md)&nbsp;**div**, **img**, or **object** elements are put in the default div.</span></span>


#### <a name="output-attributes"></a><span data-ttu-id="57e34-160">出力属性</span><span class="sxs-lookup"><span data-stu-id="57e34-160">Output attributes</span></span>

|<span data-ttu-id="57e34-161">出力属性</span><span class="sxs-lookup"><span data-stu-id="57e34-161">Output attribute</span></span>|<span data-ttu-id="57e34-162">説明</span><span class="sxs-lookup"><span data-stu-id="57e34-162">Description</span></span>|
|:------|:------|
| <span data-ttu-id="57e34-163">data-id</span><span class="sxs-lookup"><span data-stu-id="57e34-163">data-id</span></span> | <span data-ttu-id="57e34-164">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="57e34-164">A reference for the element.</span></span><br/><br/><span data-ttu-id="57e34-165">[ページ コンテンツの更新](onenote-update-page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="57e34-165">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="57e34-166">id</span><span class="sxs-lookup"><span data-stu-id="57e34-166">id</span></span> | <span data-ttu-id="57e34-167">要素の一意の生成された ID。</span><span class="sxs-lookup"><span data-stu-id="57e34-167">A unique, generated ID for the element.</span></span> <span data-ttu-id="57e34-168">`includeIDs=true` クエリ オプションを使用した場合に、[ページの *content* エンドポイントに対する GET 要求](/graph/api/page-get?view=graph-rest-1.0)から返されます。</span><span class="sxs-lookup"><span data-stu-id="57e34-168">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="57e34-169">[ページ コンテンツの更新](onenote-update-page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="57e34-169">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="57e34-170">style</span><span class="sxs-lookup"><span data-stu-id="57e34-170">style</span></span> | <span data-ttu-id="57e34-171">div の位置とサイズのプロパティ。</span><span class="sxs-lookup"><span data-stu-id="57e34-171">The position and size properties of the div.</span></span> |
 
### <a name="non-contributing-divs"></a><span data-ttu-id="57e34-172">作用していない div</span><span class="sxs-lookup"><span data-stu-id="57e34-172">Non-contributing divs</span></span>

<span data-ttu-id="57e34-p113">入力 HTML の **div** 要素がページ構造に作用しておらず、OneNote が使用する情報を含んでいない場合、API は div のコンテンツを親または既定の div に移動します。このことは次の例で示しています。</span><span class="sxs-lookup"><span data-stu-id="57e34-p113">When a **div** element in the input HTML does not contribute to the page structure or carry information that OneNote uses, the API moves the div's content into the parent or default div. This is illustrated in the following examples.</span></span>

#### <a name="input-html"></a><span data-ttu-id="57e34-175">入力 HTML</span><span class="sxs-lookup"><span data-stu-id="57e34-175">Input HTML</span></span>

<span data-ttu-id="57e34-176">作用していない入れ子型の div を含んでいます。</span><span class="sxs-lookup"><span data-stu-id="57e34-176">Contains a non-contributing, nested div.</span></span>

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

#### <a name="output-html"></a><span data-ttu-id="57e34-177">出力 HTML</span><span class="sxs-lookup"><span data-stu-id="57e34-177">Output HTML</span></span>

> <span data-ttu-id="57e34-178">**注:** div のコンテンツは親の div に移動し、入れ子状態の `<div>` タグが削除されました。</span><span class="sxs-lookup"><span data-stu-id="57e34-178">**Note:** The div's content was moved to the parent div and the nested `<div>` tags have been removed.</span></span> <span data-ttu-id="57e34-179">**data-id** などの意味情報が div に定義されていた場合は、div は保持されています (例: `<div data-id="keep-me">`)。</span><span class="sxs-lookup"><span data-stu-id="57e34-179">The div would have been preserved if it defined any semantic information, such as a **data-id** (example: `<div data-id="keep-me">`).</span></span>

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


## <a name="img-elements"></a><span data-ttu-id="57e34-180">img 要素</span><span class="sxs-lookup"><span data-stu-id="57e34-180">img elements</span></span>

<span data-ttu-id="57e34-p115">OneNote ページの画像は **img** 要素で表されます。入力 HTML および出力 HTML では、**img** 要素に次の属性を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="57e34-p115">Images on OneNote pages are represented by **img** elements. An **img** element can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="57e34-183">入力属性</span><span class="sxs-lookup"><span data-stu-id="57e34-183">Input attributes</span></span>

|<span data-ttu-id="57e34-184">入力属性</span><span class="sxs-lookup"><span data-stu-id="57e34-184">Input attribute</span></span>|<span data-ttu-id="57e34-185">説明</span><span class="sxs-lookup"><span data-stu-id="57e34-185">Description</span></span>|
|:------|:------|
| <span data-ttu-id="57e34-186">alt</span><span class="sxs-lookup"><span data-stu-id="57e34-186">alt</span></span> | <span data-ttu-id="57e34-187">画像に指定された代替テキスト。</span><span class="sxs-lookup"><span data-stu-id="57e34-187">The supplied alt text for the image.</span></span> |
| <span data-ttu-id="57e34-188">data-id</span><span class="sxs-lookup"><span data-stu-id="57e34-188">data-id</span></span> | <span data-ttu-id="57e34-189">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="57e34-189">A reference for the element.</span></span><br/><br/><span data-ttu-id="57e34-190">[ページ コンテンツの更新](onenote-update-page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="57e34-190">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="57e34-191">data-render-src</span><span class="sxs-lookup"><span data-stu-id="57e34-191">data-render-src</span></span> |<span data-ttu-id="57e34-192">**data-render-src** か **src** のいずれかが必要です。</span><span class="sxs-lookup"><span data-stu-id="57e34-192">Either **data-render-src** or **src** is required.</span></span><br/><br/><span data-ttu-id="57e34-193">OneNote ページ上のビットマップ画像として表示する Web ページ。</span><span class="sxs-lookup"><span data-stu-id="57e34-193">The webpage to render as a bit-mapped image on the OneNote page:</span></span><br/><br/> <span data-ttu-id="57e34-194">パブリック URL の場合は - `data-render-src="https://..."`。</span><span class="sxs-lookup"><span data-stu-id="57e34-194">- `data-render-src="https://..."` for a public URL.</span></span><br/><br/> <span data-ttu-id="57e34-195">[マルチパート要求](/graph/api/section-post-pages?view=graph-rest-1.0#example)の "Presentation" ブロックにある画像部分の場合は - `data-render-src="name:BlockName"`。</span><span class="sxs-lookup"><span data-stu-id="57e34-195">- `data-render-src="name:BlockName"` for an image part in the "Presentation" block of a [multipart request](/graph/api/section-post-pages?view=graph-rest-1.0#example).</span></span><br/><br/><span data-ttu-id="57e34-196">このメソッドは、OneNote ページで忠実に表示できるものよりも複雑な Web ページの場合や、ページにログイン資格情報が必要な場合に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="57e34-196">This method is useful when the webpage is more complex than the OneNote page can faithfully render, or when the page requires login credentials.</span></span>|
| <span data-ttu-id="57e34-197">data-tag</span><span class="sxs-lookup"><span data-stu-id="57e34-197">data-tag</span></span> | <span data-ttu-id="57e34-198">要素の[ノート シール](onenote-note-tags.md)。</span><span class="sxs-lookup"><span data-stu-id="57e34-198">A [note tag](onenote-note-tags.md) on the element.</span></span> |
| <span data-ttu-id="57e34-199">style</span><span class="sxs-lookup"><span data-stu-id="57e34-199">style</span></span> |<span data-ttu-id="57e34-200">画像の位置とサイズのプロパティ: **position** (**absolute** のみ)、**left**、**top**、**width**、および **height**。</span><span class="sxs-lookup"><span data-stu-id="57e34-200">The position and size properties for the image: **position** (**absolute** only), **left**, **top**, **width**, and **height**.</span></span><br/><br/><span data-ttu-id="57e34-201">任意の画像のサイズを設定できます。</span><span class="sxs-lookup"><span data-stu-id="57e34-201">Size can be set on any image.</span></span><br/><br/><span data-ttu-id="57e34-202">位置プロパティは、本文が `data-absolute-enabled="true"` に設定されていて、画像が本文の直接の子である場合にのみ、[絶対位置](onenote-abs-pos.md)の画像の作成に使用されます。</span><span class="sxs-lookup"><span data-stu-id="57e34-202">Position properties are used to create an [absolute positioned](onenote-abs-pos.md) image, only if the image is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br/><br/><span data-ttu-id="57e34-203">例: `<img style="position:absolute;width:360px;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="57e34-203">Example: `<img style="position:absolute;width:360px;top:350px;left:300px" ... />`</span></span><br/><br/><span data-ttu-id="57e34-204">出力 HTML では、画像サイズは **width** 属性と **height** 属性で別々に返されます。</span><span class="sxs-lookup"><span data-stu-id="57e34-204">In the output HTML, the image size is returned separately in **width** and **height** attributes.</span></span> |
| <span data-ttu-id="57e34-205">src</span><span class="sxs-lookup"><span data-stu-id="57e34-205">src</span></span> |<span data-ttu-id="57e34-206">**src** か **data-render-src** のいずれかが必要です。</span><span class="sxs-lookup"><span data-stu-id="57e34-206">Either **src** or **data-render-src** is required.</span></span><br/><br/><span data-ttu-id="57e34-207">OneNote ページに表示する画像。</span><span class="sxs-lookup"><span data-stu-id="57e34-207">The image to render on the OneNote page:</span></span><br/><br/><span data-ttu-id="57e34-208">インターネットで一般に使用可能な画像の URL の場合は - `src="https://..."`。</span><span class="sxs-lookup"><span data-stu-id="57e34-208">- `src="https://..."` for a URL to a publicly available image on the Internet.</span></span><br/><br/> <span data-ttu-id="57e34-209">画像を表すマルチパート要求の名前付き部分の場合は - `src="name:BlockName"`。</span><span class="sxs-lookup"><span data-stu-id="57e34-209">- `src="name:BlockName"` for a named part in a multipart request that represents the image.</span></span>|
| <span data-ttu-id="57e34-210">width、height</span><span class="sxs-lookup"><span data-stu-id="57e34-210">width, height</span></span> | <span data-ttu-id="57e34-p116">画像の幅または高さ。ピクセル単位ですが px は付けません。例: `width="400"`</span><span class="sxs-lookup"><span data-stu-id="57e34-p116">The width or height of the image, in pixels but without the px. Example: `width="400"`</span></span> |
 
> <span data-ttu-id="57e34-213">**注:** OneNote API は入力画像の種類を自動的に検出し、それを **data-fullres-src-type** として出力 HTML に返します。</span><span class="sxs-lookup"><span data-stu-id="57e34-213">**Note:** The OneNote APIs automatically detect the input image type, and return it as the **data-fullres-src-type** in the output HTML.</span></span> <span data-ttu-id="57e34-214">API は、**data-src-type** で最適化された画像の種類も返します。</span><span class="sxs-lookup"><span data-stu-id="57e34-214">The API also returns the image type of the optimized image in **data-src-type**.</span></span>
 

#### <a name="output-attributes"></a><span data-ttu-id="57e34-215">出力属性</span><span class="sxs-lookup"><span data-stu-id="57e34-215">Output attributes</span></span>

|<span data-ttu-id="57e34-216">出力属性</span><span class="sxs-lookup"><span data-stu-id="57e34-216">Output attribute</span></span>|<span data-ttu-id="57e34-217">説明</span><span class="sxs-lookup"><span data-stu-id="57e34-217">Description</span></span>|
|:------|:------|
| <span data-ttu-id="57e34-218">alt</span><span class="sxs-lookup"><span data-stu-id="57e34-218">alt</span></span> | <span data-ttu-id="57e34-219">画像に指定された代替テキスト。</span><span class="sxs-lookup"><span data-stu-id="57e34-219">The supplied alt text for the image.</span></span> |
| <span data-ttu-id="57e34-220">data-id</span><span class="sxs-lookup"><span data-stu-id="57e34-220">data-id</span></span> | <span data-ttu-id="57e34-221">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="57e34-221">A reference for the element.</span></span><br/><br/><span data-ttu-id="57e34-222">[ページ コンテンツの更新](onenote-update-page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="57e34-222">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="57e34-223">data-index</span><span class="sxs-lookup"><span data-stu-id="57e34-223">data-index</span></span> | <span data-ttu-id="57e34-p118">画像の位置。[分割された画像](#split-images)のサポート向け。</span><span class="sxs-lookup"><span data-stu-id="57e34-p118">The position of the image. For [split image](#split-images) support.</span></span> |
| <span data-ttu-id="57e34-226">data-fullres-src</span><span class="sxs-lookup"><span data-stu-id="57e34-226">data-fullres-src</span></span> | <span data-ttu-id="57e34-227">最初にページに埋め込まれていた画像リソースのバージョンのエンドポイント。</span><span class="sxs-lookup"><span data-stu-id="57e34-227">The endpoint for the version of the image resource that was originally embedded in the page.</span></span> |
| <span data-ttu-id="57e34-228">data-fullres-src-type</span><span class="sxs-lookup"><span data-stu-id="57e34-228">data-fullres-src-type</span></span> | <span data-ttu-id="57e34-229">**data-fullres-src** リソースのメディアの種類。たとえば、`image/png` または`image/jpeg`。</span><span class="sxs-lookup"><span data-stu-id="57e34-229">The media type of the **data-fullres-src** resource, for example: `image/png` or `image/jpeg`.</span></span> |
| <span data-ttu-id="57e34-230">data-options</span><span class="sxs-lookup"><span data-stu-id="57e34-230">data-options</span></span> | <span data-ttu-id="57e34-231">ソースの種類。PDF ファイルの場合は **printout**、その他のファイルはいずれも **splitimage**。</span><span class="sxs-lookup"><span data-stu-id="57e34-231">The source type: **printout** for PDF files or **splitimage** for all others.</span></span> <span data-ttu-id="57e34-232">**data-render-src** 属性で作成された、[分割された画像](#split-images)にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="57e34-232">Applies only to [split images](#split-images) created with the **data-render-src** attribute.</span></span> |
| <span data-ttu-id="57e34-233">data-render-original-src</span><span class="sxs-lookup"><span data-stu-id="57e34-233">data-render-original-src</span></span> | <span data-ttu-id="57e34-234">ソース画像が公開されたインターネットの画像で、**data-render-src** 属性を付けて作成された場合の、画像の最初のソース URL。</span><span class="sxs-lookup"><span data-stu-id="57e34-234">The original source URL of the image, if the source image is from the public internet and was created with the **data-render-src** attribute.</span></span> |
| <span data-ttu-id="57e34-235">data-src-type</span><span class="sxs-lookup"><span data-stu-id="57e34-235">data-src-type</span></span> | <span data-ttu-id="57e34-236">**src** リソースのメディアの種類。たとえば、`image/png` または`image/jpeg`。</span><span class="sxs-lookup"><span data-stu-id="57e34-236">The media type of the **src** resource, for example: `image/png` or `image/jpeg`.</span></span> |
| <span data-ttu-id="57e34-237">data-tag</span><span class="sxs-lookup"><span data-stu-id="57e34-237">data-tag</span></span> | <span data-ttu-id="57e34-238">要素の[ノート シール](onenote-note-tags.md)。</span><span class="sxs-lookup"><span data-stu-id="57e34-238">A [note tag](onenote-note-tags.md) on the element.</span></span> |
| <span data-ttu-id="57e34-239">id</span><span class="sxs-lookup"><span data-stu-id="57e34-239">id</span></span> | <span data-ttu-id="57e34-240">要素の一意の生成された ID。</span><span class="sxs-lookup"><span data-stu-id="57e34-240">A unique, generated ID for the element.</span></span> <span data-ttu-id="57e34-241">`includeIDs=true` クエリ オプションを使用した場合に、[ページの *content* エンドポイントに対する GET 要求](/graph/api/page-get?view=graph-rest-1.0)から返されます。</span><span class="sxs-lookup"><span data-stu-id="57e34-241">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="57e34-242">[ページ コンテンツの更新](onenote-update-page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="57e34-242">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="57e34-243">src</span><span class="sxs-lookup"><span data-stu-id="57e34-243">src</span></span> | <span data-ttu-id="57e34-244">Web ブラウザー、モバイル、およびタブレットのフォーム ファクター向けに最適化された画像リソースのバージョンのエンドポイント。</span><span class="sxs-lookup"><span data-stu-id="57e34-244">The endpoint for the version of the image resource that has been optimized for web browsers and mobile and tablet form factors.</span></span> |
| <span data-ttu-id="57e34-245">style</span><span class="sxs-lookup"><span data-stu-id="57e34-245">style</span></span> | <span data-ttu-id="57e34-246">画像の位置のプロパティ。</span><span class="sxs-lookup"><span data-stu-id="57e34-246">The position properties of the image.</span></span> |
| <span data-ttu-id="57e34-247">width、height</span><span class="sxs-lookup"><span data-stu-id="57e34-247">width, height</span></span> | <span data-ttu-id="57e34-248">画像の幅または高さ (ピクセル単位)。</span><span class="sxs-lookup"><span data-stu-id="57e34-248">The width or height of the image, in pixels.</span></span> |
 

### <a name="output-html-examples-for-images"></a><span data-ttu-id="57e34-249">画像の出力 HTML の例</span><span class="sxs-lookup"><span data-stu-id="57e34-249">Output HTML examples for images</span></span>

<span data-ttu-id="57e34-p121">出力 **img** 要素には、次に示すとおり、画像ファイルのリソースおよび画像の種類のためのエンドポイントが含まれています。バイナリ コンテンツを取得するには、[画像リソースのエンドポイントに対して個別に GET 要求を実行](/graph/api/resource-get?view=graph-rest-1.0)します。</span><span class="sxs-lookup"><span data-stu-id="57e34-p121">Output **img** elements contain endpoints for image file resources and the image type, as shown below. You can make separate [GET requests to image resource endpoints](/graph/api/resource-get?view=graph-rest-1.0) to retrieve their binary contents.</span></span>

```html
<img 
    src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/$value"  
    data-src-type="image/png"
    data-fullres-src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/$value"  
    data-fullres-src-type="image/png" ... />
```

<span data-ttu-id="57e34-252">次の例は、**img** 要素が出力 HTML に含む可能性がある情報を示しています。</span><span class="sxs-lookup"><span data-stu-id="57e34-252">The following examples show the information an **img** element might contain in the output HTML.</span></span>

#### <a name="image-with-web-ready-and-high-resolution-resources"></a><span data-ttu-id="57e34-253">Web 対応の高解像度リソースがある画像</span><span class="sxs-lookup"><span data-stu-id="57e34-253">Image with web-ready and high resolution resources</span></span>

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

#### <a name="image-created-by-using-the-data-render-src-attribute"></a><span data-ttu-id="57e34-254">*data-render-src* 属性を使用して作成された画像</span><span class="sxs-lookup"><span data-stu-id="57e34-254">Image created by using the *data-render-src* attribute</span></span>

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

### <a name="split-images"></a><span data-ttu-id="57e34-255">分割された画像</span><span class="sxs-lookup"><span data-stu-id="57e34-255">Split images</span></span>

<span data-ttu-id="57e34-p122">**data-render-src** 属性 (Web ページの URL または名前が付いた部分のもの) を使用して作成された画像は、パフォーマンスと表示上の理由から複数のコンポーネントの画像に分割されることがあります。コンポーネント画像には、すべて同じ **data-id** 値が割り当てられます。各コンポーネントの画像には、元の垂直レイアウトを定義するゼロベースの data-index 属性があります。</span><span class="sxs-lookup"><span data-stu-id="57e34-p122">Images that are created using the **data-render-src** attribute (from a webpage URL or a named part) might be split into multiple component images for performance and rendering reasons. Component images are all assigned the same **data-id** value. Each component image has a zero-based data-index attribute that defines the original vertical layout.</span></span>

#### <a name="split-image-with-three-component-images"></a><span data-ttu-id="57e34-259">画像を 3 つのコンポーネントの画像に分割する</span><span class="sxs-lookup"><span data-stu-id="57e34-259">Split image with three component images</span></span>

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

<span data-ttu-id="57e34-260">ユーザーがページ上で画像を移動することができるため、返されるインデックスが適切な順序になっていない場合があります。</span><span class="sxs-lookup"><span data-stu-id="57e34-260">Because users can move the images on the page, the returned indexes might be out of order.</span></span> <span data-ttu-id="57e34-261">順序は、y 方向に上から下へ、そしてもし y 方向で競合があれば x 方向に左から右へとなっていなければなりません。</span><span class="sxs-lookup"><span data-stu-id="57e34-261">Ordering should be in top to bottom y-order, and then left to right x-order if there are y-order conflicts.</span></span>

## <a name="iframe-elements"></a><span data-ttu-id="57e34-262">iframe 要素</span><span class="sxs-lookup"><span data-stu-id="57e34-262">iframe elements</span></span>

<span data-ttu-id="57e34-263">OneNote ページには、**iframe** 要素で表される埋め込みビデオを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="57e34-263">OneNote pages can contain embedded videos represented by **iframe** elements.</span></span> 

> <span data-ttu-id="57e34-264">**注:** [**object** 要素を使用してビデオ ファイルを添付する](onenote-images-files.md#adding-files)こともできます。</span><span class="sxs-lookup"><span data-stu-id="57e34-264">**Note:** You can also [attach a video file using an **object** element](onenote-images-files.md#adding-files).</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="57e34-265">入力属性</span><span class="sxs-lookup"><span data-stu-id="57e34-265">Input attributes</span></span>

|<span data-ttu-id="57e34-266">入力属性</span><span class="sxs-lookup"><span data-stu-id="57e34-266">Input attribute</span></span>|<span data-ttu-id="57e34-267">説明</span><span class="sxs-lookup"><span data-stu-id="57e34-267">Description</span></span>|
|:------|:------|
| <span data-ttu-id="57e34-268">data-original-src</span><span class="sxs-lookup"><span data-stu-id="57e34-268">data-original-src</span></span> | <span data-ttu-id="57e34-269">必須。</span><span class="sxs-lookup"><span data-stu-id="57e34-269">Required.</span></span> <span data-ttu-id="57e34-270">ビデオ ソースの URL。</span><span class="sxs-lookup"><span data-stu-id="57e34-270">The URL of the video source.</span></span> <span data-ttu-id="57e34-271">[サポートされるビデオ ソースの一覧](onenote-images-files.md#adding-videos)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="57e34-271">See the [list of supported video sources](onenote-images-files.md#adding-videos).</span></span> <br/><br/><span data-ttu-id="57e34-272">例: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span><span class="sxs-lookup"><span data-stu-id="57e34-272">Example: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span></span> |
| <span data-ttu-id="57e34-273">width、height</span><span class="sxs-lookup"><span data-stu-id="57e34-273">width, height</span></span> | <span data-ttu-id="57e34-p125">iframe の幅と高さ (ピクセル単位)。例: `width=300`</span><span class="sxs-lookup"><span data-stu-id="57e34-p125">The width or height of the iframe, in pixels. Example: `width=300`</span></span> |

#### <a name="output-attributes"></a><span data-ttu-id="57e34-276">出力属性</span><span class="sxs-lookup"><span data-stu-id="57e34-276">Output attributes</span></span>

|<span data-ttu-id="57e34-277">出力属性</span><span class="sxs-lookup"><span data-stu-id="57e34-277">Output attribute</span></span>|<span data-ttu-id="57e34-278">説明</span><span class="sxs-lookup"><span data-stu-id="57e34-278">Description</span></span>|
|:------|:------|
| <span data-ttu-id="57e34-279">data-original-src</span><span class="sxs-lookup"><span data-stu-id="57e34-279">data-original-src</span></span> | <span data-ttu-id="57e34-280">ビデオ ソースの URL。</span><span class="sxs-lookup"><span data-stu-id="57e34-280">The URL of the video source.</span></span> |
| <span data-ttu-id="57e34-281">src</span><span class="sxs-lookup"><span data-stu-id="57e34-281">src</span></span> | <span data-ttu-id="57e34-282">OneNote ページに埋め込まれたビデオへのリンク。</span><span class="sxs-lookup"><span data-stu-id="57e34-282">A link to the video that is embedded in the OneNote page.</span></span> |
| <span data-ttu-id="57e34-283">width、height</span><span class="sxs-lookup"><span data-stu-id="57e34-283">width, height</span></span> | <span data-ttu-id="57e34-284">iframe の幅と高さ (ピクセル単位)。</span><span class="sxs-lookup"><span data-stu-id="57e34-284">The width or height of the iframe, in pixels.</span></span><br/><br/><span data-ttu-id="57e34-285">例: `width=300`</span><span class="sxs-lookup"><span data-stu-id="57e34-285">Example: `width=300`</span></span> |
 
### <a name="output-html-example-for-videos"></a><span data-ttu-id="57e34-286">ビデオの出力 HTML の例</span><span class="sxs-lookup"><span data-stu-id="57e34-286">Output HTML example for videos</span></span>

<span data-ttu-id="57e34-287">次に示すように、出力 **iframe** 要素には、ソース ページとビデオに関連付けられたエンドポイントが含まれています。</span><span class="sxs-lookup"><span data-stu-id="57e34-287">Output **iframe** elements contain endpoints that link to the source page and video, as shown.</span></span> 

```html
<iframe 
    width="340" height="280" 
    data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8" 
    src="https://www.youtube.com/embed/3Ztr44aKmQ8?feature=oembed&autoplay=true" />
``` 

## <a name="object-elements"></a><span data-ttu-id="57e34-288">object 要素</span><span class="sxs-lookup"><span data-stu-id="57e34-288">object elements</span></span>

<span data-ttu-id="57e34-p126">OneNote ページには、**object** 要素で表される添付ファイルを含めることができます。**object** 要素は、入力 HTML および出力 HTML に次の属性を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="57e34-p126">OneNote pages can contain file attachments represented by **object** elements. An **object** element can contain the following attributes in the input and output HTML.</span></span>

> <span data-ttu-id="57e34-291">**注:** ファイルが画像として送信され、**data-render-src** 属性を使用する場合、OneNote API はファイルのコンテンツを画像としてページに表示できます。</span><span class="sxs-lookup"><span data-stu-id="57e34-291">**Note:** The OneNote APIs can also render file content as images in a page when the file is sent as an image and uses the **data-render-src** attribute.</span></span>
> <span data-ttu-id="57e34-292">例: `<img data-render-src="name:part-name" ... />`</span><span class="sxs-lookup"><span data-stu-id="57e34-292">Example: `<img data-render-src="name:part-name" ... />`</span></span>
 

#### <a name="input-attributes"></a><span data-ttu-id="57e34-293">入力属性</span><span class="sxs-lookup"><span data-stu-id="57e34-293">Input attributes</span></span>

|<span data-ttu-id="57e34-294">入力属性</span><span class="sxs-lookup"><span data-stu-id="57e34-294">Input attribute</span></span>|<span data-ttu-id="57e34-295">説明</span><span class="sxs-lookup"><span data-stu-id="57e34-295">Description</span></span>|
|:------|:------|
| <span data-ttu-id="57e34-296">data</span><span class="sxs-lookup"><span data-stu-id="57e34-296">data</span></span> | <span data-ttu-id="57e34-p128">必須。[マルチパート要求](/graph/api/section-post-pages?view=graph-rest-1.0#example)のファイルを表す部分の名前。</span><span class="sxs-lookup"><span data-stu-id="57e34-p128">Required. The name of the part that represents the file in the [multipart request](/graph/api/section-post-pages?view=graph-rest-1.0#example).</span></span> |
| <span data-ttu-id="57e34-299">data-attachment</span><span class="sxs-lookup"><span data-stu-id="57e34-299">data-attachment</span></span> | <span data-ttu-id="57e34-p129">必須。ファイル名。</span><span class="sxs-lookup"><span data-stu-id="57e34-p129">Required. The file name.</span></span> |
| <span data-ttu-id="57e34-302">data-id</span><span class="sxs-lookup"><span data-stu-id="57e34-302">data-id</span></span> | <span data-ttu-id="57e34-303">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="57e34-303">A reference for the element.</span></span><br/><br/><span data-ttu-id="57e34-304">[ページ コンテンツの更新](onenote-update-page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="57e34-304">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="57e34-305">style</span><span class="sxs-lookup"><span data-stu-id="57e34-305">style</span></span> | <span data-ttu-id="57e34-306">オブジェクトの位置とサイズのプロパティ: **position** (**absolute** のみ)、**left**、**top**、および **width**。</span><span class="sxs-lookup"><span data-stu-id="57e34-306">The position and size properties for the object: **position** (**absolute** only), **left**, **top**, and **width**.</span></span><br/><br/><span data-ttu-id="57e34-307">本文が `data-absolute-enabled="true"` に設定されていて、オブジェクトが本文の直接の子の場合にのみ、[絶対位置](onenote-abs-pos.md)のオブジェクトの作成に使用されます。</span><span class="sxs-lookup"><span data-stu-id="57e34-307">Used to create an [absolute positioned](onenote-abs-pos.md) object, only if the object is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br/><br/><span data-ttu-id="57e34-308">例: `<object style="position:absolute;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="57e34-308">Example: `<object style="position:absolute;top:350px;left:300px" ... />`</span></span> |
| <span data-ttu-id="57e34-309">type</span><span class="sxs-lookup"><span data-stu-id="57e34-309">type</span></span> | <span data-ttu-id="57e34-310">必須。</span><span class="sxs-lookup"><span data-stu-id="57e34-310">Required.</span></span><br/><br/><span data-ttu-id="57e34-311">標準のメディア ファイルの種類。</span><span class="sxs-lookup"><span data-stu-id="57e34-311">The standard media file type.</span></span> <span data-ttu-id="57e34-312">ファイルの種類が既知の場合は、OneNote ページ上でそのファイルの種類に関連付けられているアイコンが表示されます。</span><span class="sxs-lookup"><span data-stu-id="57e34-312">Known file types display the icon associated with the file type on the OneNote page.</span></span> <span data-ttu-id="57e34-313">ファイルの種類が不明の場合は、一般的なファイル アイコンが表示されます。</span><span class="sxs-lookup"><span data-stu-id="57e34-313">Unknown file types display a generic file icon.</span></span> |
<!--todo: add link to known file types--> 

#### <a name="output-attributes"></a><span data-ttu-id="57e34-314">出力属性</span><span class="sxs-lookup"><span data-stu-id="57e34-314">Output attributes</span></span>

|<span data-ttu-id="57e34-315">出力属性</span><span class="sxs-lookup"><span data-stu-id="57e34-315">Output attribute</span></span>|<span data-ttu-id="57e34-316">説明</span><span class="sxs-lookup"><span data-stu-id="57e34-316">Description</span></span>|
|:------|:------|
| <span data-ttu-id="57e34-317">data</span><span class="sxs-lookup"><span data-stu-id="57e34-317">data</span></span> | <span data-ttu-id="57e34-318">ファイルのリソースのエンドポイント。</span><span class="sxs-lookup"><span data-stu-id="57e34-318">The endpoint for the file resource.</span></span> |
| <span data-ttu-id="57e34-319">data-attachment</span><span class="sxs-lookup"><span data-stu-id="57e34-319">data-attachment</span></span> | <span data-ttu-id="57e34-320">ファイル名。</span><span class="sxs-lookup"><span data-stu-id="57e34-320">The file name.</span></span> |
| <span data-ttu-id="57e34-321">data-id</span><span class="sxs-lookup"><span data-stu-id="57e34-321">data-id</span></span> | <span data-ttu-id="57e34-322">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="57e34-322">A reference for the element.</span></span><br/><br/><span data-ttu-id="57e34-323">[ページ コンテンツの更新](onenote-update-page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="57e34-323">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="57e34-324">id</span><span class="sxs-lookup"><span data-stu-id="57e34-324">id</span></span> | <span data-ttu-id="57e34-325">要素の一意の生成された ID。</span><span class="sxs-lookup"><span data-stu-id="57e34-325">A unique, generated ID for the element.</span></span> <span data-ttu-id="57e34-326">`includeIDs=true` クエリ オプションを使用した場合に、[ページの *content* エンドポイントに対する GET 要求](/graph/api/page-get?view=graph-rest-1.0)から返されます。</span><span class="sxs-lookup"><span data-stu-id="57e34-326">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="57e34-327">[ページ コンテンツの更新](onenote-update-page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="57e34-327">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="57e34-328">style</span><span class="sxs-lookup"><span data-stu-id="57e34-328">style</span></span> | <span data-ttu-id="57e34-329">オブジェクトの位置のプロパティ。</span><span class="sxs-lookup"><span data-stu-id="57e34-329">The position properties of the object.</span></span> |
| <span data-ttu-id="57e34-330">type</span><span class="sxs-lookup"><span data-stu-id="57e34-330">type</span></span> | <span data-ttu-id="57e34-331">標準のメディア ファイルの種類。</span><span class="sxs-lookup"><span data-stu-id="57e34-331">The standard media file type.</span></span> |
 

#### <a name="output-html-example-for-objects"></a><span data-ttu-id="57e34-332">オブジェクトの出力 HTML の例</span><span class="sxs-lookup"><span data-stu-id="57e34-332">Output HTML example for objects</span></span>

<span data-ttu-id="57e34-333">次に示すように、出力 **object** 要素には、ページ内のファイル リソースにリンクされたエンドポイントが含まれています。</span><span class="sxs-lookup"><span data-stu-id="57e34-333">Output **object** elements contain endpoints that link to the file resources in the page, as shown.</span></span> <span data-ttu-id="57e34-334">バイナリ コンテンツを取得するには、これらの[ファイル リソースのエンドポイントに対して個別の GET 要求](/graph/api/resource-get?view=graph-rest-1.0)を実行します。</span><span class="sxs-lookup"><span data-stu-id="57e34-334">You can make separate [GET requests to file resource endpoints](/graph/api/resource-get?view=graph-rest-1.0) to retrieve their binary contents.</span></span>

```html
<object
    data="https://graph.microsoft.com/v1.0/me/onenote/resources/{file-id}/$value"
    data-attachment="fileName.pdf" 
    type="application/pdf" 
    [style="..."] />
``` 

## <a name="paragraphs-and-headings"></a><span data-ttu-id="57e34-335">段落と見出し</span><span class="sxs-lookup"><span data-stu-id="57e34-335">Paragraphs and headings</span></span>

<span data-ttu-id="57e34-336">段落、見出し、その他のテキストのコンテナーには、入力 HTML と出力 HTML の次の属性を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="57e34-336">Paragraphs, headings, and other text containers can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="57e34-337">入力属性</span><span class="sxs-lookup"><span data-stu-id="57e34-337">Input attributes</span></span>

|<span data-ttu-id="57e34-338">入力属性</span><span class="sxs-lookup"><span data-stu-id="57e34-338">Input attribute</span></span>|<span data-ttu-id="57e34-339">説明</span><span class="sxs-lookup"><span data-stu-id="57e34-339">Description</span></span>|
|:------|:------|
| <span data-ttu-id="57e34-340">data-id</span><span class="sxs-lookup"><span data-stu-id="57e34-340">data-id</span></span> | <span data-ttu-id="57e34-341">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="57e34-341">A reference for the element.</span></span><br/><br/><span data-ttu-id="57e34-342">[ページ コンテンツの更新](onenote-update-page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="57e34-342">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="57e34-343">data-tag</span><span class="sxs-lookup"><span data-stu-id="57e34-343">data-tag</span></span> | <span data-ttu-id="57e34-344">**p** 要素または **h1** - **h6** 要素上の[ノート シール](onenote-note-tags.md)。</span><span class="sxs-lookup"><span data-stu-id="57e34-344">A [note tag](onenote-note-tags.md) on a **p** or **h1** - **h6** element.</span></span> |
| <span data-ttu-id="57e34-345">style</span><span class="sxs-lookup"><span data-stu-id="57e34-345">style</span></span> | <span data-ttu-id="57e34-346">要素の CSS [スタイル](#styles)のプロパティ。</span><span class="sxs-lookup"><span data-stu-id="57e34-346">The CSS [style](#styles) properties of the element.</span></span> |
 

#### <a name="output-attributes"></a><span data-ttu-id="57e34-347">出力属性</span><span class="sxs-lookup"><span data-stu-id="57e34-347">Output attributes</span></span>

|<span data-ttu-id="57e34-348">出力属性</span><span class="sxs-lookup"><span data-stu-id="57e34-348">Output attribute</span></span>|<span data-ttu-id="57e34-349">説明</span><span class="sxs-lookup"><span data-stu-id="57e34-349">Description</span></span>|
|:------|:------|
| <span data-ttu-id="57e34-350">data-id</span><span class="sxs-lookup"><span data-stu-id="57e34-350">data-id</span></span> | <span data-ttu-id="57e34-351">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="57e34-351">A reference for the element.</span></span><br/><br/><span data-ttu-id="57e34-352">[ページ コンテンツの更新](onenote-update-page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="57e34-352">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="57e34-353">data-tag</span><span class="sxs-lookup"><span data-stu-id="57e34-353">data-tag</span></span> | <span data-ttu-id="57e34-354">**p** 要素または **h1** - **h6** 要素上の[ノート シール](onenote-note-tags.md)。</span><span class="sxs-lookup"><span data-stu-id="57e34-354">A [note tag](onenote-note-tags.md) on a **p** or **h1** - **h6** element.</span></span> |
| <span data-ttu-id="57e34-355">id</span><span class="sxs-lookup"><span data-stu-id="57e34-355">id</span></span> | <span data-ttu-id="57e34-356">要素の一意の生成された ID。</span><span class="sxs-lookup"><span data-stu-id="57e34-356">A unique, generated ID for the element.</span></span> <span data-ttu-id="57e34-357">`includeIDs=true` クエリ オプションを使用した場合に、[ページの *content* エンドポイントに対する GET 要求](/graph/api/page-get?view=graph-rest-1.0)から返されます。</span><span class="sxs-lookup"><span data-stu-id="57e34-357">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="57e34-358">[ページ コンテンツの更新](onenote-update-page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="57e34-358">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="57e34-359">style</span><span class="sxs-lookup"><span data-stu-id="57e34-359">style</span></span> | <span data-ttu-id="57e34-p134">要素の CSS [style](#styles)のプロパティ。出力 HTML では、これらの値は、適切な子要素または **span** 要素でインラインで返すことができます。</span><span class="sxs-lookup"><span data-stu-id="57e34-p134">The CSS [style](#styles) properties of the element. In the output HTML, these values may be returned inline on appropriate child elements or on **span** elements.</span></span> |
 

<span data-ttu-id="57e34-362">次の例では、テキストのコンテナーおよび返される出力 HTML にスタイルを定義するさまざまな方法を使用する入力 HTML を示しています。</span><span class="sxs-lookup"><span data-stu-id="57e34-362">The following examples show input HTML that uses different ways to define styles on text containers and the output HTML that's returned.</span></span>

#### <a name="input-html-with-styles-defined-using-inline-character-styles-in-the-start-tag-and-within-a-span-element"></a><span data-ttu-id="57e34-363">開始タグ内、および span 要素内に、インライン文字スタイルを使用して定義されたスタイル付き入力 HTML。</span><span class="sxs-lookup"><span data-stu-id="57e34-363">Input HTML with styles defined using inline character styles, in the start tag, and within a span element.</span></span>

```html
<h1>Heading <i>One</i> text</h1>
<p style="font-size:8pt;color:green;font-family:Courier;text-align:center">Some text</p>
<p>Some <span  style="font-size:16px;color:#ff0000;font-family:Segoe UI Black">more</span> text</p>
``` 

#### <a name="output-html-with-the-i-character-style-and-the-font-settings-in-the-p-start-tag-returned-as-inline-css-styles-on-span-elements"></a><span data-ttu-id="57e34-364">`<i>` 文字スタイルと `<p>` 開始タグ内のフォント設定が span 要素のインライン CSS スタイルとして返された出力 HTML。</span><span class="sxs-lookup"><span data-stu-id="57e34-364">Output HTML with the `<i>` character style and the font settings in the `<p>` start tag returned as inline CSS styles on span elements.</span></span>

```html
<h1 style="font-size:16pt;color:#1e4e79;margin-top:11pt;margin-bottom:11pt">Heading <span style="font-style:italic">One</span> text</h1>
<p style="text-align:center"><span style="font-family:Courier;font-size:8pt;color:green">Some text</span></p>
<p>Some <span style="font-family:Segoe UI Black;font-size:12pt;color:red">more</span> text</p>
``` 


## <a name="lists"></a><span data-ttu-id="57e34-365">リスト</span><span class="sxs-lookup"><span data-stu-id="57e34-365">Lists</span></span>

<span data-ttu-id="57e34-366">リストは、**li** 要素を含む **ol** 要素または **ul** 要素として表されます。</span><span class="sxs-lookup"><span data-stu-id="57e34-366">Lists are represented as **ol** or **ul** elements that contain list items represented as **li** elements.</span></span>

<span data-ttu-id="57e34-367">入力 HTML および出力 HTML には、リストとリスト項目に次の属性を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="57e34-367">Lists and list items can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="57e34-368">入力属性</span><span class="sxs-lookup"><span data-stu-id="57e34-368">Input attributes</span></span>

|<span data-ttu-id="57e34-369">入力属性</span><span class="sxs-lookup"><span data-stu-id="57e34-369">Input attribute</span></span>|<span data-ttu-id="57e34-370">説明</span><span class="sxs-lookup"><span data-stu-id="57e34-370">Description</span></span>|
|:------|:------|
| <span data-ttu-id="57e34-371">data-id</span><span class="sxs-lookup"><span data-stu-id="57e34-371">data-id</span></span> | <span data-ttu-id="57e34-372">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="57e34-372">A reference for the element.</span></span><br/><br/><span data-ttu-id="57e34-373">[ページ コンテンツの更新](onenote-update-page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="57e34-373">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="57e34-374">data-tag</span><span class="sxs-lookup"><span data-stu-id="57e34-374">data-tag</span></span> | <span data-ttu-id="57e34-375">**ul**、**ol**、または **li** の各要素上の[ノート シール](onenote-note-tags.md)。</span><span class="sxs-lookup"><span data-stu-id="57e34-375">A [note tag](onenote-note-tags.md) on a **ul**, **ol**, or **li** element.</span></span> |
| <span data-ttu-id="57e34-376">style</span><span class="sxs-lookup"><span data-stu-id="57e34-376">style</span></span> | <span data-ttu-id="57e34-377">リストまたはリスト項目の **list-style-type** および CSS [style](#styles) のプロパティ。</span><span class="sxs-lookup"><span data-stu-id="57e34-377">The **list-style-type** and the CSS [style](#styles) properties for the list or list item.</span></span> |
 

#### <a name="output-attributes"></a><span data-ttu-id="57e34-378">出力属性</span><span class="sxs-lookup"><span data-stu-id="57e34-378">Output attributes</span></span>

|<span data-ttu-id="57e34-379">出力属性</span><span class="sxs-lookup"><span data-stu-id="57e34-379">Output attribute</span></span>|<span data-ttu-id="57e34-380">説明</span><span class="sxs-lookup"><span data-stu-id="57e34-380">Description</span></span>|
|:------|:------|
| <span data-ttu-id="57e34-381">data-id</span><span class="sxs-lookup"><span data-stu-id="57e34-381">data-id</span></span> | <span data-ttu-id="57e34-382">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="57e34-382">A reference for the element.</span></span><br/><br/><span data-ttu-id="57e34-383">[ページ コンテンツの更新](onenote-update-page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="57e34-383">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="57e34-384">data-tag</span><span class="sxs-lookup"><span data-stu-id="57e34-384">data-tag</span></span> |  <span data-ttu-id="57e34-385">**li** 要素内の span 上の[ノート シール](onenote-note-tags.md)。</span><span class="sxs-lookup"><span data-stu-id="57e34-385">A [note tag](onenote-note-tags.md) on a span in an **li** element.</span></span> |
| <span data-ttu-id="57e34-386">ID</span><span class="sxs-lookup"><span data-stu-id="57e34-386">id</span></span> | <span data-ttu-id="57e34-387">要素の一意の生成された ID。</span><span class="sxs-lookup"><span data-stu-id="57e34-387">A unique, generated ID for the element.</span></span> <span data-ttu-id="57e34-388">`includeIDs=true` クエリ オプションを使用した場合に、[ページの *content* エンドポイントに対する GET 要求](/graph/api/page-get?view=graph-rest-1.0)から返されます。</span><span class="sxs-lookup"><span data-stu-id="57e34-388">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="57e34-389">[ページ コンテンツの更新](onenote-update-page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="57e34-389">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="57e34-390">style</span><span class="sxs-lookup"><span data-stu-id="57e34-390">style</span></span> | <span data-ttu-id="57e34-p136">要素の **list-style-type** および CSS [style](#styles)のプロパティ。出力 HTML では、リストレベル設定はリスト項目で返されます。既定のプロパティは返されません。</span><span class="sxs-lookup"><span data-stu-id="57e34-p136">The **list-style-type** and CSS [style](#styles) properties of the element. In the output HTML, list-level settings are returned on list items. Default properties are not returned.</span></span> |
 
### <a name="list-styles"></a><span data-ttu-id="57e34-394">リストのスタイル</span><span class="sxs-lookup"><span data-stu-id="57e34-394">List styles</span></span>

<span data-ttu-id="57e34-395">Microsoft Graph の OneNote API では、次のリストのスタイルをサポートします。</span><span class="sxs-lookup"><span data-stu-id="57e34-395">The OneNote APIs in Microsoft Graph support the following list styles:</span></span>

|<span data-ttu-id="57e34-396">番号付きリスト</span><span class="sxs-lookup"><span data-stu-id="57e34-396">Ordered list</span></span>|<span data-ttu-id="57e34-397">記号付きリスト</span><span class="sxs-lookup"><span data-stu-id="57e34-397">Unordered list</span></span>|
|:------|:------|
| <span data-ttu-id="57e34-398">none</span><span class="sxs-lookup"><span data-stu-id="57e34-398">none</span></span> | <span data-ttu-id="57e34-399">none</span><span class="sxs-lookup"><span data-stu-id="57e34-399">none</span></span> |
| <span data-ttu-id="57e34-400">decimal (default)</span><span class="sxs-lookup"><span data-stu-id="57e34-400">decimal (default)</span></span> | <span data-ttu-id="57e34-401">disc (default)</span><span class="sxs-lookup"><span data-stu-id="57e34-401">disc (default)</span></span> |
| <span data-ttu-id="57e34-402">lower-alpha</span><span class="sxs-lookup"><span data-stu-id="57e34-402">lower-alpha</span></span> | <span data-ttu-id="57e34-403">Circle</span><span class="sxs-lookup"><span data-stu-id="57e34-403">circle</span></span> |
| <span data-ttu-id="57e34-404">lower-roman</span><span class="sxs-lookup"><span data-stu-id="57e34-404">lower-roman</span></span> | <span data-ttu-id="57e34-405">square</span><span class="sxs-lookup"><span data-stu-id="57e34-405">square</span></span> |
| <span data-ttu-id="57e34-406">upper-alpha</span><span class="sxs-lookup"><span data-stu-id="57e34-406">upper-alpha</span></span> | &nbsp; |
| <span data-ttu-id="57e34-407">upper-roman</span><span class="sxs-lookup"><span data-stu-id="57e34-407">upper-roman</span></span> | &nbsp; |
 
<span data-ttu-id="57e34-408">入力 HTML の **ol** 要素または **ul** 要素のリストにはグローバル スタイルを適用できますが、スタイルは **li** 要素で返されます。</span><span class="sxs-lookup"><span data-stu-id="57e34-408">You can apply global styles for a list on the **ol** or **ul** element in the input HTML, but styles are returned on the **li** elements.</span></span>

#### <a name="homogenous-list-style"></a><span data-ttu-id="57e34-409">同種リスト スタイル</span><span class="sxs-lookup"><span data-stu-id="57e34-409">Homogenous list style</span></span>

<span data-ttu-id="57e34-410">この例は、**ol** 要素のリスト スタイルの種類と個々のリスト項目の CSS スタイルを設定する入力 HTML を示しています。</span><span class="sxs-lookup"><span data-stu-id="57e34-410">This example shows input HTML that sets the list style type on the **ol** element and CSS styles on individual list items.</span></span>

```html
<ol style="list-style-type:upper-roman;color:blue">
    <li style="font-weight:bold">Jacksonville</li>
    <li style="text-decoration:line-through">Orlando</li>
    <li style="font-family:Courier">Naples</li>
</ol>
``` 

<span data-ttu-id="57e34-p137">これは出力 HTML です。スタイルが個々の **li** 要素または **span** 要素でインラインで返されることに注目してください。</span><span class="sxs-lookup"><span data-stu-id="57e34-p137">This is the output HTML. Notice that styles are returned inline on the individual **li** or **span** elements.</span></span>

```html
<ol>
    <li style="list-style-type:upper-roman"><span style="color:blue;font-weight:bold">Jacksonville</span></li>
    <li style="list-style-type:upper-roman"><span style="color:blue;text-decoration:line-through">Orlando</span></li>
    <li style="list-style-type:upper-roman"><span style="font-family:Courier;color:blue">Naples</span></li>
</ol>
``` 

#### <a name="variable-list-styles"></a><span data-ttu-id="57e34-413">可変のリスト スタイル</span><span class="sxs-lookup"><span data-stu-id="57e34-413">Variable list styles</span></span>

<span data-ttu-id="57e34-414">この例は、**li** 要素にさまざまなリスト スタイルの種類を設定する入力 HTML を示しています。</span><span class="sxs-lookup"><span data-stu-id="57e34-414">This example shows input HTML that sets different list style types on the **li** elements.</span></span>

```html
<ul style="font-style:italic">
    <li style="list-style-type:square">square style</li>
    <li style="list-style-type:circle">circle style</li>
    <li style="list-style-type:disc">disc style (default)</li>
</ul>
``` 

<span data-ttu-id="57e34-p138">これは出力 HTML です。スタイルが個々の **li** 要素または **span** 要素でインラインで返されることに注目してください。</span><span class="sxs-lookup"><span data-stu-id="57e34-p138">This is the output HTML. Notice that styles are returned inline on the individual **li** or **span** elements.</span></span>

```html
<ul>
    <li style="list-style-type:square"><span style="font-style:italic">square style</span></li>
    <li style="list-style-type:circle"><span style="font-style:italic">circle style</span></li>
    <li><span style="font-style:italic">disc style (default)</span></li>
</ul>
``` 


## <a name="tables"></a><span data-ttu-id="57e34-417">テーブル</span><span class="sxs-lookup"><span data-stu-id="57e34-417">Tables</span></span>

<span data-ttu-id="57e34-p139">テーブルは、**tr** 要素および **td** 要素を含めることができる **table** 要素として表されます。入れ子型のテーブルがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="57e34-p139">Tables are represented as **table** elements that can contain **tr** and **td** elements. Nested tables are supported.</span></span>

<span data-ttu-id="57e34-420">入力 HTML と出力 HTML では、テーブルに次の属性を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="57e34-420">Tables can contain the following attributes in the input and output HTML.</span></span> <span data-ttu-id="57e34-421">OneNote API では、**rowspan** 属性または **colspan** 属性はサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="57e34-421">The OneNote APIs do not support **rowspan** or **colspan** attributes.</span></span> 

#### <a name="input-attributes"></a><span data-ttu-id="57e34-422">入力属性</span><span class="sxs-lookup"><span data-stu-id="57e34-422">Input attributes</span></span>

|<span data-ttu-id="57e34-423">入力属性</span><span class="sxs-lookup"><span data-stu-id="57e34-423">Input attribute</span></span>|<span data-ttu-id="57e34-424">説明</span><span class="sxs-lookup"><span data-stu-id="57e34-424">Description</span></span>|
|:------|:------|
| <span data-ttu-id="57e34-425">data-id</span><span class="sxs-lookup"><span data-stu-id="57e34-425">data-id</span></span> | <span data-ttu-id="57e34-426">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="57e34-426">A reference for the element.</span></span><br/><br/><span data-ttu-id="57e34-427">[ページ コンテンツの更新](onenote-update-page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="57e34-427">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="57e34-428">style</span><span class="sxs-lookup"><span data-stu-id="57e34-428">style</span></span> | <span data-ttu-id="57e34-429">要素の CSS の [style](#styles)のプロパティ、および:</span><span class="sxs-lookup"><span data-stu-id="57e34-429">The CSS [style](#styles) properties of the element, and also:</span></span><br/> <span data-ttu-id="57e34-p141">- **border**。0px または 1px のいずれか。</span><span class="sxs-lookup"><span data-stu-id="57e34-p141">- **border**. Can be either 0px or 1px.</span></span><br/> <span data-ttu-id="57e34-p142">- **width**。**table** および **td** でサポートされます。ピクセル数またはページ幅のパーセンテージを使用します。</span><span class="sxs-lookup"><span data-stu-id="57e34-p142">- **width**. Supported by **table** and **td** as pixels or percentage of page width.</span></span><br/><br/><span data-ttu-id="57e34-434">例: `width="100px"` または `width="60%"`</span><span class="sxs-lookup"><span data-stu-id="57e34-434">Example: `width="100px"` or `width="60%"`</span></span> |
 

#### <a name="output-attributes"></a><span data-ttu-id="57e34-435">出力属性</span><span class="sxs-lookup"><span data-stu-id="57e34-435">Output attributes</span></span>

|<span data-ttu-id="57e34-436">出力属性</span><span class="sxs-lookup"><span data-stu-id="57e34-436">Output attribute</span></span>|<span data-ttu-id="57e34-437">説明</span><span class="sxs-lookup"><span data-stu-id="57e34-437">Description</span></span>|
|:------|:------|
| <span data-ttu-id="57e34-438">data-id</span><span class="sxs-lookup"><span data-stu-id="57e34-438">data-id</span></span> | <span data-ttu-id="57e34-439">要素の参照。</span><span class="sxs-lookup"><span data-stu-id="57e34-439">A reference for the element.</span></span><br/><br/><span data-ttu-id="57e34-440">[ページ コンテンツの更新](onenote-update-page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="57e34-440">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="57e34-441">id</span><span class="sxs-lookup"><span data-stu-id="57e34-441">id</span></span> | <span data-ttu-id="57e34-442">要素の一意の生成された ID。</span><span class="sxs-lookup"><span data-stu-id="57e34-442">A unique, generated ID for the element.</span></span> <span data-ttu-id="57e34-443">`includeIDs=true` クエリ オプションを使用した場合に、[ページの *content* エンドポイントに対する GET 要求](/graph/api/page-get?view=graph-rest-1.0)から返されます。</span><span class="sxs-lookup"><span data-stu-id="57e34-443">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="57e34-444">[ページ コンテンツの更新](onenote-update-page.md)に使用します。</span><span class="sxs-lookup"><span data-stu-id="57e34-444">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="57e34-445">style</span><span class="sxs-lookup"><span data-stu-id="57e34-445">style</span></span> | <span data-ttu-id="57e34-446">要素の CSS [style](#styles)のプロパティ。</span><span class="sxs-lookup"><span data-stu-id="57e34-446">The CSS [style](#styles) properties of the element.</span></span> |
 

<span data-ttu-id="57e34-447">次の例では、さまざまな方法を使用してテーブルのスタイルと返される出力 HTML を定義する入力 HTML を示しています。</span><span class="sxs-lookup"><span data-stu-id="57e34-447">The following examples show input HTML that uses different ways to define styles on tables and the output HTML that's returned.</span></span>

#### <a name="input-html-with-optional-settings-at-different-levels"></a><span data-ttu-id="57e34-448">さまざまなレベルのオプション設定を伴う入力 HTML</span><span class="sxs-lookup"><span data-stu-id="57e34-448">Input HTML with optional settings at different levels</span></span>

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
 
#### <a name="output-html-with-css-styles-returned-inline-on-the-td-elements"></a><span data-ttu-id="57e34-449">td 要素でインラインで返される CSS スタイルを伴う出力 HTML</span><span class="sxs-lookup"><span data-stu-id="57e34-449">Output HTML with CSS styles returned inline on the td elements</span></span>

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


## <a name="styles"></a><span data-ttu-id="57e34-450">スタイル</span><span class="sxs-lookup"><span data-stu-id="57e34-450">Styles</span></span>

<span data-ttu-id="57e34-451">Microsoft Graph の OneNote API は、ページ本文の要素 (**body**、**div**、**p**、**li**、**span** など) として、次に示すインライン CSS の **style** プロパティをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="57e34-451">OneNote APIs in Microsoft Graph support the following inline CSS **style** properties for elements in the page body, such as **body**, **div**, **p**, **li**, and **span**.</span></span>

|<span data-ttu-id="57e34-452">プロパティ</span><span class="sxs-lookup"><span data-stu-id="57e34-452">Property</span></span>|<span data-ttu-id="57e34-453">例</span><span class="sxs-lookup"><span data-stu-id="57e34-453">Example</span></span>|
|:------|:------|
| <span data-ttu-id="57e34-454">background-color</span><span class="sxs-lookup"><span data-stu-id="57e34-454">background-color</span></span> | <span data-ttu-id="57e34-455">`style="background-color:#66cc66"` (既定は white)</span><span class="sxs-lookup"><span data-stu-id="57e34-455">`style="background-color:#66cc66"` (defaults to white)</span></span><br/><br/><span data-ttu-id="57e34-456">16 進数形式と名前付きの色の両方がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="57e34-456">Both hexadecimal format and named colors are supported.</span></span> |
| <span data-ttu-id="57e34-457">color</span><span class="sxs-lookup"><span data-stu-id="57e34-457">color</span></span> | <span data-ttu-id="57e34-458">`style="color:#ffffff"` (既定は black)</span><span class="sxs-lookup"><span data-stu-id="57e34-458">`style="color:#ffffff"` (defaults to black)</span></span> |
| <span data-ttu-id="57e34-459">font-family</span><span class="sxs-lookup"><span data-stu-id="57e34-459">font-family</span></span> | <span data-ttu-id="57e34-460">`style="font-family:Courier"` (既定は Calibri)</span><span class="sxs-lookup"><span data-stu-id="57e34-460">`style="font-family:Courier"` (defaults to Calibri)</span></span> |
| <span data-ttu-id="57e34-461">font-size</span><span class="sxs-lookup"><span data-stu-id="57e34-461">font-size</span></span> | <span data-ttu-id="57e34-462">`style="font-size:10pt"` (既定は 11pt)</span><span class="sxs-lookup"><span data-stu-id="57e34-462">`style="font-size:10pt"` (defaults to 11pt)</span></span><br/><br/><span data-ttu-id="57e34-463">API は *pt* または *px* のフォント サイズを受け入れますが、*px* は *pt* に変換します。</span><span class="sxs-lookup"><span data-stu-id="57e34-463">The APIs accept font size in *pt* or *px*, but converts *px* to *pt*.</span></span> <span data-ttu-id="57e34-464">10 進数の値は、最も近い n.0pt または n.5pt に四捨五入されます。</span><span class="sxs-lookup"><span data-stu-id="57e34-464">Decimal values are rounded to the nearest n.0pt or n.5pt.</span></span> |
| <span data-ttu-id="57e34-465">font-style</span><span class="sxs-lookup"><span data-stu-id="57e34-465">font-style</span></span> | <span data-ttu-id="57e34-466">`style="font-style:italic"` (標準または斜体のみ)</span><span class="sxs-lookup"><span data-stu-id="57e34-466">`style="font-style:italic"` (normal or italic only)</span></span> |
| <span data-ttu-id="57e34-467">font-weight</span><span class="sxs-lookup"><span data-stu-id="57e34-467">font-weight</span></span> | <span data-ttu-id="57e34-468">`style="font-weight:bold"` (標準または太字のみ)</span><span class="sxs-lookup"><span data-stu-id="57e34-468">`style="font-weight:bold"` (normal or bold only)</span></span> |
| <span data-ttu-id="57e34-469">strike-through</span><span class="sxs-lookup"><span data-stu-id="57e34-469">strike-through</span></span> | `style="text-decoration:line-through"` |
| <span data-ttu-id="57e34-470">text-align</span><span class="sxs-lookup"><span data-stu-id="57e34-470">text-align</span></span> | <span data-ttu-id="57e34-471">`style="text-align:center"` (ブロック要素の場合のみ)</span><span class="sxs-lookup"><span data-stu-id="57e34-471">`style="text-align:center"` (for block elements only)</span></span> |
| <span data-ttu-id="57e34-472">text-decoration</span><span class="sxs-lookup"><span data-stu-id="57e34-472">text-decoration</span></span> | <span data-ttu-id="57e34-473">`style="text-decoration:underline"` (なし、または下線のみ)</span><span class="sxs-lookup"><span data-stu-id="57e34-473">`style="text-decoration:underline"` (none or underline only)</span></span> |
 

<span data-ttu-id="57e34-474">次のインライン文字スタイルもサポートされています:</span><span class="sxs-lookup"><span data-stu-id="57e34-474">The following inline character styles are also supported:</span></span>

<table id="simpletable">
<tr>
<td id="simplecell"><span data-ttu-id="57e34-475"><b></span><span class="sxs-lookup"><span data-stu-id="57e34-475"><b></span></span></td>
<td id="simplecell"><span data-ttu-id="57e34-476"><i></span><span class="sxs-lookup"><span data-stu-id="57e34-476"><i></span></span></td>
<td id="simplecell"><span data-ttu-id="57e34-477"><u></span><span class="sxs-lookup"><span data-stu-id="57e34-477"><u></span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="57e34-478"><em></span><span class="sxs-lookup"><span data-stu-id="57e34-478"><em></span></span></td>
<td id="simplecell"><span data-ttu-id="57e34-479"><strong></span><span class="sxs-lookup"><span data-stu-id="57e34-479"><strong></span></span></td>
<td id="simplecell"><span data-ttu-id="57e34-480"><strike></span><span class="sxs-lookup"><span data-stu-id="57e34-480"><strike></span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="57e34-481"><sup></span><span class="sxs-lookup"><span data-stu-id="57e34-481"><sup></span></span></td>
<td id="simplecell"><span data-ttu-id="57e34-482"><sub></span><span class="sxs-lookup"><span data-stu-id="57e34-482"><sub></span></span></td>
<td id="simplecell"><span data-ttu-id="57e34-483"><del></span><span class="sxs-lookup"><span data-stu-id="57e34-483"><del></span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="57e34-484"><cite></span><span class="sxs-lookup"><span data-stu-id="57e34-484"><cite></span></span></td>
<td id="simplecell">&nbsp;</td>
<td id="simplecell">&nbsp;</td>
</tr>
</table>

 
## <a name="input-and-output-html-example"></a><span data-ttu-id="57e34-485">入力 HTML と出力 HTML の例</span><span class="sxs-lookup"><span data-stu-id="57e34-485">Input and output HTML example</span></span>

<span data-ttu-id="57e34-486">次の画像は、Microsoft Graph で作成された簡単なページを示しています。</span><span class="sxs-lookup"><span data-stu-id="57e34-486">The following image shows a simple page that was created with Microsoft Graph.</span></span>

![Wikipedia によるコンテンツのスタディ ノートを付記した OneNote ページの画像](images/onenote-sample-image.png)

<span data-ttu-id="57e34-488">これは、ページを作成するためにメッセージ本文で送信された入力 HTML です。</span><span class="sxs-lookup"><span data-stu-id="57e34-488">This is the input HTML sent in the message body to create the page.</span></span>

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

<span data-ttu-id="57e34-489">これは、[ページ コンテンツを取得](onenote-get-content.md)するときに Microsoft Graph が返す出力 HTML です。</span><span class="sxs-lookup"><span data-stu-id="57e34-489">This is the output HTML that Microsoft Graph returns when you [get page content](onenote-get-content.md).</span></span>

> <span data-ttu-id="57e34-490">**注:** [ページを作成する](onenote-create-page.md)ときや、[ページのメタデータを取得する](/graph/api/page-get?view=graph-rest-1.0)ときに、API は **contentUrl** プロパティのページの*コンテンツ* エンドポイント URL を返します。</span><span class="sxs-lookup"><span data-stu-id="57e34-490">**Note:** When you [create a page](onenote-create-page.md) or [get page metadata](/graph/api/page-get?view=graph-rest-1.0), the API returns the *content* endpoint URL of the page in the **contentUrl** property.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="57e34-491">関連項目</span><span class="sxs-lookup"><span data-stu-id="57e34-491">See also</span></span>

- [<span data-ttu-id="57e34-492">OneNote コンテンツと構造を取得する</span><span class="sxs-lookup"><span data-stu-id="57e34-492">Get OneNote content and structure</span></span>](onenote-get-content.md)
- [<span data-ttu-id="57e34-493">OneNote ページを作成する</span><span class="sxs-lookup"><span data-stu-id="57e34-493">Create OneNote pages</span></span>](onenote-create-page.md)
- [<span data-ttu-id="57e34-494">OneNote ページ コンテンツを更新する</span><span class="sxs-lookup"><span data-stu-id="57e34-494">Update OneNote page content</span></span>](onenote-update-page.md)
- [<span data-ttu-id="57e34-495">画像、ビデオ、ファイルを追加する</span><span class="sxs-lookup"><span data-stu-id="57e34-495">Add images, videos, and files</span></span>](onenote-images-files.md)
