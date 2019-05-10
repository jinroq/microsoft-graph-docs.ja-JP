---
title: signIns を一覧表示する
description: ディレクトリ (テナント) のアクティビティ (ベータ版) を監査するための、Microsoft Graph API (REST) の signIn リソース (エンティティ) を一覧表示する方法について説明します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fdb1358d36a0e1da34779de5505c5f18f901e681
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638684"
---
# <a name="list-signins"></a><span data-ttu-id="81369-103">signIn を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="81369-103">List signIns</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81369-104">テナントの Azure AD ユーザーのサインインを取得します。</span><span class="sxs-lookup"><span data-stu-id="81369-104">Retrieves the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="81369-105">本来対話型のサイイン (ユーザー名とパスワードが認証トークンの一部として渡される場合) と、成功したフェデレーション サインインは、現在サインイン ログに含まれています。</span><span class="sxs-lookup"><span data-stu-id="81369-105">Sign-ins that are interactive in nature (where a username/password is passed as part of authorization token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>  <span data-ttu-id="81369-106">最新の signIns が最初に返されます。</span><span class="sxs-lookup"><span data-stu-id="81369-106">The most recent signIns are returned first.</span></span>

## <a name="permissions"></a><span data-ttu-id="81369-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="81369-107">Permissions</span></span>

<span data-ttu-id="81369-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="81369-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81369-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="81369-110">Permission type</span></span>      | <span data-ttu-id="81369-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="81369-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81369-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="81369-112">Delegated (work or school account)</span></span> | <span data-ttu-id="81369-113">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="81369-113">AuditLog.Read.All</span></span> |
|<span data-ttu-id="81369-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="81369-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81369-115">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="81369-115">Not supported</span></span>   |
|<span data-ttu-id="81369-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="81369-116">Application</span></span> | <span data-ttu-id="81369-117">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="81369-117">AuditLog.Read.All</span></span> | 

<span data-ttu-id="81369-118">また、アプリは Azure AD に[正しく登録されている](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)必要があります。</span><span class="sxs-lookup"><span data-stu-id="81369-118">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="81369-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="81369-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="81369-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="81369-120">Optional query parameters</span></span>
<span data-ttu-id="81369-121">このメソッドは、応答をカスタマイズするための以下の OData クエリ パラメーターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="81369-121">This method supports the following OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="81369-122">これらのパラメーターを使用する方法の詳細については、[OData クエリ パラメーター](/graph/query_parameters)をご確認ください。</span><span class="sxs-lookup"><span data-stu-id="81369-122">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

