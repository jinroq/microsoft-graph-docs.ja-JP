---
title: リスト signIns
description: テナントの Azure AD ユーザーのサインインを取得します。 インタラクティブ (ユーザー名とパスワードは認証トークンの一部として渡す) 性質およびフェデレーション サインインが成功には、サインインの問題は現在、サインインがログに含まれます。  最新の signIns が最初に返されます。
ms.openlocfilehash: 3abca59187dcc9667789e33bcefc1bcc51d5ab10
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068090"
---
# <a name="list-signins"></a><span data-ttu-id="eeef7-105">リスト signIns</span><span class="sxs-lookup"><span data-stu-id="eeef7-105">List signIns</span></span>

<span data-ttu-id="eeef7-106">テナントの Azure AD ユーザーのサインインを取得します。</span><span class="sxs-lookup"><span data-stu-id="eeef7-106">Retrieves the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="eeef7-107">インタラクティブ (ユーザー名とパスワードは認証トークンの一部として渡す) 性質およびフェデレーション サインインが成功には、サインインの問題は現在、サインインがログに含まれます。</span><span class="sxs-lookup"><span data-stu-id="eeef7-107">Sign-ins that are interactive in nature (where a username/password is passed as part of authorization token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>  <span data-ttu-id="eeef7-108">最新の signIns が最初に返されます。</span><span class="sxs-lookup"><span data-stu-id="eeef7-108">The most recent signIns are returned first.</span></span>


## <a name="permissions"></a><span data-ttu-id="eeef7-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="eeef7-109">Permissions</span></span>
<span data-ttu-id="eeef7-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eeef7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eeef7-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="eeef7-112">Permission type</span></span>      | <span data-ttu-id="eeef7-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="eeef7-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eeef7-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="eeef7-114">Delegated (work or school account)</span></span> | <span data-ttu-id="eeef7-115">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="eeef7-115">AuditLog.Read.All</span></span> |
|<span data-ttu-id="eeef7-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="eeef7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eeef7-117">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="eeef7-117">Not supported</span></span>   |
|<span data-ttu-id="eeef7-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="eeef7-118">Application</span></span> | <span data-ttu-id="eeef7-119">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="eeef7-119">AuditLog.Read.All</span></span> | 

<span data-ttu-id="eeef7-120">さらに、アプリケーションでは、Azure AD に[適切に登録](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)をする必要があります。</span><span class="sxs-lookup"><span data-stu-id="eeef7-120">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="eeef7-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="eeef7-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="eeef7-122">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="eeef7-122">Optional query parameters</span></span>
<span data-ttu-id="eeef7-123">このメソッドは、応答をカスタマイズするための以下の OData クエリ パラメーターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="eeef7-123">This method supports the following OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="eeef7-124">これらのパラメーターを使用する方法については、 [OData クエリのパラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)を確認してください。</span><span class="sxs-lookup"><span data-stu-id="eeef7-124">Check [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) for how to use these parameters.</span></span>

|<span data-ttu-id="eeef7-125">名前</span><span class="sxs-lookup"><span data-stu-id="eeef7-125">Name</span></span>     |<span data-ttu-id="eeef7-126">説明</span><span class="sxs-lookup"><span data-stu-id="eeef7-126">Description</span></span>                            |<span data-ttu-id="eeef7-127">例</span><span class="sxs-lookup"><span data-stu-id="eeef7-127">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="eeef7-128">$filter</span><span class="sxs-lookup"><span data-stu-id="eeef7-128">$filter</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#filter-parameter)|<span data-ttu-id="eeef7-129">結果 (行) をフィルターします。</span><span class="sxs-lookup"><span data-stu-id="eeef7-129">Filters results (rows).</span></span> |`/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24`
|[<span data-ttu-id="eeef7-130">$top</span><span class="sxs-lookup"><span data-stu-id="eeef7-130">$top</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top-parameter)|<span data-ttu-id="eeef7-131">結果のページ サイズを設定します。</span><span class="sxs-lookup"><span data-stu-id="eeef7-131">Sets the page size of results.</span></span>|`/auditLogs/signIns?$top=1`|
|[<span data-ttu-id="eeef7-132">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="eeef7-132">$skiptoken</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skiptoken-parameter)|<span data-ttu-id="eeef7-133">取得の結果からの結果の次のページを設定するは、複数ページに します。</span><span class="sxs-lookup"><span data-stu-id="eeef7-133">Retrieves the next page of results from result sets that span multiple pages.</span></span>|`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="list-of-attributes-supported-by-filter-parameter"></a><span data-ttu-id="eeef7-134">$Filter パラメーターでサポートされている属性の一覧</span><span class="sxs-lookup"><span data-stu-id="eeef7-134">List of attributes supported by $filter parameter</span></span>
|<span data-ttu-id="eeef7-135">属性名</span><span class="sxs-lookup"><span data-stu-id="eeef7-135">Attribute Name</span></span> |<span data-ttu-id="eeef7-136">サポートされる演算子</span><span class="sxs-lookup"><span data-stu-id="eeef7-136">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="eeef7-137">id</span><span class="sxs-lookup"><span data-stu-id="eeef7-137">id</span></span>|<span data-ttu-id="eeef7-138">eq</span><span class="sxs-lookup"><span data-stu-id="eeef7-138">eq</span></span>|
|<span data-ttu-id="eeef7-139">userId</span><span class="sxs-lookup"><span data-stu-id="eeef7-139">userId</span></span>|<span data-ttu-id="eeef7-140">eq</span><span class="sxs-lookup"><span data-stu-id="eeef7-140">eq</span></span>|
|<span data-ttu-id="eeef7-141">appId</span><span class="sxs-lookup"><span data-stu-id="eeef7-141">appId</span></span>|<span data-ttu-id="eeef7-142">eq</span><span class="sxs-lookup"><span data-stu-id="eeef7-142">eq</span></span>|
|<span data-ttu-id="eeef7-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eeef7-143">createdDateTime</span></span>| <span data-ttu-id="eeef7-144">eq、le、ge</span><span class="sxs-lookup"><span data-stu-id="eeef7-144">eq, le, ge</span></span>|
|<span data-ttu-id="eeef7-145">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="eeef7-145">userDisplayName</span></span>| <span data-ttu-id="eeef7-146">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="eeef7-146">eq, startswith</span></span>|
|<span data-ttu-id="eeef7-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="eeef7-147">userPrincipalName</span></span>| <span data-ttu-id="eeef7-148">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="eeef7-148">eq, startswith</span></span>|
|<span data-ttu-id="eeef7-149">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="eeef7-149">appDisplayName</span></span>| <span data-ttu-id="eeef7-150">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="eeef7-150">eq, startswith</span></span>|
|<span data-ttu-id="eeef7-151">ipAddress</span><span class="sxs-lookup"><span data-stu-id="eeef7-151">ipAddress</span></span>| <span data-ttu-id="eeef7-152">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="eeef7-152">eq, startswith</span></span>|
|<span data-ttu-id="eeef7-153">場所と市区町村</span><span class="sxs-lookup"><span data-stu-id="eeef7-153">location/city</span></span>| <span data-ttu-id="eeef7-154">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="eeef7-154">eq, startswith</span></span>|
|<span data-ttu-id="eeef7-155">場所と状態</span><span class="sxs-lookup"><span data-stu-id="eeef7-155">location/state</span></span>| <span data-ttu-id="eeef7-156">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="eeef7-156">eq, startswith</span></span>|
|<span data-ttu-id="eeef7-157">場所/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="eeef7-157">location/countryOrRegion</span></span>| <span data-ttu-id="eeef7-158">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="eeef7-158">eq, startswith</span></span>|
|<span data-ttu-id="eeef7-159">ステータスまたはエラー コード</span><span class="sxs-lookup"><span data-stu-id="eeef7-159">status/errorCode</span></span>|<span data-ttu-id="eeef7-160">eq</span><span class="sxs-lookup"><span data-stu-id="eeef7-160">eq</span></span>|
|<span data-ttu-id="eeef7-161">initiatedBy、構造体、id のユーザー</span><span class="sxs-lookup"><span data-stu-id="eeef7-161">initiatedBy/user/id</span></span>|<span data-ttu-id="eeef7-162">eq</span><span class="sxs-lookup"><span data-stu-id="eeef7-162">eq</span></span>|
|<span data-ttu-id="eeef7-163">initiatedBy、構造体、displayName ユーザー</span><span class="sxs-lookup"><span data-stu-id="eeef7-163">initiatedBy/user/displayName</span></span>| <span data-ttu-id="eeef7-164">eq</span><span class="sxs-lookup"><span data-stu-id="eeef7-164">eq</span></span>|
|<span data-ttu-id="eeef7-165">userPrincipalName/initiatedBy/ユーザー</span><span class="sxs-lookup"><span data-stu-id="eeef7-165">initiatedBy/user/userPrincipalName</span></span>| <span data-ttu-id="eeef7-166">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="eeef7-166">eq, startswith</span></span>|
|<span data-ttu-id="eeef7-167">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="eeef7-167">clientAppUsed</span></span>| <span data-ttu-id="eeef7-168">eq</span><span class="sxs-lookup"><span data-stu-id="eeef7-168">eq</span></span>|
|<span data-ttu-id="eeef7-169">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="eeef7-169">conditionalAccessStatus</span></span> | <span data-ttu-id="eeef7-170">eq</span><span class="sxs-lookup"><span data-stu-id="eeef7-170">eq</span></span>|
|<span data-ttu-id="eeef7-171">deviceDetail/ブラウザー</span><span class="sxs-lookup"><span data-stu-id="eeef7-171">deviceDetail/browser</span></span>| <span data-ttu-id="eeef7-172">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="eeef7-172">eq, startswith</span></span>|
|<span data-ttu-id="eeef7-173">deviceDetail/ル</span><span class="sxs-lookup"><span data-stu-id="eeef7-173">deviceDetail/operatingSystem</span></span>| <span data-ttu-id="eeef7-174">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="eeef7-174">eq, startswith</span></span>|
|<span data-ttu-id="eeef7-175">correlationId</span><span class="sxs-lookup"><span data-stu-id="eeef7-175">correlationId</span></span>| <span data-ttu-id="eeef7-176">eq</span><span class="sxs-lookup"><span data-stu-id="eeef7-176">eq</span></span>|
|<span data-ttu-id="eeef7-177">riskDetail</span><span class="sxs-lookup"><span data-stu-id="eeef7-177">riskDetail</span></span>| <span data-ttu-id="eeef7-178">eq</span><span class="sxs-lookup"><span data-stu-id="eeef7-178">eq</span></span>|
|<span data-ttu-id="eeef7-179">riskLevelAggregated</span><span class="sxs-lookup"><span data-stu-id="eeef7-179">riskLevelAggregated</span></span>| <span data-ttu-id="eeef7-180">eq</span><span class="sxs-lookup"><span data-stu-id="eeef7-180">eq</span></span>|
|<span data-ttu-id="eeef7-181">riskLevelDuringSignIn</span><span class="sxs-lookup"><span data-stu-id="eeef7-181">riskLevelDuringSignIn</span></span>| <span data-ttu-id="eeef7-182">eq</span><span class="sxs-lookup"><span data-stu-id="eeef7-182">eq</span></span>|
|<span data-ttu-id="eeef7-183">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="eeef7-183">riskEventTypes</span></span>| <span data-ttu-id="eeef7-184">eq</span><span class="sxs-lookup"><span data-stu-id="eeef7-184">eq</span></span>|
|<span data-ttu-id="eeef7-185">riskState</span><span class="sxs-lookup"><span data-stu-id="eeef7-185">riskState</span></span>| <span data-ttu-id="eeef7-186">eq</span><span class="sxs-lookup"><span data-stu-id="eeef7-186">eq</span></span>|
|<span data-ttu-id="eeef7-187">originalRequestId</span><span class="sxs-lookup"><span data-stu-id="eeef7-187">originalRequestId</span></span>| <span data-ttu-id="eeef7-188">eq</span><span class="sxs-lookup"><span data-stu-id="eeef7-188">eq</span></span>|
|<span data-ttu-id="eeef7-189">tokenIssuerName</span><span class="sxs-lookup"><span data-stu-id="eeef7-189">tokenIssuerName</span></span>| <span data-ttu-id="eeef7-190">eq</span><span class="sxs-lookup"><span data-stu-id="eeef7-190">eq</span></span>|
|<span data-ttu-id="eeef7-191">tokenIssuerType</span><span class="sxs-lookup"><span data-stu-id="eeef7-191">tokenIssuerType</span></span>| <span data-ttu-id="eeef7-192">eq</span><span class="sxs-lookup"><span data-stu-id="eeef7-192">eq</span></span>|
|<span data-ttu-id="eeef7-193">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="eeef7-193">resourceDisplayName</span></span>| <span data-ttu-id="eeef7-194">eq</span><span class="sxs-lookup"><span data-stu-id="eeef7-194">eq</span></span>|
|<span data-ttu-id="eeef7-195">resourceId</span><span class="sxs-lookup"><span data-stu-id="eeef7-195">resourceId</span></span>| <span data-ttu-id="eeef7-196">eq</span><span class="sxs-lookup"><span data-stu-id="eeef7-196">eq</span></span>|


## <a name="response"></a><span data-ttu-id="eeef7-197">応答</span><span class="sxs-lookup"><span data-stu-id="eeef7-197">Response</span></span>
<span data-ttu-id="eeef7-198">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本体での[サインイン](../resources/signin.md)のオブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="eeef7-198">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eeef7-199">例</span><span class="sxs-lookup"><span data-stu-id="eeef7-199">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eeef7-200">要求</span><span class="sxs-lookup"><span data-stu-id="eeef7-200">Request</span></span>
<span data-ttu-id="eeef7-201">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="eeef7-201">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_signins"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
##### <a name="response"></a><span data-ttu-id="eeef7-202">応答</span><span class="sxs-lookup"><span data-stu-id="eeef7-202">Response</span></span>
<span data-ttu-id="eeef7-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="eeef7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 264
```
```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/signIns",
    "value": [{
        "id":"b01b1726-0147-425e-a7f7-21f252050400",
        "createdDateTime":"2018-11-06T18:48:33.8527147Z",
        "userDisplayName":"Jon Doe",
         "userPrincipalName":"admin@aad171.ccsctp.net",
         "userId":"d7cc485d-2c1b-422c-98fd-5ce52859a4a3",
        "appId":"c44b4083-3bb0-49c1-b47d-974e53cbdf3c",
         "appDisplayName":"Azure Portal",
         "ipAddress":"207.254.19.10",
         "clientAppUsed":"Browser",
        "mfaDetail":null,
         "correlationId":"65dd87ce-2183-419e-81a9-d6e20379bcc2",
         "conditionalAccessStatus":"notApplied",
        "originalRequestId":null,
        "isInteractive":true,
        "tokenIssuerName":null,
        "tokenIssuerType":"AzureAD",
        "processingTimeInMilliseconds":0,
        "riskDetail":"none",
        "riskLevelAggregated":"none",
        "riskLevelDuringSignIn":"none",
        "riskState":"none",
        "riskEventTypes":[

        ],
        "resourceDisplayName":"windows azure service management api",
        "resourceId":"797f4846-ba00-4fd7-ba43-dac1f8f63013",
        "authenticationMethodsUsed":[

        ],
        "status":{
            "errorCode":50140,
            "failureReason":"This error occurred due to 'Keep me signed in' interrupt when the user was signing-in.",
            "additionalDetails":null
        },
        "deviceDetail":{
            "deviceId":null,
            "displayName":null,
            "operatingSystem":"Windows 7",
            "browser":"Chrome 63.0.3239",
            "isCompliant":null,
            "isManaged":null,
            "trustType":null
        },
        "location":{
            "city":"Lithia Springs",
            "state":"Georgia",
            "countryOrRegion":"US",
            "geoCoordinates":{
                "altitude":null,
                "latitude":33.7930908203125,
                "longitude":-84.445358276367188
            }
        },
        "appliedConditionalAccessPolicies":[
            {
            "id":"6551c58c-e5da-4036-a6ea-c2c3fad264f1",
            "displayName":"New Name here4",
            "enforcedGrantControls":[
                "Mfa",
                "RequireCompliantDevice"
            ],
            "enforcedSessionControls":[

            ],
            "result":"notApplied"
            },
            {
            "id":"b645a140-20fe-4ce0-a724-18ab201e9026",
            "displayName":"PipelineTest4",
            "enforcedGrantControls":[

            ],
            "enforcedSessionControls":[

            ],
            "result":"notEnabled"
            }
        ],
        "authenticationProcessingDetails":[

        ],
        "networkLocationDetails":[

        ]
        }
    
    ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List signIns",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
