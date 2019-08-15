---
title: signIns を一覧表示する
doc_type: apiPageType
description: ディレクトリ (テナント) のアクティビティ (ベータ版) を監査するための、Microsoft Graph API (REST) の signIn リソース (エンティティ) を一覧表示する方法について説明します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5c8ca894571d843305b11402c27ea5f9f688052c
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410046"
---
# <a name="list-signins"></a><span data-ttu-id="69562-103">signIn を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="69562-103">List signIns</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69562-104">テナントの Azure AD ユーザーのサインインを取得します。</span><span class="sxs-lookup"><span data-stu-id="69562-104">Retrieve the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="69562-105">本来対話型のサイイン (ユーザー名とパスワードが認証トークンの一部として渡される場合) と、成功したフェデレーション サインインは、現在サインイン ログに含まれています。</span><span class="sxs-lookup"><span data-stu-id="69562-105">Sign-ins that are interactive in nature (where a username/password is passed as part of authorization token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>  <span data-ttu-id="69562-106">最新の signIns が最初に返されます。</span><span class="sxs-lookup"><span data-stu-id="69562-106">The most recent signIns are returned first.</span></span>

## <a name="permissions"></a><span data-ttu-id="69562-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="69562-107">Permissions</span></span>

<span data-ttu-id="69562-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="69562-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69562-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="69562-110">Permission type</span></span>      | <span data-ttu-id="69562-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="69562-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69562-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="69562-112">Delegated (work or school account)</span></span> | <span data-ttu-id="69562-113">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="69562-113">AuditLog.Read.All</span></span> |
|<span data-ttu-id="69562-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="69562-114">Delegated (work or school account)</span></span> | <span data-ttu-id="69562-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="69562-115">Directory.Read.All</span></span> |
|<span data-ttu-id="69562-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="69562-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69562-117">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="69562-117">Not supported</span></span>   |
|<span data-ttu-id="69562-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="69562-118">Application</span></span> | <span data-ttu-id="69562-119">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="69562-119">AuditLog.Read.All</span></span> | 
|<span data-ttu-id="69562-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="69562-120">Application</span></span> | <span data-ttu-id="69562-121">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="69562-121">Directory.Read.All</span></span>  | 


<span data-ttu-id="69562-122">また、アプリは Azure AD に[正しく登録されている](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)必要があります。</span><span class="sxs-lookup"><span data-stu-id="69562-122">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="69562-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="69562-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="69562-124">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="69562-124">Optional query parameters</span></span>
<span data-ttu-id="69562-125">このメソッドは、応答をカスタマイズするための以下の OData クエリ パラメーターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="69562-125">This method supports the following OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="69562-126">これらのパラメーターを使用する方法の詳細については、[OData クエリ パラメーター](/graph/query_parameters)をご確認ください。</span><span class="sxs-lookup"><span data-stu-id="69562-126">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

