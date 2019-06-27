---
title: signIns を一覧表示する
description: ディレクトリ (テナント) のアクティビティ (ベータ版) を監査するための、Microsoft Graph API (REST) の signIn リソース (エンティティ) を一覧表示する方法について説明します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e352a6ede72ef5e6b2b776e9f177680760bed0de
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271632"
---
# <a name="list-signins"></a><span data-ttu-id="105fd-103">signIn を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="105fd-103">List signIns</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="105fd-104">テナントの Azure AD ユーザーのサインインを取得します。</span><span class="sxs-lookup"><span data-stu-id="105fd-104">Retrieve the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="105fd-105">本来対話型のサイイン (ユーザー名とパスワードが認証トークンの一部として渡される場合) と、成功したフェデレーション サインインは、現在サインイン ログに含まれています。</span><span class="sxs-lookup"><span data-stu-id="105fd-105">Sign-ins that are interactive in nature (where a username/password is passed as part of authorization token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>  <span data-ttu-id="105fd-106">最新の signIns が最初に返されます。</span><span class="sxs-lookup"><span data-stu-id="105fd-106">The most recent signIns are returned first.</span></span>

## <a name="permissions"></a><span data-ttu-id="105fd-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="105fd-107">Permissions</span></span>

<span data-ttu-id="105fd-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="105fd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="105fd-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="105fd-110">Permission type</span></span>      | <span data-ttu-id="105fd-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="105fd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="105fd-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="105fd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="105fd-113">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="105fd-113">AuditLog.Read.All</span></span> |
|<span data-ttu-id="105fd-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="105fd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="105fd-115">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="105fd-115">Not supported</span></span>   |
|<span data-ttu-id="105fd-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="105fd-116">Application</span></span> | <span data-ttu-id="105fd-117">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="105fd-117">AuditLog.Read.All</span></span> | 

<span data-ttu-id="105fd-118">また、アプリは Azure AD に[正しく登録されている](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)必要があります。</span><span class="sxs-lookup"><span data-stu-id="105fd-118">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="105fd-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="105fd-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="105fd-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="105fd-120">Optional query parameters</span></span>
<span data-ttu-id="105fd-121">このメソッドは、応答をカスタマイズするための以下の OData クエリ パラメーターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="105fd-121">This method supports the following OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="105fd-122">これらのパラメーターを使用する方法の詳細については、[OData クエリ パラメーター](/graph/query_parameters)をご確認ください。</span><span class="sxs-lookup"><span data-stu-id="105fd-122">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

