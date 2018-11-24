# <a name="microsoft-graph-security-api-error-responses"></a><span data-ttu-id="e6e7c-101">Microsoft グラフ セキュリティ API のエラー応答</span><span class="sxs-lookup"><span data-stu-id="e6e7c-101">Microsoft Graph Security API error responses</span></span>

<span data-ttu-id="e6e7c-102">Graph で Microsoft グラフ セキュリティ API のエラーは、標準的な HTTP 206 部分的なコンテンツのステータス コードを使用して返されます、警告ヘッダーを使用して配信されます。</span><span class="sxs-lookup"><span data-stu-id="e6e7c-102">Errors in the Microsoft Graph Security API in Microsoft Graph are returned using standard HTTP 206 Partial Content status code and are delivered by way of a warning header.</span></span>

<span data-ttu-id="e6e7c-103">Microsoft グラフ セキュリティ API は、すべてのデータ プロバイダーから複数の応答を受信するフェデレーション サービスです。</span><span class="sxs-lookup"><span data-stu-id="e6e7c-103">The Microsoft Graph Security API is a federated service that receives multiple responses from all data providers.</span></span> <span data-ttu-id="e6e7c-104">Microsoft グラフ セキュリティ API が HTTP エラーを受信したを送信します戻る警告ヘッダーで次の形式。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="e6e7c-104">When an HTTP error is received by the Microsoft Graph Security API, it will send back a warning header in the following format: <!-- { "blockType": "ignored" } --></span></span>

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

<span data-ttu-id="e6e7c-105">この警告ヘッダーはデータ プロバイダーの 1 つ以外の 2 xx または 404 エラー コードが返されるときにクライアントにのみ送信されます。</span><span class="sxs-lookup"><span data-stu-id="e6e7c-105">This warning header is only sent back to clients when one of the data providers returns an error code other than 2xx or 404.</span></span> <span data-ttu-id="e6e7c-106">例:</span><span class="sxs-lookup"><span data-stu-id="e6e7c-106">For example:</span></span>

- <span data-ttu-id="e6e7c-107">HttpStatusCode.Forbidden (403) は、リソースへのアクセスが与えられていない場合に返される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="e6e7c-107">HttpStatusCode.Forbidden (403) might be returned if the access to the resource is not granted.</span></span>
- <span data-ttu-id="e6e7c-108">プロバイダーがタイムアウトになった場合は、警告ヘッダーの HttpStatusCode.GatewayTimeout (504) が返されます。</span><span class="sxs-lookup"><span data-stu-id="e6e7c-108">If a provider times out, HttpStatusCode.GatewayTimeout (504) is returned in the warning header.</span></span>
- <span data-ttu-id="e6e7c-109">内部プロバイダ エラーが発生した場合、HttpStatusCode.InternalServerError (500) は、warning ヘッダーで使用されます。</span><span class="sxs-lookup"><span data-stu-id="e6e7c-109">If an internal provider error happens, HttpStatusCode.InternalServerError (500) is used in the warning header.</span></span>

<span data-ttu-id="e6e7c-110">データ プロバイダーに 2 xx または 404 が返される場合に表示されませんの警告ヘッダーのこれらのコードが成功した場合に期待どおりになっているか、それぞれのデータが見つからない場合。</span><span class="sxs-lookup"><span data-stu-id="e6e7c-110">If a data provider returns 2xx or 404, it’s not shown in the warning header because these codes are expected for success or when data is not found respectively.</span></span> <span data-ttu-id="e6e7c-111">フェデレートされたシステムでは、何度もデータだけがわかっている 1 つまたはいくつか、すべてではなくプロバイダーと、404 が見つかりませんが考えられます。</span><span class="sxs-lookup"><span data-stu-id="e6e7c-111">In a federated system, a 404 not found is expected as many times the data is only known to one or several, but not all, providers.</span></span>

## <a name="example"></a><span data-ttu-id="e6e7c-112">例</span><span class="sxs-lookup"><span data-stu-id="e6e7c-112">Example</span></span>

<span data-ttu-id="e6e7c-113">ユーザーが求める`security/alerts/{alert_id}`。</span><span class="sxs-lookup"><span data-stu-id="e6e7c-113">A user asks for `security/alerts/{alert_id}`.</span></span>

    Provider 1: 404 (provider does not have a record of this alert ID)
    Provider 2: 504 (provider timed out)
    Provider 3: 200 (success)
    Provider 4: 403 (customer has not licensed this provider)

<span data-ttu-id="e6e7c-114">404 と 200 の両方が必要な条件であるため warning ヘッダーは、次の含まれています。</span><span class="sxs-lookup"><span data-stu-id="e6e7c-114">Because both 404 and 200 are expected conditions, the warning header contains the following:</span></span> 

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/10000",    (usual timeout limit is set at 10 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> <span data-ttu-id="e6e7c-115">**注:** 各 HTTP ヘッダーは、ユーザーは警告ヘッダーを列挙し、すべての項目をチェックするために、サブ項目のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="e6e7c-115">**Note:** Each HTTP header is a collection of subitems, so users can enumerate the Warning header and check all items.</span></span>

## <a name="see-also"></a><span data-ttu-id="e6e7c-116">関連項目</span><span class="sxs-lookup"><span data-stu-id="e6e7c-116">See also</span></span>

<span data-ttu-id="e6e7c-117">認証に問題がある場合は、私たちの[ブログの投稿](https://techcommunity.microsoft.com/t5/Using-Microsoft-Graph-Security/Authorization-and-Microsoft-Graph-Security-API/m-p/184376#M2)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e6e7c-117">If you’re having trouble with authorization, see our [blog post](https://techcommunity.microsoft.com/t5/Using-Microsoft-Graph-Security/Authorization-and-Microsoft-Graph-Security-API/m-p/184376#M2).</span></span>
