# <a name="use-query-parameters-to-customize-responses"></a><span data-ttu-id="e022a-101">クエリ パラメーターを使用して応答をカスタマイズする</span><span class="sxs-lookup"><span data-stu-id="e022a-101">Use query parameters to customize responses</span></span>

<span data-ttu-id="e022a-p101">Microsoft Graph にはオプションのクエリ パラメーターがあり、応答で返されるデータの量を指定したり制御したりするために使用できます。次のクエリ パラメーターがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="e022a-p101">Microsoft Graph provides optional query parameters that you can use to specify and control the amount of data returned in a response. The following query parameters are supported.</span></span>

><span data-ttu-id="e022a-104">**注:** 例をクリックして [Graph エクスプローラー][graph-explorer]で試行します。</span><span class="sxs-lookup"><span data-stu-id="e022a-104">**Note:** Click the examples to try them in [Graph Explorer][graph-explorer].</span></span>

| <span data-ttu-id="e022a-105">名前</span><span class="sxs-lookup"><span data-stu-id="e022a-105">Name</span></span>                     | <span data-ttu-id="e022a-106">説明</span><span class="sxs-lookup"><span data-stu-id="e022a-106">Description</span></span> | <span data-ttu-id="e022a-107">例</span><span class="sxs-lookup"><span data-stu-id="e022a-107">Example</span></span>
|:-------------------------|:------------|:---------|
| [<span data-ttu-id="e022a-108">$count</span><span class="sxs-lookup"><span data-stu-id="e022a-108">$count</span></span>](#count-parameter)         | <span data-ttu-id="e022a-109">一致するリソースの総数を取得します。</span><span class="sxs-lookup"><span data-stu-id="e022a-109">Retrieves the total count of matching resources.</span></span> | [`/me/messages?$top=2&$count=true`][count-example]
| [<span data-ttu-id="e022a-110">$expand</span><span class="sxs-lookup"><span data-stu-id="e022a-110">$expand</span></span>](#expand-parameter)       | <span data-ttu-id="e022a-111">関連リソースを取得します。</span><span class="sxs-lookup"><span data-stu-id="e022a-111">Retrieves related resources.</span></span>|[`/groups?$expand=members`][expand-example]
| [<span data-ttu-id="e022a-112">$filter</span><span class="sxs-lookup"><span data-stu-id="e022a-112">$filter</span></span>](#filter-parameter)       | <span data-ttu-id="e022a-113">結果 (行) をフィルターします。</span><span class="sxs-lookup"><span data-stu-id="e022a-113">Filters results (rows).</span></span>|[`/users?$filter=startswith(givenName,'J')`][filter-example]
| [<span data-ttu-id="e022a-114">$format</span><span class="sxs-lookup"><span data-stu-id="e022a-114">$format</span></span>](#format-parameter)       | <span data-ttu-id="e022a-115">指定したメディア形式で結果を返します。</span><span class="sxs-lookup"><span data-stu-id="e022a-115">Returns the results in the specified media format.</span></span>|[`/users?$format=json`][format-example]
| [<span data-ttu-id="e022a-116">$orderby</span><span class="sxs-lookup"><span data-stu-id="e022a-116">$orderby</span></span>](#orderby-parameter)     | <span data-ttu-id="e022a-117">結果を並べます。</span><span class="sxs-lookup"><span data-stu-id="e022a-117">Orders results.</span></span>|[`/users?$orderby=displayName desc`][orderby-example]
| [<span data-ttu-id="e022a-118">$search</span><span class="sxs-lookup"><span data-stu-id="e022a-118">$search</span></span>](#search-parameter)       | <span data-ttu-id="e022a-p102">検索条件に基づいて結果を返します。現在、**messages** と **person** のコレクションでサポートされています。</span><span class="sxs-lookup"><span data-stu-id="e022a-p102">Returns results based on search criteria. Currently supported on **messages** and **person** collections.</span></span>|[`/me/messages?$search=pizza`][search-example]
| [<span data-ttu-id="e022a-121">$select</span><span class="sxs-lookup"><span data-stu-id="e022a-121">$select</span></span>](#select-parameter)       | <span data-ttu-id="e022a-122">プロパティ (列) をフィルターします。</span><span class="sxs-lookup"><span data-stu-id="e022a-122">Filters properties (columns).</span></span>|[`/users?$select=givenName,surname`][select-example]
| [<span data-ttu-id="e022a-123">$skip</span><span class="sxs-lookup"><span data-stu-id="e022a-123">$skip</span></span>](#skip-parameter)           | <span data-ttu-id="e022a-p103">結果セットにインデックスを作成します。また一部の API でページングを実装するために使用されており、`$top` と組み合わせて結果を手動でページングすることもできます。</span><span class="sxs-lookup"><span data-stu-id="e022a-p103">Indexes into a result set. Also used by some APIs to implement paging and can be used together with `$top` to manually page results.</span></span> | [`/me/messages?$skip=11`][skip-example]
| [<span data-ttu-id="e022a-126">$skipToken</span><span class="sxs-lookup"><span data-stu-id="e022a-126">$skipToken</span></span>](#skiptoken-parameter) | <span data-ttu-id="e022a-p104">複数ページにわたる結果セットから、結果の次のページを取得します。(一部の API では代わりに `$skip` を使用します。)</span><span class="sxs-lookup"><span data-stu-id="e022a-p104">Retrieves the next page of results from result sets that span multiple pages. (Some APIs use `$skip` instead.)</span></span> | `/users?$skiptoken=X%274453707402000100000017...`|
| [<span data-ttu-id="e022a-129">$top</span><span class="sxs-lookup"><span data-stu-id="e022a-129">$top</span></span>](#top-parameter)             | <span data-ttu-id="e022a-130">結果のページ サイズを設定します。</span><span class="sxs-lookup"><span data-stu-id="e022a-130">Sets the page size of results.</span></span> |[`/users?$top=2`][top-example]



<span data-ttu-id="e022a-131">これらのパラメーターは、[OData V4 クエリ言語][odata-query]と互換性があります。</span><span class="sxs-lookup"><span data-stu-id="e022a-131">These parameters are compatible with the [OData V4 query language][odata-query].</span></span> <span data-ttu-id="e022a-132">すべての Microsoft Graph API で全部のパラメーターがサポートされているわけではなく、`v1.0` エンドポイントと `beta` エンドポイントの間でサポートが大幅に異なる場合があります。</span><span class="sxs-lookup"><span data-stu-id="e022a-132">Not all parameters are supported across all Microsoft Graph APIs, and support might differ significantly between the `v1.0` and `beta` endpoints.</span></span> 

> <span data-ttu-id="e022a-p106">**注:**`beta` エンドポイントでは、`$` プレフィックスはオプションです。たとえば、`$filter` の代わりに、`filter` を使用しても同じです。詳細および例については、「[Microsoft Graph における $ プレフィックスのないクエリ パラメーターのサポート](http://dev.office.com/queryparametersinMicrosoftGraph)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e022a-p106">**Note:** On the `beta` endpoint, the `$` prefix is optional. For example, instead of `$filter`, you can use `filter`. For more details and examples, see [Supporting query parameters without $ prefixes in Microsoft Graph](http://dev.office.com/queryparametersinMicrosoftGraph).</span></span>

## <a name="encoding-query-parameters"></a><span data-ttu-id="e022a-136">クエリ パラメーターのエンコード</span><span class="sxs-lookup"><span data-stu-id="e022a-136">Encoding query parameters</span></span>

<span data-ttu-id="e022a-137">クエリ パラメーターの値はパーセント エンコードされる必要があります。</span><span class="sxs-lookup"><span data-stu-id="e022a-137">The values of query parameters should be percent-encoded.</span></span> <span data-ttu-id="e022a-138">これを行ううえで役立つ HTTP クライアント、ブラウザー、およびツールが多くあります ([Graph エクスプローラー][graph-explorer]など)。</span><span class="sxs-lookup"><span data-stu-id="e022a-138">Many HTTP clients, browsers, and tools (such as the [Graph Explorer][graph-explorer]) will help you with this.</span></span> <span data-ttu-id="e022a-139">クエリが失敗する場合、クエリ パラメーターの値が適切にエンコードされていないことがその原因の 1 つとして考えられます。</span><span class="sxs-lookup"><span data-stu-id="e022a-139">If a query is failing, one possible cause is failure to encode the query parameter values appropriately.</span></span>

<span data-ttu-id="e022a-140">エンコードされていない URL は、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="e022a-140">An unencoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName, 'J')
```

<span data-ttu-id="e022a-141">正しくエンコードされている URL は、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="e022a-141">A properly encoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName%2C+'J')
```

## <a name="count-parameter"></a><span data-ttu-id="e022a-142">count パラメーター</span><span class="sxs-lookup"><span data-stu-id="e022a-142">count parameter</span></span>

<span data-ttu-id="e022a-143">クエリ パラメーターを使用し、Microsoft Graph から返されるデータ値のページにコレクション内の項目数の合計を含めます。`$count`</span><span class="sxs-lookup"><span data-stu-id="e022a-143">Use the `$count` query parameter to include a count of the total number of items in a collection alongside the page of data values returned from Microsoft Graph.</span></span> 

<span data-ttu-id="e022a-144">たとえば、次のような要求では、現在のユーザーの **contact** コレクションと、`@odata.count` プロパティ内の **contact** コレクションのアイテム数の両方が返されます。</span><span class="sxs-lookup"><span data-stu-id="e022a-144">For example, the following request will return both the **contact** collection of the current user, and the number of items in the **contact** collection in the `@odata.count` property.</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

[<span data-ttu-id="e022a-145">Graph エクスプローラーで試す</span><span class="sxs-lookup"><span data-stu-id="e022a-145">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/contacts?$count=true&method=GET&version=v1.0)


><span data-ttu-id="e022a-146">**注:** `$count` は、[user](../api-reference/v1.0/resources/user.md) や [group](../api-reference/v1.0/resources/group.md) のコレクションのような、[directoryObject](../api-reference/v1.0/resources/directoryobject.md) から派生したリソースのコレクションに対してはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e022a-146">**Note:** `$count` is not supported for collections of resources that derive from [directoryObject](../api-reference/v1.0/resources/directoryobject.md) like collections of [users](../api-reference/v1.0/resources/user.md) or [groups](../api-reference/v1.0/resources/group.md).</span></span>

## <a name="expand-parameter"></a><span data-ttu-id="e022a-147">expand パラメーター</span><span class="sxs-lookup"><span data-stu-id="e022a-147">expand parameter</span></span>

<span data-ttu-id="e022a-148">Microsoft Graph リソースの多くは、宣言されているリソースのプロパティと、他のリソースとのリレーションシップの両方を公開します。</span><span class="sxs-lookup"><span data-stu-id="e022a-148">Many Microsoft Graph resources expose both declared properties of the resource as well as its relationships with other resources.</span></span> <span data-ttu-id="e022a-149">これらのリレーションシップは、参照プロパティまたはナビゲーション プロパティとも呼ばれ、1 つのリソースまたはリソースのコレクションのいずれかを参照することができます。</span><span class="sxs-lookup"><span data-stu-id="e022a-149">These relationships are also called reference properties or navigation properties, and they can reference either a single resource or a collection of resources.</span></span> <span data-ttu-id="e022a-150">たとえば、ユーザーのメール フォルダー、マネージャー、直属の部下は、すべてリレーションシップとして公開されます。</span><span class="sxs-lookup"><span data-stu-id="e022a-150">For example, the mail folders, manager, and direct reports of a user are all exposed as relationships.</span></span> 

<span data-ttu-id="e022a-p109">通常、単一の要求では、リソースの複数のプロパティ、またはリソースのリレーションシップの 1 つのいずれかに対してクエリを実行できますが、両方は行えません。`$expand` クエリ文字列パラメーターを使用して、展開されているリソース、または単一のリレーションシップ (ナビゲーション プロパティ) で参照されているコレクションを結果に含めることができます。</span><span class="sxs-lookup"><span data-stu-id="e022a-p109">Normally, you can query either the properties of a resource or one of its relationships in a single request, but not both. You can use the `$expand` query string parameter to include the expanded resource or collection referenced by a single relationship (navigation property) in your results.</span></span>

<span data-ttu-id="e022a-153">次の例では、ドライブ内のトップレベルの子項目と共に、ルート ドライブ情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="e022a-153">The following example gets root drive information along with the top-level child items in a drive:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children
```

[<span data-ttu-id="e022a-154">Graph エクスプローラーで試す</span><span class="sxs-lookup"><span data-stu-id="e022a-154">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children&method=GET&version=v1.0)

<span data-ttu-id="e022a-p110">いくつかのリソース コレクションで、`$select` パラメーターを追加すれば、展開されたリソースで返されるプロパティを指定することもできます。次の使用例は前の例と同じクエリを実行しますが、[`$select`](#select-parameter) ステートメントを使用して、展開されている子項目に返されるプロパティを **id** プロパティと **name** プロパティに限定します。</span><span class="sxs-lookup"><span data-stu-id="e022a-p110">With some resource collections, you can also specify the properties to be returned in the expanded resources by adding a `$select` parameter. The following example performs the same query as the previous example but uses a [`$select`](#select-parameter) statement to limit the properties returned for the expanded child items to the **id** and **name** properties.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

<span data-ttu-id="e022a-157">[Graph エクスプローラーで試す][expand-example]</span><span class="sxs-lookup"><span data-stu-id="e022a-157">[Try in Graph Explorer][expand-example]</span></span>

> <span data-ttu-id="e022a-p111">**注:** すべてのリレーションシップとリソースで、`$expand` クエリ パラメーターがサポートされているわけではありません。たとえば、ユーザーの **directReports**、**manager**、**memberOf** の各リレーションシップを展開できますが、その **events**、**messages**、**photo** のリレーションシップは展開できません。すべてのリソースまたはリレーションシップで、`$select` を使用して展開されたアイテムがサポートされているわけではありません。</span><span class="sxs-lookup"><span data-stu-id="e022a-p111">**Note:** Not all relationships and resources support the `$expand` query parameter. For example, you can expand the **directReports**, **manager**, and **memberOf** relationships on a user, but you cannot expand its **events**, **messages**, or **photo** relationships. Not all resources or relationships support using `$select` on expanded items.</span></span> 
> 
> <span data-ttu-id="e022a-161">[ユーザー](../api-reference/v1.0/resources/user.md)や[グループ](../api-reference/v1.0/resources/group.md)のような、[directoryObject](../api-reference/v1.0/resources/directoryobject.md) から派生した Azure AD リソースの場合、`$expand` は `beta` でのみサポートされており、通常は展開されているリレーションシップに対し最大 20 個のアイテムを返すことができます。</span><span class="sxs-lookup"><span data-stu-id="e022a-161">With Azure AD resources that derive from [directoryObject](../api-reference/v1.0/resources/directoryobject.md), like [user](../api-reference/v1.0/resources/user.md) and [group](../api-reference/v1.0/resources/group.md), `$expand` is only supported for `beta` and  typically returns a maximum of 20 items for the expanded relationship.</span></span>

## <a name="filter-parameter"></a><span data-ttu-id="e022a-162">filter パラメーター</span><span class="sxs-lookup"><span data-stu-id="e022a-162">filter parameter</span></span>

<span data-ttu-id="e022a-163">クエリ パラメーターを使用して、コレクションのサブセットのみを取得します。`$filter`</span><span class="sxs-lookup"><span data-stu-id="e022a-163">Use the `$filter` query parameter to retrieve just a subset of a collection.</span></span> 

<span data-ttu-id="e022a-164">たとえば、表示名が「J」という文字で始まるユーザーを検索するには、`startswith` を使用します。</span><span class="sxs-lookup"><span data-stu-id="e022a-164">For example, to find users whose display name starts with the letter 'J', use `startswith`.</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'J')
```

<span data-ttu-id="e022a-165">[Graph エクスプローラーで試す][filter-example]</span><span class="sxs-lookup"><span data-stu-id="e022a-165">[Try in Graph Explorer][filter-example]</span></span>

<span data-ttu-id="e022a-166">演算子のサポートは、お使いの Microsoft Graph API によって異なります。`$filter`</span><span class="sxs-lookup"><span data-stu-id="e022a-166">Support for `$filter` operators varies across Microsoft Graph APIs.</span></span> <span data-ttu-id="e022a-167">通常、次の論理演算子がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="e022a-167">The following logical operators are generally supported:</span></span> 

- <span data-ttu-id="e022a-168">等しい (`eq`)</span><span class="sxs-lookup"><span data-stu-id="e022a-168">equals (`eq`)</span></span>
- <span data-ttu-id="e022a-169">等しくない (`ne`)</span><span class="sxs-lookup"><span data-stu-id="e022a-169">not equals (`ne`)</span></span>
- <span data-ttu-id="e022a-170">より大きい (`gt`)</span><span class="sxs-lookup"><span data-stu-id="e022a-170">greater than (`gt`)</span></span>
- <span data-ttu-id="e022a-171">以上 (`ge`)</span><span class="sxs-lookup"><span data-stu-id="e022a-171">greater than or equals (`ge`)</span></span>
- <span data-ttu-id="e022a-172">より小さい (`lt`)、以下 (`le`)</span><span class="sxs-lookup"><span data-stu-id="e022a-172">less than (`lt`), less than or equals (`le`)</span></span>
- <span data-ttu-id="e022a-173">AND (`and`)</span><span class="sxs-lookup"><span data-stu-id="e022a-173">and (`and`)</span></span>
- <span data-ttu-id="e022a-174">OR (`or`)</span><span class="sxs-lookup"><span data-stu-id="e022a-174">or (`or`)</span></span>
- <span data-ttu-id="e022a-175">NOT (`not`)</span><span class="sxs-lookup"><span data-stu-id="e022a-175">not (`not`)</span></span>
 
<span data-ttu-id="e022a-176">文字列の演算子はたいていサポートされています。`startswith`</span><span class="sxs-lookup"><span data-stu-id="e022a-176">The `startswith` string operator is often supported.</span></span> <span data-ttu-id="e022a-177">ラムダ演算子は、一部の API でサポートされています。`any`</span><span class="sxs-lookup"><span data-stu-id="e022a-177">The `any` lambda operator is supported for some APIs.</span></span> <span data-ttu-id="e022a-178">いくつかの使用例について、次の表を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e022a-178">For some  usage examples, see the following table.</span></span> <span data-ttu-id="e022a-179">構文の詳細については、「[OData プロトコル][odata-filter]」を参照してください。`$filter`</span><span class="sxs-lookup"><span data-stu-id="e022a-179">For more details about `$filter` syntax, see the [OData protocol][odata-filter].</span></span>  

<span data-ttu-id="e022a-180">次の表では、`$filter` クエリ パラメーター使用例を示します。</span><span class="sxs-lookup"><span data-stu-id="e022a-180">The following table shows some examples that use the `$filter` query parameter.</span></span>

> <span data-ttu-id="e022a-181">**注:** 例をクリックして [Graph エクスプローラー][graph-explorer]で試行します。</span><span class="sxs-lookup"><span data-stu-id="e022a-181">**Note:** Click the examples to try them in [Graph Explorer][graph-explorer].</span></span>

| <span data-ttu-id="e022a-182">説明</span><span class="sxs-lookup"><span data-stu-id="e022a-182">Description</span></span> | <span data-ttu-id="e022a-183">例</span><span class="sxs-lookup"><span data-stu-id="e022a-183">Example</span></span>
|:------------|:--------|
| <span data-ttu-id="e022a-184">複数のプロパティ間で Mary という名前を持つユーザーを検索します。</span><span class="sxs-lookup"><span data-stu-id="e022a-184">Search for users with the name Mary across multiple properties.</span></span> | [`https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'mary') or startswith(givenName,'mary') or startswith(surname,'mary') or startswith(mail,'mary') or startswith(userPrincipalName,'mary')`](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(displayName,'mary')+or+startswith(givenName,'mary')+or+startswith(surname,'mary')+or+startswith(mail,'mary')+or+startswith(userPrincipalName,'mary')&method=GET&version=v1.0) 
| <span data-ttu-id="e022a-185">2017 年 7 月 1 日以降に開始する、サインイン ユーザーのイベントすべてを取得します。</span><span class="sxs-lookup"><span data-stu-id="e022a-185">Get all the signed-in user's events that start after 7/1/2017.</span></span> | [`https://graph.microsoft.com/v1.0/me/events?$filter=start/dateTime ge '2017-07-01T08:00'`](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$filter=start/dateTime+ge+'2017-07-01T08:00'&method=GET&version=v1.0) 
| <span data-ttu-id="e022a-186">サインイン ユーザーが受信した特定のアドレスからの電子メールすべてを取得します。</span><span class="sxs-lookup"><span data-stu-id="e022a-186">Get all emails from a specific address received by the signed-in user.</span></span> | [`https://graph.microsoft.com/v1.0/me/messages?$filter=from/emailAddress/address eq 'someuser@example.com'`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=from/emailAddress/address+eq+'someuser@.com'&method=GET&version=v1.0) 
| <span data-ttu-id="e022a-187">2017 年 4 月にサインイン ユーザーが受信した電子メールすべてを取得します。</span><span class="sxs-lookup"><span data-stu-id="e022a-187">Get all emails received by the signed-in user in April 2017.</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=ReceivedDateTime ge 2017-04-01 and receivedDateTime lt 2017-05-01`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=ReceivedDateTime+ge+2017-04-01+and+receivedDateTime+lt+2017-05-01&method=GET&version=v1.0) 
| <span data-ttu-id="e022a-188">サインイン ユーザーの受信トレイから未読メールをすべて取得します。</span><span class="sxs-lookup"><span data-stu-id="e022a-188">Get all unread mail in the signed-in user's Inbox.</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=isRead eq false`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=isRead+eq+false&method=GET&version=v1.0) 
| <span data-ttu-id="e022a-189">組織内のすべての Office 365 グループの一覧</span><span class="sxs-lookup"><span data-stu-id="e022a-189">List all Office 365 groups in an organization.</span></span> | [`https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')`](https://developer.microsoft.com/graph/graph-explorer?request=groups?$filter=groupTypes/any(c:c+eq+'Unified')&method=GET&version=v1.0) 

> <span data-ttu-id="e022a-p114">**注:** Azure AD リソースでは、次の `$filter` 演算子はサポートされていません: `ne`、`gt`、`ge`、`lt`、`le`、`not`。Microsoft Graph リソースでは現在、`contains` 文字列の演算子はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e022a-p114">**Note:** The following `$filter` operators are not supported for Azure AD resources:  `ne`, `gt`, `ge`, `lt`, `le`, and `not`. The `contains` string operator is currently not supported on any Microsoft Graph resources.</span></span>

## <a name="format-parameter"></a><span data-ttu-id="e022a-192">format パラメーター</span><span class="sxs-lookup"><span data-stu-id="e022a-192">format parameter</span></span>

<span data-ttu-id="e022a-193">クエリ パラメーターを使用して、Microsoft Graph から返される項目のメディア形式を指定します。`$format`</span><span class="sxs-lookup"><span data-stu-id="e022a-193">Use the `$format` query parameter to specify the media format of the items returned from Microsoft Graph.</span></span>

<span data-ttu-id="e022a-194">たとえば、次の要求では組織のユーザーが JSON 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="e022a-194">For example, the following request returns the users in the organization in the json format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$format=json
```

<span data-ttu-id="e022a-195">[Graph エクスプローラーで試す][format-example]</span><span class="sxs-lookup"><span data-stu-id="e022a-195">[Try in Graph Explorer][format-example]</span></span>

> <span data-ttu-id="e022a-196">**注:**`$format` クエリ パラメーターは、さまざまな形式 (atom、xml、json など) をサポートしていますが、結果がすべての形式で返されるわけではありません。</span><span class="sxs-lookup"><span data-stu-id="e022a-196">**Note:** The `$format` query parameter supports a number of formats (for example, atom, xml, and json) but results may not be returned in all formats.</span></span>

## <a name="orderby-parameter"></a><span data-ttu-id="e022a-197">orderby パラメーター</span><span class="sxs-lookup"><span data-stu-id="e022a-197">orderby parameter</span></span>

<span data-ttu-id="e022a-198">クエリ パラメーターを使用して、Microsof Graph から返される項目の並べ替え順序を指定します。`$orderby`</span><span class="sxs-lookup"><span data-stu-id="e022a-198">Use the `$orderby` query parameter to specify the sort order of the items returned from Microsoft Graph.</span></span>

<span data-ttu-id="e022a-199">たとえば、次の要求では組織のユーザーが表示名順で返されます。</span><span class="sxs-lookup"><span data-stu-id="e022a-199">For example, the following request returns the users in the organization ordered by their display name:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```
<span data-ttu-id="e022a-200">[Graph エクスプローラーで試す][orderby-example]</span><span class="sxs-lookup"><span data-stu-id="e022a-200">[Try in Graph Explorer][orderby-example]</span></span>

<span data-ttu-id="e022a-p115">複合型のエンティティでも並べ替えができます。次の要求では、メッセージを取得し、それらを **emailAddress** という複合型である **from** プロパティの **address** フィールドで並べ替えます。</span><span class="sxs-lookup"><span data-stu-id="e022a-p115">You can also sort by complex type entities. The following request gets messages and sorts them by the **address** field of the **from** property, which is of the complex type **emailAddress**:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
```
[<span data-ttu-id="e022a-203">Graph エクスプローラーで試す</span><span class="sxs-lookup"><span data-stu-id="e022a-203">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/address&method=GET&version=v1.0)

<span data-ttu-id="e022a-204">昇順または降順で結果を並べ替えるには、`asc` または `desc` のいずれかをスペースで区切ってフィールド名の後に追加します。たとえば `?$orderby=name%20desc` のようにします。</span><span class="sxs-lookup"><span data-stu-id="e022a-204">To sort the results in ascending or descending order, append either `asc` or `desc` to the field name, separated by a space; for example, `?$orderby=name%20desc`.</span></span>

<span data-ttu-id="e022a-205">一部の API では、複数のプロパティの結果を並べ替えることができます。</span><span class="sxs-lookup"><span data-stu-id="e022a-205">With some APIs, you can order results on multiple properties.</span></span> <span data-ttu-id="e022a-206">たとえば、次のような要求ではユーザーの受信トレイ内のメッセージを、最初は送信者の名前で降順に並べ替え (Z から A)、次に件名で昇順 (既定) に並べ替えます。</span><span class="sxs-lookup"><span data-stu-id="e022a-206">For example, the following request orders the messages in the user's Inbox, first by the name of the person who sent it in descending order (Z to A), and then by subject in ascending order (default).</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/Inbox/messages?$orderby=from/emailAddress/name desc,subject
```

[<span data-ttu-id="e022a-207">Graph エクスプローラーで試す</span><span class="sxs-lookup"><span data-stu-id="e022a-207">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/name%20desc,subject&method=GET&version=v1.0)

<span data-ttu-id="e022a-208">$filter を指定した場合は、サーバーで結果の並べ替え順序が考慮されます。</span><span class="sxs-lookup"><span data-stu-id="e022a-208">When you specify $filter the server will infer a sort order for the results.</span></span> <span data-ttu-id="e022a-209">と `$filter` の両方を使用する場合、サーバーでは常に `$filter` の結果の並べ替え順序が考慮されるため、`$filter` 内のプロパティを他のプロパティよりも先に `$orderby` 内に配置して、`$filter` パラメーターに現れる順序で並べる必要があります。`$orderby`</span><span class="sxs-lookup"><span data-stu-id="e022a-209">If you use both `$orderby` and `$filter`, because the server always infers a sort order for the results of a `$filter`, the properties in the `$filter` must be listed first in the `$orderby` before any other properties, and they must be listed in the order that they appear in the `$filter` parameter.</span></span> 

<span data-ttu-id="e022a-210">次の例は、**Subject** と **Importance** の両方のプロパティでフィルター処理されてから、**Subject**、**Importance**、**receivedDateTime** の各プロパティで降順で並べ替えられたクエリを示しています。</span><span class="sxs-lookup"><span data-stu-id="e022a-210">The following example shows a query filtered by the **subject** and **importance** properties, and then sorted by the **subject**, **importance**, and **receivedDateTime** properties in descending order.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=Subject eq 'welcome' and importance eq 'normal'&$orderby=subject,importance,receivedDateTime desc
```

[<span data-ttu-id="e022a-211">Graph エクスプローラーで試す</span><span class="sxs-lookup"><span data-stu-id="e022a-211">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=subject%20eq%20%27welcome%27%20and%20importance%20eq%20%27normal%27%20&$orderby=subject,importance,receivedDateTime%20desc&method=GET&version=v1.0)

 > <span data-ttu-id="e022a-212">**注:** [ユーザー](../api-reference/v1.0/resources/user.md)や[グループ](../api-reference/v1.0/resources/group.md)のような、[directoryObject](../api-reference/v1.0/resources/directoryobject.md) から派生した Azure AD リソースの場合、`$orderby` 式と `$filter` 式を結合することはできません。</span><span class="sxs-lookup"><span data-stu-id="e022a-212">**Note:** With Azure AD resources that derive from [directoryObject](../api-reference/v1.0/resources/directoryobject.md), like [user](../api-reference/v1.0/resources/user.md) and [group](../api-reference/v1.0/resources/group.md), you cannot combine `$orderby` with `$filter` expressions.</span></span> 

## <a name="search-parameter"></a><span data-ttu-id="e022a-213">search パラメーター</span><span class="sxs-lookup"><span data-stu-id="e022a-213">search parameter</span></span>

<span data-ttu-id="e022a-214">クエリ パラメーターを使用して、要求の結果を検索条件と一致するものに制限します。`$search`</span><span class="sxs-lookup"><span data-stu-id="e022a-214">Use the `$search` query parameter to restrict the results of a request to match a search criterion.</span></span>

> <span data-ttu-id="e022a-p118">**注:** 現在の検索対象は、[メッセージ](../api-reference/v1.0/resources/message.md) コレクションと[人物](../api-reference/v1.0/resources/person.md)コレクション**だけ**です。`$search` 要求は最大 250 まで結果を返します。検索要求では [`$filter`](#filter-parameter) も [`$orderby`](#orderby-parameter) も使用できません。</span><span class="sxs-lookup"><span data-stu-id="e022a-p118">**Note:** You can currently search **only** [message](../api-reference/v1.0/resources/message.md) and [person](../api-reference/v1.0/resources/person.md) collections. A `$search` request returns up to 250 results. You cannot use [`$filter`](#filter-parameter) or [`$orderby`](#orderby-parameter) in a search request.</span></span>

### <a name="using-search-on-message-collections"></a><span data-ttu-id="e022a-218">メッセージ コレクションで $search を使用する</span><span class="sxs-lookup"><span data-stu-id="e022a-218">Using $search on message collections</span></span>

<span data-ttu-id="e022a-219">特定のメッセージ プロパティの値に基づいてメッセージを検索することができます。</span><span class="sxs-lookup"><span data-stu-id="e022a-219">You can search messages based on a value in specific message properties.</span></span> <span data-ttu-id="e022a-220">検索結果は、メッセージが送信された日時で並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="e022a-220">The results of the search are sorted by the date and time that the message was sent.</span></span>

<span data-ttu-id="e022a-221">メッセージで検索を行うときに、特定のメッセージ プロパティを指定せずに値のみを指定した場合、検索は既定の検索プロパティである **from**、**subject**、**body** に基づいて行われます。</span><span class="sxs-lookup"><span data-stu-id="e022a-221">If you do a search on messages and specify only a value without specific message properties, the search is carried out on the default search properties of **from**, **subject**, and **body**.</span></span>

<span data-ttu-id="e022a-222">次の例は、サインイン中のユーザーの受信トレイにあるメッセージのうち、既定の 3 つの検索プロパティのいずれかに "pizza" が含まれるメッセージをすべて返します。</span><span class="sxs-lookup"><span data-stu-id="e022a-222">The following example returns all messages in the signed-in user's Inbox that contains "pizza" in any of the three default search properties:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

<span data-ttu-id="e022a-223">[Graph エクスプローラーで試す][search-example]</span><span class="sxs-lookup"><span data-stu-id="e022a-223">[Try in Graph Explorer][search-example]</span></span>

<span data-ttu-id="e022a-224">また、キーワード クエリ言語 (KQL) 構文で認識される、以下の表のメッセージ プロパティ名を指定して、メッセージの検索をすることもできます。</span><span class="sxs-lookup"><span data-stu-id="e022a-224">Alternatively, you can search messages by specifying message property names in the following table, that are recognized by the Keyword Query Language (KQL) syntax.</span></span> <span data-ttu-id="e022a-225">これらのプロパティ名は Microsoft Graph の **message** エンティティで定義したプロパティです。</span><span class="sxs-lookup"><span data-stu-id="e022a-225">These property names correspond to properties defined in the **message** entity of Microsoft Graph.</span></span> <span data-ttu-id="e022a-226">Outlook や他の Office 365 アプリケーション (SharePoint など) では KQL 構文をサポートしており、データ ストアの共通探索ドメインの利便性が向上します。</span><span class="sxs-lookup"><span data-stu-id="e022a-226">Outlook and other Office 365 applications such as SharePoint support KQL syntax, providing the convenience of a common discovery domain for their data stores.</span></span>


| <span data-ttu-id="e022a-227">検索可能な電子メール プロパティ</span><span class="sxs-lookup"><span data-stu-id="e022a-227">Searchable email property</span></span>                | <span data-ttu-id="e022a-228">説明</span><span class="sxs-lookup"><span data-stu-id="e022a-228">Description</span></span> | <span data-ttu-id="e022a-229">例</span><span class="sxs-lookup"><span data-stu-id="e022a-229">Example</span></span> 
|:-------------------------|:------------|:---------|
| <span data-ttu-id="e022a-230">**attachment**</span><span class="sxs-lookup"><span data-stu-id="e022a-230">**attachment**</span></span>           | <span data-ttu-id="e022a-231">電子メール メッセージに添付されているファイルの名前。</span><span class="sxs-lookup"><span data-stu-id="e022a-231">The names of files attached to an email message.</span></span>|[`me/messages?$search="attachment:api-catalog.md"`][search-att-example]
| <span data-ttu-id="e022a-232">**bcc**</span><span class="sxs-lookup"><span data-stu-id="e022a-232">**bcc**</span></span>           | <span data-ttu-id="e022a-233">SMTP アドレス、表示名、エイリアスとして指定されている、電子メール メッセージの **bcc** フィールド。</span><span class="sxs-lookup"><span data-stu-id="e022a-233">The **bcc** field of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="bcc:samanthab@contoso.com"&$select=subject,bccRecipients`][search-bcc-example]
| <span data-ttu-id="e022a-234">**body**</span><span class="sxs-lookup"><span data-stu-id="e022a-234">**body**</span></span>           | <span data-ttu-id="e022a-235">電子メール メッセージの本文。</span><span class="sxs-lookup"><span data-stu-id="e022a-235">The body of an email message.</span></span>|[`me/messages?$search="body:excitement"`][search-body-example]
| <span data-ttu-id="e022a-236">**cc**</span><span class="sxs-lookup"><span data-stu-id="e022a-236">**cc**</span></span>           | <span data-ttu-id="e022a-237">SMTP アドレス、表示名、エイリアスとして指定されている、電子メール メッセージの **cc** フィールド。</span><span class="sxs-lookup"><span data-stu-id="e022a-237">The **cc** field of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="cc:danas"&$select=subject,ccRecipients`][search-cc-example]
| <span data-ttu-id="e022a-238">**from**</span><span class="sxs-lookup"><span data-stu-id="e022a-238">**from**</span></span>           | <span data-ttu-id="e022a-239">SMTP アドレス、表示名、エイリアスとして指定されている、電子メール メッセージの送信者。</span><span class="sxs-lookup"><span data-stu-id="e022a-239">The sender of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="from:randiw"&$select=subject,from`][search-from-example]
| <span data-ttu-id="e022a-240">**hasAttachment**</span><span class="sxs-lookup"><span data-stu-id="e022a-240">**hasAttachment**</span></span> | <span data-ttu-id="e022a-241">電子メール メッセージに添付ファイルがあり、そのファイルがインラインの添付ファイルでない場合は true、そうでない場合は false。</span><span class="sxs-lookup"><span data-stu-id="e022a-241">True if an email message contains an attachment that is not an inline attachment, false otherwise.</span></span> |[`me/messages?$search="hasAttachments=true"`][search-from-example]
| <span data-ttu-id="e022a-242">**importance**</span><span class="sxs-lookup"><span data-stu-id="e022a-242">**importance**</span></span>           | <span data-ttu-id="e022a-243">送信者がメッセージを送信するときに指定できる電子メール メッセージの重要度。</span><span class="sxs-lookup"><span data-stu-id="e022a-243">The importance of an email message, which a sender can specify when sending a message.</span></span> <span data-ttu-id="e022a-244">使用可能な値: `low`、`medium`、`high`。</span><span class="sxs-lookup"><span data-stu-id="e022a-244">The possible values are `low`, `medium`, or `high`.</span></span>|[`me/messages?$search="importance:high"&$select=subject,importance`][search-imp-example]
| <span data-ttu-id="e022a-245">**kind**</span><span class="sxs-lookup"><span data-stu-id="e022a-245">**kind**</span></span>           | <span data-ttu-id="e022a-246">メッセージの種類。</span><span class="sxs-lookup"><span data-stu-id="e022a-246">The type of message.</span></span> <span data-ttu-id="e022a-247">使用可能な値: `contacts`、`docs`、`email`、`faxes`、`im`、`journals`、`meetings`、`notes`、`posts`、`rssfeeds`、`tasks`、`voicemail`。</span><span class="sxs-lookup"><span data-stu-id="e022a-247">The possible values are `contacts`, `docs`, `email`, `faxes`, `im`, `journals`, `meetings`, `notes`, `posts`, `rssfeeds`, `tasks`, or `voicemail`.</span></span>|[`me/messages?$search="kind:voicemail"`][search-kind-example]
| <span data-ttu-id="e022a-248">**participants**</span><span class="sxs-lookup"><span data-stu-id="e022a-248">**participants**</span></span>           | <span data-ttu-id="e022a-249">SMTP アドレス、表示名、エイリアスとして指定されている、電子メール メッセージの **from**、**to**、**cc**、**bcc** フィールド。</span><span class="sxs-lookup"><span data-stu-id="e022a-249">The **from**, **to**, **cc**, and **bcc** fields of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="participants:danas"`][search-part-example]
| <span data-ttu-id="e022a-250">**received**</span><span class="sxs-lookup"><span data-stu-id="e022a-250">**received**</span></span>           | <span data-ttu-id="e022a-251">電子メール メッセージが受信者によって受信された日付。</span><span class="sxs-lookup"><span data-stu-id="e022a-251">The date that an email message was received by a recipient.</span></span>|[`me/messages?$search="received:07/23/2018"&$select=subject,receivedDateTime`][search-rcvd-example]
| <span data-ttu-id="e022a-252">**recipients**</span><span class="sxs-lookup"><span data-stu-id="e022a-252">**recipients**</span></span>           | <span data-ttu-id="e022a-253">SMTP アドレス、表示名、エイリアスとして指定されている、電子メール メッセージの **to**、**cc**、**bcc** フィールド。</span><span class="sxs-lookup"><span data-stu-id="e022a-253">The **to**, **cc**, and **bcc** fields of an email meesage, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="recipients:randiq"&$select=subject,toRecipients,ccRecipients,bccRecipients`][search-rcpts-example]
| <span data-ttu-id="e022a-254">**sent**</span><span class="sxs-lookup"><span data-stu-id="e022a-254">**sent**</span></span>           | <span data-ttu-id="e022a-255">送信者によって電子メール メッセージが送信された日付。</span><span class="sxs-lookup"><span data-stu-id="e022a-255">The date that an email message was sent by the sender.</span></span>|[`me/messages?$search="sent:07/23/2018"&$select=subject,sentDateTime`][search-sent-example]
| <span data-ttu-id="e022a-256">**size**</span><span class="sxs-lookup"><span data-stu-id="e022a-256">**size**</span></span>           | <span data-ttu-id="e022a-257">アイテムのサイズ (バイト数)。</span><span class="sxs-lookup"><span data-stu-id="e022a-257">The size of an item in bytes.</span></span>|[`me/messages?$search="size:1..500000"`][search-size-example]
| <span data-ttu-id="e022a-258">**subject**</span><span class="sxs-lookup"><span data-stu-id="e022a-258">**subject**</span></span>           | <span data-ttu-id="e022a-259">電子メール メッセージの件名行に含まれるテキスト。</span><span class="sxs-lookup"><span data-stu-id="e022a-259">The text in the subject line of an email message.</span></span> <span data-ttu-id="e022a-260">.</span><span class="sxs-lookup"><span data-stu-id="e022a-260"></span></span>|[`me/messages?$search="subject:has"&$select=subject`][search-sbj-example]
| <span data-ttu-id="e022a-261">**to**</span><span class="sxs-lookup"><span data-stu-id="e022a-261">**to**</span></span>           | <span data-ttu-id="e022a-262">SMTP アドレス、表示名、エイリアスとして指定されている、電子メール メッセージの **to** フィールド。</span><span class="sxs-lookup"><span data-stu-id="e022a-262">The **to** field of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="to:randiw"&$select=subject,toRecipients`][search-to-example]


<span data-ttu-id="e022a-263">検索可能な電子メール プロパティ、KQL 構文、サポートされている演算子、検索のヒントなどの詳細については、次の記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e022a-263">For more information about searchable email properties, KQL syntax, supported operators, and tips on searching, see the following articles:</span></span>

- <span data-ttu-id="e022a-264">[Exchange の検索可能なプロパティ](https://docs.microsoft.com/en-us/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators#searchable-properties-in-exchange)。</span><span class="sxs-lookup"><span data-stu-id="e022a-264">[Searchable properties in Exchange](https://docs.microsoft.com/en-us/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators#searchable-properties-in-exchange).</span></span>

- [<span data-ttu-id="e022a-265">キーワード クエリ言語 (KQL) 構文のリファレンス</span><span class="sxs-lookup"><span data-stu-id="e022a-265">Keyword Query Language (KQL) syntax reference</span></span>](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)

- <span data-ttu-id="e022a-266">[Exchange 2016 におけるインプレースの電子情報開示のためのメッセージ プロパティと検索演算子](https://technet.microsoft.com/en-us/library/dn774955(v=exchg.160).aspx)</span><span class="sxs-lookup"><span data-stu-id="e022a-266">[Message properties and search operators for In-Place eDiscovery in Exchange 2016](https://technet.microsoft.com/en-us/library/dn774955(v=exchg.160).aspx)</span></span>

### <a name="using-search-on-person-collections"></a><span data-ttu-id="e022a-267">人物コレクションで $search を使用する</span><span class="sxs-lookup"><span data-stu-id="e022a-267">Using $search on person collections</span></span>

<span data-ttu-id="e022a-p124">Microsoft Graph People API を使用してユーザーに最も関連のある人物を取得できます。関連性は、ユーザーのコミュニケーションとコラボレーション パターン、およびビジネスのリレーションシップによって決定されます。People API では、`$search` クエリ パラメーターがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="e022a-p124">You can use the Microsoft Graph People API to retrieve the people who are most relevant to a user. Relevance is determined by the user’s communication and collaboration patterns and business relationships. The People API supports the `$search` query parameter.</span></span>

<span data-ttu-id="e022a-271">[person](../api-reference/v1.0/resources/person.md) リソースの **displayName** プロパティと **emailAddress** プロパティの両方で人物の検索を行います。</span><span class="sxs-lookup"><span data-stu-id="e022a-271">Searches on people occur on both the **displayName** and **emailAddress** properties of the [person](../api-reference/v1.0/resources/person.md) resource.</span></span>

<span data-ttu-id="e022a-272">次の要求は、サインイン ユーザーの **people** コレクションに含まれる各ユーザーの **displayName** プロパティと **emailAddress** プロパティで、「Irene McGowen」という名前の人物を検索します。</span><span class="sxs-lookup"><span data-stu-id="e022a-272">The following request does a search for a person named "Irene McGowen" in the **displayName** and **emailAddress** properties in each person in the **people** collection of the signed-in user.</span></span> <span data-ttu-id="e022a-273">「Irene McGowan」という名前の人物がサインインしているユーザーに関連するため、「Irene McGowan」の情報が返されます。</span><span class="sxs-lookup"><span data-stu-id="e022a-273">Because a person named "Irene McGowan" is relevant to the signed-in user, the information for "Irene McGowan" is returned.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="Irene McGowen"
```

<span data-ttu-id="e022a-274">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="e022a-274">The following example shows the response.</span></span> 

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

<span data-ttu-id="e022a-275">People API の詳細については、「[関係する人の情報を取得する](./people_example.md#search-people)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e022a-275">To learn more about the People API, see [Get information about relevant people](./people_example.md#search-people).</span></span>  

## <a name="select-parameter"></a><span data-ttu-id="e022a-276">select パラメーター</span><span class="sxs-lookup"><span data-stu-id="e022a-276">select parameter</span></span>

<span data-ttu-id="e022a-277">クエリ パラメーターを使用して、個別リソースまたはリソースのコレクションの既定値とは異なるプロパティのセットを返します。`$select`</span><span class="sxs-lookup"><span data-stu-id="e022a-277">Use the `$select` query parameter to return a set of properties that are different than the default set for an individual resource or a collection of resources.</span></span> <span data-ttu-id="e022a-278">$Select で、既定のプロパティのサブセットまたはスーパーセットを指定できます。</span><span class="sxs-lookup"><span data-stu-id="e022a-278">With $select, you can specify a subset or a superset of the default properties.</span></span>

<span data-ttu-id="e022a-279">たとえば、サインイン ユーザーのメッセージを取得するとき、**from** プロパティと **subject** プロパティだけを返すよう指定できます。</span><span class="sxs-lookup"><span data-stu-id="e022a-279">For example, when retrieving the messages of the signed-in user, you can specify that only the **from** and **subject** properties be returned:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

<span data-ttu-id="e022a-280">[Graph エクスプローラーで試す][select-example]</span><span class="sxs-lookup"><span data-stu-id="e022a-280">[Try in Graph Explorer][select-example]</span></span>

> <span data-ttu-id="e022a-281">**重要:** 通常は、`$select` を使用して、クエリから返されるプロパティをお使いのアプリで必要なものだけに制限することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="e022a-281">**Important:** In general, we recommend that you use `$select` to limit the properties returned by a query to those needed by your app.</span></span> <span data-ttu-id="e022a-282">これは特に、クエリが大きな結果セットを返す可能性がある場合に該当します。</span><span class="sxs-lookup"><span data-stu-id="e022a-282">This is especially true of queries that might potentially return a large result set.</span></span> <span data-ttu-id="e022a-283">行ごとに返されるプロパティを制限すれば、ネットワークの負荷を軽減し、アプリのパフォーマンスを向上させることができます。</span><span class="sxs-lookup"><span data-stu-id="e022a-283">Limiting the properties returned in each row will reduce network load and help improve your app's performance.</span></span>
>
> <span data-ttu-id="e022a-p128">では、[ユーザー](../api-reference/v1.0/resources/user.md)と[グループ](../api-reference/v1.0/resources/group.md)のような、[directoryObject](../api-reference/v1.0/resources/directoryobject.md) から派生した一部の Azure AD リソースは、読み取り時に制限された既定値のプロパティ サブセットを返します。既定のセット以外のプロパティを返すには、これらのリソースに対して `$select` を使用する必要があります。`v1.0`</span><span class="sxs-lookup"><span data-stu-id="e022a-p128">In `v1.0`, some Azure AD resources that derive from [directoryObject](../api-reference/v1.0/resources/directoryobject.md), like [user](../api-reference/v1.0/resources/user.md) and [group](../api-reference/v1.0/resources/group.md), return a limited, default subset of properties on reads. For these resources, you must use `$select` to return properties outside of the default set.</span></span>  

## <a name="skip-parameter"></a><span data-ttu-id="e022a-286">skip パラメーター</span><span class="sxs-lookup"><span data-stu-id="e022a-286">skip parameter</span></span>

<span data-ttu-id="e022a-p129">コレクションを開始するときにスキップする項目数を設定するには、`$skip` クエリ パラメーターを使用します。たとえば、次の要求はユーザーのイベントを、コレクション内の 21 番目以降のイベントから作成日順で返します。</span><span class="sxs-lookup"><span data-stu-id="e022a-p129">Use the `$skip` query parameter to set the number of items to skip at the start of a collection. For example, the following request returns events for the user sorted by date created, starting with the 21st event in the collection:</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```
<span data-ttu-id="e022a-289">[Graph エクスプローラーで試す][skip-example]</span><span class="sxs-lookup"><span data-stu-id="e022a-289">[Try in Graph Explorer][skip-example]</span></span>

> <span data-ttu-id="e022a-290">**注:** Outlook のメールやカレンダーなど、いくつかの Microsoft Graph API (**message**、**event**、**calendar**) は、`$skip` を使用してページングを実装します。</span><span class="sxs-lookup"><span data-stu-id="e022a-290">**Note:** Some Microsoft Graph APIs, like Outlook Mail and Calendars (**message**, **event**, and **calendar**), use `$skip` to implement paging.</span></span> <span data-ttu-id="e022a-291">クエリの結果が複数ページにまたがる場合、これらの API は `@odata:nextLink` プロパティと共に `$skip` パラメーターが含まれる URL を返します。</span><span class="sxs-lookup"><span data-stu-id="e022a-291">When results of a query span multiple pages, these APIs will return an `@odata:nextLink` property with a URL that contains a `$skip` parameter.</span></span> <span data-ttu-id="e022a-292">この URL を使用して、結果の次のページに戻れます。</span><span class="sxs-lookup"><span data-stu-id="e022a-292">You can use this URL to return the next page of results.</span></span> <span data-ttu-id="e022a-293">詳細については、「[ページング](./paging.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e022a-293">To learn more, see [Paging](./paging.md).</span></span>

## <a name="skiptoken-parameter"></a><span data-ttu-id="e022a-294">skipToken パラメーター</span><span class="sxs-lookup"><span data-stu-id="e022a-294">skipToken parameter</span></span>

<span data-ttu-id="e022a-p131">要求の中には、サーバー側のページングを使用したり、応答におけるページ サイズを限定するために [`$top`](#top-parameter) パラメーターを使用したりすることによって、複数のデータ ページを返すものがあります。Microsoft Graph API の多くは、`skipToken` クエリ パラメーターを使用して、結果の後続のページを参照します。`$skiptoken` パラメーターは、結果の次のページを参照する不透明トークンを含んでおり、応答の `@odata.nextLink` プロパティで指定される URL で返されます。詳細については、「[ページング](./paging.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e022a-p131">Some requests return multiple pages of data either due to server-side paging or due to the use of the [`$top`](#top-parameter) parameter to limit the page size of the response. Many Microsoft Graph APIs use the `skipToken` query parameter to reference subsequent pages of the result. The `$skiptoken` parameter contains an opaque token that references the next page of results and is returned in the URL provided in the `@odata.nextLink` property in the response. To learn more, see [Paging](./paging.md).</span></span>


## <a name="top-parameter"></a><span data-ttu-id="e022a-299">top パラメーター</span><span class="sxs-lookup"><span data-stu-id="e022a-299">top parameter</span></span>

<span data-ttu-id="e022a-300">クエリ パラメーターを使用して、結果セットのページ サイズを指定します。`$top`</span><span class="sxs-lookup"><span data-stu-id="e022a-300">Use the `$top` query parameter to specify the page size of the result set.</span></span> 

<span data-ttu-id="e022a-301">結果セットにさらに項目が残っている場合、応答本文に `@odata.nextLink` パラメーターが含まれます。</span><span class="sxs-lookup"><span data-stu-id="e022a-301">If more items remain in the result set, the response body will contain an `@odata.nextLink` parameter.</span></span> <span data-ttu-id="e022a-302">このパラメーターには、結果の次のページを取得するために使用できる URL が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e022a-302">This parameter contains a URL that you can use to get the next page of results.</span></span> <span data-ttu-id="e022a-303">詳細については、「[ページング](./paging.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e022a-303">To learn more, see [Paging](./paging.md).</span></span> 

<span data-ttu-id="e022a-304">たとえば、次の要求はユーザーのメールボックスの最初の 5 つのメッセージを返します。</span><span class="sxs-lookup"><span data-stu-id="e022a-304">For example, the following request returns the first five messages in the user's mailbox:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```

<span data-ttu-id="e022a-305">[Graph エクスプローラーで試す][top-example]</span><span class="sxs-lookup"><span data-stu-id="e022a-305">[Try in Graph Explorer][top-example]</span></span>


## <a name="error-handling-for-query-parameters"></a><span data-ttu-id="e022a-306">クエリ パラメーターのエラー処理</span><span class="sxs-lookup"><span data-stu-id="e022a-306">Error handling for query parameters</span></span>

<span data-ttu-id="e022a-p133">指定されたクエリ パラメーターがサポートされていない場合、一部の要求はエラー メッセージを返します。たとえば、`$expand` を `user/photo` のリレーションシップで使用することはできません。</span><span class="sxs-lookup"><span data-stu-id="e022a-p133">Some requests will return an error message if a specified query parameter is not supported. For example, you cannot use `$expand` on the `user/photo` relationship.</span></span> 

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

<span data-ttu-id="e022a-309">ただし、要求で指定されたクエリ パラメーターが警告なしで失敗する可能性があるため、注意が必要です。</span><span class="sxs-lookup"><span data-stu-id="e022a-309">However, it is important to note that query parameters specified in a request might fail silently.</span></span> <span data-ttu-id="e022a-310">これは、クエリ パラメーターがサポートされていない場合や、クエリ パラメーターの組み合わせがサポートされていない場合に起こり得ます。</span><span class="sxs-lookup"><span data-stu-id="e022a-310">This can be true for unsupported query parameters as well as for unsupported combinations of query parameters.</span></span> <span data-ttu-id="e022a-311">その場合、要求によって返されたデータを調べ、指定したクエリ パラメーターに期待どおりの効果があったかどうかを確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e022a-311">In these cases, you should examine the data returned by the request to determine whether the query parameters you specified had the desired effect.</span></span> 

[graph-explorer]: https://developer.microsoft.com/graph/graph-explorer
[odata-filter]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752358
[odata-query]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752356
[count-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$top=2%26$count=true&method=GET&version=v1.0
[expand-example]: https://developer.microsoft.com/graph/graph-explorer?request=groups$expand=members&method=GET&version=v1.0
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

