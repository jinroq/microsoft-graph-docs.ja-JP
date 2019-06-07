---
title: クエリ パラメーターを使用して応答をカスタマイズする
description: Microsoft Graph にはオプションのクエリ パラメーターがあり、応答で返されるデータの量を指定したり制御したりするために使用できます。次のクエリ パラメーターがサポートされています。
author: piotrci
localization_priority: Priority
ms.openlocfilehash: 1962ee481d89ccef14d436edb41195a9b5b2529a
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "34750169"
---
# <a name="use-query-parameters-to-customize-responses"></a><span data-ttu-id="7ff49-104">クエリ パラメーターを使用して応答をカスタマイズする</span><span class="sxs-lookup"><span data-stu-id="7ff49-104">Use query parameters to customize responses</span></span>

<span data-ttu-id="7ff49-105">Microsoft Graph はオプションのクエリ パラメーターをサポートしており、応答で返されるデータの量を指定したり制御したりするために使用できます。</span><span class="sxs-lookup"><span data-stu-id="7ff49-105">Microsoft Graph supports optional query parameters that you can use to specify and control the amount of data returned in a response.</span></span> <span data-ttu-id="7ff49-106">正確なクエリ パラメーターのサポートは、API 操作ごとに異なり、API によっては、v1.0 とベータ版エンドポイントかでも異なることがあります。</span><span class="sxs-lookup"><span data-stu-id="7ff49-106">The support for the exact query parameters varies from one API operation to another, and depending on the API, can differ between the v1.0 and beta endpoints.</span></span> 

> [!TIP] 
> <span data-ttu-id="7ff49-107">ベータ版エンドポイントでは、`$`プレフィックスが省略可能です。</span><span class="sxs-lookup"><span data-stu-id="7ff49-107">`$` On the v1.0 and beta endpoints, the  prefix is optional.</span></span> <span data-ttu-id="7ff49-108">たとえば、`filter` とせずに、`$filter` と指定することもできます。</span><span class="sxs-lookup"><span data-stu-id="7ff49-108">For example, instead of `$filter`, you can use `filter`.</span></span> <span data-ttu-id="7ff49-109">v1 エンドポイントでは、API のサブセットに対してのみ`$`プレフィックスが省略可能です。</span><span class="sxs-lookup"><span data-stu-id="7ff49-109">On the v1 endpoint, the `$` prefix is optional for only a subset of APIs.</span></span> <span data-ttu-id="7ff49-110">要するに、v1 エンドポイントを使用している場合は、常に`$`が含まれます。</span><span class="sxs-lookup"><span data-stu-id="7ff49-110">For simplicity, always include `$` if using the v1 endpoint.</span></span>

<span data-ttu-id="7ff49-111">クエリ パラメーターには、OData のシステム クエリ オプションまたは他のクエリ パラメーターを使用できます。</span><span class="sxs-lookup"><span data-stu-id="7ff49-111">Query parameters can be OData system query options or other query parameters.</span></span> 

## <a name="odata-system-query-options"></a><span data-ttu-id="7ff49-112">OData のシステム クエリ オプション</span><span class="sxs-lookup"><span data-stu-id="7ff49-112">OData system query options</span></span>
<span data-ttu-id="7ff49-113">Microsoft Graph API 操作は、次の OData のシステム クエリ オプションの 1 つ以上をサポートする可能性があります。</span><span class="sxs-lookup"><span data-stu-id="7ff49-113">A Microsoft Graph API operation might support one or more of the following OData system query options.</span></span> <span data-ttu-id="7ff49-114">これらのクエリ オプションは、[OData V4 クエリ言語][odata-query]と互換性があります。</span><span class="sxs-lookup"><span data-stu-id="7ff49-114">These query options are compatible with the [OData V4 query language][odata-query].</span></span>

><span data-ttu-id="7ff49-115">**注:** 例をクリックして [Graph エクスプローラー][graph-explorer]で試行します。</span><span class="sxs-lookup"><span data-stu-id="7ff49-115">**Note:** Click the examples to try them in [Graph Explorer][graph-explorer].</span></span>

