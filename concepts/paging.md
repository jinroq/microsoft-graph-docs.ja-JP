
# <a name="paging-microsoft-graph-data-in-your-app"></a><span data-ttu-id="0f8f0-101">アプリで Microsoft Graph データをページングする</span><span class="sxs-lookup"><span data-stu-id="0f8f0-101">Paging Microsoft Graph data in your app</span></span> 

<span data-ttu-id="0f8f0-p101">Microsoft Graph に対するクエリの中には、サーバー側のページングを使用したり、1 つの要求におけるページ サイズを限定するために `$top` クエリ パラメーターを使用したりすることによって、複数のデータ ページを返すものがあります。要求セットが複数ページにまたがる場合、Microsoft Graph は、結果の次のページへの URL が含まれる `@odata.nextLink` プロパティを応答で返します。</span><span class="sxs-lookup"><span data-stu-id="0f8f0-p101">Some queries against Microsoft Graph return multiple pages of data either due to server-side paging or due to the use of the `$top` query parameter to specifically limit the page size in a request. When a result set spans multiple pages, Microsoft Graph returns an `@odata.nextLink` property in the response that contains a URL to the next page of results.</span></span> 

<span data-ttu-id="0f8f0-104">たとえば、次の URL の場合、組織内のすべてのユーザーのうち、`$top` クエリ パラメーターで指定されたページ サイズ 5 のユーザーを要求します。</span><span class="sxs-lookup"><span data-stu-id="0f8f0-104">For example, the following URL requests all of the users in an organization with a page size of 5 specified with the `$top` query parameter:</span></span>

```html
https://graph.microsoft.com/v1.0/users?$top=5
```

<span data-ttu-id="0f8f0-105">結果に 5 人を超えるユーザーが含まれる場合、Microsoft Graph は、最初のページのユーザーに加えて、次のような `odata:nextLink` プロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="0f8f0-105">If the result contains more than 5 users, Microsoft Graph will return an `odata:nextLink` property similar to the following along with the first page of users.</span></span>

```json
"@odata.nextLink": "https://graph.microsoft.com/v1.0/users?$top=5&$skiptoken=X%274453707 ... 6633B900000000000000000000%27"
```

<span data-ttu-id="0f8f0-106">この `@odata:nextLink` プロパティの URL 値を Microsoft Graph に送信することによって、結果の次のページを取得できます。</span><span class="sxs-lookup"><span data-stu-id="0f8f0-106">You can retrieve the next page of results by sending the URL value of the `@odata:nextLink` property to Microsoft Graph.</span></span> 

```html
https://graph.microsoft.com/v1.0/users?$top=5&$skiptoken=X%274453707 ... 6633B900000000000000000000%27
```

<span data-ttu-id="0f8f0-107">その後、Microsoft Graph はすべての結果ページが読み取られるまで、それぞれの応答の `@odata:nextLink` プロパティ内の次のページのデータへの参照を返します。</span><span class="sxs-lookup"><span data-stu-id="0f8f0-107">Microsoft Graph will continue to return a reference to the next page of data in the `@odata:nextLink` property with each response until all pages of the result have been read.</span></span>

><span data-ttu-id="0f8f0-p102">**重要:**結果の次のページの要求には、`@odata:nextLink` プロパティの URL 全体を含める必要があります。クエリの実行対象の API によって、`@odata:nextLink` URL 値には `$skiptoken` と `$skip` のいずれかのクエリ パラメーターが入ります。また、URL には、元の要求にある他のクエリ パラメーターすべても含まれます。`$skiptoken` 値または `$skip` 値を抽出して、別の要求で使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="0f8f0-p102">**Important:** You should include the entire URL in the `@odata:nextLink` property in your request for the next page of results. Depending on the API that the query is being performed against, the `@odata:nextLink` URL value will contain either a `$skiptoken` or a `$skip` query parameter. The URL also contains all of the other query parameters present in the original request. Do not try to extract the `$skiptoken` or `$skip` value and use it in a different request.</span></span> 

<span data-ttu-id="0f8f0-p103">ページング動作は、それぞれの Microsoft Graph API によって異なります。ページングされたデータを扱う場合には、以下の事柄を考慮してください。</span><span class="sxs-lookup"><span data-stu-id="0f8f0-p103">Paging behavior varies across different Microsoft Graph APIs. You should consider the following when working with paged data:</span></span>

- <span data-ttu-id="0f8f0-114">API によって、既定および最大のページ サイズが異なる場合があります。</span><span class="sxs-lookup"><span data-stu-id="0f8f0-114">Different APIs may have different default and maximum page sizes.</span></span>
- <span data-ttu-id="0f8f0-p104">(`$top` クエリ パラメーターを使用して) 対象の API の最大ページ サイズを超えるページ サイズを指定する場合には、API によって動作が異なる可能性があります。API によっては要求されたページ サイズが無視されることがあります。対象 API の最大ページ サイズに既定で設定されたり、Microsoft Graph によってエラーが返されたりする場合があります。</span><span class="sxs-lookup"><span data-stu-id="0f8f0-p104">Different APIs may behave differently if you specify a page size (via the `$top` query parameter) that exceeds the maximum page size for that API. Depending on the API, the requested page size may be ignored, it may default to the maximum page size for that API, or Microsoft Graph may return an error.</span></span> 
- <span data-ttu-id="0f8f0-p105">すべてのリソースまたはリレーションシップでページングがサポートされているわけではありません。たとえば、[directoryRoles](../api-reference/v1.0/resources/directoryrole.md) に対するクエリではページングはサポートされていません。これにはロール メンバーおよびロール オブジェクト自体の読み取りも含まれます。</span><span class="sxs-lookup"><span data-stu-id="0f8f0-p105">Not all resources or relationships support paging. For example, queries against [directoryRoles](../api-reference/v1.0/resources/directoryrole.md) do not support paging. This includes reading role objects themselves as well as role members.</span></span>
- <span data-ttu-id="0f8f0-p106">一部の Microsoft Graph API では、`previous-page` クエリ パラメーター (`&previous-page=true`) を `@odata:nextLink` プロパティの URL 値に追加することによって、後方ページングがサポートされます。このパラメーターを要求に追加すると、後続の応答の `@odata:nextLink` URL 値にも含まれます。空の結果が含まれる応答が返されるまで、後方へのページングを継続できます。その後もページングを続けると、エラーが返されます。または、結果の次のページの要求を送信するときに `previous-page` パラメーターを削除することによって、現在の応答以降、前方ページングを再開できます。</span><span class="sxs-lookup"><span data-stu-id="0f8f0-p106">Some Microsoft Graph APIs support backward paging by appending the `previous-page` query parameter (`&previous-page=true`) to the URL value of the `@odata:nextLink` property. Once you append this parameter to a request, the `@odata:nextLink` URL value in subsequent responses will include it. You can continue to page backward until a response with an empty result is returned. Paging further will return an error. Alternatively, you can resume paging forward from the current response by removing the `previous-page` parameter when you send the request for the next page of results.</span></span> 

