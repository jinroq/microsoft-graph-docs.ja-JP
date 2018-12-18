---
title: Microsoft グラフ セキュリティ API のエラー応答
description: セキュリティ api には、Microsoft のグラフのエラーは、標準の HTTP 206 部分的なコンテンツのステータス コードを使用して返され、警告ヘッダーを経由して配信。
author: Preetikr
ms.openlocfilehash: 6685d69f202696e33422d9bd3a877cba02fd10dd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329653"
---
# <a name="microsoft-graph-security-api-error-responses"></a><span data-ttu-id="7aca1-103">Microsoft グラフ セキュリティ API のエラー応答</span><span class="sxs-lookup"><span data-stu-id="7aca1-103">Microsoft Graph Security API error responses</span></span>

<span data-ttu-id="7aca1-104">セキュリティ api には、Microsoft のグラフのエラーは、標準の HTTP 206 部分的なコンテンツのステータス コードを使用して返され、警告ヘッダーを経由して配信。</span><span class="sxs-lookup"><span data-stu-id="7aca1-104">Errors in the Microsoft Graph Security API are returned using the standard HTTP 206 Partial Content status code and are delivered via a warning header.</span></span>

## <a name="errors"></a><span data-ttu-id="7aca1-105">エラー</span><span class="sxs-lookup"><span data-stu-id="7aca1-105">Errors</span></span>

<span data-ttu-id="7aca1-106">Microsoft グラフ セキュリティ API は、すべてのデータ プロバイダーから複数の応答を受信するフェデレーション サービスです。</span><span class="sxs-lookup"><span data-stu-id="7aca1-106">The Microsoft Graph Security API is a federated service that receives multiple responses from all data providers.</span></span> <span data-ttu-id="7aca1-107">Microsoft グラフ セキュリティ API が HTTP エラーを受信したを送信します戻る警告ヘッダーで次の形式。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="7aca1-107">When an HTTP error is received by the Microsoft Graph Security API, it will send back a warning header in the following format: <!-- { "blockType": "ignored" } --></span></span>

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

<span data-ttu-id="7aca1-108">この警告ヘッダーはデータ プロバイダーの 1 つ以外の 2 xx または 404 エラー コードが返されるときにクライアントにのみ送信されます。</span><span class="sxs-lookup"><span data-stu-id="7aca1-108">This warning header is only sent back to clients when one of the data providers returns an error code other than 2xx or 404.</span></span> <span data-ttu-id="7aca1-109">次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="7aca1-109">For example:</span></span>

- <span data-ttu-id="7aca1-110">HttpStatusCode.Forbidden (403) は、リソースへのアクセスが与えられていない場合に返される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="7aca1-110">HttpStatusCode.Forbidden (403) might be returned if the access to the resource is not granted.</span></span>
- <span data-ttu-id="7aca1-111">プロバイダーがタイムアウトになった場合は、警告ヘッダーの HttpStatusCode.GatewayTimeout (504) が返されます。</span><span class="sxs-lookup"><span data-stu-id="7aca1-111">If a provider times out, HttpStatusCode.GatewayTimeout (504) is returned in the warning header.</span></span>
- <span data-ttu-id="7aca1-112">内部プロバイダ エラーが発生した場合、HttpStatusCode.InternalServerError (500) は、warning ヘッダーで使用されます。</span><span class="sxs-lookup"><span data-stu-id="7aca1-112">If an internal provider error happens, HttpStatusCode.InternalServerError (500) is used in the warning header.</span></span>

<span data-ttu-id="7aca1-113">データ プロバイダーに 2 xx または 404 が返される場合に表示されませんの警告ヘッダーのこれらのコードが成功した場合に期待どおりになっているか、それぞれのデータが見つからない場合。</span><span class="sxs-lookup"><span data-stu-id="7aca1-113">If a data provider returns 2xx or 404, it’s not shown in the warning header because these codes are expected for success or when data is not found respectively.</span></span> <span data-ttu-id="7aca1-114">フェデレートされたシステムでは、何度もデータだけがわかっている 1 つまたはいくつか、すべてではなくプロバイダーと、404 が見つかりませんが考えられます。</span><span class="sxs-lookup"><span data-stu-id="7aca1-114">In a federated system, a 404 not found is expected as many times the data is only known to one or several, but not all, providers.</span></span>

