# <a name="use-note-tags-in-onenote-pages"></a><span data-ttu-id="45d1b-101">OneNote ページでノート シールを使用する</span><span class="sxs-lookup"><span data-stu-id="45d1b-101">Use note tags in OneNote pages</span></span>

<span data-ttu-id="45d1b-102">*__適用対象:__ OneDrive のコンシューマー ノートブック | Office 365 のエンタープライズ ノートブック*</span><span class="sxs-lookup"><span data-stu-id="45d1b-102">*__Applies to:__ Consumer notebooks on OneDrive | Enterprise notebooks on Office 365*</span></span>

<span data-ttu-id="45d1b-103">次の図に示すように、`data-tag` 属性を使用してチェック ボックス、星、その他の組み込みノート シールを OneNote ページに追加したり、更新したりします。</span><span class="sxs-lookup"><span data-stu-id="45d1b-103">Use the `data-tag` attribute to add and update check boxes, stars, and other built-in note tags on a OneNote page, as shown in the following image.</span></span>

![OneNote ページに表示される 3 つのノート シール。](images/note-tags-example.PNG)


<a name="attributes"></a>
## <a name="note-tag-attributes"></a><span data-ttu-id="45d1b-105">ノート シールの属性</span><span class="sxs-lookup"><span data-stu-id="45d1b-105">Note tag attributes</span></span>

<span data-ttu-id="45d1b-106">OneNote ページの HTML では、ノート シールは `data-tag` 属性として示されます。</span><span class="sxs-lookup"><span data-stu-id="45d1b-106">In the HTML of a OneNote page, a note tag is represented by the `data-tag` attribute.</span></span> <span data-ttu-id="45d1b-107">例:</span><span class="sxs-lookup"><span data-stu-id="45d1b-107">For example:</span></span>