|<span data-ttu-id="81369-123">Name</span><span class="sxs-lookup"><span data-stu-id="81369-123">Name</span></span>     |<span data-ttu-id="81369-124">説明</span><span class="sxs-lookup"><span data-stu-id="81369-124">Description</span></span>                            |<span data-ttu-id="81369-125">例</span><span class="sxs-lookup"><span data-stu-id="81369-125">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="81369-126">$filter</span><span class="sxs-lookup"><span data-stu-id="81369-126">$filter</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#filter-parameter)|<span data-ttu-id="81369-127">結果 (行) をフィルターします。</span><span class="sxs-lookup"><span data-stu-id="81369-127">Filters results (rows).</span></span> |`/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24`
|[<span data-ttu-id="81369-128">$top</span><span class="sxs-lookup"><span data-stu-id="81369-128">$top</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top-parameter)|<span data-ttu-id="81369-129">結果のページ サイズを設定します。</span><span class="sxs-lookup"><span data-stu-id="81369-129">Sets the page size of results.</span></span>|`/auditLogs/signIns?$top=1`|
|[<span data-ttu-id="81369-130">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="81369-130">$skiptoken</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skiptoken-parameter)|<span data-ttu-id="81369-131">複数ページにわたる結果セットから、結果の次のページを取得します。</span><span class="sxs-lookup"><span data-stu-id="81369-131">Retrieves the next page of results from result sets that span multiple pages.</span></span>|`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="list-of-attributes-supported-by-filter-parameter"></a><span data-ttu-id="81369-132">$Filter パラメーターにサポートされる属性の一覧</span><span class="sxs-lookup"><span data-stu-id="81369-132">List of attributes supported by $filter parameter</span></span>
|<span data-ttu-id="81369-133">属性名</span><span class="sxs-lookup"><span data-stu-id="81369-133">Attribute Name</span></span> |<span data-ttu-id="81369-134">サポートされる演算子</span><span class="sxs-lookup"><span data-stu-id="81369-134">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="81369-135">id</span><span class="sxs-lookup"><span data-stu-id="81369-135">id</span></span>|<span data-ttu-id="81369-136">eq</span><span class="sxs-lookup"><span data-stu-id="81369-136">eq</span></span>|
|<span data-ttu-id="81369-137">userId</span><span class="sxs-lookup"><span data-stu-id="81369-137">userId</span></span>|<span data-ttu-id="81369-138">eq</span><span class="sxs-lookup"><span data-stu-id="81369-138">eq</span></span>|
|<span data-ttu-id="81369-139">appId</span><span class="sxs-lookup"><span data-stu-id="81369-139">appId</span></span>|<span data-ttu-id="81369-140">eq</span><span class="sxs-lookup"><span data-stu-id="81369-140">eq</span></span>|
|<span data-ttu-id="81369-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="81369-141">createdDateTime</span></span>| <span data-ttu-id="81369-142">eq、le、ge</span><span class="sxs-lookup"><span data-stu-id="81369-142">eq, le, ge</span></span>|
|<span data-ttu-id="81369-143">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="81369-143">userDisplayName</span></span>| <span data-ttu-id="81369-144">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="81369-144">eq, startswith</span></span>|
|<span data-ttu-id="81369-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="81369-145">userPrincipalName</span></span>| <span data-ttu-id="81369-146">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="81369-146">eq, startswith</span></span>|
|<span data-ttu-id="81369-147">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="81369-147">appDisplayName</span></span>| <span data-ttu-id="81369-148">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="81369-148">eq, startswith</span></span>|
|<span data-ttu-id="81369-149">ipAddress</span><span class="sxs-lookup"><span data-stu-id="81369-149">ipAddress</span></span>| <span data-ttu-id="81369-150">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="81369-150">eq, startswith</span></span>|
|<span data-ttu-id="81369-151">location/city</span><span class="sxs-lookup"><span data-stu-id="81369-151">location/city</span></span>| <span data-ttu-id="81369-152">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="81369-152">eq, startswith</span></span>|
|<span data-ttu-id="81369-153">location/state</span><span class="sxs-lookup"><span data-stu-id="81369-153">location/state</span></span>| <span data-ttu-id="81369-154">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="81369-154">eq, startswith</span></span>|
|<span data-ttu-id="81369-155">location/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="81369-155">location/countryOrRegion</span></span>| <span data-ttu-id="81369-156">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="81369-156">eq, startswith</span></span>|
|<span data-ttu-id="81369-157">status/errorCode</span><span class="sxs-lookup"><span data-stu-id="81369-157">status/errorCode</span></span>|<span data-ttu-id="81369-158">eq</span><span class="sxs-lookup"><span data-stu-id="81369-158">eq</span></span>|
|<span data-ttu-id="81369-159">initiatedBy/user/id</span><span class="sxs-lookup"><span data-stu-id="81369-159">initiatedBy/user/id</span></span>|<span data-ttu-id="81369-160">eq</span><span class="sxs-lookup"><span data-stu-id="81369-160">eq</span></span>|
|<span data-ttu-id="81369-161">initiatedBy/user/displayName</span><span class="sxs-lookup"><span data-stu-id="81369-161">initiatedBy/user/displayName</span></span>| <span data-ttu-id="81369-162">eq</span><span class="sxs-lookup"><span data-stu-id="81369-162">eq</span></span>|
|<span data-ttu-id="81369-163">initiatedBy/user/userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="81369-163">initiatedBy/user/userPrincipalName</span></span>| <span data-ttu-id="81369-164">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="81369-164">eq, startswith</span></span>|
|<span data-ttu-id="81369-165">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="81369-165">clientAppUsed</span></span>| <span data-ttu-id="81369-166">eq</span><span class="sxs-lookup"><span data-stu-id="81369-166">eq</span></span>|
|<span data-ttu-id="81369-167">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="81369-167">conditionalAccessStatus</span></span> | <span data-ttu-id="81369-168">eq</span><span class="sxs-lookup"><span data-stu-id="81369-168">eq</span></span>|
|<span data-ttu-id="81369-169">deviceDetail/browser</span><span class="sxs-lookup"><span data-stu-id="81369-169">deviceDetail/browser</span></span>| <span data-ttu-id="81369-170">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="81369-170">eq, startswith</span></span>|
|<span data-ttu-id="81369-171">deviceDetail/operatingSystem</span><span class="sxs-lookup"><span data-stu-id="81369-171">deviceDetail/operatingSystem</span></span>| <span data-ttu-id="81369-172">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="81369-172">eq, startswith</span></span>|
|<span data-ttu-id="81369-173">correlationId</span><span class="sxs-lookup"><span data-stu-id="81369-173">correlationId</span></span>| <span data-ttu-id="81369-174">eq</span><span class="sxs-lookup"><span data-stu-id="81369-174">eq</span></span>|
|<span data-ttu-id="81369-175">riskDetail</span><span class="sxs-lookup"><span data-stu-id="81369-175">riskDetail</span></span>| <span data-ttu-id="81369-176">eq</span><span class="sxs-lookup"><span data-stu-id="81369-176">eq</span></span>|
|<span data-ttu-id="81369-177">riskLevelAggregated</span><span class="sxs-lookup"><span data-stu-id="81369-177">riskLevelAggregated</span></span>| <span data-ttu-id="81369-178">eq</span><span class="sxs-lookup"><span data-stu-id="81369-178">eq</span></span>|
|<span data-ttu-id="81369-179">riskLevelDuringSignIn</span><span class="sxs-lookup"><span data-stu-id="81369-179">riskLevelDuringSignIn</span></span>| <span data-ttu-id="81369-180">eq</span><span class="sxs-lookup"><span data-stu-id="81369-180">eq</span></span>|
|<span data-ttu-id="81369-181">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="81369-181">riskEventTypes</span></span>| <span data-ttu-id="81369-182">eq</span><span class="sxs-lookup"><span data-stu-id="81369-182">eq</span></span>|
|<span data-ttu-id="81369-183">riskState</span><span class="sxs-lookup"><span data-stu-id="81369-183">riskState</span></span>| <span data-ttu-id="81369-184">eq</span><span class="sxs-lookup"><span data-stu-id="81369-184">eq</span></span>|
|<span data-ttu-id="81369-185">originalRequestId</span><span class="sxs-lookup"><span data-stu-id="81369-185">originalRequestId</span></span>| <span data-ttu-id="81369-186">eq</span><span class="sxs-lookup"><span data-stu-id="81369-186">eq</span></span>|
|<span data-ttu-id="81369-187">tokenIssuerName</span><span class="sxs-lookup"><span data-stu-id="81369-187">tokenIssuerName</span></span>| <span data-ttu-id="81369-188">eq</span><span class="sxs-lookup"><span data-stu-id="81369-188">eq</span></span>|
|<span data-ttu-id="81369-189">tokenIssuerType</span><span class="sxs-lookup"><span data-stu-id="81369-189">tokenIssuerType</span></span>| <span data-ttu-id="81369-190">eq</span><span class="sxs-lookup"><span data-stu-id="81369-190">eq</span></span>|
|<span data-ttu-id="81369-191">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="81369-191">resourceDisplayName</span></span>| <span data-ttu-id="81369-192">eq</span><span class="sxs-lookup"><span data-stu-id="81369-192">eq</span></span>|
|<span data-ttu-id="81369-193">resourceId</span><span class="sxs-lookup"><span data-stu-id="81369-193">resourceId</span></span>| <span data-ttu-id="81369-194">eq</span><span class="sxs-lookup"><span data-stu-id="81369-194">eq</span></span>|


## <a name="response"></a><span data-ttu-id="81369-195">応答</span><span class="sxs-lookup"><span data-stu-id="81369-195">Response</span></span>
<span data-ttu-id="81369-196">成功した場合、このメソッドは `200 OK` 応答コードと、[signIn](../resources/signin.md) オブジェクトのコレクションを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="81369-196">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="81369-197">例</span><span class="sxs-lookup"><span data-stu-id="81369-197">Example</span></span>
##### <a name="request"></a><span data-ttu-id="81369-198">要求</span><span class="sxs-lookup"><span data-stu-id="81369-198">Request</span></span>
<span data-ttu-id="81369-199">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="81369-199">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_signins"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
##### <a name="response"></a><span data-ttu-id="81369-200">応答</span><span class="sxs-lookup"><span data-stu-id="81369-200">Response</span></span>
<span data-ttu-id="81369-201">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="81369-201">Here is an example of the response.</span></span> 

><span data-ttu-id="81369-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="81369-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="81369-204">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="81369-204">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="81369-205">C#</span><span class="sxs-lookup"><span data-stu-id="81369-205">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_signins-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="81369-206">Javascript</span><span class="sxs-lookup"><span data-stu-id="81369-206">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_signins-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
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
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/signin-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/signin-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
