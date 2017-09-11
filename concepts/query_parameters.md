# <a name="use-query-parameters-to-customize-responses"></a><span data-ttu-id="c7730-101">クエリ パラメーターを使用して応答をカスタマイズする</span><span class="sxs-lookup"><span data-stu-id="c7730-101">Use query parameters to customize responses</span></span>

<span data-ttu-id="c7730-p101">Microsoft Graph にはオプションのクエリ パラメーターがあり、応答で返されるデータの量を指定したり制御したりするために使用できます。次のクエリ パラメーターがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="c7730-p101">Microsoft Graph provides optional query parameters that you can use to specify and control the amount of data returned in a response. The following following query parameters are supported.</span></span>

|<span data-ttu-id="c7730-104">名前</span><span class="sxs-lookup"><span data-stu-id="c7730-104">Name</span></span>|<span data-ttu-id="c7730-105">説明</span><span class="sxs-lookup"><span data-stu-id="c7730-105">Description</span></span>|<span data-ttu-id="c7730-106">例 (例をクリックして [Graph エクスプローラー][graph-explorer]で試行します)</span><span class="sxs-lookup"><span data-stu-id="c7730-106">Example (click examples to try in [Graph Explorer][graph-explorer])</span></span>
|:---------------|:--------|:-------|
|[<span data-ttu-id="c7730-107">$count</span><span class="sxs-lookup"><span data-stu-id="c7730-107">$count</span></span>](#count)|<span data-ttu-id="c7730-108">一致するリソースの総数を取得します。</span><span class="sxs-lookup"><span data-stu-id="c7730-108">Retrieves the total count of matching resources.</span></span>|[`/me/messages?$top=2&$count=true`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$top=2%26$count=true&method=GET&version=v1.0)
|[<span data-ttu-id="c7730-109">$expand</span><span class="sxs-lookup"><span data-stu-id="c7730-109">$expand</span></span>](#expand)|<span data-ttu-id="c7730-110">関連リソースを取得します。</span><span class="sxs-lookup"><span data-stu-id="c7730-110">Retrieves related resources.</span></span>|[`/groups?$expand=members`](https://developer.microsoft.com/graph/graph-explorer?request=groups$expand=members&method=GET&version=v1.0)
|[<span data-ttu-id="c7730-111">$filter</span><span class="sxs-lookup"><span data-stu-id="c7730-111">$filter</span></span>](#filter)|<span data-ttu-id="c7730-112">結果 (行) をフィルターします。</span><span class="sxs-lookup"><span data-stu-id="c7730-112">Filters results (rows).</span></span>|[`/users?$filter=startswith(givenName,'J')`](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0)
|[<span data-ttu-id="c7730-113">$orderby</span><span class="sxs-lookup"><span data-stu-id="c7730-113">$orderby</span></span>](#orderby)|<span data-ttu-id="c7730-114">結果を並べます。</span><span class="sxs-lookup"><span data-stu-id="c7730-114">Orders results.</span></span>|[`/users?$orderby=displayName desc`](https://developer.microsoft.com/graph/graph-explorer?request=users?$orderby=displayName%20DESC&method=GET&version=v1.0)
|[<span data-ttu-id="c7730-115">$search</span><span class="sxs-lookup"><span data-stu-id="c7730-115">Search</span></span>](#search)| <span data-ttu-id="c7730-p102">検索条件に基づいて結果を返します。現在、`messages` と `person` のコレクションでサポートされています。</span><span class="sxs-lookup"><span data-stu-id="c7730-p102">Returns results based on search criteria. Currently supported on `messages` and `person` collections.</span></span>|[`/me/messages?$search=pizza`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=pizza&method=GET&version=v1.0)
|[<span data-ttu-id="c7730-118">$select</span><span class="sxs-lookup"><span data-stu-id="c7730-118">$select</span></span>](#select)|<span data-ttu-id="c7730-119">プロパティ (列) をフィルターします。</span><span class="sxs-lookup"><span data-stu-id="c7730-119">Filters properties (columns).</span></span>|[`/users?$select=givenName,surname`](https://developer.microsoft.com/graph/graph-explorer?request=users?$select=givenName,surname&method=GET&version=v1.0)
|[<span data-ttu-id="c7730-120">$skip</span><span class="sxs-lookup"><span data-stu-id="c7730-120">$skip</span></span>](#skip)|<span data-ttu-id="c7730-p103">結果セットにインデックスを作成します。また一部の API でページングを実装するために使用されており、`$top` と組み合わせて結果を手動でページングすることもできます。</span><span class="sxs-lookup"><span data-stu-id="c7730-p103">Indexes into a result set. Also used by some APIs to implement paging and can be used together with `$top` to manually page results.</span></span>  | [`/me/messages?$skip=11`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$skip=11&method=GET&version=v1.0)
|[<span data-ttu-id="c7730-123">$skipToken</span><span class="sxs-lookup"><span data-stu-id="c7730-123">$skipToken</span></span>](#skiptoken)|<span data-ttu-id="c7730-p104">複数ページにわたる結果セットから、結果の次のページを取得します。(一部の API では代わりに `$skip` を使用します。)</span><span class="sxs-lookup"><span data-stu-id="c7730-p104">Retrieves the next page of results from result sets that span multiple pages. (Some APIs use `$skip` instead.)</span></span> | `https://graph.microsoft.com/v1.0/users?$skiptoken=X%274453707402000100000017 ... 65612D643839392D343230372D613033662D306332623836633432363932B900000000000000000000%27`
|[<span data-ttu-id="c7730-126">$top</span><span class="sxs-lookup"><span data-stu-id="c7730-126">$top</span></span>](#top)|<span data-ttu-id="c7730-127">結果のページ サイズを設定します。</span><span class="sxs-lookup"><span data-stu-id="c7730-127">Sets the page size of results.</span></span> |[`/users?$top=2`](https://developer.microsoft.com/graph/graph-explorer?request=users?$top=2&method=GET&version=v1.0)

<span data-ttu-id="c7730-p105">これらのパラメーターは、[OData V4 クエリ言語][odata-query]と互換性があります。すべての Microsoft Graph API で全部のパラメーターがサポートされているわけではなく、`v1.0` エンドポイントと `beta` エンドポイントの間でサポートが大幅に異なる場合があります。</span><span class="sxs-lookup"><span data-stu-id="c7730-p105">These parameters are compatible with the [OData V4 query language][odata-query]. Not all parameters are supported across all Microsoft Graph APIs and support may differ significantly between the `v1.0` and `beta` endpoints.</span></span> 

> <span data-ttu-id="c7730-p106">**注:**`beta` エンドポイントでは、`$` プレフィックスはオプションです。たとえば、`$filter` の代わりに、`filter` を使用しても同じです。詳細および例については、「[Microsoft Graph における $ プレフィックスのないクエリ パラメーターのサポート](http://dev.office.com/queryparametersinMicrosoftGraph)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c7730-p106">**Note:** On the `beta` endpoint, the `$` prefix is optional. For example, instead of `$filter`, you can use `filter`. For more details and examples, see [Supporting query parameters without $ prefixes in Microsoft Graph](http://dev.office.com/queryparametersinMicrosoftGraph).</span></span>

<span data-ttu-id="c7730-133">**クエリ パラメーターのエンコード:**</span><span class="sxs-lookup"><span data-stu-id="c7730-133">**Encoding query parameters:**</span></span>

<span data-ttu-id="c7730-p107">クエリ パラメーターの値はパーセント エンコードされる必要があります。これを行ううえで役立つ HTTP クライアント、ブラウザー、およびツールが多くあります (たとえば [Graph エクスプローラー][graph-explorer])。クエリが失敗する場合、クエリ パラメーターの値が適切にエンコードされていないことがその理由の 1 つとして考えられます。</span><span class="sxs-lookup"><span data-stu-id="c7730-p107">The values of query parameters should be percent-encoded. Many HTTP clients, browsers and tools (e.g., the [Graph Explorer][graph-explorer]) will help you with this. If a query is failing, one possible reason is failure to encode the values of query parameters appropriately.</span></span>

<span data-ttu-id="c7730-137">エンコードされていない URL は、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="c7730-137">An unencoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName, 'J')
```

<span data-ttu-id="c7730-138">正しくエンコードされている URL は、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="c7730-138">A properly encoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName%2C+'J')
```

## <a name="count"></a><span data-ttu-id="c7730-139">count</span><span class="sxs-lookup"><span data-stu-id="c7730-139">count</span></span>

<span data-ttu-id="c7730-140">`$count` クエリ パラメーターを使用し、Microsoft Graph から返されるデータ値のページにコレクション内の項目数の合計を含めます。</span><span class="sxs-lookup"><span data-stu-id="c7730-140">Use `$count` as a query parameter to include a count of the total number of items in a collection alongside the page of data values returned from the Graph, as in the following example:</span></span> 

<span data-ttu-id="c7730-141">たとえば、次のような要求によって、現在のユーザーの `contacts` コレクションと、`@odata.count` プロパティ内の `contacts` コレクションのアイテム数の両方が返されます。</span><span class="sxs-lookup"><span data-stu-id="c7730-141">For example, the following request will return both the `contacts` collection of the current user, and the number of items in the `contacts` collection in the `@odata.count` property.</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

[<span data-ttu-id="c7730-142">Graph エクスプローラーで試す</span><span class="sxs-lookup"><span data-stu-id="c7730-142">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/contacts?$count=true&method=GET&version=v1.0)


><span data-ttu-id="c7730-143">**注:** `$count` は、[ユーザー](../api-reference/v1.0/resources/user.md)や[グループ](../api-reference/v1.0/resources/group.md)のコレクションのような、[`directoryObject`](../api-reference/v1.0/resources/directoryobject.md) から派生したリソースのコレクションに対してはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c7730-143">**Note:** `$count` is not supported for collections of resources that derive from [`directoryObject`](../api-reference/v1.0/resources/directoryobject.md) like collections of [user](../api-reference/v1.0/resources/user.md) or [group](../api-reference/v1.0/resources/group.md).</span></span>

## <a name="expand"></a><span data-ttu-id="c7730-144">expand</span><span class="sxs-lookup"><span data-stu-id="c7730-144">expand</span></span>

<span data-ttu-id="c7730-p108">Microsoft Graph リソースの多くは、宣言されているリソースのプロパティと、他のリソースとのリレーションシップの両方を公開します。これらのリレーションシップは、参照プロパティまたはナビゲーション プロパティとも呼ばれ、1 つのリソースまたはリソースのコレクションのいずれかを参照することができます。たとえば、ユーザーのメール フォルダー、マネージャー、直属の部下は、すべてリレーションシップとして公開されます。</span><span class="sxs-lookup"><span data-stu-id="c7730-p108">Many Microsoft Graph resources expose both declared properties of the resource as well as its relationships with other resources. These relationships are also called reference properties or navigation properties and they can reference either a single resource or a collection of resources. For example, the mail folders, manager, and direct reports of a user are all exposed as relationships.</span></span> 

<span data-ttu-id="c7730-p109">通常、単一の要求では、リソースの複数のプロパティ、またはリソースのリレーションシップの 1 つのいずれかに対してクエリを実行できますが、両方は行えません。`$expand` クエリ文字列パラメーターを使用して、展開されているリソース、または単一のリレーションシップ (ナビゲーション プロパティ) で参照されているコレクションを結果に含めることができます。</span><span class="sxs-lookup"><span data-stu-id="c7730-p109">Normally, you can query either the properties of a resource or one of its relationships in a single request, but not both. You can use the `$expand` query string parameter to include the expanded resource or collection referenced by a single relationship (navigation property) in your results.</span></span>

<span data-ttu-id="c7730-150">次の例では、ドライブ内のトップレベルの子項目と共に、ルート ドライブ情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="c7730-150">The following example gets root drive information along with the top level child items in a drive:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children
```

[<span data-ttu-id="c7730-151">Graph エクスプローラーで試す</span><span class="sxs-lookup"><span data-stu-id="c7730-151">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children&method=GET&version=v1.0)

<span data-ttu-id="c7730-p110">いくつかのリソース コレクションで、`$select` パラメーターを追加すれば、展開されたリソースで返されるプロパティを指定することもできます。次の使用例は前の例と同じクエリを実行しますが、[`$select`](#select) ステートメントを使用して、展開されている子項目に返されるプロパティを `id` プロパティと `name` プロパティに限定します。</span><span class="sxs-lookup"><span data-stu-id="c7730-p110">With some resource collections, you can also specify the properties to be returned in the expanded resources by adding a `$select` parameter. The following example performs the same query as the previous example but uses a [`$select`](#select) statement to limit the properties returned for the expanded child items to the `id` and `name` properties.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

<span data-ttu-id="c7730-154">[Graph エクスプローラーで試す](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children($select=id,name)&method=GET&version=v1.0)</span><span class="sxs-lookup"><span data-stu-id="c7730-154">[Try in Graph Explorer](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children($select=id,name)&method=GET&version=v1.0)</span></span>

> <span data-ttu-id="c7730-p111">**注:** すべてのリレーションシップとリソースで、`$expand` クエリ パラメーターがサポートされているわけではありません。たとえば、ユーザーの `directReports`、`manager`、`memberOf` の各リレーションシップを展開できますが、その `events`、`messages`、`photo` のリレーションシップは展開できません。すべてのリソースまたはリレーションシップで、`$select` を使用して展開されたアイテムがサポートされているわけではありません。</span><span class="sxs-lookup"><span data-stu-id="c7730-p111">**Note:** Not all relationships and resources support the `$expand` query parameter. For example, you can expand the `directReports`, `manager`, and `memberOf` relationships on a user, but you cannot expand its `events`, `messages`, or `photo` relationships. Not all resources or relationships support using `$select` on expanded items.</span></span> 
> 
> <span data-ttu-id="c7730-158">[ユーザー](../api-reference/v1.0/resources/user.md)や[グループ](../api-reference/v1.0/resources/group.md)のような、[directoryObject](../api-reference/v1.0/resources/directoryobject.md) から派生した Azure AD リソースの場合、`$expand` は `beta` でのみサポートされており、通常は展開されているリレーションシップに対し最大 20 個のアイテムを返すことができます。</span><span class="sxs-lookup"><span data-stu-id="c7730-158">With Azure AD resources that derive from [directoryObject](../api-reference/v1.0/resources/directoryobject.md), like [user](../api-reference/v1.0/resources/user.md) and [group](../api-reference/v1.0/resources/group.md), `$expand` is only supported for `beta` and  typically returns a maximum of 20 items for the expanded relationship.</span></span>

## <a name="filter"></a><span data-ttu-id="c7730-159">filter</span><span class="sxs-lookup"><span data-stu-id="c7730-159">filter</span></span>

<span data-ttu-id="c7730-160">`$filter` クエリ パラメーターを使用して、コレクションのサブセットのみを取得します。</span><span class="sxs-lookup"><span data-stu-id="c7730-160">Use the `$filter` query parameter to retrieve just a subset of a collection.</span></span> 

<span data-ttu-id="c7730-161">たとえば、表示名が「J」という文字で始まるユーザーを検索するには、`startswith` を使用します。</span><span class="sxs-lookup"><span data-stu-id="c7730-161">For example, to find users whose display name starts with the letter 'J', use `startswith`.</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'J')
```

<span data-ttu-id="c7730-162">[Graph エクスプローラーで試す](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0)</span><span class="sxs-lookup"><span data-stu-id="c7730-162">[Try in Graph Explorer](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0)</span></span>

<span data-ttu-id="c7730-p112">`$filter` 演算子へのサポートは、お使いの Microsoft Graph API によって異なります。通常、次の論理演算子はサポートされています。等しい (`eq`)、等しくない (`ne`)、より大きい (`gt`)、以上 (`ge`)、より小さい (`lt`)、以下 (`le`)、かつ (`and`)、または (`or`)、否定 (`not`)。`startswith` 文字列の演算子はたいていサポートされています。`any` ラムダ演算子は、一部の API でサポートされています。いくつかの使用例について、下の表を参照してください。`$filter` 構文の詳細については、「[OData プロトコル][odata-filter]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c7730-p112">Support for `$filter` operators varies across Microsoft Graph APIs. The following logical operators are generally supported: equals (`eq`), not equals (`ne`), greater than (`gt`), greater than or equals (`ge`), less than (`lt`), less than or equals (`le`), and (`and`), or (`or`), and not (`not`). The `startswith` string operator is often supported. The `any` lambda operator is supported for some APIs. For some  usage examples, see the table below. For additional details on `$filter` syntax, see the [OData protocol][odata-filter].</span></span>  

<span data-ttu-id="c7730-169">次の表では、`$filter` クエリ パラメーター使用例を示します。</span><span class="sxs-lookup"><span data-stu-id="c7730-169">The following table shows some examples using the `$filter` query parameter.</span></span>

|<span data-ttu-id="c7730-170">説明</span><span class="sxs-lookup"><span data-stu-id="c7730-170">Description</span></span>|<span data-ttu-id="c7730-171">例 (例をクリックして [Graph エクスプローラー][graph-explorer]で試行します)</span><span class="sxs-lookup"><span data-stu-id="c7730-171">Example (click examples to try in [Graph Explorer][graph-explorer])</span></span>|
|:--------|:-------|
|  <span data-ttu-id="c7730-172">複数のプロパティ間で Mary という名前を持つユーザーを検索します。</span><span class="sxs-lookup"><span data-stu-id="c7730-172">Search for users with the name Mary across multiple properties.</span></span> | [`https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'mary') or startswith(givenName,'mary') or startswith(surname,'mary') or startswith(mail,'mary') or startswith(userPrincipalName,'mary')`](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(displayName,'mary')+or+startswith(givenName,'mary')+or+startswith(surname,'mary')+or+startswith(mail,'mary')+or+startswith(userPrincipalName,'mary')&method=GET&version=v1.0) |
| <span data-ttu-id="c7730-173">2017 年 7 月 1 日以降に開始する、サインイン ユーザーのイベントすべてを取得します。</span><span class="sxs-lookup"><span data-stu-id="c7730-173">Get all of the signed-in user's events that start after 7/1/2017.</span></span> | [`https://graph.microsoft.com/v1.0/me/events?$filter=start/dateTime ge '2017-07-01T08:00'`](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$filter=start/dateTime+ge+'2017-07-01T08:00'&method=GET&version=v1.0) |
| <span data-ttu-id="c7730-174">サインイン ユーザーが受信した特定のアドレスからの電子メールすべてを取得します。</span><span class="sxs-lookup"><span data-stu-id="c7730-174">Get all emails from a specific address received by the signed-in user.</span></span> | [`https://graph.microsoft.com/v1.0/me/messages?$filter=from/emailAddress/address eq 'someuser@example.com'`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=from/emailAddress/address+eq+'someuser@.com'&method=GET&version=v1.0) |
| <span data-ttu-id="c7730-175">2017 年 4 月にサインイン ユーザーが受信した電子メールすべてを取得します。</span><span class="sxs-lookup"><span data-stu-id="c7730-175">Get all emails received by the signed-in user in April 2017</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=ReceivedDateTime ge 2017-04-01 and receivedDateTime lt 2017-05-01`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=ReceivedDateTime+ge+2017-04-01+and+receivedDateTime+lt+2017-05-01&method=GET&version=v1.0) |
| <span data-ttu-id="c7730-176">サインイン ユーザーの受信トレイから未読メールをすべて取得します。</span><span class="sxs-lookup"><span data-stu-id="c7730-176">Get all unread mails in the signed-in user's Inbox.</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=isRead eq false`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=isRead+eq+false&method=GET&version=v1.0) |
| <span data-ttu-id="c7730-177">組織内のすべての Office 365 グループの一覧</span><span class="sxs-lookup"><span data-stu-id="c7730-177">List all Office 365 groups in an organization</span></span> | [`https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')`](https://developer.microsoft.com/graph/graph-explorer?request=groups?$filter=groupTypes/any(c:c+eq+'Unified')&method=GET&version=v1.0) |

> <span data-ttu-id="c7730-p113">**注:** Azure AD リソースでは、次の `$filter` 演算子はサポートされていません: `ne`、`gt`、`ge`、`lt`、`le`、`not`。Microsoft Graph リソースでは現在、`contains` 文字列の演算子はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c7730-p113">**Note:** The following `$filter` operators are not supported for Azure AD resources:  `ne`, `gt`, `ge`, `lt`, `le`, and `not`. The `contains` string operator is currently not supported on any Microsoft Graph resources.</span></span>

## <a name="orderby"></a><span data-ttu-id="c7730-180">orderby</span><span class="sxs-lookup"><span data-stu-id="c7730-180">orderby</span></span>

<span data-ttu-id="c7730-181">`$orderby` クエリ パラメーターを使用して、Microsof Graph から返される項目の並べ替え順序を指定します。</span><span class="sxs-lookup"><span data-stu-id="c7730-181">Use the `$orderby` query parameter to specify the sort order of the items returned from Microsoft Graph.</span></span>

<span data-ttu-id="c7730-182">たとえば、次の要求では組織のユーザーが表示名順で返されます。</span><span class="sxs-lookup"><span data-stu-id="c7730-182">For example, to return the users in the organization ordered by their display name, the syntax is as follows:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```
[<span data-ttu-id="c7730-183">Graph エクスプローラーで試す</span><span class="sxs-lookup"><span data-stu-id="c7730-183">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=users?$orderby=displayName&method=GET&version=v1.0)

<span data-ttu-id="c7730-p114">複合型のエンティティでも並べ替えが可能です。次の要求では、メッセージを取得し、それらを `emailAddress` という複合型である `from` プロパティの `address` フィールドで並べ替えます。</span><span class="sxs-lookup"><span data-stu-id="c7730-p114">You can also sort by complex type entities. The following example gets messages and sorts them by the `address` field of the `from` property, which is of the complex type `emailAddress`:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
```
[<span data-ttu-id="c7730-186">Graph エクスプローラーで試す</span><span class="sxs-lookup"><span data-stu-id="c7730-186">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/address&method=GET&version=v1.0)

<span data-ttu-id="c7730-187">昇順または降順で結果を並べ替えるには、`asc` または `desc` のいずれかをスペースで区切ってフィールド名の後に追加します。たとえば `?$orderby=name%20desc` のようにします。</span><span class="sxs-lookup"><span data-stu-id="c7730-187">To sort the results in ascending or descending order, append either `asc` or `desc` to the field name, separated by a space, for example, `?$orderby=name%20desc`.</span></span>

<span data-ttu-id="c7730-p115">一部の API では、複数のプロパティの結果を並べ替えることができます。たとえば、次のような要求ではユーザーの受信トレイ内のメッセージを、最初は送信者の名前で降順に並べ替え (Z から A)、次に件名で昇順 (既定) に並べ替えます。</span><span class="sxs-lookup"><span data-stu-id="c7730-p115">With some APIs, you can order results on multiple properties. For example, the following request orders the messages in the user's Inbox first by the name of the person who sent it in descending order (Z to A) and then by subject in ascending order (default).</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/Inbox/messages?$orderby=from/emailAddress/name desc,subject
```
[<span data-ttu-id="c7730-190">Graph エクスプローラーで試す</span><span class="sxs-lookup"><span data-stu-id="c7730-190">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/name%20desc,subject&method=GET&version=v1.0)


 > <span data-ttu-id="c7730-191">**注:** [ユーザー](../api-reference/v1.0/resources/user.md)や[グループ](../api-reference/v1.0/resources/group.md)のような、[directoryObject](../api-reference/v1.0/resources/directoryobject.md) から派生した Azure AD リソースの場合、`$orderby` 式と `$filter` 式を結合することはできません。</span><span class="sxs-lookup"><span data-stu-id="c7730-191">**Note:** With Azure AD resources that derive from [directoryObject](../api-reference/v1.0/resources/directoryobject.md), like [user](../api-reference/v1.0/resources/user.md) and [group](../api-reference/v1.0/resources/group.md), you cannot combine `$orderby` with `$filter` expressions.</span></span> 

## <a name="search"></a><span data-ttu-id="c7730-192">search</span><span class="sxs-lookup"><span data-stu-id="c7730-192">search</span></span>

<span data-ttu-id="c7730-193">`$search` クエリ パラメーターを使用して、要求の結果を検索条件と一致するものに制限します。</span><span class="sxs-lookup"><span data-stu-id="c7730-193">Use the `$search` query parameter to restrict the results of a request to match a search criterion.</span></span>

> <span data-ttu-id="c7730-p116">**注:** 現在の検索対象は、[メッセージ](../api-reference/v1.0/resources/message.md) コレクションと[人物](../api-reference/v1.0/resources/person.md)コレクション**だけ**です。`$search` 要求は最大 250 まで結果を返します。検索要求では [`$filter`](#filter) も [`$orderby`](#orderby) も使用できません。</span><span class="sxs-lookup"><span data-stu-id="c7730-p116">**Note:** You can currently **only** search [message](../api-reference/v1.0/resources/message.md) and [person](../api-reference/v1.0/resources/person.md) collections. A `$search` request returns up to 250 results. You cannot use [`$filter`](#filter) or [`$orderby`](#orderby) in a search request.</span></span>

### <a name="using-search-on-message-collections"></a><span data-ttu-id="c7730-197">`message` コレクションで $Search を使用する</span><span class="sxs-lookup"><span data-stu-id="c7730-197">Using $search on `message` collections</span></span>

<span data-ttu-id="c7730-p117">メッセージの検索条件は、[高度な検索テクニック (AQS)](https://support.office.com/article/Search-Mail-and-People-in-Outlook-com-and-Outlook-on-the-web-for-business-88108edf-028e-4306-b87e-7400bbb40aa7) を使用して表現されます。結果は、メッセージが送信された日時で並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="c7730-p117">Search criteria are expressed using Advanced Query Syntax (AQS). The results are sorted by the date and time that the message was sent.</span></span>

<span data-ttu-id="c7730-200">`$search` で `message` に対する次のプロパティを指定できます: `attachments`、`bccRecipients`、`body`、`category`、`ccRecipients`、`content`、`from`、`hasAttachments`、`participants`、`receivedDateTime`、`sender`、`subject`、`toRecipients`</span><span class="sxs-lookup"><span data-stu-id="c7730-200">You can specify the following properties on a `message` in a `$search` criterion: `attachments`, `bccRecipients`, `body`, `category`, `ccRecipients`, `content`, `from`, `hasAttachments`, `participants`, `receivedDateTime`, `sender`, `subject`, `toRecipients`</span></span>

<span data-ttu-id="c7730-201">メッセージで検索を行うときに値のみ指定した場合、検索は既定の検索プロパティである `from`、`subject` および `body` に基づいて行われます。</span><span class="sxs-lookup"><span data-stu-id="c7730-201">If you do a search on messages and specify only a value, the search is carried out on the default search properties of `from`, `subject` and `body`.</span></span>

<span data-ttu-id="c7730-202">次の例は、サインイン中のユーザーの受信トレイにあるメッセージのうち、既定の 3 つの検索プロパティのいずれかに "pizza" が含まれるメッセージをすべて返します。</span><span class="sxs-lookup"><span data-stu-id="c7730-202">The following example returns all messages in the signed-in user's Inbox that contains "pizza" in any of the three default search properties:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

<span data-ttu-id="c7730-203">次の例は、ユーザーの受信トレイにあるメッセージのうち、特定のメール アドレスから送信されたメッセージをすべて検索します。</span><span class="sxs-lookup"><span data-stu-id="c7730-203">The next example searches all messages in the user's Inbox that were sent from a specific email address:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="from:help@contoso.com"
```

### <a name="using-search-on-person-collections"></a><span data-ttu-id="c7730-204">`person` コレクションで $Search を使用する</span><span class="sxs-lookup"><span data-stu-id="c7730-204">Using $search on `person` collections</span></span>

<span data-ttu-id="c7730-p118">Microsoft Graph People API を使用してユーザーに最も関連のある人物を取得できます。関連性は、ユーザーのコミュニケーションとコラボレーション パターン、およびビジネスのリレーションシップによって決定されます。People API では、`$search` クエリ パラメーターがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="c7730-p118">You can use the Microsoft Graph People API to retrieve the people who are most relevant to a user. Relevance is determined by the user’s communication and collaboration patterns and business relationships. The People API supports the `$search` query parameter.</span></span>

<span data-ttu-id="c7730-p119">[人物](../api-reference/v1.0/resources/person.md)リソースの `displayName` プロパティと `emailAddress` プロパティの両方で人物の検索を行います。検索は、あいまい一致のアルゴリズムを実装します。これにより、完全に一致する項目と、検索目的の推論に基づく結果が返されます。たとえば、サインイン ユーザーの `people` コレクション内で、"Tyler Lee" の表示名および tylerle@example.com というメール アドレスを持つユーザーを想定してください。次の検索はすべて、Tyler を含む検索結果を返します。</span><span class="sxs-lookup"><span data-stu-id="c7730-p119">Searches on people occur on both the `displayName` and `emailAddress` properties of the [person](../api-reference/v1.0/resources/person.md) resource. Searches implement a fuzzy matching algorithm. They will return results based on an exact match and also on inferences about the intent of the search. For example, imagine a user with a display name of "Tyler Lee" and an email address of tylerle@example.com who is in the `people` collection of the signed-in user. All of the following searches will return results that contain Tyler.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people?$search=tyler                //matches both Tyler's name and email
GET https://graph.microsoft.com/v1.0/me/people?$search=tylerle              //matches Tyler's email
GET https://graph.microsoft.com/v1.0/me/people?$search="tylerle@example.com"  //matches Tyler's email. Note the quotes to enclose '@'.
GET https://graph.microsoft.com/v1.0/me/people?$search=tiler                //fuzzy match with Tyler's name 
GET https://graph.microsoft.com/v1.0/me/people?$search="tyler lee"          //matches Tyler's name. Note the quotes to enclose the space.
```

<span data-ttu-id="c7730-p120">特定のトピックに興味のある人物の検索を実行することもできます。ユーザーのメールのスレッドから引き出した推測に基づいて検索を実行します。たとえば、次の検索は、サインイン ユーザーに関連のある人物のうち、そのユーザーとの通信の中でピザに興味を示した人のコレクションを返します。検索語句を引用符で囲んでいることに注目してください。</span><span class="sxs-lookup"><span data-stu-id="c7730-p120">You can also perform searches for people who are interested in a particular topic. Searches are performed based on inferences derived from the user's mail conversations. For example, the following search will return a collection of people relevant to the signed-in user who have expressed an interest in pizza in communications with that user. Note that the search phrase is enclosed in quotes.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="topic:pizza"                
```

<span data-ttu-id="c7730-217">最後に、2 種類の検索式を組み合わせることによって、同じ要求内に人の検索とトピックの検索の両方をまとめることができます。</span><span class="sxs-lookup"><span data-stu-id="c7730-217">Finally, you can combine both people searches and topic searches in the same request by combining the two types of search expression.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="tyl topic:pizza"                
```
<span data-ttu-id="c7730-p121">この要求は本質的には 2 つの検索を行います。サインイン ユーザーに関連する人物の `displayName` プロパティと `emailAddress` プロパティに対するあいまい検索、そしてユーザーに関連する人物に対する「ピザ」というトピックの検索です。次いで結果をランク付けし、並べ替え、返します。この検索は制限的ではありません。「tyl」とあいまい一致する人物、「ピザ」に関心を示す人物、または両方の結果を取得する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="c7730-p121">This request essentially conducts two searches: a fuzzy search against `displayName` and `emailAddress` properties of the signed-in user's relevant people and a topic search for "pizza" against the user's relevant people. The results are then ranked, ordered, and returned. Note that the search is not restrictive; you may get results that contain people that fuzzy match "tyl", or that are interested in "pizza", or both.</span></span>

<span data-ttu-id="c7730-221">People API についてもっと知るには、「[関係する人の情報を取得する](./people_example.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c7730-221">To learn more about the People API, see [Get information about relevant people](./people_example.md).</span></span>  

## <a name="select"></a><span data-ttu-id="c7730-222">select</span><span class="sxs-lookup"><span data-stu-id="c7730-222">select</span></span>

<span data-ttu-id="c7730-p122">`$select` クエリ パラメーターを使用して、個別リソースまたはリソースのコレクションの既定値とは異なるプロパティのセットを返します。$Select で、既定のプロパティのサブセットまたはスーパー セットを指定できます。</span><span class="sxs-lookup"><span data-stu-id="c7730-p122">Use the `$select` query parameter to return a set of properties different than the default set for an individual resource or a collection of resources. With $select you can specify a subset or a superset of the default properties.</span></span>

<span data-ttu-id="c7730-225">たとえば、サインイン ユーザーのメッセージを取得するとき、`from` プロパティと `subject` プロパティだけを返すよう指定できます。</span><span class="sxs-lookup"><span data-stu-id="c7730-225">For example, when retrieving the messages of the signed-in user, you can specify that only the `from` and `subject` properties be returned:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

[<span data-ttu-id="c7730-226">Graph エクスプローラーで試す</span><span class="sxs-lookup"><span data-stu-id="c7730-226">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$select=from,subject&method=GET&version=v1.0)

> <span data-ttu-id="c7730-p123">**重要:**通常は、`$select` を使用して、クエリから返されるプロパティをお使いのアプリで必要なものだけに制限することをお勧めします。これは特に、クエリが大きな結果セットを返す可能性がある場合に該当します。行ごとに返されるプロパティを制限すれば、ネットワークの負荷を軽減し、アプリのパフォーマンスを向上させることができます。</span><span class="sxs-lookup"><span data-stu-id="c7730-p123">**Important:** In general, we recommend that you use `$select` to limit the properties returned by a query to those needed by your app. This is especially true of queries that may potentially return a large result set. Limiting the properties returned in each row will reduce network load and help improve your app's performance.</span></span>
>
> <span data-ttu-id="c7730-p124">`v1.0`では、[ユーザー](../api-reference/v1.0/resources/user.md)と[グループ](../api-reference/v1.0/resources/group.md)のような、[directoryObject](../api-reference/v1.0/resources/directoryobject.md) から派生した一部の Azure AD リソースは、読み取り時に制限された既定値のプロパティ サブセットを返します。既定のセット以外のプロパティを返すには、これらのリソースに対して `$select` を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c7730-p124">In `v1.0`, some Azure AD resources that derive from [directoryObject](../api-reference/v1.0/resources/directoryobject.md), like [user](../api-reference/v1.0/resources/user.md) and [group](../api-reference/v1.0/resources/group.md), return a limited, default subset of properties on reads. For these resources, you must use `$select` to return properties outside of the default set.</span></span>  

## <a name="skip"></a><span data-ttu-id="c7730-232">skip</span><span class="sxs-lookup"><span data-stu-id="c7730-232">skip</span></span>

<span data-ttu-id="c7730-p125">コレクションを開始するときにスキップする項目数を設定するには、`$skip` クエリ パラメーターを使用します。たとえば、次の要求はユーザーのイベントを、コレクション内の 21 番目以降のイベントから作成日順で返します。</span><span class="sxs-lookup"><span data-stu-id="c7730-p125">Use the `$skip` query parameter to set the number of items to skip at the start of a collection. For example, the following request returns events for the user sorted by date created, starting with the 21st event in the collection:</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```
[<span data-ttu-id="c7730-235">Graph エクスプローラーで試す</span><span class="sxs-lookup"><span data-stu-id="c7730-235">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$orderby=createdDateTime&$skip=20&method=GET&version=v1.0)

> <span data-ttu-id="c7730-p126">**注:** Outlook メール/カレンダーなどいくつかの Microsoft Graph API (`message`、`event`、`calendar`) は、`$skip` を使用してページングを実装します。クエリの結果が複数ページにまたがる場合、これらの API は`@odata:nextLink` プロパティと共に `$skip` パラメーターが含まれる URL を返します。この URL を使用して、結果の次のページに戻れます。詳細については、「[ページング](./paging.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c7730-p126">**Note:** Some Microsoft Graph APIs, like Outlook Mail and Calendars (`message`, `event`, and, `calendar`), use `$skip` to implement paging. When results of a query span multiple pages, these APIs will return an `@odata:nextLink` property with a URL that contains a `$skip` parameter. You can use this URL to return the next page of results. To learn more, see [Paging](./paging.md).</span></span>

## <a name="skiptoken"></a><span data-ttu-id="c7730-240">skipToken</span><span class="sxs-lookup"><span data-stu-id="c7730-240">skipToken</span></span>

<span data-ttu-id="c7730-p127">要求の中には、サーバー側のページングを使用したり、応答におけるページ サイズを限定するために [`$top`](#top) パラメーターを使用したりすることによって、複数のデータ ページを返すものがあります。Microsoft Graph API の多くは、`skipToken` クエリ パラメーターを使用して、結果の後続のページを参照します。`$skiptoken` パラメーターは、結果の次のページを参照する不透明トークンを含んでおり、応答の `@odata.nextLink` プロパティで指定される URL で返されます。詳細については、「[ページング](./paging.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c7730-p127">Some requests return multiple pages of data either due to server-side paging or due to the use of the [`$top`](#top) parameter to limit the page size of the response. Many Microsoft Graph APIs use the `skipToken` query parameter to reference subsequent pages of the result. The `$skiptoken` parameter contains an opaque token that references the next page of results and is returned in the URL provided in the `@odata.nextLink` property in the response. To learn more, see [Paging](./paging.md).</span></span>


## <a name="top"></a><span data-ttu-id="c7730-245">top</span><span class="sxs-lookup"><span data-stu-id="c7730-245">top</span></span>

<span data-ttu-id="c7730-246">`$top` クエリ パラメーターを使用して、結果セットのページ サイズを指定します。</span><span class="sxs-lookup"><span data-stu-id="c7730-246">Use the `$top` query parameter to specify the page size of the result set.</span></span> 

<span data-ttu-id="c7730-p128">残りの結果セットにさらに項目がある場合、応答本文に `@odata.nextLink` パラメーターが含まれます。このパラメーターには、結果の次のページを取得するために使用できる URL が含まれています。詳細については、「[ページング](./paging.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c7730-p128">If there are more items remaining in the result set, the response body will contain an `@odata.nextLink` parameter. This parameter contains a URL that you can use to get the next page of results. To learn more, see [Paging](./paging.md).</span></span> 

<span data-ttu-id="c7730-250">たとえば、次の要求はユーザーのメールボックスの最初の 5 つのメッセージを返します。</span><span class="sxs-lookup"><span data-stu-id="c7730-250">For example, the following request returns the first five messages in the user's mailbox:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```

[<span data-ttu-id="c7730-251">Graph エクスプローラーで試す</span><span class="sxs-lookup"><span data-stu-id="c7730-251">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$top=5&method=GET&version=v1.0)


## <a name="error-handling-for-query-parameters"></a><span data-ttu-id="c7730-252">クエリ パラメーターのエラー処理</span><span class="sxs-lookup"><span data-stu-id="c7730-252">Error handling for query parameters</span></span>

<span data-ttu-id="c7730-p129">指定されたクエリ パラメーターがサポートされていない場合、一部の要求はエラー メッセージを返します。たとえば、`$expand` を `user/photo` のリレーションシップで使用することはできません。</span><span class="sxs-lookup"><span data-stu-id="c7730-p129">Some requests will return an error message if a specified query parameter is not supported. For example, you cannot use `$expand` on the `user/photo` relationship.</span></span> 

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

<span data-ttu-id="c7730-p130">ただし、要求で指定されたクエリ パラメーターが警告なしで失敗する可能性があるため、注意が必要です。これは、クエリ パラメーターがサポートされていない場合や、クエリ パラメーターの組み合わせがサポートされていない場合に起こり得ます。その場合、要求によって返されたデータを調べ、指定したクエリ パラメーターに期待どおりの効果があったかどうかを確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c7730-p130">However, it is important to note that query parameters specified in a request may fail silently. This can be true for unsupported query parameters as well as for unsupported combinations of query parameters. In these cases, you should examine the data returned by the request to determine whether the query parameters you specified had the desired effect.</span></span> 

[graph-explorer]: https://developer.microsoft.com/graph/graph-explorer
[odata-filter]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752358
[odata-query]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752356