- <span data-ttu-id="45d1b-108">チェック マークのない To Do ホックス:  `<p data-tag="to-do">`</span><span class="sxs-lookup"><span data-stu-id="45d1b-108">An unchecked to-do box:  \`</span></span> 
- <span data-ttu-id="45d1b-109">チェック マークのある To Do ホックス:  `<p data-tag="to-do:completed">`</span><span class="sxs-lookup"><span data-stu-id="45d1b-109">A checked to-do box:  \`</span></span> 
- <span data-ttu-id="45d1b-110">星:  `<h2 data-tag="important">`</span><span class="sxs-lookup"><span data-stu-id="45d1b-110">A star:  \`</span></span> 

<span data-ttu-id="45d1b-111">`data-tag` の値は shape で構成されますが、status の場合もあります。</span><span class="sxs-lookup"><span data-stu-id="45d1b-111">A `data-tag` value is composed of a shape, and sometimes a status.</span></span> <span data-ttu-id="45d1b-112">(*すべての[サポートされる値](#built-in-note-tags-for-onenote)をご覧ください*)</span><span class="sxs-lookup"><span data-stu-id="45d1b-112">(*see all [supported values](#built-in-note-tags-for-onenote)*)</span></span>

| <span data-ttu-id="45d1b-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="45d1b-113">Property</span></span> | <span data-ttu-id="45d1b-114">説明</span><span class="sxs-lookup"><span data-stu-id="45d1b-114">Description</span></span> |  
|:------|:------|  
| <span data-ttu-id="45d1b-115">shape</span><span class="sxs-lookup"><span data-stu-id="45d1b-115">shape</span></span> | <span data-ttu-id="45d1b-116">ノート シールの識別子 (例: `to-do` または `important`)。</span><span class="sxs-lookup"><span data-stu-id="45d1b-116">The identifier of the note tag (example: `to-do` or `important`).</span></span> |  
| <span data-ttu-id="45d1b-117">status</span><span class="sxs-lookup"><span data-stu-id="45d1b-117">status</span></span> | <span data-ttu-id="45d1b-p103">チェック ボックス ノート シールの状態。チェック ボックスを完了状態に設定する場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="45d1b-p103">The status of check-box note tags. This is used only to set check boxes as completed.</span></span> |  
 

<a name="note-tags"></a>
## <a name="add-or-update-note-tags"></a><span data-ttu-id="45d1b-120">ノート シールの追加または更新</span><span class="sxs-lookup"><span data-stu-id="45d1b-120">Add or update note tags</span></span>

<span data-ttu-id="45d1b-121">組み込みのノート シールは、サポートされた要素で `data-tag` 属性を使用するだけで、追加したり更新したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="45d1b-121">To add or update a built-in note tag, just use the `data-tag` attribute on a supported element.</span></span> <span data-ttu-id="45d1b-122">例として、important というマークが付けられた段落を次に示します。</span><span class="sxs-lookup"><span data-stu-id="45d1b-122">For example, here's a paragraph marked as important:</span></span>

```html
<p data-tag="important">...</p>
```

<span data-ttu-id="45d1b-123">複数のノート シールはコンマで区切ります。</span><span class="sxs-lookup"><span data-stu-id="45d1b-123">Separate multiple note tags with commas:</span></span>

```html
<p data-tag="important, critical">...</p>
```

<span data-ttu-id="45d1b-124">次に示す要素で、`data-tag` を定義できます。</span><span class="sxs-lookup"><span data-stu-id="45d1b-124">You can define a `data-tag` on the following elements:</span></span>

- <span data-ttu-id="45d1b-125">p</span><span class="sxs-lookup"><span data-stu-id="45d1b-125">p</span></span> 
- <span data-ttu-id="45d1b-126">ul、ol、li (*詳細については、「[リストのノート シール](#note-tags-on-lists)」を参照*)</span><span class="sxs-lookup"><span data-stu-id="45d1b-126">ul, ol, li (*see more about [note tags on lists](#note-tags-on-lists)*)</span></span>
- <span data-ttu-id="45d1b-127">img</span><span class="sxs-lookup"><span data-stu-id="45d1b-127">img</span></span> 
- <span data-ttu-id="45d1b-128">h1 から h6</span><span class="sxs-lookup"><span data-stu-id="45d1b-128">h1 - h6</span></span> 
- <span data-ttu-id="45d1b-129">title</span><span class="sxs-lookup"><span data-stu-id="45d1b-129">title</span></span> 

<span data-ttu-id="45d1b-130">Microsoft Graph で使用できるノート シールのリストの「[組み込みノート シール](#built-in-note-tags-for-onenote)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="45d1b-130">See [Built-in note tags](#built-in-note-tags-for-onenote) for a list of note tags that you can use with the OneNote API.</span></span> <span data-ttu-id="45d1b-131">Microsoft Graph を使用したカスタム シールの追加または更新はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="45d1b-131">Adding or updating custom tags using the OneNote API is not supported.</span></span>
 
<span data-ttu-id="45d1b-132">**例**</span><span class="sxs-lookup"><span data-stu-id="45d1b-132">**Examples**</span></span>

<span data-ttu-id="45d1b-133">最初の項目が完了状態の簡単な To Do リストを以下に示します。</span><span class="sxs-lookup"><span data-stu-id="45d1b-133">Here's a simple to-do list with the first item completed.</span></span>

```html 
<p data-tag="to-do:completed" data-id="prep">Till garden bed</p> 
<p data-tag="to-do" data-id="spring">Plant peas and spinach</p>
<p data-tag="to-do" data-id="summer">Plant tomatoes and peppers</p>
```

<span data-ttu-id="45d1b-134">上記の `<p>` タグには、それぞれ `data-id` 属性が含まれている点に注意してください。</span><span class="sxs-lookup"><span data-stu-id="45d1b-134">Note that the `<p>` tags above each include a `data-id` attribute.</span></span> <span data-ttu-id="45d1b-135">このようにすると、チェック ボックス ノート シールの更新が簡単になります。</span><span class="sxs-lookup"><span data-stu-id="45d1b-135">This makes it easier to update the check-box note tags.</span></span> <span data-ttu-id="45d1b-136">たとえば、次に示す要求では、春植え (spring planting) の To Do 項目に完了のマークを付けます。</span><span class="sxs-lookup"><span data-stu-id="45d1b-136">For example, the following request marks the spring planting to-do item as completed.</span></span>

``` 
PATCH https://graph.microsoft.com/v1.0/me/onenote/notebooks/pages/{page-id}/content