| <span data-ttu-id="7ff49-116">名前</span><span class="sxs-lookup"><span data-stu-id="7ff49-116">Name</span></span>                     | <span data-ttu-id="7ff49-117">説明</span><span class="sxs-lookup"><span data-stu-id="7ff49-117">Description</span></span> | <span data-ttu-id="7ff49-118">例</span><span class="sxs-lookup"><span data-stu-id="7ff49-118">Example</span></span>
|:-------------------------|:------------|:---------|
| [<span data-ttu-id="7ff49-119">$count</span><span class="sxs-lookup"><span data-stu-id="7ff49-119">$count</span></span>](#count-parameter)         | <span data-ttu-id="7ff49-120">一致するリソースの総数を取得します。</span><span class="sxs-lookup"><span data-stu-id="7ff49-120">Retrieves the total count of matching resources.</span></span> | [`/me/messages?$top=2&$count=true`][count-example]
| [<span data-ttu-id="7ff49-121">$expand</span><span class="sxs-lookup"><span data-stu-id="7ff49-121">$expand</span></span>](#expand-parameter)       | <span data-ttu-id="7ff49-122">関連リソースを取得します。</span><span class="sxs-lookup"><span data-stu-id="7ff49-122">Retrieves related resources.</span></span>|[`/groups?$expand=members`][expand-example]
| [<span data-ttu-id="7ff49-123">$filter</span><span class="sxs-lookup"><span data-stu-id="7ff49-123">$filter</span></span>](#filter-parameter)       | <span data-ttu-id="7ff49-124">結果 (行) をフィルターします。</span><span class="sxs-lookup"><span data-stu-id="7ff49-124">Filters results (rows).</span></span>|[`/users?$filter=startswith(givenName,'J')`][filter-example]
| [<span data-ttu-id="7ff49-125">$format</span><span class="sxs-lookup"><span data-stu-id="7ff49-125">$format</span></span>](#format-parameter)       | <span data-ttu-id="7ff49-126">指定したメディア形式で結果を返します。</span><span class="sxs-lookup"><span data-stu-id="7ff49-126">Returns the results in the specified media format.</span></span>|[`/users?$format=json`][format-example]
| [<span data-ttu-id="7ff49-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="7ff49-127">$orderby</span></span>](#orderby-parameter)     | <span data-ttu-id="7ff49-128">結果を並べます。</span><span class="sxs-lookup"><span data-stu-id="7ff49-128">Orders results.</span></span>|[`/users?$orderby=displayName desc`][orderby-example]
| [<span data-ttu-id="7ff49-129">$search</span><span class="sxs-lookup"><span data-stu-id="7ff49-129">$search</span></span>](#search-parameter)       | <span data-ttu-id="7ff49-p105">検索条件に基づいて結果を返します。現在、**messages** と **person** のコレクションでサポートされています。</span><span class="sxs-lookup"><span data-stu-id="7ff49-p105">Returns results based on search criteria. Currently supported on **messages** and **person** collections.</span></span>|[`/me/messages?$search=pizza`][search-example]
| [<span data-ttu-id="7ff49-132">$select</span><span class="sxs-lookup"><span data-stu-id="7ff49-132">$select</span></span>](#select-parameter)       | <span data-ttu-id="7ff49-133">プロパティ (列) をフィルターします。</span><span class="sxs-lookup"><span data-stu-id="7ff49-133">Filters properties (columns).</span></span>|[`/users?$select=givenName,surname`][select-example]
| [<span data-ttu-id="7ff49-134">$skip</span><span class="sxs-lookup"><span data-stu-id="7ff49-134">$skip</span></span>](#skip-parameter)           | <span data-ttu-id="7ff49-p106">結果セットにインデックスを作成します。また一部の API でページングを実装するために使用されており、`$top` と組み合わせて手動で結果をページングすることもできます。</span><span class="sxs-lookup"><span data-stu-id="7ff49-p106">Indexes into a result set. Also used by some APIs to implement paging and can be used together with `$top` to manually page results.</span></span> | [`/me/messages?$skip=11`][skip-example]
| [<span data-ttu-id="7ff49-137">$top</span><span class="sxs-lookup"><span data-stu-id="7ff49-137">$top</span></span>](#top-parameter)             | <span data-ttu-id="7ff49-138">結果のページ サイズを設定します。</span><span class="sxs-lookup"><span data-stu-id="7ff49-138">Sets the page size of results.</span></span> |[`/users?$top=2`][top-example]


## <a name="other-query-parameters"></a><span data-ttu-id="7ff49-139">その他のクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7ff49-139">Other query parameters</span></span>

| <span data-ttu-id="7ff49-140">名前</span><span class="sxs-lookup"><span data-stu-id="7ff49-140">Name</span></span>                     | <span data-ttu-id="7ff49-141">説明</span><span class="sxs-lookup"><span data-stu-id="7ff49-141">Description</span></span> | <span data-ttu-id="7ff49-142">例</span><span class="sxs-lookup"><span data-stu-id="7ff49-142">Example</span></span>
|:-------------------------|:------------|:---------|
| [<span data-ttu-id="7ff49-143">$skipToken</span><span class="sxs-lookup"><span data-stu-id="7ff49-143">$skipToken</span></span>](#skiptoken-parameter) | <span data-ttu-id="7ff49-p107">複数ページにわたる結果セットから、結果の次のページを取得します。(一部の API では代わりに `$skip` を使用します。)</span><span class="sxs-lookup"><span data-stu-id="7ff49-p107">Retrieves the next page of results from result sets that span multiple pages. (Some APIs use `$skip` instead.)</span></span> | `/users?$skiptoken=X%274453707402000100000017...`|

## <a name="encoding-query-parameters"></a><span data-ttu-id="7ff49-146">クエリ パラメーターのエンコード</span><span class="sxs-lookup"><span data-stu-id="7ff49-146">Encoding query parameters</span></span>

<span data-ttu-id="7ff49-147">クエリ パラメーターの値はパーセント エンコードされる必要があります。</span><span class="sxs-lookup"><span data-stu-id="7ff49-147">The values of query parameters should be percent-encoded.</span></span> <span data-ttu-id="7ff49-148">これを行ううえで役立つ HTTP クライアント、ブラウザー、およびツールが多くあります ([Graph エクスプローラー][graph-explorer]など)。</span><span class="sxs-lookup"><span data-stu-id="7ff49-148">Many HTTP clients, browsers, and tools (such as the [Graph Explorer][graph-explorer]) will help you with this.</span></span> <span data-ttu-id="7ff49-149">クエリが失敗する場合、クエリ パラメーターの値が適切にエンコードされていないことがその原因の 1 つとして考えられます。</span><span class="sxs-lookup"><span data-stu-id="7ff49-149">If a query is failing, one possible cause is failure to encode the query parameter values appropriately.</span></span>

<span data-ttu-id="7ff49-150">エンコードされていない URL は、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="7ff49-150">An unencoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName, 'J')
```

<span data-ttu-id="7ff49-151">正しくエンコードされている URL は、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="7ff49-151">A properly encoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName%2C+'J')
```

### <a name="escaping-single-quotes"></a><span data-ttu-id="7ff49-152">一重引用符のエスケープ</span><span class="sxs-lookup"><span data-stu-id="7ff49-152">Escaping single quotes</span></span>

<span data-ttu-id="7ff49-153">一重引用符を使用する依頼の場合、いずれかのパラメーター値にも一重引用符が含まれている場合は、それらを二重エスケープにする必要があります。 そうでないと、無効な構文とみなされ、依頼が失敗します。</span><span class="sxs-lookup"><span data-stu-id="7ff49-153">For requests that use single quotes, if any parameter values also contain single quotes, those must be double escaped; otherwise, the request will fail due to invalid syntax.</span></span> <span data-ttu-id="7ff49-154">この例では、文字列値の `let''s meet for lunch?` では一重引用符がエスケープされています。</span><span class="sxs-lookup"><span data-stu-id="7ff49-154">In the example, the string value `let''s meet for lunch?` has the single quote escaped.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=subject eq 'let''s meet for lunch?'
```

## <a name="count-parameter"></a><span data-ttu-id="7ff49-155">count パラメーター</span><span class="sxs-lookup"><span data-stu-id="7ff49-155">count parameter</span></span>

<span data-ttu-id="7ff49-156">`$count` クエリ パラメーターを使用し、Microsoft Graph から返されるデータ値のページにコレクション内の項目数の合計を含めます。</span><span class="sxs-lookup"><span data-stu-id="7ff49-156">Use the `$count` query parameter to include a count of the total number of items in a collection alongside the page of data values returned from Microsoft Graph.</span></span> 

<span data-ttu-id="7ff49-157">たとえば、次のような要求では、現在のユーザーの **contact** コレクションと、`@odata.count` プロパティ内の **contact** コレクションのアイテム数の両方が返されます。</span><span class="sxs-lookup"><span data-stu-id="7ff49-157">For example, the following request will return both the **contact** collection of the current user, and the number of items in the **contact** collection in the `@odata.count` property.</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

[<span data-ttu-id="7ff49-158">Graph エクスプローラーで試す</span><span class="sxs-lookup"><span data-stu-id="7ff49-158">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/contacts?$count=true&method=GET&version=v1.0)


><span data-ttu-id="7ff49-159">**注:** `$count` は、[user](/graph/api/resources/user?view=graph-rest-1.0) や [group](/graph/api/resources/group?view=graph-rest-1.0) のコレクションのような、[directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0) から派生したリソースのコレクションに対してはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7ff49-159">**Note:** `$count` is not supported for collections of resources that derive from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0) like collections of [users](/graph/api/resources/user?view=graph-rest-1.0) or [groups](/graph/api/resources/group?view=graph-rest-1.0).</span></span>

## <a name="expand-parameter"></a><span data-ttu-id="7ff49-160">expand パラメーター</span><span class="sxs-lookup"><span data-stu-id="7ff49-160">expand parameter</span></span>

<span data-ttu-id="7ff49-161">Microsoft Graph リソースの多くは、宣言されているリソースのプロパティと、他のリソースとのリレーションシップの両方を公開します。</span><span class="sxs-lookup"><span data-stu-id="7ff49-161">Many Microsoft Graph resources expose both declared properties of the resource as well as its relationships with other resources.</span></span> <span data-ttu-id="7ff49-162">これらのリレーションシップは、参照プロパティまたはナビゲーション プロパティとも呼ばれ、1 つのリソースまたはリソースのコレクションのいずれかを参照することができます。</span><span class="sxs-lookup"><span data-stu-id="7ff49-162">These relationships are also called reference properties or navigation properties, and they can reference either a single resource or a collection of resources.</span></span> <span data-ttu-id="7ff49-163">たとえば、ユーザーのメール フォルダー、マネージャー、直属の部下は、すべてリレーションシップとして公開されます。</span><span class="sxs-lookup"><span data-stu-id="7ff49-163">For example, the mail folders, manager, and direct reports of a user are all exposed as relationships.</span></span> 

<span data-ttu-id="7ff49-p111">通常、単一の要求では、リソースの複数のプロパティ、またはリソースのリレーションシップの 1 つのいずれかに対してクエリを実行できますが、両方は行えません。`$expand` クエリ文字列パラメーターを使用して、展開されているリソース、または単一のリレーションシップ (ナビゲーション プロパティ) で参照されているコレクションを結果に含めることができます。</span><span class="sxs-lookup"><span data-stu-id="7ff49-p111">Normally, you can query either the properties of a resource or one of its relationships in a single request, but not both. You can use the `$expand` query string parameter to include the expanded resource or collection referenced by a single relationship (navigation property) in your results.</span></span>

<span data-ttu-id="7ff49-166">次の例では、ドライブ内のトップレベルの子項目と共に、ルート ドライブ情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="7ff49-166">The following example gets root drive information along with the top-level child items in a drive:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children
```

[<span data-ttu-id="7ff49-167">Graph エクスプローラーで試す</span><span class="sxs-lookup"><span data-stu-id="7ff49-167">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children&method=GET&version=v1.0)

<span data-ttu-id="7ff49-p112">いくつかのリソース コレクションで、`$select` パラメーターを追加すれば、展開されたリソースで返されるプロパティを指定することもできます。次の使用例は前の例と同じクエリを実行しますが、[`$select`](#select-parameter) ステートメントを使用して、展開されている子項目に返されるプロパティを **id** プロパティと **name** プロパティに限定します。</span><span class="sxs-lookup"><span data-stu-id="7ff49-p112">With some resource collections, you can also specify the properties to be returned in the expanded resources by adding a `$select` parameter. The following example performs the same query as the previous example but uses a [`$select`](#select-parameter) statement to limit the properties returned for the expanded child items to the **id** and **name** properties.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

<span data-ttu-id="7ff49-170">[Graph エクスプローラーで試す][expand-example]</span><span class="sxs-lookup"><span data-stu-id="7ff49-170">[Try in Graph Explorer][expand-example]</span></span>

> <span data-ttu-id="7ff49-p113">**注:** すべてのリレーションシップとリソースで、`$expand` クエリ パラメーターがサポートされているわけではありません。たとえば、ユーザーの **directReports**、**manager**、**memberOf** の各リレーションシップを展開できますが、その **events**、**messages**、**photo** のリレーションシップは展開できません。すべてのリソースまたはリレーションシップで、`$select` を使用して展開されたアイテムがサポートされているわけではありません。</span><span class="sxs-lookup"><span data-stu-id="7ff49-p113">**Note:** Not all relationships and resources support the `$expand` query parameter. For example, you can expand the **directReports**, **manager**, and **memberOf** relationships on a user, but you cannot expand its **events**, **messages**, or **photo** relationships. Not all resources or relationships support using `$select` on expanded items.</span></span> 
> 
> <span data-ttu-id="7ff49-174">[ユーザー](/graph/api/resources/user?view=graph-rest-1.0)や[グループ](/graph/api/resources/group?view=graph-rest-1.0)のような、[directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0) から派生した Azure AD リソースの場合、`$expand` は `beta` でのみサポートされており、通常は展開されているリレーションシップに対し最大 20 個のアイテムを返すことができます。</span><span class="sxs-lookup"><span data-stu-id="7ff49-174">With Azure AD resources that derive from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0), like [user](/graph/api/resources/user?view=graph-rest-1.0) and [group](/graph/api/resources/group?view=graph-rest-1.0), `$expand` is only supported for `beta` and  typically returns a maximum of 20 items for the expanded relationship.</span></span>

## <a name="filter-parameter"></a><span data-ttu-id="7ff49-175">filter パラメーター</span><span class="sxs-lookup"><span data-stu-id="7ff49-175">filter parameter</span></span>

<span data-ttu-id="7ff49-176">`$filter` クエリ パラメーターを使用して、コレクションのサブセットのみを取得します。</span><span class="sxs-lookup"><span data-stu-id="7ff49-176">Use the `$filter` query parameter to retrieve just a subset of a collection.</span></span> 

<span data-ttu-id="7ff49-177">たとえば、表示名が「J」という文字で始まるユーザーを検索するには、`startswith` を使用します。</span><span class="sxs-lookup"><span data-stu-id="7ff49-177">For example, to find users whose display name starts with the letter 'J', use `startswith`.</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'J')
```

<span data-ttu-id="7ff49-178">[Graph エクスプローラーで試す][filter-example]</span><span class="sxs-lookup"><span data-stu-id="7ff49-178">[Try in Graph Explorer][filter-example]</span></span>

<span data-ttu-id="7ff49-179">`$filter` 演算子のサポートは、お使いの Microsoft Graph API によって異なります。</span><span class="sxs-lookup"><span data-stu-id="7ff49-179">Support for `$filter` operators varies across Microsoft Graph APIs.</span></span> <span data-ttu-id="7ff49-180">通常、次の論理演算子がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="7ff49-180">The following logical operators are generally supported:</span></span> 

- <span data-ttu-id="7ff49-181">等しい (`eq`)</span><span class="sxs-lookup"><span data-stu-id="7ff49-181">equals (`eq`)</span></span>
- <span data-ttu-id="7ff49-182">等しくない (`ne`)</span><span class="sxs-lookup"><span data-stu-id="7ff49-182">not equals (`ne`)</span></span>
- <span data-ttu-id="7ff49-183">より大きい (`gt`)</span><span class="sxs-lookup"><span data-stu-id="7ff49-183">greater than (`gt`)</span></span>
- <span data-ttu-id="7ff49-184">以上 (`ge`)</span><span class="sxs-lookup"><span data-stu-id="7ff49-184">greater than or equals (`ge`)</span></span>
- <span data-ttu-id="7ff49-185">より小さい (`lt`)、以下 (`le`)</span><span class="sxs-lookup"><span data-stu-id="7ff49-185">less than (`lt`), less than or equals (`le`)</span></span>
- <span data-ttu-id="7ff49-186">AND (`and`)</span><span class="sxs-lookup"><span data-stu-id="7ff49-186">and (`and`)</span></span>
- <span data-ttu-id="7ff49-187">OR (`or`)</span><span class="sxs-lookup"><span data-stu-id="7ff49-187">or (`or`)</span></span>
- <span data-ttu-id="7ff49-188">NOT (`not`)</span><span class="sxs-lookup"><span data-stu-id="7ff49-188">not (`not`)</span></span>
 
<span data-ttu-id="7ff49-189">`startswith` 文字列の演算子はたいていサポートされています。</span><span class="sxs-lookup"><span data-stu-id="7ff49-189">The `startswith` string operator is often supported.</span></span> <span data-ttu-id="7ff49-190">`any` ラムダ演算子は、一部の API でサポートされています。</span><span class="sxs-lookup"><span data-stu-id="7ff49-190">The `any` lambda operator is supported for some APIs.</span></span> <span data-ttu-id="7ff49-191">いくつかの使用例について、次の表を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7ff49-191">For some  usage examples, see the following table.</span></span> <span data-ttu-id="7ff49-192">`$filter` 構文の詳細については、「[OData プロトコル][odata-filter]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7ff49-192">For more details about `$filter` syntax, see the [OData protocol][odata-filter].</span></span>  

<span data-ttu-id="7ff49-193">次の表では、`$filter` クエリ パラメーター使用例を示します。</span><span class="sxs-lookup"><span data-stu-id="7ff49-193">The following table shows some examples that use the `$filter` query parameter.</span></span>

> <span data-ttu-id="7ff49-194">**注:** 例をクリックして [Graph エクスプローラー][graph-explorer]で試行します。</span><span class="sxs-lookup"><span data-stu-id="7ff49-194">**Note:** Click the examples to try them in [Graph Explorer][graph-explorer].</span></span>

| <span data-ttu-id="7ff49-195">説明</span><span class="sxs-lookup"><span data-stu-id="7ff49-195">Description</span></span> | <span data-ttu-id="7ff49-196">例</span><span class="sxs-lookup"><span data-stu-id="7ff49-196">Example</span></span>
|:------------|:--------|
| <span data-ttu-id="7ff49-197">複数のプロパティ間で Mary という名前を持つユーザーを検索します。</span><span class="sxs-lookup"><span data-stu-id="7ff49-197">Search for users with the name Mary across multiple properties.</span></span> | [`https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'mary') or startswith(givenName,'mary') or startswith(surname,'mary') or startswith(mail,'mary') or startswith(userPrincipalName,'mary')`](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(displayName,'mary')+or+startswith(givenName,'mary')+or+startswith(surname,'mary')+or+startswith(mail,'mary')+or+startswith(userPrincipalName,'mary')&method=GET&version=v1.0) 
| <span data-ttu-id="7ff49-198">2017 年 7 月 1 日以降に開始する、サインイン ユーザーのイベントすべてを取得します。</span><span class="sxs-lookup"><span data-stu-id="7ff49-198">Get all the signed-in user's events that start after 7/1/2017.</span></span> | [`https://graph.microsoft.com/v1.0/me/events?$filter=start/dateTime ge '2017-07-01T08:00'`](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$filter=start/dateTime+ge+'2017-07-01T08:00'&method=GET&version=v1.0) 
| <span data-ttu-id="7ff49-199">サインイン ユーザーが受信した特定のアドレスからの電子メールすべてを取得します。</span><span class="sxs-lookup"><span data-stu-id="7ff49-199">Get all emails from a specific address received by the signed-in user.</span></span> | [`https://graph.microsoft.com/v1.0/me/messages?$filter=from/emailAddress/address eq 'someuser@example.com'`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=from/emailAddress/address+eq+'someuser@.com'&method=GET&version=v1.0) 
| <span data-ttu-id="7ff49-200">2017 年 4 月にサインイン ユーザーが受信した電子メールすべてを取得します。</span><span class="sxs-lookup"><span data-stu-id="7ff49-200">Get all emails received by the signed-in user in April 2017.</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=ReceivedDateTime ge 2017-04-01 and receivedDateTime lt 2017-05-01`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=ReceivedDateTime+ge+2017-04-01+and+receivedDateTime+lt+2017-05-01&method=GET&version=v1.0) 
| <span data-ttu-id="7ff49-201">サインイン ユーザーの受信トレイから未読メールをすべて取得します。</span><span class="sxs-lookup"><span data-stu-id="7ff49-201">Get all unread mail in the signed-in user's Inbox.</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=isRead eq false`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=isRead+eq+false&method=GET&version=v1.0) 
| <span data-ttu-id="7ff49-202">組織内のすべての Office 365 グループの一覧</span><span class="sxs-lookup"><span data-stu-id="7ff49-202">List all Office 365 groups in an organization.</span></span> | [`https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')`](https://developer.microsoft.com/graph/graph-explorer?request=groups?$filter=groupTypes/any(c:c+eq+'Unified')&method=GET&version=v1.0) 

> <span data-ttu-id="7ff49-p116">**注:** Azure AD リソースでは、次の `$filter` 演算子はサポートされていません: `ne`、`gt`、`ge`、`lt`、`le`、`not`。Microsoft Graph リソースでは現在、`contains` 文字列の演算子はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7ff49-p116">**Note:** The following `$filter` operators are not supported for Azure AD resources:  `ne`, `gt`, `ge`, `lt`, `le`, and `not`. The `contains` string operator is currently not supported on any Microsoft Graph resources.</span></span>

## <a name="format-parameter"></a><span data-ttu-id="7ff49-205">format パラメーター</span><span class="sxs-lookup"><span data-stu-id="7ff49-205">format parameter</span></span>

<span data-ttu-id="7ff49-206">`$format` クエリ パラメーターを使用して、Microsoft Graph から返される項目のメディア形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="7ff49-206">Use the `$format` query parameter to specify the media format of the items returned from Microsoft Graph.</span></span>

<span data-ttu-id="7ff49-207">たとえば、次の要求では組織のユーザーが JSON 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="7ff49-207">For example, the following request returns the users in the organization in the json format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$format=json
```

<span data-ttu-id="7ff49-208">[Graph エクスプローラーで試す][format-example]</span><span class="sxs-lookup"><span data-stu-id="7ff49-208">[Try in Graph Explorer][format-example]</span></span>

> <span data-ttu-id="7ff49-209">**注:**`$format` クエリ パラメーターは、さまざまな形式 (atom、xml、json など) をサポートしていますが、結果がすべての形式で返されるわけではありません。</span><span class="sxs-lookup"><span data-stu-id="7ff49-209">**Note:** The `$format` query parameter supports a number of formats (for example, atom, xml, and json) but results may not be returned in all formats.</span></span>

## <a name="orderby-parameter"></a><span data-ttu-id="7ff49-210">orderby パラメーター</span><span class="sxs-lookup"><span data-stu-id="7ff49-210">orderby parameter</span></span>

<span data-ttu-id="7ff49-211">`$orderby` クエリ パラメーターを使用して、Microsof Graph から返される項目の並べ替え順序を指定します。</span><span class="sxs-lookup"><span data-stu-id="7ff49-211">Use the `$orderby` query parameter to specify the sort order of the items returned from Microsoft Graph.</span></span>

<span data-ttu-id="7ff49-212">たとえば、次の要求では組織のユーザーが表示名順で返されます。</span><span class="sxs-lookup"><span data-stu-id="7ff49-212">For example, the following request returns the users in the organization ordered by their display name:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```
<span data-ttu-id="7ff49-213">[Graph エクスプローラーで試す][orderby-example]</span><span class="sxs-lookup"><span data-stu-id="7ff49-213">[Try in Graph Explorer][orderby-example]</span></span>

<span data-ttu-id="7ff49-p117">複合型のエンティティでも並べ替えができます。次の要求では、メッセージを取得し、それらを **emailAddress** という複合型である **from** プロパティの **address** フィールドで並べ替えます。</span><span class="sxs-lookup"><span data-stu-id="7ff49-p117">You can also sort by complex type entities. The following request gets messages and sorts them by the **address** field of the **from** property, which is of the complex type **emailAddress**:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
```
[<span data-ttu-id="7ff49-216">Graph エクスプローラーで試す</span><span class="sxs-lookup"><span data-stu-id="7ff49-216">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/address&method=GET&version=v1.0)

<span data-ttu-id="7ff49-217">昇順または降順で結果を並べ替えるには、`asc` または `desc` のいずれかをスペースで区切ってフィールド名の後に追加します。たとえば `?$orderby=name%20desc` のようにします。</span><span class="sxs-lookup"><span data-stu-id="7ff49-217">To sort the results in ascending or descending order, append either `asc` or `desc` to the field name, separated by a space; for example, `?$orderby=name%20desc`.</span></span>

<span data-ttu-id="7ff49-218">一部の API では、複数のプロパティの結果を並べ替えることができます。</span><span class="sxs-lookup"><span data-stu-id="7ff49-218">With some APIs, you can order results on multiple properties.</span></span> <span data-ttu-id="7ff49-219">たとえば、次のような要求ではユーザーの受信トレイ内のメッセージを、最初は送信者の名前で降順に並べ替え (Z から A)、次に件名で昇順 (既定) に並べ替えます。</span><span class="sxs-lookup"><span data-stu-id="7ff49-219">For example, the following request orders the messages in the user's Inbox, first by the name of the person who sent it in descending order (Z to A), and then by subject in ascending order (default).</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/Inbox/messages?$orderby=from/emailAddress/name desc,subject
```

[<span data-ttu-id="7ff49-220">Graph エクスプローラーで試す</span><span class="sxs-lookup"><span data-stu-id="7ff49-220">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/name%20desc,subject&method=GET&version=v1.0)

<span data-ttu-id="7ff49-221">$filter を指定した場合は、サーバーで結果の並べ替え順序が考慮されます。</span><span class="sxs-lookup"><span data-stu-id="7ff49-221">When you specify $filter the server will infer a sort order for the results.</span></span> <span data-ttu-id="7ff49-222">`$orderby` と `$filter` の両方を使用する場合、サーバーでは常に `$filter` の結果の並べ替え順序が考慮されるため、`$filter` 内のプロパティを他のプロパティよりも先に `$orderby` 内に配置して、`$filter` パラメーターに現れる順序で並べる必要があります。</span><span class="sxs-lookup"><span data-stu-id="7ff49-222">If you use both `$orderby` and `$filter`, because the server always infers a sort order for the results of a `$filter`, the properties in the `$filter` must be listed first in the `$orderby` before any other properties, and they must be listed in the order that they appear in the `$filter` parameter.</span></span> 

<span data-ttu-id="7ff49-223">次の例は、**Subject** と **Importance** の両方のプロパティでフィルター処理されてから、**Subject**、**Importance**、**receivedDateTime** の各プロパティで降順で並べ替えられたクエリを示しています。</span><span class="sxs-lookup"><span data-stu-id="7ff49-223">The following example shows a query filtered by the **subject** and **importance** properties, and then sorted by the **subject**, **importance**, and **receivedDateTime** properties in descending order.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=Subject eq 'welcome' and importance eq 'normal'&$orderby=subject,importance,receivedDateTime desc
```

[<span data-ttu-id="7ff49-224">Graph エクスプローラーで試す</span><span class="sxs-lookup"><span data-stu-id="7ff49-224">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=subject%20eq%20%27welcome%27%20and%20importance%20eq%20%27normal%27%20&$orderby=subject,importance,receivedDateTime%20desc&method=GET&version=v1.0)

 > <span data-ttu-id="7ff49-225">**注:** [ユーザー](/graph/api/resources/user?view=graph-rest-1.0)や[グループ](/graph/api/resources/group?view=graph-rest-1.0)のような、[directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0) から派生した Azure AD リソースの場合、`$orderby` 式と `$filter` 式を結合することはできません。</span><span class="sxs-lookup"><span data-stu-id="7ff49-225">**Note:** With Azure AD resources that derive from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0), like [user](/graph/api/resources/user?view=graph-rest-1.0) and [group](/graph/api/resources/group?view=graph-rest-1.0), you cannot combine `$orderby` with `$filter` expressions.</span></span> 

## <a name="search-parameter"></a><span data-ttu-id="7ff49-226">search パラメーター</span><span class="sxs-lookup"><span data-stu-id="7ff49-226">search parameter</span></span>

<span data-ttu-id="7ff49-227">`$search` クエリ パラメーターを使用して、要求の結果を検索条件と一致するものに制限します。</span><span class="sxs-lookup"><span data-stu-id="7ff49-227">Use the `$search` query parameter to restrict the results of a request to match a search criterion.</span></span>

> <span data-ttu-id="7ff49-p120">**注:** 現在の検索対象は、[メッセージ](/graph/api/resources/message?view=graph-rest-1.0) コレクションと[人物](/graph/api/resources/person?view=graph-rest-1.0)コレクション**だけ**です。`$search` 要求は最大 250 まで結果を返します。検索要求では [`$filter`](#filter-parameter) も [`$orderby`](#orderby-parameter) も使用できません。</span><span class="sxs-lookup"><span data-stu-id="7ff49-p120">**Note:** You can currently search **only** [message](/graph/api/resources/message?view=graph-rest-1.0) and [person](/graph/api/resources/person?view=graph-rest-1.0) collections. A `$search` request returns up to 250 results. You cannot use [`$filter`](#filter-parameter) or [`$orderby`](#orderby-parameter) in a search request.</span></span>

### <a name="using-search-on-message-collections"></a><span data-ttu-id="7ff49-231">メッセージ コレクションで $search を使用する</span><span class="sxs-lookup"><span data-stu-id="7ff49-231">Using $search on message collections</span></span>

<span data-ttu-id="7ff49-232">特定のメッセージ プロパティの値に基づいてメッセージを検索することができます。</span><span class="sxs-lookup"><span data-stu-id="7ff49-232">You can search messages based on a value in specific message properties.</span></span> <span data-ttu-id="7ff49-233">検索結果は、メッセージが送信された日時で並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="7ff49-233">The results of the search are sorted by the date and time that the message was sent.</span></span>

<span data-ttu-id="7ff49-234">メッセージで検索を行うときに、特定のメッセージ プロパティを指定せずに値のみを指定した場合、検索は既定の検索プロパティである **from**、**subject**、**body** に基づいて行われます。</span><span class="sxs-lookup"><span data-stu-id="7ff49-234">If you do a search on messages and specify only a value without specific message properties, the search is carried out on the default search properties of **from**, **subject**, and **body**.</span></span>

<span data-ttu-id="7ff49-235">次の例は、サインイン中のユーザーの受信トレイにあるメッセージのうち、既定の 3 つの検索プロパティのいずれかに "pizza" が含まれるメッセージをすべて返します。</span><span class="sxs-lookup"><span data-stu-id="7ff49-235">The following example returns all messages in the signed-in user's Inbox that contains "pizza" in any of the three default search properties:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

<span data-ttu-id="7ff49-236">[Graph エクスプローラーで試す][search-example]</span><span class="sxs-lookup"><span data-stu-id="7ff49-236">[Try in Graph Explorer][search-example]</span></span>

<span data-ttu-id="7ff49-237">また、キーワード クエリ言語 (KQL) 構文で認識される、以下の表のメッセージ プロパティ名を指定して、メッセージの検索をすることもできます。</span><span class="sxs-lookup"><span data-stu-id="7ff49-237">Alternatively, you can search messages by specifying message property names in the following table, that are recognized by the Keyword Query Language (KQL) syntax.</span></span> <span data-ttu-id="7ff49-238">これらのプロパティ名は Microsoft Graph の **message** エンティティで定義したプロパティです。</span><span class="sxs-lookup"><span data-stu-id="7ff49-238">These property names correspond to properties defined in the **message** entity of Microsoft Graph.</span></span> <span data-ttu-id="7ff49-239">Outlook や他の Office 365 アプリケーション (SharePoint など) では KQL 構文をサポートしており、データ ストアの共通探索ドメインの利便性が向上します。</span><span class="sxs-lookup"><span data-stu-id="7ff49-239">Outlook and other Office 365 applications such as SharePoint support KQL syntax, providing the convenience of a common discovery domain for their data stores.</span></span>


| <span data-ttu-id="7ff49-240">検索可能な電子メール プロパティ</span><span class="sxs-lookup"><span data-stu-id="7ff49-240">Searchable email property</span></span>                | <span data-ttu-id="7ff49-241">説明</span><span class="sxs-lookup"><span data-stu-id="7ff49-241">Description</span></span> | <span data-ttu-id="7ff49-242">例</span><span class="sxs-lookup"><span data-stu-id="7ff49-242">Example</span></span> 
|:-------------------------|:------------|:---------|
| <span data-ttu-id="7ff49-243">**attachment**</span><span class="sxs-lookup"><span data-stu-id="7ff49-243">**attachment**</span></span>           | <span data-ttu-id="7ff49-244">電子メール メッセージに添付されているファイルの名前。</span><span class="sxs-lookup"><span data-stu-id="7ff49-244">The names of files attached to an email message.</span></span>|[`me/messages?$search="attachment:api-catalog.md"`][search-att-example]
| <span data-ttu-id="7ff49-245">**bcc**</span><span class="sxs-lookup"><span data-stu-id="7ff49-245">**bcc**</span></span>           | <span data-ttu-id="7ff49-246">SMTP アドレス、表示名、エイリアスとして指定されている、電子メール メッセージの **bcc** フィールド。</span><span class="sxs-lookup"><span data-stu-id="7ff49-246">The **bcc** field of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="bcc:samanthab@contoso.com"&$select=subject,bccRecipients`][search-bcc-example]
| <span data-ttu-id="7ff49-247">**body**</span><span class="sxs-lookup"><span data-stu-id="7ff49-247">**body**</span></span>           | <span data-ttu-id="7ff49-248">電子メール メッセージの本文。</span><span class="sxs-lookup"><span data-stu-id="7ff49-248">The body of an email message.</span></span>|[`me/messages?$search="body:excitement"`][search-body-example]
| <span data-ttu-id="7ff49-249">**cc**</span><span class="sxs-lookup"><span data-stu-id="7ff49-249">**cc**</span></span>           | <span data-ttu-id="7ff49-250">SMTP アドレス、表示名、エイリアスとして指定されている、電子メール メッセージの **cc** フィールド。</span><span class="sxs-lookup"><span data-stu-id="7ff49-250">The **cc** field of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="cc:danas"&$select=subject,ccRecipients`][search-cc-example]
| <span data-ttu-id="7ff49-251">**from**</span><span class="sxs-lookup"><span data-stu-id="7ff49-251">**from**</span></span>           | <span data-ttu-id="7ff49-252">SMTP アドレス、表示名、エイリアスとして指定されている、電子メール メッセージの送信者。</span><span class="sxs-lookup"><span data-stu-id="7ff49-252">The sender of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="from:randiw"&$select=subject,from`][search-from-example]
| <span data-ttu-id="7ff49-253">**hasAttachment**</span><span class="sxs-lookup"><span data-stu-id="7ff49-253">**hasAttachment**</span></span> | <span data-ttu-id="7ff49-254">電子メール メッセージに添付ファイルがあり、そのファイルがインラインの添付ファイルでない場合は true、そうでない場合は false。</span><span class="sxs-lookup"><span data-stu-id="7ff49-254">True if an email message contains an attachment that is not an inline attachment, false otherwise.</span></span> |[`me/messages?$search="hasAttachments=true"`][search-from-example]
| <span data-ttu-id="7ff49-255">**importance**</span><span class="sxs-lookup"><span data-stu-id="7ff49-255">**importance**</span></span>           | <span data-ttu-id="7ff49-256">送信者がメッセージを送信するときに指定できる電子メール メッセージの重要度。</span><span class="sxs-lookup"><span data-stu-id="7ff49-256">The importance of an email message, which a sender can specify when sending a message.</span></span> <span data-ttu-id="7ff49-257">使用可能な値: `low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="7ff49-257">The possible values are `low`, `medium`, or `high`.</span></span>|[`me/messages?$search="importance:high"&$select=subject,importance`][search-imp-example]
| <span data-ttu-id="7ff49-258">**kind**</span><span class="sxs-lookup"><span data-stu-id="7ff49-258">**kind**</span></span>           | <span data-ttu-id="7ff49-259">メッセージの種類。</span><span class="sxs-lookup"><span data-stu-id="7ff49-259">The type of message.</span></span> <span data-ttu-id="7ff49-260">使用可能な値: `contacts`、`docs`、`email`、`faxes`、`im`、`journals`、`meetings`、`notes`、`posts`、`rssfeeds`、`tasks`、`voicemail`。</span><span class="sxs-lookup"><span data-stu-id="7ff49-260">The possible values are `contacts`, `docs`, `email`, `faxes`, `im`, `journals`, `meetings`, `notes`, `posts`, `rssfeeds`, `tasks`, or `voicemail`.</span></span>|[`me/messages?$search="kind:voicemail"`][search-kind-example]
| <span data-ttu-id="7ff49-261">**participants**</span><span class="sxs-lookup"><span data-stu-id="7ff49-261">**participants**</span></span>           | <span data-ttu-id="7ff49-262">SMTP アドレス、表示名、エイリアスとして指定されている、電子メール メッセージの **from**、**to**、**cc**、**bcc** フィールド。</span><span class="sxs-lookup"><span data-stu-id="7ff49-262">The **from**, **to**, **cc**, and **bcc** fields of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="participants:danas"`][search-part-example]
| <span data-ttu-id="7ff49-263">**received**</span><span class="sxs-lookup"><span data-stu-id="7ff49-263">**received**</span></span>           | <span data-ttu-id="7ff49-264">電子メール メッセージが受信者によって受信された日付。</span><span class="sxs-lookup"><span data-stu-id="7ff49-264">The date that an email message was received by a recipient.</span></span>|[`me/messages?$search="received:07/23/2018"&$select=subject,receivedDateTime`][search-rcvd-example]
| <span data-ttu-id="7ff49-265">**recipients**</span><span class="sxs-lookup"><span data-stu-id="7ff49-265">**recipients**</span></span>           | <span data-ttu-id="7ff49-266">SMTP アドレス、表示名、エイリアスとして指定されている、電子メール メッセージの **to**、**cc**、**bcc** フィールド。</span><span class="sxs-lookup"><span data-stu-id="7ff49-266">The **to**, **cc**, and **bcc** fields of an email meesage, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="recipients:randiq"&$select=subject,toRecipients,ccRecipients,bccRecipients`][search-rcpts-example]
| <span data-ttu-id="7ff49-267">**sent**</span><span class="sxs-lookup"><span data-stu-id="7ff49-267">**sent**</span></span>           | <span data-ttu-id="7ff49-268">送信者によって電子メール メッセージが送信された日付。</span><span class="sxs-lookup"><span data-stu-id="7ff49-268">The date that an email message was sent by the sender.</span></span>|[`me/messages?$search="sent:07/23/2018"&$select=subject,sentDateTime`][search-sent-example]
| <span data-ttu-id="7ff49-269">**size**</span><span class="sxs-lookup"><span data-stu-id="7ff49-269">**size**</span></span>           | <span data-ttu-id="7ff49-270">アイテムのサイズ (バイト数)。</span><span class="sxs-lookup"><span data-stu-id="7ff49-270">The size of an item in bytes.</span></span>|[`me/messages?$search="size:1..500000"`][search-size-example]
| <span data-ttu-id="7ff49-271">**subject**</span><span class="sxs-lookup"><span data-stu-id="7ff49-271">**subject**</span></span>           | <span data-ttu-id="7ff49-272">電子メール メッセージの件名行に含まれるテキスト。</span><span class="sxs-lookup"><span data-stu-id="7ff49-272">The text in the subject line of an email message.</span></span> <span data-ttu-id="7ff49-273">.</span><span class="sxs-lookup"><span data-stu-id="7ff49-273"></span></span>|[`me/messages?$search="subject:has"&$select=subject`][search-sbj-example]
| <span data-ttu-id="7ff49-274">**to**</span><span class="sxs-lookup"><span data-stu-id="7ff49-274">**to**</span></span>           | <span data-ttu-id="7ff49-275">SMTP アドレス、表示名、エイリアスとして指定されている、電子メール メッセージの **to** フィールド。</span><span class="sxs-lookup"><span data-stu-id="7ff49-275">The **to** field of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="to:randiw"&$select=subject,toRecipients`][search-to-example]


<span data-ttu-id="7ff49-276">検索可能な電子メール プロパティ、KQL 構文、サポートされている演算子、検索のヒントなどの詳細については、次の記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7ff49-276">For more information about searchable email properties, KQL syntax, supported operators, and tips on searching, see the following articles:</span></span>

- <span data-ttu-id="7ff49-277">
  [Exchange の検索可能なプロパティ](https://docs.microsoft.com/ja-JP/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators#searchable-properties-in-exchange)。</span><span class="sxs-lookup"><span data-stu-id="7ff49-277">[Searchable properties in Exchange](https://docs.microsoft.com/en-us/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators#searchable-properties-in-exchange).</span></span>

- <span data-ttu-id="7ff49-278">
  [キーワード クエリ言語 (KQL) 構文のリファレンス](https://docs.microsoft.com/ja-JP/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)</span><span class="sxs-lookup"><span data-stu-id="7ff49-278">[Keyword Query Language (KQL) syntax reference](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)</span></span>

- <span data-ttu-id="7ff49-279">
  [Exchange 2016 におけるインプレースの電子情報開示のためのメッセージ プロパティと検索演算子](https://technet.microsoft.com/ja-JP/library/dn774955(v=exchg.160).aspx)</span><span class="sxs-lookup"><span data-stu-id="7ff49-279">[Message properties and search operators for In-Place eDiscovery in Exchange 2016](https://technet.microsoft.com/en-us/library/dn774955(v=exchg.160).aspx)</span></span>

### <a name="using-search-on-person-collections"></a><span data-ttu-id="7ff49-280">人物コレクションで $search を使用する</span><span class="sxs-lookup"><span data-stu-id="7ff49-280">Using $search on person collections</span></span>

<span data-ttu-id="7ff49-p126">Microsoft Graph People API を使用してユーザーに最も関連のある人物を取得できます。関連性は、ユーザーのコミュニケーションとコラボレーション パターン、およびビジネスのリレーションシップによって決定されます。People API では、`$search` クエリ パラメーターがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="7ff49-p126">You can use the Microsoft Graph People API to retrieve the people who are most relevant to a user. Relevance is determined by the user’s communication and collaboration patterns and business relationships. The People API supports the `$search` query parameter.</span></span>

<span data-ttu-id="7ff49-284">[person](/graph/api/resources/person?view=graph-rest-1.0) リソースの **displayName** プロパティと **emailAddress** プロパティの両方で人物の検索を行います。</span><span class="sxs-lookup"><span data-stu-id="7ff49-284">Searches on people occur on both the **displayName** and **emailAddress** properties of the [person](/graph/api/resources/person?view=graph-rest-1.0) resource.</span></span>

<span data-ttu-id="7ff49-285">次の要求は、サインイン ユーザーの **people** コレクションに含まれる各ユーザーの **displayName** プロパティと **emailAddress** プロパティで、「Irene McGowen」という名前の人物を検索します。</span><span class="sxs-lookup"><span data-stu-id="7ff49-285">The following request does a search for a person named "Irene McGowen" in the **displayName** and **emailAddress** properties in each person in the **people** collection of the signed-in user.</span></span> <span data-ttu-id="7ff49-286">「Irene McGowan」という名前の人物がサインインしているユーザーに関連するため、「Irene McGowan」の情報が返されます。</span><span class="sxs-lookup"><span data-stu-id="7ff49-286">Because a person named "Irene McGowan" is relevant to the signed-in user, the information for "Irene McGowan" is returned.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="Irene McGowen"
```

<span data-ttu-id="7ff49-287">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="7ff49-287">The following example shows the response.</span></span> 

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
       {
           "id": "C0BD1BA1-A84E-4796-9C65-F8A0293741D1",
           "displayName": "Irene McGowan",
           "givenName": "Irene",
           "surname": "McGowan",
           "birthday": "",
           "personNotes": "",
           "isFavorite": false,
           "jobTitle": "Auditor",
           "companyName": null,
           "yomiCompany": "",
           "department": "Finance",
           "officeLocation": "12/1110",
           "profession": "",
           "userPrincipalName": "irenem@contoso.onmicrosoft.com",
           "imAddress": "sip:irenem@contoso.onmicrosoft.com",
           "scoredEmailAddresses": [
               {
                   "address": "irenem@contoso.onmicrosoft.com",
                   "relevanceScore": -16.446060612802224
               }
           ],
           "phones": [
               {
                   "type": "Business",
                   "number": "+1 412 555 0109"
               }
           ],
           "postalAddresses": [],
           "websites": [],
           "personType": {
               "class": "Person",
               "subclass": "OrganizationUser"
           }
       }
   ]
}
```

<span data-ttu-id="7ff49-288">People API の詳細については、「[関係する人の情報を取得する](./people-example.md#search-people)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7ff49-288">To learn more about the People API, see [Get information about relevant people](./people-example.md#search-people).</span></span>  

## <a name="select-parameter"></a><span data-ttu-id="7ff49-289">select パラメーター</span><span class="sxs-lookup"><span data-stu-id="7ff49-289">select parameter</span></span>

<span data-ttu-id="7ff49-290">`$select` クエリ パラメーターを使用して、個別リソースまたはリソースのコレクションの既定値とは異なるプロパティのセットを返します。</span><span class="sxs-lookup"><span data-stu-id="7ff49-290">Use the `$select` query parameter to return a set of properties that are different than the default set for an individual resource or a collection of resources.</span></span> <span data-ttu-id="7ff49-291">$Select で、既定のプロパティのサブセットまたはスーパーセットを指定できます。</span><span class="sxs-lookup"><span data-stu-id="7ff49-291">With $select, you can specify a subset or a superset of the default properties.</span></span>

<span data-ttu-id="7ff49-292">たとえば、サインイン ユーザーのメッセージを取得するとき、**from** プロパティと **subject** プロパティだけを返すよう指定できます。</span><span class="sxs-lookup"><span data-stu-id="7ff49-292">For example, when retrieving the messages of the signed-in user, you can specify that only the **from** and **subject** properties be returned:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

<span data-ttu-id="7ff49-293">[Graph エクスプローラーで試す][select-example]</span><span class="sxs-lookup"><span data-stu-id="7ff49-293">[Try in Graph Explorer][select-example]</span></span>

> <span data-ttu-id="7ff49-294">**重要:** 通常は、`$select` を使用して、クエリから返されるプロパティをお使いのアプリで必要なものだけに制限することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="7ff49-294">**Important:** In general, we recommend that you use `$select` to limit the properties returned by a query to those needed by your app.</span></span> <span data-ttu-id="7ff49-295">これは特に、クエリが大きな結果セットを返す可能性がある場合に該当します。</span><span class="sxs-lookup"><span data-stu-id="7ff49-295">This is especially true of queries that might potentially return a large result set.</span></span> <span data-ttu-id="7ff49-296">行ごとに返されるプロパティを制限すれば、ネットワークの負荷を軽減し、アプリのパフォーマンスを向上させることができます。</span><span class="sxs-lookup"><span data-stu-id="7ff49-296">Limiting the properties returned in each row will reduce network load and help improve your app's performance.</span></span>
>
> <span data-ttu-id="7ff49-p130">`v1.0`では、[ユーザー](/graph/api/resources/user?view=graph-rest-1.0)と[グループ](/graph/api/resources/group?view=graph-rest-1.0)のような、[directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0) から派生した一部の Azure AD リソースは、読み取り時に制限された既定値のプロパティ サブセットを返します。既定のセット以外のプロパティを返すには、これらのリソースに対して `$select` を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7ff49-p130">In `v1.0`, some Azure AD resources that derive from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0), like [user](/graph/api/resources/user?view=graph-rest-1.0) and [group](/graph/api/resources/group?view=graph-rest-1.0), return a limited, default subset of properties on reads. For these resources, you must use `$select` to return properties outside of the default set.</span></span>  

## <a name="skip-parameter"></a><span data-ttu-id="7ff49-299">skip パラメーター</span><span class="sxs-lookup"><span data-stu-id="7ff49-299">skip parameter</span></span>

<span data-ttu-id="7ff49-p131">コレクションを開始するときにスキップする項目数を設定するには、`$skip` クエリ パラメーターを使用します。たとえば、次の要求はユーザーのイベントを、コレクション内の 21 番目以降のイベントから作成日順で返します。</span><span class="sxs-lookup"><span data-stu-id="7ff49-p131">Use the `$skip` query parameter to set the number of items to skip at the start of a collection. For example, the following request returns events for the user sorted by date created, starting with the 21st event in the collection:</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```
<span data-ttu-id="7ff49-302">[Graph エクスプローラーで試す][skip-example]</span><span class="sxs-lookup"><span data-stu-id="7ff49-302">[Try in Graph Explorer][skip-example]</span></span>

> <span data-ttu-id="7ff49-303">**注:** Outlook のメールやカレンダーなど、いくつかの Microsoft Graph API (**message**、**event**、**calendar**) は、`$skip` を使用してページングを実装します。</span><span class="sxs-lookup"><span data-stu-id="7ff49-303">**Note:** Some Microsoft Graph APIs, like Outlook Mail and Calendars (**message**, **event**, and **calendar**), use `$skip` to implement paging.</span></span> <span data-ttu-id="7ff49-304">クエリの結果が複数ページにまたがる場合、これらの API は `@odata:nextLink` プロパティと共に `$skip` パラメーターが含まれる URL を返します。</span><span class="sxs-lookup"><span data-stu-id="7ff49-304">When results of a query span multiple pages, these APIs will return an `@odata:nextLink` property with a URL that contains a `$skip` parameter.</span></span> <span data-ttu-id="7ff49-305">この URL を使用して、結果の次のページに戻れます。</span><span class="sxs-lookup"><span data-stu-id="7ff49-305">You can use this URL to return the next page of results.</span></span> <span data-ttu-id="7ff49-306">詳細については、「[ページング](./paging.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7ff49-306">To learn more, see [Paging](./paging.md).</span></span>

## <a name="skiptoken-parameter"></a><span data-ttu-id="7ff49-307">skipToken パラメーター</span><span class="sxs-lookup"><span data-stu-id="7ff49-307">skipToken parameter</span></span>

<span data-ttu-id="7ff49-p133">要求の中には、サーバー側のページングを使用したり、応答におけるページ サイズを限定するために [`$top`](#top-parameter) パラメーターを使用したりすることによって、複数のデータ ページを返すものがあります。Microsoft Graph API の多くは、`skipToken` クエリ パラメーターを使用して、結果の後続のページを参照します。`$skiptoken` パラメーターは、結果の次のページを参照する不透明トークンを含んでおり、応答の `@odata.nextLink` プロパティで指定される URL で返されます。詳細については、「[ページング](./paging.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7ff49-p133">Some requests return multiple pages of data either due to server-side paging or due to the use of the [`$top`](#top-parameter) parameter to limit the page size of the response. Many Microsoft Graph APIs use the `skipToken` query parameter to reference subsequent pages of the result. The `$skiptoken` parameter contains an opaque token that references the next page of results and is returned in the URL provided in the `@odata.nextLink` property in the response. To learn more, see [Paging](./paging.md).</span></span>


## <a name="top-parameter"></a><span data-ttu-id="7ff49-312">top パラメーター</span><span class="sxs-lookup"><span data-stu-id="7ff49-312">top parameter</span></span>

<span data-ttu-id="7ff49-313">`$top` クエリ パラメーターを使用して、結果セットのページ サイズを指定します。</span><span class="sxs-lookup"><span data-stu-id="7ff49-313">Use the `$top` query parameter to specify the page size of the result set.</span></span> 

<span data-ttu-id="7ff49-314">結果セットにさらに項目が残っている場合、応答本文に `@odata.nextLink` パラメーターが含まれます。</span><span class="sxs-lookup"><span data-stu-id="7ff49-314">If more items remain in the result set, the response body will contain an `@odata.nextLink` parameter.</span></span> <span data-ttu-id="7ff49-315">このパラメーターには、結果の次のページを取得するために使用できる URL が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7ff49-315">This parameter contains a URL that you can use to get the next page of results.</span></span> <span data-ttu-id="7ff49-316">詳細については、「[ページング](./paging.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7ff49-316">To learn more, see [Paging](./paging.md).</span></span> 

<span data-ttu-id="7ff49-317">たとえば、次の要求はユーザーのメールボックスの最初の 5 つのメッセージを返します。</span><span class="sxs-lookup"><span data-stu-id="7ff49-317">For example, the following request returns the first five messages in the user's mailbox:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```

<span data-ttu-id="7ff49-318">[Graph エクスプローラーで試す][top-example]</span><span class="sxs-lookup"><span data-stu-id="7ff49-318">[Try in Graph Explorer][top-example]</span></span>


## <a name="error-handling-for-query-parameters"></a><span data-ttu-id="7ff49-319">クエリ パラメーターのエラー処理</span><span class="sxs-lookup"><span data-stu-id="7ff49-319">Error handling for query parameters</span></span>

<span data-ttu-id="7ff49-p135">指定されたクエリ パラメーターがサポートされていない場合、一部の要求はエラー メッセージを返します。たとえば、`$expand` を `user/photo` のリレーションシップで使用することはできません。</span><span class="sxs-lookup"><span data-stu-id="7ff49-p135">Some requests will return an error message if a specified query parameter is not supported. For example, you cannot use `$expand` on the `user/photo` relationship.</span></span> 

```http
https://graph.microsoft.com/beta/me?$expand=photo
```

```json
{
    "error":{
        "code":"ExpandNotSupported",
        "message":"Expand is not allowed for property 'Photo' according to the entity schema.",
        "innerError":{
            "request-id":"1653fefd-bc31-484b-bb10-8dc33cb853ec",
            "date":"2017-07-31T20:55:01"
        }
    }
}
```

<span data-ttu-id="7ff49-322">ただし、要求で指定されたクエリ パラメーターが警告なしで失敗する可能性があるため、注意が必要です。</span><span class="sxs-lookup"><span data-stu-id="7ff49-322">However, it is important to note that query parameters specified in a request might fail silently.</span></span> <span data-ttu-id="7ff49-323">これは、クエリ パラメーターがサポートされていない場合や、クエリ パラメーターの組み合わせがサポートされていない場合に起こり得ます。</span><span class="sxs-lookup"><span data-stu-id="7ff49-323">This can be true for unsupported query parameters as well as for unsupported combinations of query parameters.</span></span> <span data-ttu-id="7ff49-324">その場合、要求によって返されたデータを調べ、指定したクエリ パラメーターに期待どおりの効果があったかどうかを確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7ff49-324">In these cases, you should examine the data returned by the request to determine whether the query parameters you specified had the desired effect.</span></span> 

[graph-explorer]: https://developer.microsoft.com/graph/graph-explorer
[odata-filter]: https://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752358
[odata-query]: https://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752356
[count-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$top=2%26$count=true&method=GET&version=v1.0
[expand-example]: https://developer.microsoft.com/graph/graph-explorer?request=groups?$expand=members&method=GET&version=v1.0
[filter-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0
[format-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$format=json&method=GET&version=v1.0
[orderby-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$orderby=displayName%20DESC&method=GET&version=v1.0
[search-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=pizza&method=GET&version=v1.0
[select-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$select=givenName,surname&method=GET&version=v1.0
[skip-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$skip=11&method=GET&version=v1.0
[top-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$top=2&method=GET&version=v1.0

[search-att-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22attachment%3Aapi-catalog%2Emd%22&method=GET&version=v1.0
[search-bcc-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22bcc%3Asamanthab%40contoso%2Ecom%22%26$select=subject,bccRecipients&method=GET&version=v1.0
[search-body-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22body%3Aexcitement%22&method=GET&version=v1.0
[search-cc-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22cc%3Adanas%22%26$select=subject,ccRecipients&method=GET&version=v1.0
[search-from-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22from%3Arandiw%22%26$select=subject,from&method=GET&version=v1.0
[search-hasatt-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22hasAttachments=true%22&method=GET&version=v1.0
[search-imp-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22importance%3Ahigh%22%26$select=subject,importance&method=GET&version=v1.0
[search-kind-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22kind%3Avoicemail%22&method=GET&version=v1.0
[search-part-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22participants%3Adanas%22&method=GET&version=v1.0

[search-rcvd-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22received%3A07/23/2018%22%26$select=subject,receivedDateTime&method=GET&version=v1.0

[search-rcpts-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22recipients%3Arandiw%22%26$select=subject,toRecipients,ccRecipients,bccRecipients&method=GET&version=v1.0
[search-sent-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22sent%3A07/23/2018%22%26$select=subject,sentDateTime&method=GET&version=v1.0
[search-size-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22size%3A1%2E%2E500000%22&method=GET&version=v1.0

[search-sbj-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22subject%3Ahas%22%26$select=subject&method=GET&version=v1.
[search-to-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22to%3Arandiw%22%26$select=subject,toRecipients&method=GET&version=v1.0