|<span data-ttu-id="69562-127">Name</span><span class="sxs-lookup"><span data-stu-id="69562-127">Name</span></span>     |<span data-ttu-id="69562-128">説明</span><span class="sxs-lookup"><span data-stu-id="69562-128">Description</span></span>                            |<span data-ttu-id="69562-129">例</span><span class="sxs-lookup"><span data-stu-id="69562-129">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="69562-130">$filter</span><span class="sxs-lookup"><span data-stu-id="69562-130">$filter</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#filter-parameter)|<span data-ttu-id="69562-131">結果 (行) をフィルターします。</span><span class="sxs-lookup"><span data-stu-id="69562-131">Filters results (rows).</span></span> |`/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24`
|[<span data-ttu-id="69562-132">$top</span><span class="sxs-lookup"><span data-stu-id="69562-132">$top</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top-parameter)|<span data-ttu-id="69562-133">結果のページ サイズを設定します。</span><span class="sxs-lookup"><span data-stu-id="69562-133">Sets the page size of results.</span></span>|`/auditLogs/signIns?$top=1`|
|[<span data-ttu-id="69562-134">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="69562-134">$skiptoken</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skiptoken-parameter)|<span data-ttu-id="69562-135">複数ページにわたる結果セットから、結果の次のページを取得します。</span><span class="sxs-lookup"><span data-stu-id="69562-135">Retrieves the next page of results from result sets that span multiple pages.</span></span>|`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="list-of-attributes-supported-by-filter-parameter"></a><span data-ttu-id="69562-136">$Filter パラメーターにサポートされる属性の一覧</span><span class="sxs-lookup"><span data-stu-id="69562-136">List of attributes supported by $filter parameter</span></span>
|<span data-ttu-id="69562-137">属性名</span><span class="sxs-lookup"><span data-stu-id="69562-137">Attribute Name</span></span> |<span data-ttu-id="69562-138">サポートされる演算子</span><span class="sxs-lookup"><span data-stu-id="69562-138">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="69562-139">id</span><span class="sxs-lookup"><span data-stu-id="69562-139">id</span></span>|<span data-ttu-id="69562-140">eq</span><span class="sxs-lookup"><span data-stu-id="69562-140">eq</span></span>|
|<span data-ttu-id="69562-141">userId</span><span class="sxs-lookup"><span data-stu-id="69562-141">userId</span></span>|<span data-ttu-id="69562-142">eq</span><span class="sxs-lookup"><span data-stu-id="69562-142">eq</span></span>|
|<span data-ttu-id="69562-143">appId</span><span class="sxs-lookup"><span data-stu-id="69562-143">appId</span></span>|<span data-ttu-id="69562-144">eq</span><span class="sxs-lookup"><span data-stu-id="69562-144">eq</span></span>|
|<span data-ttu-id="69562-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="69562-145">createdDateTime</span></span>| <span data-ttu-id="69562-146">eq、le、ge</span><span class="sxs-lookup"><span data-stu-id="69562-146">eq, le, ge</span></span>|
|<span data-ttu-id="69562-147">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="69562-147">userDisplayName</span></span>| <span data-ttu-id="69562-148">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="69562-148">eq, startswith</span></span>|
|<span data-ttu-id="69562-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="69562-149">userPrincipalName</span></span>| <span data-ttu-id="69562-150">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="69562-150">eq, startswith</span></span>|
|<span data-ttu-id="69562-151">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="69562-151">appDisplayName</span></span>| <span data-ttu-id="69562-152">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="69562-152">eq, startswith</span></span>|
|<span data-ttu-id="69562-153">ipAddress</span><span class="sxs-lookup"><span data-stu-id="69562-153">ipAddress</span></span>| <span data-ttu-id="69562-154">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="69562-154">eq, startswith</span></span>|
|<span data-ttu-id="69562-155">location/city</span><span class="sxs-lookup"><span data-stu-id="69562-155">location/city</span></span>| <span data-ttu-id="69562-156">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="69562-156">eq, startswith</span></span>|
|<span data-ttu-id="69562-157">location/state</span><span class="sxs-lookup"><span data-stu-id="69562-157">location/state</span></span>| <span data-ttu-id="69562-158">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="69562-158">eq, startswith</span></span>|
|<span data-ttu-id="69562-159">location/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="69562-159">location/countryOrRegion</span></span>| <span data-ttu-id="69562-160">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="69562-160">eq, startswith</span></span>|
|<span data-ttu-id="69562-161">status/errorCode</span><span class="sxs-lookup"><span data-stu-id="69562-161">status/errorCode</span></span>|<span data-ttu-id="69562-162">eq</span><span class="sxs-lookup"><span data-stu-id="69562-162">eq</span></span>|
|<span data-ttu-id="69562-163">initiatedBy/user/id</span><span class="sxs-lookup"><span data-stu-id="69562-163">initiatedBy/user/id</span></span>|<span data-ttu-id="69562-164">eq</span><span class="sxs-lookup"><span data-stu-id="69562-164">eq</span></span>|
|<span data-ttu-id="69562-165">initiatedBy/user/displayName</span><span class="sxs-lookup"><span data-stu-id="69562-165">initiatedBy/user/displayName</span></span>| <span data-ttu-id="69562-166">eq</span><span class="sxs-lookup"><span data-stu-id="69562-166">eq</span></span>|
|<span data-ttu-id="69562-167">initiatedBy/user/userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="69562-167">initiatedBy/user/userPrincipalName</span></span>| <span data-ttu-id="69562-168">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="69562-168">eq, startswith</span></span>|
|<span data-ttu-id="69562-169">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="69562-169">clientAppUsed</span></span>| <span data-ttu-id="69562-170">eq</span><span class="sxs-lookup"><span data-stu-id="69562-170">eq</span></span>|
|<span data-ttu-id="69562-171">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="69562-171">conditionalAccessStatus</span></span> | <span data-ttu-id="69562-172">eq</span><span class="sxs-lookup"><span data-stu-id="69562-172">eq</span></span>|
|<span data-ttu-id="69562-173">deviceDetail/browser</span><span class="sxs-lookup"><span data-stu-id="69562-173">deviceDetail/browser</span></span>| <span data-ttu-id="69562-174">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="69562-174">eq, startswith</span></span>|
|<span data-ttu-id="69562-175">deviceDetail/operatingSystem</span><span class="sxs-lookup"><span data-stu-id="69562-175">deviceDetail/operatingSystem</span></span>| <span data-ttu-id="69562-176">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="69562-176">eq, startswith</span></span>|
|<span data-ttu-id="69562-177">correlationId</span><span class="sxs-lookup"><span data-stu-id="69562-177">correlationId</span></span>| <span data-ttu-id="69562-178">eq</span><span class="sxs-lookup"><span data-stu-id="69562-178">eq</span></span>|
|<span data-ttu-id="69562-179">riskDetail</span><span class="sxs-lookup"><span data-stu-id="69562-179">riskDetail</span></span>| <span data-ttu-id="69562-180">eq</span><span class="sxs-lookup"><span data-stu-id="69562-180">eq</span></span>|
|<span data-ttu-id="69562-181">riskLevelAggregated</span><span class="sxs-lookup"><span data-stu-id="69562-181">riskLevelAggregated</span></span>| <span data-ttu-id="69562-182">eq</span><span class="sxs-lookup"><span data-stu-id="69562-182">eq</span></span>|
|<span data-ttu-id="69562-183">riskLevelDuringSignIn</span><span class="sxs-lookup"><span data-stu-id="69562-183">riskLevelDuringSignIn</span></span>| <span data-ttu-id="69562-184">eq</span><span class="sxs-lookup"><span data-stu-id="69562-184">eq</span></span>|
|<span data-ttu-id="69562-185">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="69562-185">riskEventTypes</span></span>| <span data-ttu-id="69562-186">eq</span><span class="sxs-lookup"><span data-stu-id="69562-186">eq</span></span>|
|<span data-ttu-id="69562-187">riskState</span><span class="sxs-lookup"><span data-stu-id="69562-187">riskState</span></span>| <span data-ttu-id="69562-188">eq</span><span class="sxs-lookup"><span data-stu-id="69562-188">eq</span></span>|
|<span data-ttu-id="69562-189">originalRequestId</span><span class="sxs-lookup"><span data-stu-id="69562-189">originalRequestId</span></span>| <span data-ttu-id="69562-190">eq</span><span class="sxs-lookup"><span data-stu-id="69562-190">eq</span></span>|
|<span data-ttu-id="69562-191">tokenIssuerName</span><span class="sxs-lookup"><span data-stu-id="69562-191">tokenIssuerName</span></span>| <span data-ttu-id="69562-192">eq</span><span class="sxs-lookup"><span data-stu-id="69562-192">eq</span></span>|
|<span data-ttu-id="69562-193">tokenIssuerType</span><span class="sxs-lookup"><span data-stu-id="69562-193">tokenIssuerType</span></span>| <span data-ttu-id="69562-194">eq</span><span class="sxs-lookup"><span data-stu-id="69562-194">eq</span></span>|
|<span data-ttu-id="69562-195">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="69562-195">resourceDisplayName</span></span>| <span data-ttu-id="69562-196">eq</span><span class="sxs-lookup"><span data-stu-id="69562-196">eq</span></span>|
|<span data-ttu-id="69562-197">resourceId</span><span class="sxs-lookup"><span data-stu-id="69562-197">resourceId</span></span>| <span data-ttu-id="69562-198">eq</span><span class="sxs-lookup"><span data-stu-id="69562-198">eq</span></span>|


## <a name="response"></a><span data-ttu-id="69562-199">応答</span><span class="sxs-lookup"><span data-stu-id="69562-199">Response</span></span>
<span data-ttu-id="69562-200">成功した場合、このメソッドは `200 OK` 応答コードと、[signIn](../resources/signin.md) オブジェクトのコレクションを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="69562-200">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="69562-201">例</span><span class="sxs-lookup"><span data-stu-id="69562-201">Example</span></span>
##### <a name="request"></a><span data-ttu-id="69562-202">要求</span><span class="sxs-lookup"><span data-stu-id="69562-202">Request</span></span>
<span data-ttu-id="69562-203">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="69562-203">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="69562-204">プロトコル</span><span class="sxs-lookup"><span data-stu-id="69562-204">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signins"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="69562-205">C#</span><span class="sxs-lookup"><span data-stu-id="69562-205">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signins-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="69562-206">JavaScript</span><span class="sxs-lookup"><span data-stu-id="69562-206">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signins-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="69562-207">目的-C</span><span class="sxs-lookup"><span data-stu-id="69562-207">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signins-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="69562-208">応答</span><span class="sxs-lookup"><span data-stu-id="69562-208">Response</span></span>
<span data-ttu-id="69562-209">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="69562-209">Here is an example of the response.</span></span> 

><span data-ttu-id="69562-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="69562-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