Content-Type: application/json
Authorization: Bearer {token}

[
   {
    'target':'#spring',
    'action':'replace',
    'content':'<p data-tag="to-do:completed"  data-id="spring">Plant peas and spinach</p>'
  }
]
```

<span data-ttu-id="45d1b-137">次に示す要求では、すべての[組み込みノート シール](#built-in-note-tags-for-onenote)を含んだページを作成します。</span><span class="sxs-lookup"><span data-stu-id="45d1b-137">The following request creates a page that contains all [built-in note tags](#built-in-note-tags-for-onenote).</span></span>

``` 
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/pages

Content-Type: text/html
Authorization: Bearer {token}


<!DOCTYPE html>
<html>
  <head>
    <title data-tag="to-do:completed">All built-in note tags</title>
  </head>
  <body>
    <h1 data-tag="important">Paragraphs with built-in note tags</h1>
    <p data-tag="to-do">to-do</p>
    <p data-tag="important">important</p>
    <p data-tag="question">question</p>
    <p data-tag="definition">definition</p>
    <p data-tag="highlight">highlight</p>
    <p data-tag="contact">contact</p>
    <p data-tag="address">address</p>
    <p data-tag="phone-number">phone-number</p>
    <p data-tag="web-site-to-visit">web-site-to-visit</p>
    <p data-tag="idea">idea</p>
    <p data-tag="password">password</p>
    <p data-tag="critical">critical</p>
    <p data-tag="project-a">project-a</p>
    <p data-tag="project-b">project-b</p>
    <p data-tag="remember-for-later">remember-for-later</p>
    <p data-tag="movie-to-see">movie-to-see</p>
    <p data-tag="book-to-read">book-to-read</p>
    <p data-tag="music-to-listen-to">music-to-listen-to</p>
    <p data-tag="source-for-article">source-for-article</p>
    <p data-tag="remember-for-blog">remember-for-blog</p>
    <p data-tag="discuss-with-person-a">discuss-with-person-a</p>
    <p data-tag="discuss-with-person-b">discuss-with-person-b</p>
    <p data-tag="discuss-with-manager">discuss-with-manager</p>
    <p data-tag="send-in-email">send-in-email</p>
    <p data-tag="schedule-meeting">schedule-meeting</p>
    <p data-tag="call-back">call-back</p>
    <p data-tag="to-do-priority-1">to-do-priority-1</p>
    <p data-tag="to-do-priority-2">to-do-priority-2</p>
    <p data-tag="client-request">client-request</p>
    <h1 data-tag="important">Paragraphs with check boxes marked with "completed" status</h1>
    <p data-tag="to-do:completed">to-do:completed</p>
    <p data-tag="discuss-with-person-a:completed">discuss-with-person-a:completed</p>
    <p data-tag="discuss-with-person-b:completed">discuss-with-person-b:completed</p>
    <p data-tag="discuss-with-manager:completed">discuss-with-manager:completed</p>
    <p data-tag="schedule-meeting:completed">schedule-meeting:completed</p>
    <p data-tag="call-back:completed">call-back:completed</p>
    <p data-tag="to-do-priority-1:completed">to-do-priority-1:completed</p>
    <p data-tag="to-do-priority-2:completed">to-do-priority-2:completed</p>
    <p data-tag="client-request:completed">client-request:completed</p>
    <h1 data-tag="important">Multiple note tags</h1>
    <p data-tag="project-a,  client-request:completed">Two note tags:  project-a, client-request:completed</p>
    <p data-tag="idea, send-in-email, question">Three note tags:  idea, send-in-email, question</p>
    <h1 data-tag="important">Using note tags with other elements</h1>
    <p><b>Note tag on a list item:</b></p>
    <ul>
      <li data-tag="to-do-priority-1:completed">Make a to-do list</li>
    </ul>
    <p><b>Note tag on an image:</b></p>
    <img data-tag="source-for-article" src="http://placecorgi.com/200" />
    <p><b>Note tag with embedded style:</b></p>
    <p data-tag="important">Next time, <b>don't</b> forget to invite <span style="background-color:yellow">Dan</span>.</p>
  </body>
