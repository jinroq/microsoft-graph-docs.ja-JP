---
title: Microsoft Graph セキュリティ API のエラー応答
description: Microsoft Graph セキュリティ API のエラーは、標準の HTTP 206 の部分的なコンテンツ状態コードを使用して返され、警告ヘッダーによって配信されます。
author: preetikr
localization_priority: Normal
ms.prod: security
doc_type: conceptualPageType
ms.openlocfilehash: 2d77a0f21623a98e4041b845e92a23c7574a415d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008559"
---
# <a name="microsoft-graph-security-api-error-responses"></a><span data-ttu-id="3e450-103">Microsoft Graph セキュリティ API のエラー応答</span><span class="sxs-lookup"><span data-stu-id="3e450-103">Microsoft Graph Security API error responses</span></span>

<span data-ttu-id="3e450-104">Microsoft Graph セキュリティ API のエラーは、標準の HTTP 206 の部分的なコンテンツ状態コードを使用して返され、警告ヘッダーによって配信されます。</span><span class="sxs-lookup"><span data-stu-id="3e450-104">Errors in the Microsoft Graph Security API are returned using the standard HTTP 206 Partial Content status code and are delivered via a warning header.</span></span>

## <a name="errors"></a><span data-ttu-id="3e450-105">Errors</span><span class="sxs-lookup"><span data-stu-id="3e450-105">Errors</span></span>

<span data-ttu-id="3e450-106">Microsoft Graph セキュリティ API は、すべてのデータプロバイダーから複数の応答を受け取るフェデレーションサービスです。</span><span class="sxs-lookup"><span data-stu-id="3e450-106">The Microsoft Graph Security API is a federated service that receives multiple responses from all data providers.</span></span> <span data-ttu-id="3e450-107">Microsoft Graph セキュリティ API で HTTP エラーが受信されると、次の形式の警告ヘッダーが返されます。</span><span class="sxs-lookup"><span data-stu-id="3e450-107">When an HTTP error is received by the Microsoft Graph Security API, it will send back a warning header in the following format:</span></span>
<!-- { "blockType": "ignored" } -->

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

<span data-ttu-id="3e450-108">この警告ヘッダーは、いずれかのデータプロバイダーが2xx または404以外のエラーコードを返した場合にのみクライアントに返されます。</span><span class="sxs-lookup"><span data-stu-id="3e450-108">This warning header is only sent back to clients when one of the data providers returns an error code other than 2xx or 404.</span></span> <span data-ttu-id="3e450-109">次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="3e450-109">For example:</span></span>

- <span data-ttu-id="3e450-110">リソースへのアクセス許可が付与されていない場合、HttpStatusCode (403) が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3e450-110">HttpStatusCode.Forbidden (403) might be returned if the access to the resource is not granted.</span></span>
- <span data-ttu-id="3e450-111">プロバイダーがタイムアウトになると、HttpStatusCode (504) が警告ヘッダーに返されます。</span><span class="sxs-lookup"><span data-stu-id="3e450-111">If a provider times out, HttpStatusCode.GatewayTimeout (504) is returned in the warning header.</span></span>
- <span data-ttu-id="3e450-112">内部プロバイダエラーが発生した場合は、HttpStatusCode エラー (500) が警告ヘッダーで使用されます。</span><span class="sxs-lookup"><span data-stu-id="3e450-112">If an internal provider error happens, HttpStatusCode.InternalServerError (500) is used in the warning header.</span></span>

<span data-ttu-id="3e450-113">データプロバイダーが2xx または404を返した場合は、これらのコードが正常に終了したか、またはデータが検出されなかった場合は、警告ヘッダーに表示されません。</span><span class="sxs-lookup"><span data-stu-id="3e450-113">If a data provider returns 2xx or 404, it’s not shown in the warning header because these codes are expected for success or when data is not found respectively.</span></span> <span data-ttu-id="3e450-114">フェデレーションシステムでは、404が見つからない場合は、1つまたはいくつかのプロバイダーのみがデータを認識できる回数である必要があります。</span><span class="sxs-lookup"><span data-stu-id="3e450-114">In a federated system, a 404 not found is expected as many times the data is only known to one or several, but not all, providers.</span></span>

