---
title: OneNote ページで絶対位置を指定した要素を作成する
description: OneNote ページの本文には、直接の子要素 `div`、`img`、`object` を複数含めることができます。これらの要素はページ上に独立して配置できます。
ms.openlocfilehash: 8478f5ae0da4d8c4617573fb99f91646a67d9356
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092399"
---
# <a name="create-absolute-positioned-elements-in-onenote-pages"></a><span data-ttu-id="2b258-103">OneNote ページで絶対位置を指定した要素を作成する</span><span class="sxs-lookup"><span data-stu-id="2b258-103">Create absolute positioned elements in OneNote pages</span></span>

<span data-ttu-id="2b258-104">OneNote ページの本文には、直接の子要素 `div`、`img`、`object` を複数含めることができます。これらの要素はページ上に独立して配置できます。</span><span class="sxs-lookup"><span data-stu-id="2b258-104">The body of a OneNote page can contain multiple direct `div`, `img`, and `object` child elements that can be positioned independently on the page.</span></span>

<a name="attributes"></a>

## <a name="attributes-and-positioning-behavior"></a><span data-ttu-id="2b258-105">属性と配置動作</span><span class="sxs-lookup"><span data-stu-id="2b258-105">Attributes and positioning behavior</span></span>

<span data-ttu-id="2b258-106">次に示すように、`data-absolute-enabled` 属性および [`style`](#supported-css-style-attributes) 属性を使用して、ページ上に絶対配置要素を作成します。</span><span class="sxs-lookup"><span data-stu-id="2b258-106">Use the `data-absolute-enabled` and [`style`](#supported-css-style-attributes) attributes to create absolute positioned elements on a page, as follows:</span></span>

- <span data-ttu-id="2b258-p101">body 要素は、`data-absolute-enabled="true"` を指定する必要があります。省略したり `false` に設定したりすると、API によって作成される `_default` 絶対配置 div の内側にすべての本文のコンテンツが表示され、すべての位置設定が無視されます。</span><span class="sxs-lookup"><span data-stu-id="2b258-p101">The body element must specify `data-absolute-enabled="true"`. If omitted or set to `false`, all body content is rendered inside a `_default` absolute positioned div that the API creates, and all position settings are ignored.</span></span>

- <span data-ttu-id="2b258-109">`div`、`img`、および `object` 要素のみが絶対配置要素になります。</span><span class="sxs-lookup"><span data-stu-id="2b258-109">Only `div`, `img`, and `object` elements can be absolute positioned elements.</span></span> 

- <span data-ttu-id="2b258-110">絶対配置要素は、`style="position:absolute"` を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2b258-110">Absolute positioned elements must specify `style="position:absolute"`.</span></span>

- <span data-ttu-id="2b258-p102">絶対配置要素は、`body` 要素の直接の子にする必要があります。body の直接の子要素が絶対配置でない `div`、`img`、または `object` 要素の場合は、絶対配置の `_default` div の内側に静的コンテンツとして表示されます。</span><span class="sxs-lookup"><span data-stu-id="2b258-p102">Absolute positioned elements must be direct children of the `body` element. Any direct children of the body that aren't absolute positioned `div`, `img`, or `object` elements are rendered as static content inside the absolute positioned `_default` div.</span></span>

- <span data-ttu-id="2b258-113">絶対配置要素は、指定された上と左の座標 (開始位置 0:0 を基準とした、タイトル領域の上部でページの左隅) に配置されます。</span><span class="sxs-lookup"><span data-stu-id="2b258-113">Absolute positioned elements are positioned at their specified top and left coordinates, relative to the 0:0 starting position at the top, left corner of the page above the title area.</span></span>

- <span data-ttu-id="2b258-p103">絶対配置要素が top または left の座標を省略していると、不足している座標には既定値の `top:120px` または `left:48px` が設定されます。これらの既定の座標は、title エリアの直下の位置を指定します。座標を省略すると、複数の要素の上部が積み重なることがある点に注意してください。</span><span class="sxs-lookup"><span data-stu-id="2b258-p103">If an absolute positioned element omits the top or left coordinate, the missing coordinate is set to its default value: `top:120px` or `left:48px`. These default coordinates specify a position just below the title area. Be aware that omitting coordinates can result in elements that are stacked on top of each other.</span></span>

- <span data-ttu-id="2b258-p104">絶対配置要素は、入れ子状態にしたり、定位置要素を含めたりすることはできません。API は、絶対配置の div 内の入れ子型の要素で指定された位置設定をすべて無視し、絶対配置の親 div 内の入れ子型のコンテンツを表示するとともに、応答の **api.diagnostics** プロパティで警告を返します。</span><span class="sxs-lookup"><span data-stu-id="2b258-p104">Absolute positioned elements cannot be nested or contain positioned elements. The API ignores any position settings specified on nested elements inside an absolute positioned div, renders the nested content inside the absolute positioned parent div, and returns a warning in the **api.diagnostics** property in the response.</span></span>


### <a name="example"></a><span data-ttu-id="2b258-119">例</span><span class="sxs-lookup"><span data-stu-id="2b258-119">Example</span></span>

<span data-ttu-id="2b258-120">次の例には、`p` の直接の子、絶対配置 div、非絶対配置 div が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2b258-120">The following example contains a direct `p` child, an absolute positioned div, and a non-absolute positioned div.</span></span>

#### <a name="input-html"></a><span data-ttu-id="2b258-121">入力 HTML</span><span class="sxs-lookup"><span data-stu-id="2b258-121">Input HTML</span></span>  

   ```html 
   <body data-absolute-enabled="true">
       <p>This content will appear in the _default div.</p>
       <div style="position:absolute;top:175px;left:100px" data-id="div1">
         <p>This content will appear in an absolute positioned div.</p>
       </div>
       <div>
           <p>This content will also appear in the _default div.</p>
       </div>
   </body>
   ```

<span data-ttu-id="2b258-p105">API は既定の div に非絶対配置 div を表示します。入れ子になった `<div>` タグは意味情報 (`data-id` など) を定義しないため、破棄されます。</span><span class="sxs-lookup"><span data-stu-id="2b258-p105">The API renders the non-absolute positioned div in the default div. Note that the nested  `<div>` tags are discarded because they do not define any semantic information (such as `data-id`).</span></span>

#### <a name="output-html"></a><span data-ttu-id="2b258-124">出力 HTML</span><span class="sxs-lookup"><span data-stu-id="2b258-124">Output HTML</span></span> 

   ```html 
   <body data-absolute-enabled="true" style="font-family:Calibri;font-size:11pt">
       <div data-id="_default" style="position:absolute;left:48px;top:120px;width:624px">
           <p>This content will appear in the _default div.</p>
           <p>This content will also appear in the _default div.</p>
       </div>
       <div data-id="div1" style="position:absolute;left:99px;top:174px;width:624px">
           <p>This content will appear in an absolute positioned div.</p>
       </div>
   </body>
   ```

### <a name="example"></a><span data-ttu-id="2b258-125">例</span><span class="sxs-lookup"><span data-stu-id="2b258-125">Example</span></span>

<span data-ttu-id="2b258-126">次の例では、絶対配置の div と絶対配置のイメージを 1 つずつ含むページを作成します。</span><span class="sxs-lookup"><span data-stu-id="2b258-126">The following example creates a page that contains one absolute positioned div and one absolute positioned image.</span></span>


#### <a name="input-html"></a><span data-ttu-id="2b258-127">入力 HTML</span><span class="sxs-lookup"><span data-stu-id="2b258-127">Input HTML</span></span>  

```html 
<html>
    <head>
        <title>Page Title</title>
    </head>
    <body data-absolute-enabled="true">
        <div style="position:absolute;width:280px;top:120px;left:68px">
            <p>Some text</p>
            <img style="width:120px" src="https://officeimg.vo.msecnd.net/en-us/files/018/949/ZA103278226.png" />
            <div>
                <p>More text inside a regular, nested div</p>
            </div>
        </div>
        <img style="position:absolute;width:360px;top:350px;left:300px" src="https://officeimg.vo.msecnd.net/en-us/files/018/949/ZA103278226.png" />
    </body>
</html>
```
 
<span data-ttu-id="2b258-p106">OneNote API は入力 HTML を評価し、OneNote によりサポートされるすべての意味内容と任意の意味情報を保持します。結果のページは、次に示すイメージのように表示されます (div とイメージの境界線は表示されません)。</span><span class="sxs-lookup"><span data-stu-id="2b258-p106">The OneNote API evaluates the input HTML and preserves all semantic content and any structural information that is supported by OneNote. The resulting page renders as shown in the following image (but without the visible borders for the div and image).</span></span> 

![絶対配置の div とイメージのある結果のページ](images/abs-pos.png)

<span data-ttu-id="2b258-p107">入力 HTML から変更された、作用していない入れ子になった div に注意してください。API は div のコンテンツを保持しますが、`<div>` タグは破棄します。これは、div は意味情報 (`data-id` など) を定義しないためです。</span><span class="sxs-lookup"><span data-stu-id="2b258-p107">Notice the changes to the non-contributing, nested div from the input HTML. The API preserves the div's content but discards the `<div>` tags because the div doesn't define semantic information (such as `data-id`).</span></span>

<span data-ttu-id="2b258-133">OneNote API が入力 HTML と出力 HTML を処理する方法の詳細については、「[OneNote ページの入力 HTML と出力 HTML](onenote-input-output-html.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2b258-133">For more information about how the OneNote API handles input and output HTML, see [Input and output HTML for OneNote pages](onenote-input-output-html.md).</span></span>

<a name="style-attributes"></a>

## <a name="supported-css-style-attributes"></a><span data-ttu-id="2b258-134">サポートされている CSS スタイルの属性</span><span class="sxs-lookup"><span data-stu-id="2b258-134">Supported CSS style attributes</span></span>

<span data-ttu-id="2b258-p108">絶対配置要素は、上と左の座標を指定できます。div とイメージでは幅を指定でき、イメージでは高さも指定できます。たとえば、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="2b258-p108">All absolute positioned elements can specify top and left positions. Divs and images can specify width, and images can also specify height. For example:</span></span>

```html
<img style="position:absolute;top:140px;left:95px;width:480px;height:665px" src="..." />
```

| <span data-ttu-id="2b258-138">属性</span><span class="sxs-lookup"><span data-stu-id="2b258-138">Attribute</span></span> | <span data-ttu-id="2b258-139">サポートされる要素</span><span class="sxs-lookup"><span data-stu-id="2b258-139">Supported element</span></span> | <span data-ttu-id="2b258-140">説明</span><span class="sxs-lookup"><span data-stu-id="2b258-140">Description</span></span> |  
|:------|:------|:------|  
| <span data-ttu-id="2b258-141">top</span><span class="sxs-lookup"><span data-stu-id="2b258-141">top</span></span> | <span data-ttu-id="2b258-142">div、img、object</span><span class="sxs-lookup"><span data-stu-id="2b258-142">div, img, object</span></span> | <span data-ttu-id="2b258-p109">要素の上部境界線の Y 軸座標 (ピクセル単位のみ)。既定は 120 ピクセル。</span><span class="sxs-lookup"><span data-stu-id="2b258-p109">The y-axis coordinate of the element's top border, in pixels only. Default is 120 pixels.</span></span><br/><br/><span data-ttu-id="2b258-145">例: `top:140px`</span><span class="sxs-lookup"><span data-stu-id="2b258-145">Example: `top:140px`</span></span> |  
| <span data-ttu-id="2b258-146">left</span><span class="sxs-lookup"><span data-stu-id="2b258-146">left</span></span> |  <span data-ttu-id="2b258-147">div、img、object</span><span class="sxs-lookup"><span data-stu-id="2b258-147">div, img, object</span></span>  | <span data-ttu-id="2b258-p110">要素の左境界線の X 軸座標 (ピクセル単位のみ)。既定は 48 ピクセル。</span><span class="sxs-lookup"><span data-stu-id="2b258-p110">The x-axis coordinate of the element's left border, in pixels only. Default is 48 pixels.</span></span><br/><br/><span data-ttu-id="2b258-150">例: `left:95px`</span><span class="sxs-lookup"><span data-stu-id="2b258-150">Example: `left:95px`</span></span> |  
| <span data-ttu-id="2b258-151">width</span><span class="sxs-lookup"><span data-stu-id="2b258-151">width</span></span> |  <span data-ttu-id="2b258-152">div、img</span><span class="sxs-lookup"><span data-stu-id="2b258-152">div, img</span></span>  | <span data-ttu-id="2b258-153">要素の幅 (ピクセル単位のみ)。</span><span class="sxs-lookup"><span data-stu-id="2b258-153">The width of the element, in pixels only.</span></span><br/><br/><span data-ttu-id="2b258-154">例: `width:480px`</span><span class="sxs-lookup"><span data-stu-id="2b258-154">Example: `width:480px`</span></span> |  
| <span data-ttu-id="2b258-155">height</span><span class="sxs-lookup"><span data-stu-id="2b258-155">height</span></span> | <span data-ttu-id="2b258-156">img</span><span class="sxs-lookup"><span data-stu-id="2b258-156">img</span></span> | <span data-ttu-id="2b258-p111">要素の高さ (ピクセル単位のみ)div の場合、高さは実行時に計算されるため、指定された高さの値は無視されます。</span><span class="sxs-lookup"><span data-stu-id="2b258-p111">The height of the element, in pixels only. For divs, height is calculated at runtime and any specified height value is ignored.</span></span><br/><br/><span data-ttu-id="2b258-159">例: `height:665px`</span><span class="sxs-lookup"><span data-stu-id="2b258-159">Example: `height:665px`</span></span> |  
 
<span data-ttu-id="2b258-p112">その他の位置属性、たとえば `z-index` などは無視されます。絶対配置の画像には、`data-render-src` または `src` のいずれかを使用できます。</span><span class="sxs-lookup"><span data-stu-id="2b258-p112">Other position attributes, such as `z-index`, are ignored. Absolute positioned images can use either the `data-render-src` or `src` attribute.</span></span>


<a name="request-response-info"></a>

## <a name="response-information"></a><span data-ttu-id="2b258-162">応答情報</span><span class="sxs-lookup"><span data-stu-id="2b258-162">Response information</span></span>

<span data-ttu-id="2b258-163">OneNote API は、次の情報を応答で返します。</span><span class="sxs-lookup"><span data-stu-id="2b258-163">The OneNote API returns the following information in the response.</span></span>

| <span data-ttu-id="2b258-164">応答データ</span><span class="sxs-lookup"><span data-stu-id="2b258-164">Response data</span></span> | <span data-ttu-id="2b258-165">説明</span><span class="sxs-lookup"><span data-stu-id="2b258-165">Description</span></span> |  
|:------|:------|  
| <span data-ttu-id="2b258-166">成功コード</span><span class="sxs-lookup"><span data-stu-id="2b258-166">Success code</span></span> | <span data-ttu-id="2b258-167">成功した POST 要求に対しては 201 HTTP ステータス コード、成功した PATCH 要求に対しては 204 HTTP ステータス コードが戻ります。</span><span class="sxs-lookup"><span data-stu-id="2b258-167">A 201 HTTP status code for a successful POST request, and a 204 HTTP status code for a successful PATCH request.</span></span> |  
| <span data-ttu-id="2b258-168">エラー</span><span class="sxs-lookup"><span data-stu-id="2b258-168">Errors</span></span> | <span data-ttu-id="2b258-169">Microsoft Graph から返されることのある OneNote エラーに関する詳細については、「[Microsoft Graph の OneNote API のエラー コード](onenote-error-codes.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2b258-169">Read [Error codes for OneNote APIs in Microsoft Graph](onenote-error-codes.md) to learn about OneNote errors that Microsoft Graph can return.</span></span> |  
  


<a name="permissions"></a>

## <a name="permissions"></a><span data-ttu-id="2b258-170">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2b258-170">Permissions</span></span>

<span data-ttu-id="2b258-p113">OneNote ページを作成または更新するには、適切なアクセス許可を要求する必要があります。アプリの動作に必要な最低限のアクセス許可を選択してください。</span><span class="sxs-lookup"><span data-stu-id="2b258-p113">To create or update OneNote pages, you'll need to request appropriate permissions. Choose the lowest level of permissions that your app needs to do its work.</span></span>

#### <a name="permissions-for-post-pages"></a><span data-ttu-id="2b258-173">POST ページのアクセス許可</span><span class="sxs-lookup"><span data-stu-id="2b258-173">Permissions for POST pages</span></span> 

- <span data-ttu-id="2b258-174">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="2b258-174">Notes.Create</span></span>
- <span data-ttu-id="2b258-175">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b258-175">Notes.ReadWrite</span></span>
- <span data-ttu-id="2b258-176">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b258-176">Notes.ReadWrite.All</span></span>  


#### <a name="permissions-for-patch-pages"></a><span data-ttu-id="2b258-177">PATCH ページのアクセス許可</span><span class="sxs-lookup"><span data-stu-id="2b258-177">Permissions for PATCH pages</span></span> 

- <span data-ttu-id="2b258-178">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b258-178">Notes.ReadWrite</span></span>
- <span data-ttu-id="2b258-179">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b258-179">Notes.ReadWrite.All</span></span>

<span data-ttu-id="2b258-180">アクセス許可のスコープと動作のしくみの詳細については、「[OneNote のアクセス許可のスコープ](permissions-reference.md#notes-permissions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2b258-180">For more information about permission scopes and how they work, see [OneNote permission scopes](permissions-reference.md#notes-permissions).</span></span>


<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="2b258-181">関連項目</span><span class="sxs-lookup"><span data-stu-id="2b258-181">See also</span></span>

- [<span data-ttu-id="2b258-182">OneNote ページを作成する</span><span class="sxs-lookup"><span data-stu-id="2b258-182">Create OneNote pages</span></span>](onenote-create-page.md)
- [<span data-ttu-id="2b258-183">OneNote ページ コンテンツを更新する</span><span class="sxs-lookup"><span data-stu-id="2b258-183">Update OneNote page content</span></span>](onenote-update-page.md)
- [<span data-ttu-id="2b258-184">OneNote との統合</span><span class="sxs-lookup"><span data-stu-id="2b258-184">Integrate with OneNote</span></span>](integrate-with-onenote.md)
- [<span data-ttu-id="2b258-185">OneNote の開発者ブログ</span><span class="sxs-lookup"><span data-stu-id="2b258-185">OneNote Developer Blog</span></span>](https://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="2b258-186">Stack Overflow 掲載の OneNote の開発に関する質問</span><span class="sxs-lookup"><span data-stu-id="2b258-186">OneNote development questions on Stack Overflow</span></span>](https://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="2b258-187">OneNote GitHub のリポジトリ</span><span class="sxs-lookup"><span data-stu-id="2b258-187">OneNote GitHub repos</span></span>](https://go.microsoft.com/fwlink/?LinkID=390178)  