</html>
``` 

<span data-ttu-id="45d1b-138">ページ作成の詳細については、「[OneNote ページの作成](onenote-create-page.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="45d1b-138">For more information about creating pages, see [Create OneNote pages](onenote-create-page.md).</span></span> <span data-ttu-id="45d1b-139">ページ更新の詳細については、「[OneNote ページの更新](onenote_update_page.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="45d1b-139">For more about updating pages, see [Update OneNote pages](onenote_update_page.md).</span></span>


<a name="note-tags-lists"></a>
### <a name="note-tags-on-lists"></a><span data-ttu-id="45d1b-140">リストのノート シール</span><span class="sxs-lookup"><span data-stu-id="45d1b-140">Note tags on lists</span></span>

<span data-ttu-id="45d1b-141">リストのノート シールの処理方法に関するいくつかのガイドラインを次に示します。</span><span class="sxs-lookup"><span data-stu-id="45d1b-141">Here are some guidelines for working with note tags on lists:</span></span>

- <span data-ttu-id="45d1b-142">To Do リストには、`p` 要素を使用します。</span><span class="sxs-lookup"><span data-stu-id="45d1b-142">Use `p` elements for to-do lists.</span></span> <span data-ttu-id="45d1b-143">この要素は行頭文字や行頭番号を表示しません。また、簡単に更新できます。</span><span class="sxs-lookup"><span data-stu-id="45d1b-143">They don't display a bullet or number, and they're easier to update.</span></span>

- <span data-ttu-id="45d1b-144">すべてのリスト項目に対して**同じ**ノート シールを表示するリストを作成または更新する場合は、次の操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="45d1b-144">To create or update lists that display the **same** note tag for all list items:</span></span>
  
   <p id="indent"><span data-ttu-id="45d1b-145">`ul` または `ol` に `data-tag` を定義します。</span><span class="sxs-lookup"><span data-stu-id="45d1b-145">Define `data-tag` on the `ul` or `ol`.</span></span> <span data-ttu-id="45d1b-146">リスト全体を更新するには、`ul` または `ol` に `data-tag` を再定義する必要があります。</span><span class="sxs-lookup"><span data-stu-id="45d1b-146">To update the entire list, you'll need to redefine `data-tag` on the `ul` or `ol`.</span></span></p>

- <span data-ttu-id="45d1b-147">一部またはすべてのリスト項目に対して**一意**のノート シールを表示するリストを作成または更新する場合は、次の操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="45d1b-147">To create or update lists that display **unique** note tag for some or all list items:</span></span>
  
   <p id="indent"><span data-ttu-id="45d1b-148">`li` 要素に `data-tag` を定義します。この `li` 要素は、`ul` または `ol` でネストしてはいけません。</span><span class="sxs-lookup"><span data-stu-id="45d1b-148">Define `data-tag` on `li` elements, and don't nest the `li` elements in a `ul` or `ol`.</span></span> <span data-ttu-id="45d1b-149">リスト全体を更新するには、出力 HTML で返される `ul` を削除して、ネストされていない `li` 要素のみを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="45d1b-149">To update the entire list, you'll need to remove the `ul` that's returned in the output HTML and provide only the unnested `li` elements.</span></span></p>

- <span data-ttu-id="45d1b-150">特定の `li` 要素を更新するには、次の操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="45d1b-150">To update specific `li` elements:</span></span>

   <p id="indent"><span data-ttu-id="45d1b-151">それぞれの `li` 要素を個別にターゲットにして、`li` 要素に `data-tag` を定義します。</span><span class="sxs-lookup"><span data-stu-id="45d1b-151">Target the `li` elements individually and define the `data-tag` on the `li` element.</span></span> <span data-ttu-id="45d1b-152">個別に処理された `li` 要素は、元のリストがどのように定義されていても、一意のノート シールを表示するように更新できます。</span><span class="sxs-lookup"><span data-stu-id="45d1b-152">Any individually addressed `li` element can be updated to display a unique note tag, no matter how the list was originally defined.</span></span></p>

<span data-ttu-id="45d1b-153">ガイドラインは Microsoft Graph により適用される次の規則に基づいています。</span><span class="sxs-lookup"><span data-stu-id="45d1b-153">The guidelines are based on the following rules that are applied by the OneNote API:</span></span>

- <span data-ttu-id="45d1b-154">`ul` または `ol` の `data-tag` 設定は、子 `li` 要素の設定をすべて上書きします。</span><span class="sxs-lookup"><span data-stu-id="45d1b-154">The `data-tag` setting for a `ul` or `ol` overrides all settings on child `li` elements.</span></span> <span data-ttu-id="45d1b-155">これは、子 `li` 要素でのみ `data-tag` を指定している (`ul` または `ol` では指定していない) 場合にも当てはまります。</span><span class="sxs-lookup"><span data-stu-id="45d1b-155">This applies even when the `ul` or `ol` doesn't specify a `data-tag` but its child `li` elements do.</span></span>

   <span data-ttu-id="45d1b-156">たとえば、`data-tag="project-a"` を定義している `ul` または `ol` を作成すると、そのリスト項目のすべてが *Project A* ノート シールを表示するようになります。</span><span class="sxs-lookup"><span data-stu-id="45d1b-156">For example, if you create a `ul` or `ol` that defines `data-tag="project-a"`, all its list items will display the *Project A* note tag.</span></span> <span data-ttu-id="45d1b-157">また、`ul` または `ol` で `data-tag` を定義していない場合は、そのどの項目にもノート シールが表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="45d1b-157">Or if the `ul` or `ol` doesn't define a `data-tag`, none of its items will display a note tag.</span></span> <span data-ttu-id="45d1b-158">この上書きは、子 `li` 要素の明示的な設定に関係なく発生します。</span><span class="sxs-lookup"><span data-stu-id="45d1b-158">This override happens regardless of any explicit settings on child `li` elements.</span></span>

- <span data-ttu-id="45d1b-159">次に示す条件下では、固有の `data-tag` 設定がリスト項目に適用されます。</span><span class="sxs-lookup"><span data-stu-id="45d1b-159">Unique `data-tag` settings are honored for list items under the following conditions:</span></span>

   - <span data-ttu-id="45d1b-160">作成要求または更新要求で、`li` 要素が `ul` または `ol` 内でネストされていない。</span><span class="sxs-lookup"><span data-stu-id="45d1b-160">The `li` elements are not nested in a `ul` or `ol` in a create or update request.</span></span>

   - <span data-ttu-id="45d1b-161">更新要求で、`li` 要素が個別に処理される。</span><span class="sxs-lookup"><span data-stu-id="45d1b-161">An `li` element is individually addressed in an update request.</span></span>

- <span data-ttu-id="45d1b-162">入力 HTML で送信されるネストされていない `li` 要素は、出力 HTML では `ul` で返されます。</span><span class="sxs-lookup"><span data-stu-id="45d1b-162">Unnested `li` elements sent in input HTML are returned in a `ul` in the output HTML.</span></span>

- <span data-ttu-id="45d1b-163">出力 HTML では、すべての `data-tag` リストの設定が、リスト項目の `span` 要素で定義されます。</span><span class="sxs-lookup"><span data-stu-id="45d1b-163">In output HTML, all `data-tag` list settings are defined on `span` elements on the list items.</span></span>

<br /><span data-ttu-id="45d1b-p114"> 次のコードは、これらの規則の一部がどのように適用されるかを示しています。入力 HTML は、ノート シールが含まれる 2 つのリストを作成します。出力 HTML は、ページ コンテンツを取得するときに返されるリストです。</span><span class="sxs-lookup"><span data-stu-id="45d1b-p114"> The following code shows how some of these rules are applied. The input HTML creates two lists with note tags. The output HTML is what's returned for the lists when you retrieve page content.</span></span>

<span data-ttu-id="45d1b-167">**入力 HTML**</span><span class="sxs-lookup"><span data-stu-id="45d1b-167">**Input HTML**</span></span>

```html 
<!--To display the same note tag on all list items, define note tags on the ul or ol.--> 
<ul data-tag="project-a" data-id="agenda">
  <li>An item with a Project A note tag</li>
  <li>An item with a Project A note tag</li>
