# <a name="security-api-error-responses"></a><span data-ttu-id="5ea8e-101">セキュリティ API のエラー応答</span><span class="sxs-lookup"><span data-stu-id="5ea8e-101">Security API error responses</span></span>

<span data-ttu-id="5ea8e-102">Microsoft Graph のセキュリティ API のエラーは、標準の HTTP ステータス コードを使用して返され、警告ヘッダーを介して配信されます。</span><span class="sxs-lookup"><span data-stu-id="5ea8e-102">Errors in the security API in Microsoft Graph are returned using standard HTTP status codes and are delivered by way of a warning header.</span></span>

<span data-ttu-id="5ea8e-103">セキュリティ API は、すべてのデータ プロバイダーから複数の応答を受信するフェデレーション サービスです。</span><span class="sxs-lookup"><span data-stu-id="5ea8e-103">The security API is a federated service that receives multiple responses from all data providers.</span></span> <span data-ttu-id="5ea8e-104">セキュリティ API は HTTP エラーを受信すると、次の形式の警告ヘッダーを送信して返します。 <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5ea8e-104">When an HTTP error is received by the security API, it will send back a warning header in the following format: <!-- { "blockType": "ignored" } --></span></span>

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

<span data-ttu-id="5ea8e-105">この警告ヘッダーは、データ プロバイダーの 1 つが 2 xx または 404 以外のエラー コードを返すときにのみ、クライアントに送信して返されます。</span><span class="sxs-lookup"><span data-stu-id="5ea8e-105">This warning header is only sent back to clients when one of the data providers returns an error code other than 2xx or 404.</span></span> <span data-ttu-id="5ea8e-106">例:</span><span class="sxs-lookup"><span data-stu-id="5ea8e-106">For example:</span></span>

- <span data-ttu-id="5ea8e-107">リソースへのアクセスが与えられていない場合は、HttpStatusCode.Forbidden (403) が返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="5ea8e-107">HttpStatusCode.Forbidden (403) might be returned if the access to the resource is not granted.</span></span>
- <span data-ttu-id="5ea8e-108">プロバイダーがタイムアウトになった場合は、警告ヘッダー内に HttpStatusCode.GatewayTimeout (504) が返されます。</span><span class="sxs-lookup"><span data-stu-id="5ea8e-108">If a provider times out, HttpStatusCode.GatewayTimeout (504) is returned in the warning header.</span></span>
- <span data-ttu-id="5ea8e-109">内部プロバイダ エラーが発生した場合は、警告ヘッダー内で HttpStatusCode.InternalServerError (500) が使用されます。</span><span class="sxs-lookup"><span data-stu-id="5ea8e-109">If an internal provider error happens, HttpStatusCode.InternalServerError (500) is used in the warning header.</span></span>

<span data-ttu-id="5ea8e-110">データ プロバイダーが 2xx または 404 を返す場合は、それは警告ヘッダーに表示されません。なぜなら、2xx は成功した場合、404 はデータが見つからない場合に想定されるコードであるからです。</span><span class="sxs-lookup"><span data-stu-id="5ea8e-110">If a data provider returns 2xx or 404, it’s not shown in the warning header because these codes are expected for success or when data is not found respectively.</span></span> <span data-ttu-id="5ea8e-111">フェデレーション システムでは、多くの場合、データが 1 つまたはいくつかのプロバイダーには知られていても、すべてのプロバイダーには知られていないため、データが見つからない場合の 404 が返されることが想定されます。</span><span class="sxs-lookup"><span data-stu-id="5ea8e-111">In a federated system, a 404 not found is expected as many times the data is only known to one or several, but not all, providers.</span></span>

## <a name="example"></a><span data-ttu-id="5ea8e-112">例</span><span class="sxs-lookup"><span data-stu-id="5ea8e-112">Example</span></span>

<span data-ttu-id="5ea8e-113">ユーザーが `security/alerts/{alert_id}` を求めます。</span><span class="sxs-lookup"><span data-stu-id="5ea8e-113">A user asks for `security/alerts/{alert_id}`.</span></span>

    Provider 1: 404 (provider does not have a record of this alert ID)
    Provider 2: 504 (provider timed out)
    Provider 3: 200 (success)
    Provider 4: 403 (customer has not licensed this provider)

<span data-ttu-id="5ea8e-114">404 と 200 の両方は想定される条件であるため、警告ヘッダーには次のものが含まれます。</span><span class="sxs-lookup"><span data-stu-id="5ea8e-114">Because both 404 and 200 are expected conditions, the warning header contains the following:</span></span> 

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/29000",    (usual timeout limit is set at 29 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> <span data-ttu-id="5ea8e-115">**注:** 各 HTTP ヘッダーはサブ項目のコレクションであるため、ユーザーは警告ヘッダーを列挙して、すべての項目をチェックすることができます。</span><span class="sxs-lookup"><span data-stu-id="5ea8e-115">**Note:** Each HTTP header is a collection of subitems, so users can enumerate the Warning header and check all items.</span></span>

## <a name="see-also"></a><span data-ttu-id="5ea8e-116">関連項目</span><span class="sxs-lookup"><span data-stu-id="5ea8e-116">See also</span></span>

<span data-ttu-id="5ea8e-117">承認に問題がある場合は、私たちの[ブログ記事](https://techcommunity.microsoft.com/t5/Using-Microsoft-Graph-Security/Authorization-and-Microsoft-Graph-Security-API/m-p/184376#M2)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="5ea8e-117">If you’re having trouble with authorization, see our [blog post](https://techcommunity.microsoft.com/t5/Using-Microsoft-Graph-Security/Authorization-and-Microsoft-Graph-Security-API/m-p/184376#M2).</span></span>
