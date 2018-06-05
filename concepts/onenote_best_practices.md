# <a name="best-practices-for-working-with-the-onenote-api-in-microsoft-graph"></a><span data-ttu-id="09adf-101">Microsoft Graph で OneNote API を使用する場合のベスト プラクティス</span><span class="sxs-lookup"><span data-stu-id="09adf-101">Best practices for working with the OneNote API in Microsoft Graph</span></span>

<span data-ttu-id="09adf-102">この記事では、Microsoft Graph で OneNote API を使用するための推奨事項を提供します。</span><span class="sxs-lookup"><span data-stu-id="09adf-102">This article provides recommendations for working with the OneNote APIs in Microsoft Graph.</span></span> <span data-ttu-id="09adf-103">これらの推奨事項は、Stack Overflow と Twitter でよく寄せられる質問への回答に基づいています。</span><span class="sxs-lookup"><span data-stu-id="09adf-103">These recommendations are based on answers to common questions we see on StackOverflow and Twitter.</span></span>

## <a name="use-select-to-select-the-minimum-set-of-properties-you-need"></a><span data-ttu-id="09adf-104">$Select を使用して、必要なプロパティの最小限のセットを選択する</span><span class="sxs-lookup"><span data-stu-id="09adf-104">Use $select to select the minimum set of properties you need</span></span>
<span data-ttu-id="09adf-105">リソース (たとえば、ノートブック内のセクション) のクエリを実行するときには、次のような要求を行います。</span><span class="sxs-lookup"><span data-stu-id="09adf-105">When you query for a resource (for example, sections inside a notebook), you make a request similar to the following.</span></span>

```http
GET ~/notebooks/{id}/sections
```

<span data-ttu-id="09adf-106">これは、セクションのすべてのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="09adf-106">This retrieves all the properties of the sections.</span></span> <span data-ttu-id="09adf-107">ただし、すべてのプロパティが必要とは限りません。</span><span class="sxs-lookup"><span data-stu-id="09adf-107">However, you might not need all properties.</span></span> <span data-ttu-id="09adf-108">次の例のように、`$select` クエリ パラメーターを使用して、必要なプロパティだけを返すことができます。</span><span class="sxs-lookup"><span data-stu-id="09adf-108">You can use the `$select` query parameter to return just the properties that you want, as shown in the following example.</span></span>

```http
GET ~/notebooks/{id}/sections?$select=id,displayName
```

<span data-ttu-id="09adf-109">同じアプローチは、他の OneNote API に適用されます。</span><span class="sxs-lookup"><span data-stu-id="09adf-109">The same approach applies to other OneNote APIs.</span></span>

## <a name="use-expand-instead-of-making-multiple-api-calls"></a><span data-ttu-id="09adf-110">複数の API 呼び出しを実行するのではなく、$expand を使用します。</span><span class="sxs-lookup"><span data-stu-id="09adf-110">Use $expand instead of making multiple API calls</span></span>
<span data-ttu-id="09adf-111">ユーザーのノートブック、セクション、およびセクション グループのすべてを階層的なビューで取得します。</span><span class="sxs-lookup"><span data-stu-id="09adf-111">Suppose you want to retrieve all of the user’s notebooks, sections, and section groups in a hierarchical view.</span></span> <span data-ttu-id="09adf-112">次の方法でこれを行います。</span><span class="sxs-lookup"><span data-stu-id="09adf-112">You might accomplish that by doing the following:</span></span>

* <span data-ttu-id="09adf-113">`GET ~/notebooks` を呼び出して、ノートブックの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="09adf-113">Call `GET ~/notebooks` to get the list of notebooks.</span></span>
* <span data-ttu-id="09adf-114">取得したすべてのノートブックについて、`GET ~/notebooks/{notebookId}/sections` を呼び出してセクションの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="09adf-114">For every retrieved notebook, call `GET ~/notebooks/{notebookId}/sections` to retrieve the list of sections.</span></span>
* <span data-ttu-id="09adf-115">取得したすべてのノートブックについて、`GET ~/notebooks/{notebookId}/sectionGroups` を呼び出してセクション グループの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="09adf-115">For every retrieved notebook, call `GET ~/notebooks/{notebookId}/sectionGroups` to retrieve the list of section groups.</span></span>
* <span data-ttu-id="09adf-116">必要に応じて、セクション グループを再帰的に反復処理できます。</span><span class="sxs-lookup"><span data-stu-id="09adf-116">Optionally recursively iterate through section groups.</span></span>