</ul>

<!--To display unique note tags on list items, don't nest li elements in a ul or ol.--> 
<li data-tag="idea" data-id="my-idea">An item with an Idea note tag</li>
<li data-tag="question" data-id="my-question">An item with a Question note tag</li>
```
 
<span data-ttu-id="45d1b-168">**出力 HTML**</span><span class="sxs-lookup"><span data-stu-id="45d1b-168">**Output HTML**</span></span>

```html 
<ul>
  <li><span data-tag="project-a">An item with a Project A note tag</span></li>
  <li><span data-tag="project-a">An item with a Project A note tag</span></li>
</ul>
<br />
<ul>
  <li style="..."><span data-tag="idea">An item with an Idea note tag</span></li>
  <li style="..."><span data-tag="question">An item with a Question note tag</span></li>
</ul>
```

<a name="output-html"></a>
## <a name="retrieve-note-tags"></a><span data-ttu-id="45d1b-169">ノート シールの取得</span><span class="sxs-lookup"><span data-stu-id="45d1b-169">Retrieve note tags</span></span>

<span data-ttu-id="45d1b-170">ページのコンテンツを取得する場合、組み込みのノート シールは出力 HTML に含まれています。</span><span class="sxs-lookup"><span data-stu-id="45d1b-170">Built-in note tags are included in the output HTML when you get page content:</span></span>

`GET ../api/v1.0/pages/{page-id}/content` 

<span data-ttu-id="45d1b-171">出力 HTML 内の `data-tag` 属性には、常に shape 値が含まれています。完了状態に設定されたチェック ボックス ノート シールを表す場合にのみ status も含まれます。</span><span class="sxs-lookup"><span data-stu-id="45d1b-171">A `data-tag` attribute in the output HTML always includes a shape value, and it only includes a status if it represents a check-box note tag that's set to completed.</span></span> <span data-ttu-id="45d1b-172">次の例は、いくつかのノート シールを作成する入力 HTML と、返される出力 HTML を示しています。</span><span class="sxs-lookup"><span data-stu-id="45d1b-172">The following examples show the input HTML used to create some note tags and the output HTML that's returned.</span></span>

<span data-ttu-id="45d1b-173">**入力 HTML**</span><span class="sxs-lookup"><span data-stu-id="45d1b-173">**Input HTML**</span></span>

```html 
<h1>Status meeting</h1>
<p data-tag="important">Next week's meeting has been moved to <b>Wednesday</b>.</p>
<p data-tag="question">What are the exact dates for the conference?</p>
<p>Upcoming training opportunities. See Katie for more info.</p>
<p data-tag="project-a">Around the room updates.</p>
<ul data-tag="critical">
  <li>Design handouts</li>
  <li>Plan keynote</li>