|<span data-ttu-id="105fd-123">Name</span><span class="sxs-lookup"><span data-stu-id="105fd-123">Name</span></span>     |<span data-ttu-id="105fd-124">説明</span><span class="sxs-lookup"><span data-stu-id="105fd-124">Description</span></span>                            |<span data-ttu-id="105fd-125">例</span><span class="sxs-lookup"><span data-stu-id="105fd-125">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="105fd-126">$filter</span><span class="sxs-lookup"><span data-stu-id="105fd-126">$filter</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#filter-parameter)|<span data-ttu-id="105fd-127">結果 (行) をフィルターします。</span><span class="sxs-lookup"><span data-stu-id="105fd-127">Filters results (rows).</span></span> |`/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24`
|[<span data-ttu-id="105fd-128">$top</span><span class="sxs-lookup"><span data-stu-id="105fd-128">$top</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top-parameter)|<span data-ttu-id="105fd-129">結果のページ サイズを設定します。</span><span class="sxs-lookup"><span data-stu-id="105fd-129">Sets the page size of results.</span></span>|`/auditLogs/signIns?$top=1`|
|[<span data-ttu-id="105fd-130">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="105fd-130">$skiptoken</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skiptoken-parameter)|<span data-ttu-id="105fd-131">複数ページにわたる結果セットから、結果の次のページを取得します。</span><span class="sxs-lookup"><span data-stu-id="105fd-131">Retrieves the next page of results from result sets that span multiple pages.</span></span>|`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="list-of-attributes-supported-by-filter-parameter"></a><span data-ttu-id="105fd-132">$Filter パラメーターにサポートされる属性の一覧</span><span class="sxs-lookup"><span data-stu-id="105fd-132">List of attributes supported by $filter parameter</span></span>
|<span data-ttu-id="105fd-133">属性名</span><span class="sxs-lookup"><span data-stu-id="105fd-133">Attribute Name</span></span> |<span data-ttu-id="105fd-134">サポートされる演算子</span><span class="sxs-lookup"><span data-stu-id="105fd-134">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="105fd-135">id</span><span class="sxs-lookup"><span data-stu-id="105fd-135">id</span></span>|<span data-ttu-id="105fd-136">eq</span><span class="sxs-lookup"><span data-stu-id="105fd-136">eq</span></span>|
|<span data-ttu-id="105fd-137">userId</span><span class="sxs-lookup"><span data-stu-id="105fd-137">userId</span></span>|<span data-ttu-id="105fd-138">eq</span><span class="sxs-lookup"><span data-stu-id="105fd-138">eq</span></span>|
|<span data-ttu-id="105fd-139">appId</span><span class="sxs-lookup"><span data-stu-id="105fd-139">appId</span></span>|<span data-ttu-id="105fd-140">eq</span><span class="sxs-lookup"><span data-stu-id="105fd-140">eq</span></span>|
|<span data-ttu-id="105fd-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="105fd-141">createdDateTime</span></span>| <span data-ttu-id="105fd-142">eq、le、ge</span><span class="sxs-lookup"><span data-stu-id="105fd-142">eq, le, ge</span></span>|
|<span data-ttu-id="105fd-143">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="105fd-143">userDisplayName</span></span>| <span data-ttu-id="105fd-144">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="105fd-144">eq, startswith</span></span>|
|<span data-ttu-id="105fd-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="105fd-145">userPrincipalName</span></span>| <span data-ttu-id="105fd-146">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="105fd-146">eq, startswith</span></span>|
|<span data-ttu-id="105fd-147">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="105fd-147">appDisplayName</span></span>| <span data-ttu-id="105fd-148">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="105fd-148">eq, startswith</span></span>|
|<span data-ttu-id="105fd-149">ipAddress</span><span class="sxs-lookup"><span data-stu-id="105fd-149">ipAddress</span></span>| <span data-ttu-id="105fd-150">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="105fd-150">eq, startswith</span></span>|
|<span data-ttu-id="105fd-151">location/city</span><span class="sxs-lookup"><span data-stu-id="105fd-151">location/city</span></span>| <span data-ttu-id="105fd-152">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="105fd-152">eq, startswith</span></span>|
|<span data-ttu-id="105fd-153">location/state</span><span class="sxs-lookup"><span data-stu-id="105fd-153">location/state</span></span>| <span data-ttu-id="105fd-154">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="105fd-154">eq, startswith</span></span>|
|<span data-ttu-id="105fd-155">location/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="105fd-155">location/countryOrRegion</span></span>| <span data-ttu-id="105fd-156">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="105fd-156">eq, startswith</span></span>|
|<span data-ttu-id="105fd-157">status/errorCode</span><span class="sxs-lookup"><span data-stu-id="105fd-157">status/errorCode</span></span>|<span data-ttu-id="105fd-158">eq</span><span class="sxs-lookup"><span data-stu-id="105fd-158">eq</span></span>|
|<span data-ttu-id="105fd-159">initiatedBy/user/id</span><span class="sxs-lookup"><span data-stu-id="105fd-159">initiatedBy/user/id</span></span>|<span data-ttu-id="105fd-160">eq</span><span class="sxs-lookup"><span data-stu-id="105fd-160">eq</span></span>|
|<span data-ttu-id="105fd-161">initiatedBy/user/displayName</span><span class="sxs-lookup"><span data-stu-id="105fd-161">initiatedBy/user/displayName</span></span>| <span data-ttu-id="105fd-162">eq</span><span class="sxs-lookup"><span data-stu-id="105fd-162">eq</span></span>|
|<span data-ttu-id="105fd-163">initiatedBy/user/userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="105fd-163">initiatedBy/user/userPrincipalName</span></span>| <span data-ttu-id="105fd-164">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="105fd-164">eq, startswith</span></span>|
|<span data-ttu-id="105fd-165">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="105fd-165">clientAppUsed</span></span>| <span data-ttu-id="105fd-166">eq</span><span class="sxs-lookup"><span data-stu-id="105fd-166">eq</span></span>|
|<span data-ttu-id="105fd-167">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="105fd-167">conditionalAccessStatus</span></span> | <span data-ttu-id="105fd-168">eq</span><span class="sxs-lookup"><span data-stu-id="105fd-168">eq</span></span>|
|<span data-ttu-id="105fd-169">deviceDetail/browser</span><span class="sxs-lookup"><span data-stu-id="105fd-169">deviceDetail/browser</span></span>| <span data-ttu-id="105fd-170">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="105fd-170">eq, startswith</span></span>|
|<span data-ttu-id="105fd-171">deviceDetail/operatingSystem</span><span class="sxs-lookup"><span data-stu-id="105fd-171">deviceDetail/operatingSystem</span></span>| <span data-ttu-id="105fd-172">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="105fd-172">eq, startswith</span></span>|
|<span data-ttu-id="105fd-173">correlationId</span><span class="sxs-lookup"><span data-stu-id="105fd-173">correlationId</span></span>| <span data-ttu-id="105fd-174">eq</span><span class="sxs-lookup"><span data-stu-id="105fd-174">eq</span></span>|
|<span data-ttu-id="105fd-175">riskDetail</span><span class="sxs-lookup"><span data-stu-id="105fd-175">riskDetail</span></span>| <span data-ttu-id="105fd-176">eq</span><span class="sxs-lookup"><span data-stu-id="105fd-176">eq</span></span>|
|<span data-ttu-id="105fd-177">riskLevelAggregated</span><span class="sxs-lookup"><span data-stu-id="105fd-177">riskLevelAggregated</span></span>| <span data-ttu-id="105fd-178">eq</span><span class="sxs-lookup"><span data-stu-id="105fd-178">eq</span></span>|
|<span data-ttu-id="105fd-179">riskLevelDuringSignIn</span><span class="sxs-lookup"><span data-stu-id="105fd-179">riskLevelDuringSignIn</span></span>| <span data-ttu-id="105fd-180">eq</span><span class="sxs-lookup"><span data-stu-id="105fd-180">eq</span></span>|
|<span data-ttu-id="105fd-181">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="105fd-181">riskEventTypes</span></span>| <span data-ttu-id="105fd-182">eq</span><span class="sxs-lookup"><span data-stu-id="105fd-182">eq</span></span>|
|<span data-ttu-id="105fd-183">riskState</span><span class="sxs-lookup"><span data-stu-id="105fd-183">riskState</span></span>| <span data-ttu-id="105fd-184">eq</span><span class="sxs-lookup"><span data-stu-id="105fd-184">eq</span></span>|
|<span data-ttu-id="105fd-185">originalRequestId</span><span class="sxs-lookup"><span data-stu-id="105fd-185">originalRequestId</span></span>| <span data-ttu-id="105fd-186">eq</span><span class="sxs-lookup"><span data-stu-id="105fd-186">eq</span></span>|
|<span data-ttu-id="105fd-187">tokenIssuerName</span><span class="sxs-lookup"><span data-stu-id="105fd-187">tokenIssuerName</span></span>| <span data-ttu-id="105fd-188">eq</span><span class="sxs-lookup"><span data-stu-id="105fd-188">eq</span></span>|
|<span data-ttu-id="105fd-189">tokenIssuerType</span><span class="sxs-lookup"><span data-stu-id="105fd-189">tokenIssuerType</span></span>| <span data-ttu-id="105fd-190">eq</span><span class="sxs-lookup"><span data-stu-id="105fd-190">eq</span></span>|
|<span data-ttu-id="105fd-191">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="105fd-191">resourceDisplayName</span></span>| <span data-ttu-id="105fd-192">eq</span><span class="sxs-lookup"><span data-stu-id="105fd-192">eq</span></span>|
|<span data-ttu-id="105fd-193">resourceId</span><span class="sxs-lookup"><span data-stu-id="105fd-193">resourceId</span></span>| <span data-ttu-id="105fd-194">eq</span><span class="sxs-lookup"><span data-stu-id="105fd-194">eq</span></span>|


## <a name="response"></a><span data-ttu-id="105fd-195">応答</span><span class="sxs-lookup"><span data-stu-id="105fd-195">Response</span></span>
<span data-ttu-id="105fd-196">成功した場合、このメソッドは `200 OK` 応答コードと、[signIn](../resources/signin.md) オブジェクトのコレクションを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="105fd-196">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="105fd-197">例</span><span class="sxs-lookup"><span data-stu-id="105fd-197">Example</span></span>
##### <a name="request"></a><span data-ttu-id="105fd-198">要求</span><span class="sxs-lookup"><span data-stu-id="105fd-198">Request</span></span>
<span data-ttu-id="105fd-199">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="105fd-199">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_signins"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
##### <a name="response"></a><span data-ttu-id="105fd-200">応答</span><span class="sxs-lookup"><span data-stu-id="105fd-200">Response</span></span>
<span data-ttu-id="105fd-201">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="105fd-201">Here is an example of the response.</span></span> 

><span data-ttu-id="105fd-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="105fd-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="105fd-204">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="105fd-204">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="105fd-205">C#</span><span class="sxs-lookup"><span data-stu-id="105fd-205">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_signins-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="105fd-206">Javascript</span><span class="sxs-lookup"><span data-stu-id="105fd-206">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_signins-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="105fd-207">目的-C</span><span class="sxs-lookup"><span data-stu-id="105fd-207">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_signins-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/signin-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/signin-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/signin-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