<span data-ttu-id="09adf-117">この方法 (サービスへ何回かの連続した余分なラウンドトリップを実行) でも可能ですが、より優れたアプローチは、`$expand` クエリ パラメーターを使用することです。</span><span class="sxs-lookup"><span data-stu-id="09adf-117">While this will work (with a few extra sequential roundtrips to the service), a better approach is to use the `$expand` query parameter.</span></span> 

```http
GET ~/notebooks?$expand=sections,sectionGroups($expand=sections)
```

<span data-ttu-id="09adf-118">これにより、1 回のネットワーク ラウンドトリップで同じ結果が得られ、より良いパフォーマンスが得られます。</span><span class="sxs-lookup"><span data-stu-id="09adf-118">This will yield the same results in one network roundtrip, with better performance.</span></span>

## <a name="when-getting-all-pages-for-a-user-do-so-for-each-section-separately"></a><span data-ttu-id="09adf-119">ユーザーに対してすべてのページを取得する場合は、セクションごとに個別に行ってください。</span><span class="sxs-lookup"><span data-stu-id="09adf-119">When getting all pages for a user, do so for each section separately</span></span>

<span data-ttu-id="09adf-120">Microsoft Graph はすべてのページを取得するためにエンドポイントを公開しますが、これはユーザーがアクセス権を持っているすべてのページを取得する最良の方法ではありません。</span><span class="sxs-lookup"><span data-stu-id="09adf-120">While Microsoft Graph exposes an endpoint to retrieve all pages, this isn't the best way to get all the pages the user has access to.</span></span> <span data-ttu-id="09adf-121">ユーザーが持つセクションが多すぎると、これによりタイムアウトやパフォーマンスの低下を招きます。</span><span class="sxs-lookup"><span data-stu-id="09adf-121">When the user has too many sections, this can lead to timeouts or bad performance.</span></span> <span data-ttu-id="09adf-122">各セクションを反復処理して、個別にそれぞれのページを取得することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="09adf-122">It is better to iterate each section, getting pages for each one separately.</span></span>

<span data-ttu-id="09adf-123">たとえば、この呼び出しを使用する代わりに、(この API はページ化されているので、すべてのページを一度にフェッチすることはできません):</span><span class="sxs-lookup"><span data-stu-id="09adf-123">For example, instead of using this call (this API is paged, so you won't be able to fetch the pages all at once):</span></span>

```http
GET ~/pages
```

<span data-ttu-id="09adf-124">(特にすべてのセクションが必要ない場合は) 次の呼び出しを何回か使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="09adf-124">It is better to use the following call several times (especially if you don't need all sections):</span></span>

```http
GET ~/sections/{id}/pages
```

<span data-ttu-id="09adf-125">ページのメタデータを取得するには、既定値 `lastModifiedDateTime` の順序付けを上書きします。</span><span class="sxs-lookup"><span data-stu-id="09adf-125">When getting page metadata, override the default `lastModifiedDateTime` ordering.</span></span> <span data-ttu-id="09adf-126">それらを `lastModifiedDateTime` で並べ替える必要がないときには、より速くページを取得できます。</span><span class="sxs-lookup"><span data-stu-id="09adf-126">It is faster to get pages when you don't have to sort them by `lastModifiedDateTime`.</span></span> <span data-ttu-id="09adf-127">これを行うには、たとえば他の任意のプロパティで並べ替えることができます。</span><span class="sxs-lookup"><span data-stu-id="09adf-127">To do this, you can sort by any other property; for example:</span></span>

```http
GET ~/sections/{id}/pages?$select=id,title,createdDateTime&$orderby=createdDateTime
```
