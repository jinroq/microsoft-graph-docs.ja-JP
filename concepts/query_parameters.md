# <a name="use-query-parameters-to-customize-responses"></a><span data-ttu-id="9986e-101">クエリ パラメーターを使用して応答をカスタマイズする</span><span class="sxs-lookup"><span data-stu-id="9986e-101">Use query parameters to customize responses</span></span>

<span data-ttu-id="9986e-p101">Microsoft Graph にはオプションのクエリ パラメーターがあり、応答で返されるデータの量を指定したり制御したりするために使用できます。次のクエリ パラメーターがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="9986e-p101">Microsoft Graph provides optional query parameters that you can use to specify and control the amount of data returned in a response. The following query parameters are supported.</span></span>

><span data-ttu-id="9986e-104">**注:**例をクリックして [Graph エクスプローラー][graph-explorer]で試行します。</span><span class="sxs-lookup"><span data-stu-id="9986e-104">**Note:** Click the examples to try them in [Graph Explorer][graph-explorer].</span></span>

|<span data-ttu-id="9986e-105">名前</span><span class="sxs-lookup"><span data-stu-id="9986e-105">Name</span></span>|<span data-ttu-id="9986e-106">説明</span><span class="sxs-lookup"><span data-stu-id="9986e-106">Description</span></span>|<span data-ttu-id="9986e-107">例</span><span class="sxs-lookup"><span data-stu-id="9986e-107">Example</span></span>|
|:---------------|:--------|:-------|
|[<span data-ttu-id="9986e-108">$count</span><span class="sxs-lookup"><span data-stu-id="9986e-108">$count</span></span>](#count)|<span data-ttu-id="9986e-109">一致するリソースの総数を取得します。</span><span class="sxs-lookup"><span data-stu-id="9986e-109">Retrieves the total count of matching resources.</span></span>|[`/me/messages?$top=2&$count=true`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$top=2%26$count=true&method=GET&version=v1.0)
|[<span data-ttu-id="9986e-110">$expand</span><span class="sxs-lookup"><span data-stu-id="9986e-110">$expand</span></span>](#expand)|<span data-ttu-id="9986e-111">関連リソースを取得します。</span><span class="sxs-lookup"><span data-stu-id="9986e-111">Retrieves related resources.</span></span>|[`/groups?$expand=members`](https://developer.microsoft.com/graph/graph-explorer?request=groups$expand=members&method=GET&version=v1.0)
|[<span data-ttu-id="9986e-112">$filter</span><span class="sxs-lookup"><span data-stu-id="9986e-112">$filter</span></span>](#filter)|<span data-ttu-id="9986e-113">結果 (行) をフィルターします。</span><span class="sxs-lookup"><span data-stu-id="9986e-113">Filters results (rows).</span></span>|[`/users?$filter=startswith(givenName,'J')`](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0)
|[<span data-ttu-id="9986e-114">$orderby</span><span class="sxs-lookup"><span data-stu-id="9986e-114">$orderby</span></span>](#orderby)|<span data-ttu-id="9986e-115">結果を並べます。</span><span class="sxs-lookup"><span data-stu-id="9986e-115">Orders results.</span></span>|[`/users?$orderby=displayName desc`](https://developer.microsoft.com/graph/graph-explorer?request=users?$orderby=displayName%20DESC&method=GET&version=v1.0)
|[<span data-ttu-id="9986e-116">$search</span><span class="sxs-lookup"><span data-stu-id="9986e-116">$search</span></span>](#search)| <span data-ttu-id="9986e-p102">検索条件に基づいて結果を返します。現在、`messages` と `person` のコレクションでサポートされています。</span><span class="sxs-lookup"><span data-stu-id="9986e-p102">Returns results based on search criteria. Currently supported on `messages` and `person` collections.</span></span>|[`/me/messages?$search=pizza`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=pizza&method=GET&version=v1.0)
|[<span data-ttu-id="9986e-119">$select</span><span class="sxs-lookup"><span data-stu-id="9986e-119">$select</span></span>](#select)|<span data-ttu-id="9986e-120">プロパティ (列) をフィルターします。</span><span class="sxs-lookup"><span data-stu-id="9986e-120">Filters properties (columns).</span></span>|[`/users?$select=givenName,surname`](https://developer.microsoft.com/graph/graph-explorer?request=users?$select=givenName,surname&method=GET&version=v1.0)
|[<span data-ttu-id="9986e-121">$skip</span><span class="sxs-lookup"><span data-stu-id="9986e-121">$skip</span></span>](#skip)|<span data-ttu-id="9986e-p103">結果セットにインデックスを作成します。また一部の API でページングを実装するために使用されており、`$top` と組み合わせて結果を手動でページングすることもできます。</span><span class="sxs-lookup"><span data-stu-id="9986e-p103">Indexes into a result set. Also used by some APIs to implement paging and can be used together with `$top` to manually page results.</span></span>  | [`/me/messages?$skip=11`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$skip=11&method=GET&version=v1.0)
|[<span data-ttu-id="9986e-124">$skipToken</span><span class="sxs-lookup"><span data-stu-id="9986e-124">$skipToken</span></span>](#skiptoken)|<span data-ttu-id="9986e-p104">複数ページにわたる結果セットから、結果の次のページを取得します。(一部の API では代わりに `$skip` を使用します。)</span><span class="sxs-lookup"><span data-stu-id="9986e-p104">Retrieves the next page of results from result sets that span multiple pages. (Some APIs use `$skip` instead.)</span></span> | `https://graph.microsoft.com/v1.0/users?$skiptoken=X%274453707402000100000017 ... 65612D643839392D343230372D613033662D306332623836633432363932B900000000000000000000%27`
|[<span data-ttu-id="9986e-127">$top</span><span class="sxs-lookup"><span data-stu-id="9986e-127">$top</span></span>](#top)|<span data-ttu-id="9986e-128">結果のページ サイズを設定します。</span><span class="sxs-lookup"><span data-stu-id="9986e-128">Sets the page size of results.</span></span> |[`/users?$top=2`](https://developer.microsoft.com/graph/graph-explorer?request=users?$top=2&method=GET&version=v1.0)

<span data-ttu-id="9986e-129">これらのパラメーターは、[OData V4 クエリ言語][odata-query]と互換性があります。</span><span class="sxs-lookup"><span data-stu-id="9986e-129">These parameters are compatible with the [OData V4 query language][odata-query].</span></span> <span data-ttu-id="9986e-130">すべての Microsoft Graph API で全部のパラメーターがサポートされているわけではなく、`v1.0` エンドポイントと `beta` エンドポイントの間でサポートが大幅に異なる場合があります。</span><span class="sxs-lookup"><span data-stu-id="9986e-130">These parameters are compatible with the OData V4 query language. Not all parameters are supported across all Microsoft Graph APIs and support may differ significantly between the `v1.0` and `beta` endpoints.</span></span> 

> <span data-ttu-id="9986e-p106">**注:**`beta` エンドポイントでは、`$` プレフィックスはオプションです。たとえば、`$filter` の代わりに、`filter` を使用しても同じです。詳細および例については、「[Microsoft Graph における $ プレフィックスのないクエリ パラメーターのサポート](http://dev.office.com/queryparametersinMicrosoftGraph)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9986e-p106">**Note:** On the `beta` endpoint, the `$` prefix is optional. For example, instead of `$filter`, you can use `filter`. For more details and examples, see [Supporting query parameters without $ prefixes in Microsoft Graph](http://dev.office.com/queryparametersinMicrosoftGraph).</span></span>

## <a name="encoding-query-parameters"></a><span data-ttu-id="9986e-134">クエリ パラメーターのエンコード</span><span class="sxs-lookup"><span data-stu-id="9986e-134">Encoding query parameters</span></span>

<span data-ttu-id="9986e-135">クエリ パラメーターの値はパーセント エンコードされる必要があります。</span><span class="sxs-lookup"><span data-stu-id="9986e-135">The values of query parameters should be percent-encoded.</span></span> <span data-ttu-id="9986e-136">これを行ううえで役立つ HTTP クライアント、ブラウザー、およびツールが多くあります ([Graph エクスプローラー][graph-explorer]など)。</span><span class="sxs-lookup"><span data-stu-id="9986e-136">Many HTTP clients, browsers, and tools (such as the [Graph Explorer][graph-explorer]) will help you with this.</span></span> <span data-ttu-id="9986e-137">クエリが失敗する場合、クエリ パラメーターの値が適切にエンコードされていないことがその原因の 1 つとして考えられます。</span><span class="sxs-lookup"><span data-stu-id="9986e-137">If a query is failing, one possible cause is failure to encode the query parameter values appropriately.</span></span>

<span data-ttu-id="9986e-138">エンコードされていない URL は、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="9986e-138">An unencoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName, 'J')
```

<span data-ttu-id="9986e-139">正しくエンコードされている URL は、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="9986e-139">A properly encoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName%2C+'J')
```

## <a name="count"></a><span data-ttu-id="9986e-140">count</span><span class="sxs-lookup"><span data-stu-id="9986e-140">count</span></span>

<span data-ttu-id="9986e-141">`$count` クエリ パラメーターを使用し、Microsoft Graph から返されるデータ値のページにコレクション内の項目数の合計を含めます。</span><span class="sxs-lookup"><span data-stu-id="9986e-141">Use the `$count` query parameter to include a count of the total number of items in a collection alongside the page of data values returned from Microsoft Graph.</span></span> 

<span data-ttu-id="9986e-142">たとえば、次のような要求によって、現在のユーザーの `contacts` コレクションと、`@odata.count` プロパティ内の `contacts` コレクションのアイテム数の両方が返されます。</span><span class="sxs-lookup"><span data-stu-id="9986e-142">For example, the following request will return both the `contacts` collection of the current user, and the number of items in the `contacts` collection in the `@odata.count` property.</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

[<span data-ttu-id="9986e-143">Graph エクスプローラーで試す</span><span class="sxs-lookup"><span data-stu-id="9986e-143">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/contacts?$count=true&method=GET&version=v1.0)


><span data-ttu-id="9986e-144">**注:** `$count` は、[ユーザー](../api-reference/v1.0/resources/user.md)や[グループ](../api-reference/v1.0/resources/group.md)のコレクションのような、[`directoryObject`](../api-reference/v1.0/resources/directoryobject.md) から派生したリソースのコレクションに対してはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9986e-144">**Note:** `$count` is not supported for collections of resources that derive from [`directoryObject`](../api-reference/v1.0/resources/directoryobject.md) like collections of [user](../api-reference/v1.0/resources/user.md) or [group](../api-reference/v1.0/resources/group.md).</span></span>

## <a name="expand"></a><span data-ttu-id="9986e-145">expand</span><span class="sxs-lookup"><span data-stu-id="9986e-145">expand</span></span>

<span data-ttu-id="9986e-146">Microsoft Graph リソースの多くは、宣言されているリソースのプロパティと、他のリソースとのリレーションシップの両方を公開します。</span><span class="sxs-lookup"><span data-stu-id="9986e-146">Many Microsoft Graph resources expose both declared properties of the resource as well as its relationships with other resources.</span></span> <span data-ttu-id="9986e-147">これらのリレーションシップは、参照プロパティまたはナビゲーション プロパティとも呼ばれ、1 つのリソースまたはリソースのコレクションのいずれかを参照することができます。</span><span class="sxs-lookup"><span data-stu-id="9986e-147">These relationships are also called reference properties or navigation properties, and they can reference either a single resource or a collection of resources.</span></span> <span data-ttu-id="9986e-148">たとえば、ユーザーのメール フォルダー、マネージャー、直属の部下は、すべてリレーションシップとして公開されます。</span><span class="sxs-lookup"><span data-stu-id="9986e-148">For example, the mail folders, manager, and direct reports of a user are all exposed as relationships.</span></span> 

<span data-ttu-id="9986e-p109">通常、単一の要求では、リソースの複数のプロパティ、またはリソースのリレーションシップの 1 つのいずれかに対してクエリを実行できますが、両方は行えません。`$expand` クエリ文字列パラメーターを使用して、展開されているリソース、または単一のリレーションシップ (ナビゲーション プロパティ) で参照されているコレクションを結果に含めることができます。</span><span class="sxs-lookup"><span data-stu-id="9986e-p109">Normally, you can query either the properties of a resource or one of its relationships in a single request, but not both. You can use the `$expand` query string parameter to include the expanded resource or collection referenced by a single relationship (navigation property) in your results.</span></span>

<span data-ttu-id="9986e-151">次の例では、ドライブ内のトップレベルの子項目と共に、ルート ドライブ情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="9986e-151">The following example gets root drive information along with the top level child items in a drive:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children
```

[<span data-ttu-id="9986e-152">Graph エクスプローラーで試す</span><span class="sxs-lookup"><span data-stu-id="9986e-152">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children&method=GET&version=v1.0)

<span data-ttu-id="9986e-p110">いくつかのリソース コレクションで、`$select` パラメーターを追加すれば、展開されたリソースで返されるプロパティを指定することもできます。次の使用例は前の例と同じクエリを実行しますが、[`$select`](#select) ステートメントを使用して、展開されている子項目に返されるプロパティを `id` プロパティと `name` プロパティに限定します。</span><span class="sxs-lookup"><span data-stu-id="9986e-p110">With some resource collections, you can also specify the properties to be returned in the expanded resources by adding a `$select` parameter. The following example performs the same query as the previous example but uses a [`$select`](#select) statement to limit the properties returned for the expanded child items to the `id` and `name` properties.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

<span data-ttu-id="9986e-155">[Graph エクスプローラーで試す](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children($select=id,name)&method=GET&version=v1.0)</span><span class="sxs-lookup"><span data-stu-id="9986e-155">[Try in Graph Explorer](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children($select=id,name)&method=GET&version=v1.0)</span></span>

> <span data-ttu-id="9986e-p111">**注:** すべてのリレーションシップとリソースで、`$expand` クエリ パラメーターがサポートされているわけではありません。たとえば、ユーザーの `directReports`、`manager`、`memberOf` の各リレーションシップを展開できますが、その `events`、`messages`、`photo` のリレーションシップは展開できません。すべてのリソースまたはリレーションシップで、`$select` を使用して展開されたアイテムがサポートされているわけではありません。</span><span class="sxs-lookup"><span data-stu-id="9986e-p111">**Note:** Not all relationships and resources support the `$expand` query parameter. For example, you can expand the `directReports`, `manager`, and `memberOf` relationships on a user, but you cannot expand its `events`, `messages`, or `photo` relationships. Not all resources or relationships support using `$select` on expanded items.</span></span> 
> 
> <span data-ttu-id="9986e-159">[ユーザー](../api-reference/v1.0/resources/user.md)や[グループ](../api-reference/v1.0/resources/group.md)のような、[directoryObject](../api-reference/v1.0/resources/directoryobject.md) から派生した Azure AD リソースの場合、`$expand` は `beta` でのみサポートされており、通常は展開されているリレーションシップに対し最大 20 個のアイテムを返すことができます。</span><span class="sxs-lookup"><span data-stu-id="9986e-159">With Azure AD resources that derive from [directoryObject](../api-reference/v1.0/resources/directoryobject.md), like [user](../api-reference/v1.0/resources/user.md) and [group](../api-reference/v1.0/resources/group.md), `$expand` is only supported for `beta` and  typically returns a maximum of 20 items for the expanded relationship.</span></span>

## <a name="filter"></a><span data-ttu-id="9986e-160">filter</span><span class="sxs-lookup"><span data-stu-id="9986e-160">filter</span></span>

<span data-ttu-id="9986e-161">`$filter` クエリ パラメーターを使用して、コレクションのサブセットのみを取得します。</span><span class="sxs-lookup"><span data-stu-id="9986e-161">Use the `$filter` query parameter to retrieve just a subset of a collection.</span></span> 

<span data-ttu-id="9986e-162">たとえば、表示名が「J」という文字で始まるユーザーを検索するには、`startswith` を使用します。</span><span class="sxs-lookup"><span data-stu-id="9986e-162">For example, to find users whose display name starts with the letter 'J', use `startswith`.</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'J')
```

<span data-ttu-id="9986e-163">[Graph エクスプローラーで試す](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0)</span><span class="sxs-lookup"><span data-stu-id="9986e-163">[Try in Graph Explorer](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0)</span></span>

<span data-ttu-id="9986e-164">`$filter` 演算子へのサポートは、お使いの Microsoft Graph API によって異なります。</span><span class="sxs-lookup"><span data-stu-id="9986e-164">Support for `$filter` operators varies across Microsoft Graph APIs.</span></span> <span data-ttu-id="9986e-165">通常、次の論理演算子がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="9986e-165">The following logical operators are generally supported:</span></span> 

- <span data-ttu-id="9986e-166">等しい (`eq`)</span><span class="sxs-lookup"><span data-stu-id="9986e-166">equals (`eq`)</span></span>
- <span data-ttu-id="9986e-167">等しくない (`ne`)</span><span class="sxs-lookup"><span data-stu-id="9986e-167">not equals (`ne`)</span></span>
- <span data-ttu-id="9986e-168">より大きい (`gt`)</span><span class="sxs-lookup"><span data-stu-id="9986e-168">Greater than (>`gt`)</span></span>
- <span data-ttu-id="9986e-169">以上 (`ge`)</span><span class="sxs-lookup"><span data-stu-id="9986e-169">greater than or equals (`ge`)</span></span>
- <span data-ttu-id="9986e-170">より小さい (`lt`)、以下 (`le`)</span><span class="sxs-lookup"><span data-stu-id="9986e-170">less than (`lt`), less than or equals (`le`)</span></span>
- <span data-ttu-id="9986e-171">AND (`and`)</span><span class="sxs-lookup"><span data-stu-id="9986e-171">and (`and`)</span></span>
- <span data-ttu-id="9986e-172">OR (`or`)</span><span class="sxs-lookup"><span data-stu-id="9986e-172">or -</span></span>
- <span data-ttu-id="9986e-173">NOT (`not`)</span><span class="sxs-lookup"><span data-stu-id="9986e-173">not (`not`)</span></span>
 
<span data-ttu-id="9986e-174">`startswith` 文字列の演算子はたいていサポートされています。</span><span class="sxs-lookup"><span data-stu-id="9986e-174">The `startswith` string operator is often supported.</span></span> <span data-ttu-id="9986e-175">`any` ラムダ演算子は、一部の API でサポートされています。</span><span class="sxs-lookup"><span data-stu-id="9986e-175">The `any` lambda operator is supported for some APIs.</span></span> <span data-ttu-id="9986e-176">いくつかの使用例について、次の表を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9986e-176">For some  usage examples, see the following table.</span></span> <span data-ttu-id="9986e-177">`$filter` 構文の詳細については、「[OData プロトコル][odata-filter]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9986e-177">For more details about `$filter` syntax, see the [OData protocol][odata-filter].</span></span>  

<span data-ttu-id="9986e-178">次の表では、`$filter` クエリ パラメーター使用例を示します。</span><span class="sxs-lookup"><span data-stu-id="9986e-178">The following table shows some examples using the `$filter` query parameter.</span></span>

><span data-ttu-id="9986e-179">**注:**例をクリックして [Graph エクスプローラー][graph-explorer]で試行します。</span><span class="sxs-lookup"><span data-stu-id="9986e-179">**Note:** Click the examples to try them in [Graph Explorer][graph-explorer].</span></span>

|<span data-ttu-id="9986e-180">説明</span><span class="sxs-lookup"><span data-stu-id="9986e-180">Description</span></span>|<span data-ttu-id="9986e-181">例</span><span class="sxs-lookup"><span data-stu-id="9986e-181">Example</span></span>|
|:--------|:-------|
|  <span data-ttu-id="9986e-182">複数のプロパティ間で Mary という名前を持つユーザーを検索します。</span><span class="sxs-lookup"><span data-stu-id="9986e-182">Search for users with the name Mary across multiple properties.</span></span> | [`https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'mary') or startswith(givenName,'mary') or startswith(surname,'mary') or startswith(mail,'mary') or startswith(userPrincipalName,'mary')`](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(displayName,'mary')+or+startswith(givenName,'mary')+or+startswith(surname,'mary')+or+startswith(mail,'mary')+or+startswith(userPrincipalName,'mary')&method=GET&version=v1.0) |
| <span data-ttu-id="9986e-183">2017 年 7 月 1 日以降に開始する、サインイン ユーザーのイベントすべてを取得します。</span><span class="sxs-lookup"><span data-stu-id="9986e-183">Get all of the signed-in user's events that start after 7/1/2017.</span></span> | [`https://graph.microsoft.com/v1.0/me/events?$filter=start/dateTime ge '2017-07-01T08:00'`](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$filter=start/dateTime+ge+'2017-07-01T08:00'&method=GET&version=v1.0) |
| <span data-ttu-id="9986e-184">サインイン ユーザーが受信した特定のアドレスからの電子メールすべてを取得します。</span><span class="sxs-lookup"><span data-stu-id="9986e-184">Get all emails from a specific address received by the signed-in user.</span></span> | [`https://graph.microsoft.com/v1.0/me/messages?$filter=from/emailAddress/address eq 'someuser@example.com'`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=from/emailAddress/address+eq+'someuser@.com'&method=GET&version=v1.0) |
| <span data-ttu-id="9986e-185">2017 年 4 月にサインイン ユーザーが受信した電子メールすべてを取得します。</span><span class="sxs-lookup"><span data-stu-id="9986e-185">Get all emails received by the signed-in user in April 2017</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=ReceivedDateTime ge 2017-04-01 and receivedDateTime lt 2017-05-01`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=ReceivedDateTime+ge+2017-04-01+and+receivedDateTime+lt+2017-05-01&method=GET&version=v1.0) |
| <span data-ttu-id="9986e-186">サインイン ユーザーの受信トレイから未読メールをすべて取得します。</span><span class="sxs-lookup"><span data-stu-id="9986e-186">Get all unread mails in the signed-in user's Inbox.</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=isRead eq false`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=isRead+eq+false&method=GET&version=v1.0) |
| <span data-ttu-id="9986e-187">組織内のすべての Office 365 グループの一覧</span><span class="sxs-lookup"><span data-stu-id="9986e-187">List all Office 365 groups in an organization</span></span> | [`https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')`](https://developer.microsoft.com/graph/graph-explorer?request=groups?$filter=groupTypes/any(c:c+eq+'Unified')&method=GET&version=v1.0) |

> <span data-ttu-id="9986e-p114">**注:** Azure AD リソースでは、次の `$filter` 演算子はサポートされていません: `ne`、`gt`、`ge`、`lt`、`le`、`not`。Microsoft Graph リソースでは現在、`contains` 文字列の演算子はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9986e-p114">**Note:** The following `$filter` operators are not supported for Azure AD resources:  `ne`, `gt`, `ge`, `lt`, `le`, and `not`. The `contains` string operator is currently not supported on any Microsoft Graph resources.</span></span>

## <a name="orderby"></a><span data-ttu-id="9986e-190">orderby</span><span class="sxs-lookup"><span data-stu-id="9986e-190">orderby</span></span>

<span data-ttu-id="9986e-191">`$orderby` クエリ パラメーターを使用して、Microsof Graph から返される項目の並べ替え順序を指定します。</span><span class="sxs-lookup"><span data-stu-id="9986e-191">Use the `$orderby` query parameter to specify the sort order of the items returned from Microsoft Graph.</span></span>

<span data-ttu-id="9986e-192">たとえば、次の要求では組織のユーザーが表示名順で返されます。</span><span class="sxs-lookup"><span data-stu-id="9986e-192">For example, the following request returns the users in the organization ordered by their display name:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```
[<span data-ttu-id="9986e-193">Graph エクスプローラーで試す</span><span class="sxs-lookup"><span data-stu-id="9986e-193">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=users?$orderby=displayName&method=GET&version=v1.0)

<span data-ttu-id="9986e-p115">複合型のエンティティでも並べ替えが可能です。次の要求では、メッセージを取得し、それらを `emailAddress` という複合型である `from` プロパティの `address` フィールドで並べ替えます。</span><span class="sxs-lookup"><span data-stu-id="9986e-p115">You can also sort by complex type entities. The following request gets messages and sorts them by the `address` field of the `from` property, which is of the complex type `emailAddress`:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
```
[<span data-ttu-id="9986e-196">Graph エクスプローラーで試す</span><span class="sxs-lookup"><span data-stu-id="9986e-196">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/address&method=GET&version=v1.0)

<span data-ttu-id="9986e-197">昇順または降順で結果を並べ替えるには、`asc` または `desc` のいずれかをスペースで区切ってフィールド名の後に追加します。たとえば `?$orderby=name%20desc` のようにします。</span><span class="sxs-lookup"><span data-stu-id="9986e-197">To sort the results in ascending or descending order, append either `asc` or `desc` to the field name, separated by a space, for example, `?$orderby=name%20desc`.</span></span>

<span data-ttu-id="9986e-198">一部の API では、複数のプロパティの結果を並べ替えることができます。</span><span class="sxs-lookup"><span data-stu-id="9986e-198">With some APIs, you can order results on multiple properties.</span></span> <span data-ttu-id="9986e-199">たとえば、次のような要求ではユーザーの受信トレイ内のメッセージを、最初は送信者の名前で降順に並べ替え (Z から A)、次に件名で昇順 (既定) に並べ替えます。</span><span class="sxs-lookup"><span data-stu-id="9986e-199">With some APIs, you can order results on multiple properties. For example, the following request orders the messages in the user's Inbox first by the name of the person who sent it in descending order (Z to A) and then by subject in ascending order (default).</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/Inbox/messages?$orderby=from/emailAddress/name desc,subject
```
[<span data-ttu-id="9986e-200">Graph エクスプローラーで試す</span><span class="sxs-lookup"><span data-stu-id="9986e-200">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/name%20desc,subject&method=GET&version=v1.0)


 > <span data-ttu-id="9986e-201">**注:** [ユーザー](../api-reference/v1.0/resources/user.md)や[グループ](../api-reference/v1.0/resources/group.md)のような、[directoryObject](../api-reference/v1.0/resources/directoryobject.md) から派生した Azure AD リソースの場合、`$orderby` 式と `$filter` 式を結合することはできません。</span><span class="sxs-lookup"><span data-stu-id="9986e-201">**Note:** With Azure AD resources that derive from [directoryObject](../api-reference/v1.0/resources/directoryobject.md), like [user](../api-reference/v1.0/resources/user.md) and [group](../api-reference/v1.0/resources/group.md), you cannot combine `$orderby` with `$filter` expressions.</span></span> 

## <a name="search"></a><span data-ttu-id="9986e-202">検索</span><span class="sxs-lookup"><span data-stu-id="9986e-202">search</span></span>

<span data-ttu-id="9986e-203">`$search` クエリ パラメーターを使用して、要求の結果を検索条件と一致するものに制限します。</span><span class="sxs-lookup"><span data-stu-id="9986e-203">Use the `$search` query parameter to restrict the results of a request to match a search criterion.</span></span>

> <span data-ttu-id="9986e-p117">**注:** 現在の検索対象は、[メッセージ](../api-reference/v1.0/resources/message.md) コレクションと[人物](../api-reference/v1.0/resources/person.md)コレクション**だけ**です。`$search` 要求は最大 250 まで結果を返します。検索要求では [`$filter`](#filter) も [`$orderby`](#orderby) も使用できません。</span><span class="sxs-lookup"><span data-stu-id="9986e-p117">**Note:** You can currently search **only** [message](../api-reference/v1.0/resources/message.md) and [person](../api-reference/v1.0/resources/person.md) collections. A `$search` request returns up to 250 results. You cannot use [`$filter`](#filter) or [`$orderby`](#orderby) in a search request.</span></span>

### <a name="using-search-on-message-collections"></a><span data-ttu-id="9986e-207">`message` コレクションで $Search を使用する</span><span class="sxs-lookup"><span data-stu-id="9986e-207">Using $search on `message` collections</span></span>

<span data-ttu-id="9986e-p118">メッセージの検索条件は、[高度な検索テクニック (AQS)](https://support.office.com/article/Search-Mail-and-People-in-Outlook-com-and-Outlook-on-the-web-for-business-88108edf-028e-4306-b87e-7400bbb40aa7) を使用して表現されます。結果は、メッセージが送信された日時で並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="9986e-p118">Search criteria on messages are expressed using [Advanced Query Syntax (AQS)](https://support.office.com/article/Search-Mail-and-People-in-Outlook-com-and-Outlook-on-the-web-for-business-88108edf-028e-4306-b87e-7400bbb40aa7). The results are sorted by the date and time that the message was sent.</span></span>

<span data-ttu-id="9986e-210">`$search` で `message` に対する次のプロパティを指定できます:</span><span class="sxs-lookup"><span data-stu-id="9986e-210">You can specify the following properties on a `message` in a `$search` criterion: , , , , , , , , , , , , </span></span>

- `attachments`
- `bccRecipients`
- `body`
- `category`
- `ccRecipients`
- `content`
- `from`
- `hasAttachments`
- `participants`
- `receivedDateTime`
- `sender`
- `subject`
- `toRecipients`

<span data-ttu-id="9986e-211">メッセージで検索を行うときに値のみ指定した場合、検索は既定の検索プロパティである `from`、`subject` および `body` に基づいて行われます。</span><span class="sxs-lookup"><span data-stu-id="9986e-211">If you do a search on messages and specify only a value, the search is carried out on the default search properties of `from`, `subject` and `body`.</span></span>

<span data-ttu-id="9986e-212">次の例は、サインイン中のユーザーの受信トレイにあるメッセージのうち、既定の 3 つの検索プロパティのいずれかに "pizza" が含まれるメッセージをすべて返します。</span><span class="sxs-lookup"><span data-stu-id="9986e-212">The following example returns all messages in the signed-in user's Inbox that contains "pizza" in any of the three default search properties:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

<span data-ttu-id="9986e-213">次の例は、ユーザーの受信トレイにあるメッセージのうち、特定のメール アドレスから送信されたメッセージをすべて検索します。</span><span class="sxs-lookup"><span data-stu-id="9986e-213">The next example searches all messages in the user's Inbox that were sent from a specific email address:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="from:help@contoso.com"
```

### <a name="using-search-on-person-collections"></a><span data-ttu-id="9986e-214">`person` コレクションで $Search を使用する</span><span class="sxs-lookup"><span data-stu-id="9986e-214">Using $search on `person` collections</span></span>

<span data-ttu-id="9986e-p119">Microsoft Graph People API を使用してユーザーに最も関連のある人物を取得できます。関連性は、ユーザーのコミュニケーションとコラボレーション パターン、およびビジネスのリレーションシップによって決定されます。People API では、`$search` クエリ パラメーターがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="9986e-p119">You can use the Microsoft Graph People API to retrieve the people who are most relevant to a user. Relevance is determined by the user’s communication and collaboration patterns and business relationships. The People API supports the `$search` query parameter.</span></span>

<span data-ttu-id="9986e-p120">[人物](../api-reference/v1.0/resources/person.md)リソースの `displayName` プロパティと `emailAddress` プロパティの両方で人物の検索を行います。検索は、あいまい一致のアルゴリズムを実装します。これにより、完全に一致する項目と、検索目的の推論に基づく結果が返されます。たとえば、サインイン ユーザーの `people` コレクション内で、"Tyler Lee" の表示名および tylerle@example.com というメール アドレスを持つユーザーを想定してください。次の検索はすべて、Tyler を含む検索結果を返します。</span><span class="sxs-lookup"><span data-stu-id="9986e-p120">Searches on people occur on both the `displayName` and `emailAddress` properties of the [person](../api-reference/v1.0/resources/person.md) resource. Searches implement a fuzzy matching algorithm. They will return results based on an exact match and also on inferences about the intent of the search. For example, imagine a user with a display name of "Tyler Lee" and an email address of tylerle@example.com who is in the `people` collection of the signed-in user. All of the following searches will return results that contain Tyler.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people?$search=tyler                //matches both Tyler's name and email
GET https://graph.microsoft.com/v1.0/me/people?$search=tylerle              //matches Tyler's email
GET https://graph.microsoft.com/v1.0/me/people?$search="tylerle@example.com"  //matches Tyler's email. Note the quotes to enclose '@'.
GET https://graph.microsoft.com/v1.0/me/people?$search=tiler                //fuzzy match with Tyler's name 
GET https://graph.microsoft.com/v1.0/me/people?$search="tyler lee"          //matches Tyler's name. Note the quotes to enclose the space.
```

<span data-ttu-id="9986e-p121">特定のトピックに興味のある人物の検索を実行することもできます。ユーザーのメールのスレッドから引き出した推測に基づいて検索を実行します。たとえば、次の検索は、サインイン ユーザーに関連のある人物のうち、そのユーザーとの通信の中でピザに興味を示した人のコレクションを返します。検索語句を引用符で囲んでいることに注目してください。</span><span class="sxs-lookup"><span data-stu-id="9986e-p121">You can also perform searches for people who are interested in a particular topic. Searches are performed based on inferences derived from the user's mail conversations. For example, the following search will return a collection of people relevant to the signed-in user who have expressed an interest in pizza in communications with that user. Note that the search phrase is enclosed in quotes.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="topic:pizza"                
```

<span data-ttu-id="9986e-227">最後に、2 種類の検索式を組み合わせることによって、同じ要求内に人の検索とトピックの検索の両方をまとめることができます。</span><span class="sxs-lookup"><span data-stu-id="9986e-227">Finally, you can combine both people searches and topic searches in the same request by combining the two types of search expression.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="tyl topic:pizza"                
```
<span data-ttu-id="9986e-228">この要求は本質的には 2 つの検索を行います。サインイン ユーザーに関連する人物の `displayName` プロパティと `emailAddress` プロパティに対するあいまい検索、そしてユーザーに関連する人物に対する「ピザ」というトピックの検索です。</span><span class="sxs-lookup"><span data-stu-id="9986e-228">This request essentially conducts two searches: a fuzzy search against `displayName` and `emailAddress` properties of the signed-in user's relevant people and a topic search for "pizza" against the user's relevant people. The results are then ranked, ordered, and returned. Note that the search is not restrictive; you may get results that contain people that fuzzy match "tyl", or that are interested in "pizza", or both.</span></span> <span data-ttu-id="9986e-229">次いで結果をランク付けし、並べ替え、返します。</span><span class="sxs-lookup"><span data-stu-id="9986e-229">The results are then ranked, ordered, and returned.</span></span> <span data-ttu-id="9986e-230">この検索は制限的ではありません。「tyl」とあいまい一致する人物、「ピザ」に関心を示す人物、または両方の結果を取得する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="9986e-230">Note that the search is not restrictive; you might get results that contain people that fuzzy match "tyl", or that are interested in "pizza", or both.</span></span>

<span data-ttu-id="9986e-231">People API についてもっと知るには、「[関係する人の情報を取得する](./people_example.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9986e-231">To learn more about the People API, see [Get information about relevant people](./people_example.md).</span></span>  

## <a name="select"></a><span data-ttu-id="9986e-232">select</span><span class="sxs-lookup"><span data-stu-id="9986e-232">select</span></span>

<span data-ttu-id="9986e-233">`$select` クエリ パラメーターを使用して、個別リソースまたはリソースのコレクションの既定値とは異なるプロパティのセットを返します。</span><span class="sxs-lookup"><span data-stu-id="9986e-233">Use the `$select` query parameter to return a set of properties different than the default set for an individual resource or a collection of resources. With $select you can specify a subset or a superset of the default properties.</span></span> <span data-ttu-id="9986e-234">$Select で、既定のプロパティのサブセットまたはスーパー セットを指定できます。</span><span class="sxs-lookup"><span data-stu-id="9986e-234">With $select, you can specify a subset or a superset of the default properties.</span></span>

<span data-ttu-id="9986e-235">たとえば、サインイン ユーザーのメッセージを取得するとき、`from` プロパティと `subject` プロパティだけを返すよう指定できます。</span><span class="sxs-lookup"><span data-stu-id="9986e-235">For example, when retrieving the messages of the signed-in user, you can specify that only the `from` and `subject` properties be returned:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

[<span data-ttu-id="9986e-236">Graph エクスプローラーで試す</span><span class="sxs-lookup"><span data-stu-id="9986e-236">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$select=from,subject&method=GET&version=v1.0)

> <span data-ttu-id="9986e-237">**重要:**通常は、`$select` を使用して、クエリから返されるプロパティをお使いのアプリで必要なものだけに制限することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="9986e-237">**Important:** In general, we recommend that you use `$select` to limit the properties returned by a query to those needed by your app.</span></span> <span data-ttu-id="9986e-238">これは特に、クエリが大きな結果セットを返す可能性がある場合に該当します。</span><span class="sxs-lookup"><span data-stu-id="9986e-238">This is especially true of queries that might potentially return a large result set.</span></span> <span data-ttu-id="9986e-239">行ごとに返されるプロパティを制限すれば、ネットワークの負荷を軽減し、アプリのパフォーマンスを向上させることができます。</span><span class="sxs-lookup"><span data-stu-id="9986e-239">Limiting the properties returned in each row will reduce network load and help improve your app's performance.</span></span>
>
> <span data-ttu-id="9986e-p125">`v1.0`では、[ユーザー](../api-reference/v1.0/resources/user.md)と[グループ](../api-reference/v1.0/resources/group.md)のような、[directoryObject](../api-reference/v1.0/resources/directoryobject.md) から派生した一部の Azure AD リソースは、読み取り時に制限された既定値のプロパティ サブセットを返します。既定のセット以外のプロパティを返すには、これらのリソースに対して `$select` を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9986e-p125">In `v1.0`, some Azure AD resources that derive from [directoryObject](../api-reference/v1.0/resources/directoryobject.md), like [user](../api-reference/v1.0/resources/user.md) and [group](../api-reference/v1.0/resources/group.md), return a limited, default subset of properties on reads. For these resources, you must use `$select` to return properties outside of the default set.</span></span>  

## <a name="skip"></a><span data-ttu-id="9986e-242">skip</span><span class="sxs-lookup"><span data-stu-id="9986e-242">skip</span></span>

<span data-ttu-id="9986e-p126">コレクションを開始するときにスキップする項目数を設定するには、`$skip` クエリ パラメーターを使用します。たとえば、次の要求はユーザーのイベントを、コレクション内の 21 番目以降のイベントから作成日順で返します。</span><span class="sxs-lookup"><span data-stu-id="9986e-p126">Use the `$skip` query parameter to set the number of items to skip at the start of a collection. For example, the following request returns events for the user sorted by date created, starting with the 21st event in the collection:</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```
[<span data-ttu-id="9986e-245">Graph エクスプローラーで試す</span><span class="sxs-lookup"><span data-stu-id="9986e-245">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$orderby=createdDateTime&$skip=20&method=GET&version=v1.0)

> <span data-ttu-id="9986e-246">**注:**Outlook メール/カレンダーなどいくつかの Microsoft Graph API (`message`、`event`、`calendar`) は、`$skip` を使用してページングを実装します。</span><span class="sxs-lookup"><span data-stu-id="9986e-246">**Note:** Some Microsoft Graph APIs, like Outlook Mail and Calendars (`message`, `event`, and `calendar`), use `$skip` to implement paging.</span></span> <span data-ttu-id="9986e-247">クエリの結果が複数ページにまたがる場合、これらの API は `@odata:nextLink` プロパティと共に `$skip` パラメーターが含まれる URL を返します。</span><span class="sxs-lookup"><span data-stu-id="9986e-247">When results of a query span multiple pages, these APIs will return an `@odata:nextLink` property with a URL that contains a `$skip` parameter.</span></span> <span data-ttu-id="9986e-248">この URL を使用して、結果の次のページに戻れます。</span><span class="sxs-lookup"><span data-stu-id="9986e-248">You can use this URL to return the next page of results.</span></span> <span data-ttu-id="9986e-249">詳細については、「[ページング](./paging.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9986e-249">To learn more, see [Paging](./paging.md).</span></span>

## <a name="skiptoken"></a><span data-ttu-id="9986e-250">skipToken</span><span class="sxs-lookup"><span data-stu-id="9986e-250">skipToken</span></span>

<span data-ttu-id="9986e-p128">要求の中には、サーバー側のページングを使用したり、応答におけるページ サイズを限定するために [`$top`](#top) パラメーターを使用したりすることによって、複数のデータ ページを返すものがあります。Microsoft Graph API の多くは、`skipToken` クエリ パラメーターを使用して、結果の後続のページを参照します。`$skiptoken` パラメーターは、結果の次のページを参照する不透明トークンを含んでおり、応答の `@odata.nextLink` プロパティで指定される URL で返されます。詳細については、「[ページング](./paging.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9986e-p128">Some requests return multiple pages of data either due to server-side paging or due to the use of the [`$top`](#top) parameter to limit the page size of the response. Many Microsoft Graph APIs use the `skipToken` query parameter to reference subsequent pages of the result. The `$skiptoken` parameter contains an opaque token that references the next page of results and is returned in the URL provided in the `@odata.nextLink` property in the response. To learn more, see [Paging](./paging.md).</span></span>


## <a name="top"></a><span data-ttu-id="9986e-255">top</span><span class="sxs-lookup"><span data-stu-id="9986e-255">top</span></span>

<span data-ttu-id="9986e-256">`$top` クエリ パラメーターを使用して、結果セットのページ サイズを指定します。</span><span class="sxs-lookup"><span data-stu-id="9986e-256">Use the `$top` query parameter to specify the page size of the result set.</span></span> 

<span data-ttu-id="9986e-257">結果セットにさらに項目が残っている場合、応答本文に `@odata.nextLink` パラメーターが含まれます。</span><span class="sxs-lookup"><span data-stu-id="9986e-257">If more items remain in the result set, the response body will contain an `@odata.nextLink` parameter.</span></span> <span data-ttu-id="9986e-258">このパラメーターには、結果の次のページを取得するために使用できる URL が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9986e-258">If there are more items remaining in the result set, the response body will contain an  parameter. This parameter contains a URL that you can use to get the next page of results. To learn more, see Paging.</span></span> <span data-ttu-id="9986e-259">詳細については、「[ページング](./paging.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9986e-259">To learn more, see [Paging](./paging.md).</span></span> 

<span data-ttu-id="9986e-260">たとえば、次の要求はユーザーのメールボックスの最初の 5 つのメッセージを返します。</span><span class="sxs-lookup"><span data-stu-id="9986e-260">For example, the following request returns the first five messages in the user's mailbox:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```

[<span data-ttu-id="9986e-261">Graph エクスプローラーで試す</span><span class="sxs-lookup"><span data-stu-id="9986e-261">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$top=5&method=GET&version=v1.0)


## <a name="error-handling-for-query-parameters"></a><span data-ttu-id="9986e-262">クエリ パラメーターのエラー処理</span><span class="sxs-lookup"><span data-stu-id="9986e-262">Error handling for query parameters</span></span>

<span data-ttu-id="9986e-p130">指定されたクエリ パラメーターがサポートされていない場合、一部の要求はエラー メッセージを返します。たとえば、`$expand` を `user/photo` のリレーションシップで使用することはできません。</span><span class="sxs-lookup"><span data-stu-id="9986e-p130">Some requests will return an error message if a specified query parameter is not supported. For example, you cannot use `$expand` on the `user/photo` relationship.</span></span> 

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

<span data-ttu-id="9986e-265">ただし、要求で指定されたクエリ パラメーターが警告なしで失敗する可能性があるため、注意が必要です。</span><span class="sxs-lookup"><span data-stu-id="9986e-265">However, it is important to note that query parameters specified in a request might fail silently.</span></span> <span data-ttu-id="9986e-266">これは、クエリ パラメーターがサポートされていない場合や、クエリ パラメーターの組み合わせがサポートされていない場合に起こり得ます。</span><span class="sxs-lookup"><span data-stu-id="9986e-266">This can be true for unsupported query parameters as well as for unsupported combinations of query parameters.</span></span> <span data-ttu-id="9986e-267">その場合、要求によって返されたデータを調べ、指定したクエリ パラメーターに期待どおりの効果があったかどうかを確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9986e-267">However, it is important to note that query parameters specified in a request may fail silently. This can be true for unsupported query parameters as well as for unsupported combinations of query parameters. In these cases, you should examine the data returned by the request to determine whether the query parameters you specified had the desired effect.</span></span> 

[graph-explorer]: https://developer.microsoft.com/graph/graph-explorer
[odata-filter]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752358
[odata-query]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752356