## <a name="example"></a><span data-ttu-id="3e450-115">例</span><span class="sxs-lookup"><span data-stu-id="3e450-115">Example</span></span>

<span data-ttu-id="3e450-116">ユーザーが要求`security/alerts/{alert_id}`します。</span><span class="sxs-lookup"><span data-stu-id="3e450-116">A user asks for `security/alerts/{alert_id}`.</span></span>

    Provider 1: 404 (provider does not have a record of this alert ID)
    Provider 2: 504 (provider timed out)
    Provider 3: 200 (success)
    Provider 4: 403 (customer has not licensed this provider)

<span data-ttu-id="3e450-117">404と200の両方が想定される条件であるため、警告ヘッダーには次の内容が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3e450-117">Because both 404 and 200 are expected conditions, the warning header contains the following:</span></span>

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/10000",    (usual timeout limit is set at 10 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> <span data-ttu-id="3e450-118">**注:** 各 HTTP ヘッダーはサブアイテムのコレクションであるため、ユーザーは警告ヘッダーを列挙してすべてのアイテムをチェックできます。</span><span class="sxs-lookup"><span data-stu-id="3e450-118">**Note:** Each HTTP header is a collection of subitems, so users can enumerate the Warning header and check all items.</span></span>

## <a name="constraints"></a><span data-ttu-id="3e450-119">制約</span><span class="sxs-lookup"><span data-stu-id="3e450-119">Constraints</span></span>

<span data-ttu-id="3e450-120">`$top` Odata クエリパラメーターには、1000通知の制限があり、odata クエリ`$top`  +  `$skip`パラメーターの組み合わせは、6000通知を超えることはできません。</span><span class="sxs-lookup"><span data-stu-id="3e450-120">The `$top` OData query parameter has a limit of 1000 alerts, and a combination of `$top` + `$skip` OData query parameters cannot exceed 6000 alerts.</span></span> <span data-ttu-id="3e450-121">例えば、`/security/alerts?$top=10&$skip=5990` は応答コード `200 OK` を返しますが、`/security/alerts?$top=10&$skip=5991` は応答コード `400 Bad Request` を返します。</span><span class="sxs-lookup"><span data-stu-id="3e450-121">For example, `/security/alerts?$top=10&$skip=5990` will return a `200 OK` response code, but `/security/alerts?$top=10&$skip=5991` will return a `400 Bad Request` response code.</span></span>

<span data-ttu-id="3e450-122">この制限の回避策は、 `$filter` OData クエリパラメーターを Microsoft GRAPH セキュリティ API の`eventDateTime` alert エンティティので使用し、dateTime 値を`?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}`最後 (6000th) 通知で置き換えることです。</span><span class="sxs-lookup"><span data-stu-id="3e450-122">A work-around for this limit is to use the `$filter` OData query parameter with the `eventDateTime` of the alert entity from the Microsoft Graph Security API, using `?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}` and replacing the dateTime value with the last (6000th) alert.</span></span> <span data-ttu-id="3e450-123">また、 `eventDateTime`の範囲を設定することもできます。たとえば、*警告? $filter = eventdatetime **gt** 2018-11-**11**T00:00: 00.000 z&eventdatetime **lt** 2018-11-**12**T00:00: 00.000 z*</span><span class="sxs-lookup"><span data-stu-id="3e450-123">You can also set a range for the `eventDateTime`; for example, *alerts?$filter=eventDateTime **gt** 2018-11-**11**T00:00:00.000Z&eventDateTime **lt** 2018-11-**12**T00:00:00.000Z*</span></span>

## <a name="see-also"></a><span data-ttu-id="3e450-124">関連項目</span><span class="sxs-lookup"><span data-stu-id="3e450-124">See also</span></span>

<span data-ttu-id="3e450-125">承認の問題が発生している場合は、「 [authorization and The Microsoft Graph SECURITY API](/graph/security-authorization)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3e450-125">If you’re having trouble with authorization, see [Authorization and the Microsoft Graph Security API](/graph/security-authorization).</span></span>