## <a name="example"></a><span data-ttu-id="7aca1-115">例</span><span class="sxs-lookup"><span data-stu-id="7aca1-115">Example</span></span>

<span data-ttu-id="7aca1-116">ユーザーが求める`security/alerts/{alert_id}`。</span><span class="sxs-lookup"><span data-stu-id="7aca1-116">A user asks for `security/alerts/{alert_id}`.</span></span>

    Provider 1: 404 (provider does not have a record of this alert ID)
    Provider 2: 504 (provider timed out)
    Provider 3: 200 (success)
    Provider 4: 403 (customer has not licensed this provider)

<span data-ttu-id="7aca1-117">404 と 200 の両方が必要な条件であるため warning ヘッダーは、次の含まれています。</span><span class="sxs-lookup"><span data-stu-id="7aca1-117">Because both 404 and 200 are expected conditions, the warning header contains the following:</span></span>

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/10000",    (usual timeout limit is set at 10 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> <span data-ttu-id="7aca1-118">**注:** 各 HTTP ヘッダーは、ユーザーは警告ヘッダーを列挙し、すべての項目をチェックするために、サブ項目のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="7aca1-118">**Note:** Each HTTP header is a collection of subitems, so users can enumerate the Warning header and check all items.</span></span>

## <a name="constraints"></a><span data-ttu-id="7aca1-119">制約</span><span class="sxs-lookup"><span data-stu-id="7aca1-119">Constraints</span></span>

<span data-ttu-id="7aca1-120">`$top` OData クエリ パラメーターには、1000 の警告との組み合わせの制限`$top`  +  `$skip` OData クエリのパラメーターは、警告が 6000 を超えることはできません。</span><span class="sxs-lookup"><span data-stu-id="7aca1-120">The `$top` OData query parameter has a limit of 1000 alerts, and a combination of `$top` + `$skip` OData query parameters cannot exceed 6000 alerts.</span></span> <span data-ttu-id="7aca1-121">などの`/security/alerts?$top=10&$skip=5990`を返します、`200 OK`応答コードの場合が、`/security/alerts?$top=10&$skip=5991`を返します、`400 Bad Request`応答コード。</span><span class="sxs-lookup"><span data-stu-id="7aca1-121">For example, `/security/alerts?$top=10&$skip=5990` will return a `200 OK` response code, but `/security/alerts?$top=10&$skip=5991` will return a `400 Bad Request` response code.</span></span>

<span data-ttu-id="7aca1-122">回避制限値については、使用する、`$filter`で OData クエリのパラメーター、 `eventDateTime` Microsoft グラフ セキュリティ API から通知のエンティティを使用して`?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}`(6000th) の最後の警告で、日時の値を置き換えることです。</span><span class="sxs-lookup"><span data-stu-id="7aca1-122">A work-around for this limit is to use the `$filter` OData query parameter with the `eventDateTime` of the alert entity from the Microsoft Graph Security API, using `?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}` and replacing the dateTime value with the last (6000th) alert.</span></span> <span data-ttu-id="7aca1-123">範囲を設定することも、 `eventDateTime`。たとえば、 *alerts?$ フィルター = eventDateTime **gt** 2018-11-**11**T00:00:00.000Z & eventDateTime **lt** 2018-11-**12**T00:00:00.000Z*</span><span class="sxs-lookup"><span data-stu-id="7aca1-123">You can also set a range for the `eventDateTime`; for example, *alerts?$filter=eventDateTime **gt** 2018-11-**11**T00:00:00.000Z&eventDateTime **lt** 2018-11-**12**T00:00:00.000Z*</span></span>

## <a name="see-also"></a><span data-ttu-id="7aca1-124">関連項目</span><span class="sxs-lookup"><span data-stu-id="7aca1-124">See also</span></span>

<span data-ttu-id="7aca1-125">認証に問題がある場合は、[承認、および Microsoft のグラフのセキュリティ API](/graph/security-authorization)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7aca1-125">If you’re having trouble with authorization, see [Authorization and the Microsoft Graph Security API](/graph/security-authorization).</span></span>