</ul>
```

<span data-ttu-id="45d1b-174">**出力 HTML**</span><span class="sxs-lookup"><span data-stu-id="45d1b-174">**Output HTML**</span></span>

```html 
<h1 style="...">Status meeting</h1>
<p data-tag="important">Next week's meeting has been moved to <span style="font-weight:bold">Wednesday</span>.</p>
<p data-tag="question">What are the exact dates for the conference?</p>
<p>Upcoming training opportunities. See Katie for more info.</p>
<p data-tag="project-a">Around the room updates.</p>
<ul>
  <li><span data-tag="critical">Design handouts</span></li>
  <li><span data-tag="critical">Plan keynote</span></li>
</ul>
```

<span data-ttu-id="45d1b-175">リスト レベルで定義された `data-tag` 属性がリスト項目にプッシュされていることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="45d1b-175">Note that the `data-tag` attribute defined at the list level is pushed to its list items.</span></span> <span data-ttu-id="45d1b-176">リストにノート シールを使用することに関する詳細については、「[リストのノート シール](#note-tags-on-lists)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="45d1b-176">For more information about using note tags with lists, see [Note tags on lists](#note-tags-on-lists).</span></span>

> <span data-ttu-id="45d1b-177">**注:** 出力 HTML では、[定義] ノート シールと [要確認] ノート シールが、どちらも `data-tag="remember-for-later"` として返されます。</span><span class="sxs-lookup"><span data-stu-id="45d1b-177">In the output HTML, the definition and remember-for-later note tags are both returned as `data-tag="remember-for-later"`.</span></span> <span data-ttu-id="45d1b-178">`title` 要素はノート シールの情報を返しません。</span><span class="sxs-lookup"><span data-stu-id="45d1b-178">The `title` element doesn't return any note tag information.</span></span>

<a name="built-in-tags"></a>
## <a name="built-in-note-tags-for-onenote"></a><span data-ttu-id="45d1b-179">OneNote の組み込みノート シール</span><span class="sxs-lookup"><span data-stu-id="45d1b-179">Built-in note tags for OneNote</span></span>

<span data-ttu-id="45d1b-180">OneNote には、次に示す組み込みのノート シールが用意されています。</span><span class="sxs-lookup"><span data-stu-id="45d1b-180">OneNote includes the following built-in note tags:</span></span>

![すべての組み込みノート シール。](images/note-tags-all.png)

<span data-ttu-id="45d1b-182">`data-tag` 属性に割り当てられる値は、次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="45d1b-182">The values you can assign to the `data-tag` attribute are shown below.</span></span> <span data-ttu-id="45d1b-183">カスタム シールはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="45d1b-183">Custom tags are not supported.</span></span>

||<span data-ttu-id="45d1b-184">タグ</span><span class="sxs-lookup"><span data-stu-id="45d1b-184">Tags</span></span>||
|:---|:---|:-----|
| `shape[:status]` |`to-do`<br />`to-do:completed`|`important`|
|`question`|`definition`|`highlight`|
|`contact`|`address`|`phone-number`|
|`web-site-to-visit`|`idea`|`password`|
|`critical`|`project-a`|`project-b`|
|`remember-for-later`|`movie-to-see`|`book-to-read`|
|`music-to-listen-to`|`source-for-article`|`remember-for-blog`|
|`discuss-with-person-a`<br />`discuss-with-person-a:completed`|`discuss-with-person-b`<br />`discuss-with-person-b:completed`|`discuss-with-manager`<br />`discuss-with-manager:completed`|
|`send-in-email`|`schedule-meeting`<br />`schedule-meeting:completed`|`call-back`<br />`call-back:completed`|
|`to-do-priority-1`<br />`to-do-priority-1:completed`|`to-do-priority-2`<br />`to-do-priority-2:completed`|`client-request`<br />`client-request:completed`|


<a name="request-response-info"></a>
## <a name="response-information"></a><span data-ttu-id="45d1b-185">応答情報</span><span class="sxs-lookup"><span data-stu-id="45d1b-185">Response information</span></span>
<span data-ttu-id="45d1b-186">Microsoft Graph は、次の情報を応答で返します。</span><span class="sxs-lookup"><span data-stu-id="45d1b-186">The OneNote API returns the following information in the response.</span></span>

| <span data-ttu-id="45d1b-187">応答データ</span><span class="sxs-lookup"><span data-stu-id="45d1b-187">Response data</span></span> | <span data-ttu-id="45d1b-188">説明</span><span class="sxs-lookup"><span data-stu-id="45d1b-188">Description</span></span> |  
|------|------|  
| <span data-ttu-id="45d1b-189">成功コード</span><span class="sxs-lookup"><span data-stu-id="45d1b-189">Success code</span></span> | <span data-ttu-id="45d1b-190">成功した POST 要求に対しては 201 HTTP ステータス コード、成功した PATCH 要求に対しては 204 HTTP ステータス コードが戻ります。</span><span class="sxs-lookup"><span data-stu-id="45d1b-190">A 201 HTTP status code for a successful POST request, and a 204 HTTP status code for a successful PATCH request.</span></span> |  
| <span data-ttu-id="45d1b-191">エラー</span><span class="sxs-lookup"><span data-stu-id="45d1b-191">Errors</span></span> | <span data-ttu-id="45d1b-192">Microsoft Graph から返されることのある OneNote エラーに関する詳細については、「[Microsoft Graph の OneNote API のエラー コード](onenote_error_codes.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="45d1b-192">Read [Error codes for OneNote APIs in Microsoft Graph](onenote_error_codes.md) to learn about OneNote errors that Microsoft Graph can return.</span></span> |  


<a name="permissions"></a>
## <a name="permissions"></a><span data-ttu-id="45d1b-193">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="45d1b-193">Permissions</span></span>

<span data-ttu-id="45d1b-p119">OneNote ページを作成または更新するには、適切なアクセス許可を要求する必要があります。アプリの動作に必要な最低限のアクセス許可を選択してください。</span><span class="sxs-lookup"><span data-stu-id="45d1b-p119">To create or update OneNote pages, you'll need to request appropriate permissions. Choose the lowest level of permissions that your app needs to do its work.</span></span>

<span data-ttu-id="45d1b-196">**_POST pages_ のアクセス許可**</span><span class="sxs-lookup"><span data-stu-id="45d1b-196">**Permissions for _POST pages_**</span></span>

- <span data-ttu-id="45d1b-197">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="45d1b-197">Notes.Create</span></span>
- <span data-ttu-id="45d1b-198">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="45d1b-198">Notes.ReadWrite</span></span>
- <span data-ttu-id="45d1b-199">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45d1b-199">Notes.ReadWrite.All</span></span>  

<span data-ttu-id="45d1b-200">**_PATCH pages_ のアクセス許可**</span><span class="sxs-lookup"><span data-stu-id="45d1b-200">**Permissions for _PATCH pages_**</span></span>

- <span data-ttu-id="45d1b-201">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="45d1b-201">Notes.ReadWrite</span></span>
- <span data-ttu-id="45d1b-202">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45d1b-202">Notes.ReadWrite.All</span></span>  

<span data-ttu-id="45d1b-203">アクセス許可のスコープと動作のしくみの詳細については、「[OneNote のアクセス許可のスコープ](permissions_reference.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="45d1b-203">For more information about permission scopes and how they work, see [OneNote permission scopes](permissions_reference.md).</span></span>


<a name="see-also"></a>
## <a name="additional-resources"></a><span data-ttu-id="45d1b-204">その他のリソース</span><span class="sxs-lookup"><span data-stu-id="45d1b-204">Additional resources</span></span>

- [<span data-ttu-id="45d1b-205">OneNote ページの作成</span><span class="sxs-lookup"><span data-stu-id="45d1b-205">Create OneNote pages</span></span>](onenote-create-page.md)
- [<span data-ttu-id="45d1b-206">OneNote ページ コンテンツを更新する</span><span class="sxs-lookup"><span data-stu-id="45d1b-206">Update OneNote page content</span></span>](onenote_update_page.md)
- [<span data-ttu-id="45d1b-207">OneNote との統合</span><span class="sxs-lookup"><span data-stu-id="45d1b-207">Integrate with OneNote</span></span>](integrate_with_onenote.md)
- [<span data-ttu-id="45d1b-208">OneNote の開発者ブログ</span><span class="sxs-lookup"><span data-stu-id="45d1b-208">OneNote Developer Blog</span></span>](http://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="45d1b-209">Stack Overflow 掲載の OneNote の開発に関する質問</span><span class="sxs-lookup"><span data-stu-id="45d1b-209">OneNote development questions on Stack Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="45d1b-210">OneNote GitHub のリポジトリ</span><span class="sxs-lookup"><span data-stu-id="45d1b-210">OneNote GitHub repos</span></span>](http://go.microsoft.com/fwlink/?LinkID=390178)  
 


