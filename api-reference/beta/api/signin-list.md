---
title: signIns を一覧表示する
description: テナントの Azure AD ユーザーのサインインを取得します。 本来対話型のサイイン (ユーザー名とパスワードが認証トークンの一部として渡される場合) と、成功したフェデレーション サインインは、現在サインイン ログに含まれています。  最新の signIns が最初に返されます。
localization_priority: Priority
ms.openlocfilehash: 8596bd168a3e10cbea9e15e2f61d6bd668fd27b5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545158"
---
# <a name="list-signins"></a><span data-ttu-id="762d2-105">signIns を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="762d2-105">List sign-ins</span></span>

<span data-ttu-id="762d2-106">テナントの Azure AD ユーザーのサインインを取得します。</span><span class="sxs-lookup"><span data-stu-id="762d2-106">Retrieves the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="762d2-107">本来対話型のサイイン (ユーザー名とパスワードが認証トークンの一部として渡される場合) と、成功したフェデレーション サインインは、現在サインイン ログに含まれています。</span><span class="sxs-lookup"><span data-stu-id="762d2-107">Sign-ins that are interactive in nature (where a username/password is passed as part of authorization token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>  <span data-ttu-id="762d2-108">最新の signIns が最初に返されます。</span><span class="sxs-lookup"><span data-stu-id="762d2-108">The most recent signIns are returned first.</span></span>


## <a name="permissions"></a><span data-ttu-id="762d2-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="762d2-109">Permissions</span></span>
<span data-ttu-id="762d2-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="762d2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="762d2-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="762d2-112">Permission type</span></span>      | <span data-ttu-id="762d2-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="762d2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="762d2-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="762d2-114">Delegated (work or school account)</span></span> | <span data-ttu-id="762d2-115">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="762d2-115">AuditLog.Read.All</span></span> |
|<span data-ttu-id="762d2-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="762d2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="762d2-117">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="762d2-117">Not supported</span></span>   |
|<span data-ttu-id="762d2-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="762d2-118">Application</span></span> | <span data-ttu-id="762d2-119">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="762d2-119">AuditLog.Read.All</span></span> | 

<span data-ttu-id="762d2-120">また、アプリは Azure AD に[正しく登録されている](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)必要があります。</span><span class="sxs-lookup"><span data-stu-id="762d2-120">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="762d2-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="762d2-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="762d2-122">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="762d2-122">Optional query parameters</span></span>
<span data-ttu-id="762d2-123">このメソッドは、応答をカスタマイズするための以下の OData クエリ パラメーターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="762d2-123">This method supports the following OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="762d2-124">[OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)でこれらのパラメーターを使用する方法について確認してください。</span><span class="sxs-lookup"><span data-stu-id="762d2-124">Check [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) for how to use these parameters.</span></span>

|<span data-ttu-id="762d2-125">名前</span><span class="sxs-lookup"><span data-stu-id="762d2-125">Name</span></span>     |<span data-ttu-id="762d2-126">説明</span><span class="sxs-lookup"><span data-stu-id="762d2-126">Description</span></span>                            |<span data-ttu-id="762d2-127">例</span><span class="sxs-lookup"><span data-stu-id="762d2-127">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="762d2-128">$filter</span><span class="sxs-lookup"><span data-stu-id="762d2-128">$filter</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#filter-parameter)|<span data-ttu-id="762d2-129">結果 (行) をフィルターします。</span><span class="sxs-lookup"><span data-stu-id="762d2-129">Filters results (rows).</span></span> |`/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24`
|[<span data-ttu-id="762d2-130">$top</span><span class="sxs-lookup"><span data-stu-id="762d2-130">$top</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top-parameter)|<span data-ttu-id="762d2-131">結果のページ サイズを設定します。</span><span class="sxs-lookup"><span data-stu-id="762d2-131">Sets the page size of results.</span></span>|`/auditLogs/signIns?$top=1`|
|[<span data-ttu-id="762d2-132">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="762d2-132">$skiptoken</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skiptoken-parameter)|<span data-ttu-id="762d2-133">複数ページにわたる結果セットから、結果の次のページを取得します。</span><span class="sxs-lookup"><span data-stu-id="762d2-133">Retrieves the next page of results from result sets that span multiple pages.</span></span>|`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="list-of-attributes-supported-by-filter-parameter"></a><span data-ttu-id="762d2-134">$Filter パラメーターにサポートされる属性の一覧</span><span class="sxs-lookup"><span data-stu-id="762d2-134">List of attributes supported by $filter parameter</span></span>
|<span data-ttu-id="762d2-135">属性名</span><span class="sxs-lookup"><span data-stu-id="762d2-135">Attribute Name</span></span> |<span data-ttu-id="762d2-136">サポートされる演算子</span><span class="sxs-lookup"><span data-stu-id="762d2-136">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="762d2-137">id</span><span class="sxs-lookup"><span data-stu-id="762d2-137">id</span></span>|<span data-ttu-id="762d2-138">eq</span><span class="sxs-lookup"><span data-stu-id="762d2-138">eq</span></span>|
|<span data-ttu-id="762d2-139">userId</span><span class="sxs-lookup"><span data-stu-id="762d2-139">userId</span></span>|<span data-ttu-id="762d2-140">eq</span><span class="sxs-lookup"><span data-stu-id="762d2-140">eq</span></span>|
|<span data-ttu-id="762d2-141">appId</span><span class="sxs-lookup"><span data-stu-id="762d2-141">appId</span></span>|<span data-ttu-id="762d2-142">eq</span><span class="sxs-lookup"><span data-stu-id="762d2-142">eq</span></span>|
|<span data-ttu-id="762d2-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="762d2-143">createdDateTime</span></span>| <span data-ttu-id="762d2-144">eq、le、ge</span><span class="sxs-lookup"><span data-stu-id="762d2-144">eq, ge, le</span></span>|
|<span data-ttu-id="762d2-145">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="762d2-145">userDisplayName</span></span>| <span data-ttu-id="762d2-146">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="762d2-146">eq, startswith</span></span>|
|<span data-ttu-id="762d2-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="762d2-147">userPrincipalName</span></span>| <span data-ttu-id="762d2-148">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="762d2-148">eq, startswith</span></span>|
|<span data-ttu-id="762d2-149">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="762d2-149">appDisplayName</span></span>| <span data-ttu-id="762d2-150">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="762d2-150">eq, startswith</span></span>|
|<span data-ttu-id="762d2-151">ipAddress</span><span class="sxs-lookup"><span data-stu-id="762d2-151">ipAddress</span></span>| <span data-ttu-id="762d2-152">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="762d2-152">eq, startswith</span></span>|
|<span data-ttu-id="762d2-153">location/city</span><span class="sxs-lookup"><span data-stu-id="762d2-153">location/city</span></span>| <span data-ttu-id="762d2-154">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="762d2-154">eq, startswith</span></span>|
|<span data-ttu-id="762d2-155">location/state</span><span class="sxs-lookup"><span data-stu-id="762d2-155">location/state</span></span>| <span data-ttu-id="762d2-156">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="762d2-156">eq, startswith</span></span>|
|<span data-ttu-id="762d2-157">location/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="762d2-157">location/countryOrRegion</span></span>| <span data-ttu-id="762d2-158">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="762d2-158">eq, startswith</span></span>|
|<span data-ttu-id="762d2-159">status/errorCode</span><span class="sxs-lookup"><span data-stu-id="762d2-159">status/errorCode</span></span>|<span data-ttu-id="762d2-160">eq</span><span class="sxs-lookup"><span data-stu-id="762d2-160">eq</span></span>|
|<span data-ttu-id="762d2-161">initiatedBy/user/id</span><span class="sxs-lookup"><span data-stu-id="762d2-161">initiatedBy/user/id</span></span>|<span data-ttu-id="762d2-162">eq</span><span class="sxs-lookup"><span data-stu-id="762d2-162">eq</span></span>|
|<span data-ttu-id="762d2-163">initiatedBy/user/displayName</span><span class="sxs-lookup"><span data-stu-id="762d2-163">initiatedBy/user/displayName</span></span>| <span data-ttu-id="762d2-164">eq</span><span class="sxs-lookup"><span data-stu-id="762d2-164">eq</span></span>|
|<span data-ttu-id="762d2-165">initiatedBy/user/userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="762d2-165">initiatedBy/user/userPrincipalName</span></span>| <span data-ttu-id="762d2-166">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="762d2-166">eq, startswith</span></span>|
|<span data-ttu-id="762d2-167">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="762d2-167">clientAppUsed</span></span>| <span data-ttu-id="762d2-168">eq</span><span class="sxs-lookup"><span data-stu-id="762d2-168">eq</span></span>|
|<span data-ttu-id="762d2-169">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="762d2-169">conditionalAccessStatus</span></span> | <span data-ttu-id="762d2-170">eq</span><span class="sxs-lookup"><span data-stu-id="762d2-170">eq</span></span>|
|<span data-ttu-id="762d2-171">deviceDetail/browser</span><span class="sxs-lookup"><span data-stu-id="762d2-171">deviceDetail/browser</span></span>| <span data-ttu-id="762d2-172">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="762d2-172">eq, startswith</span></span>|
|<span data-ttu-id="762d2-173">deviceDetail/operatingSystem</span><span class="sxs-lookup"><span data-stu-id="762d2-173">deviceDetail/operatingSystem</span></span>| <span data-ttu-id="762d2-174">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="762d2-174">eq, startswith</span></span>|
|<span data-ttu-id="762d2-175">correlationId</span><span class="sxs-lookup"><span data-stu-id="762d2-175">correlationId</span></span>| <span data-ttu-id="762d2-176">eq</span><span class="sxs-lookup"><span data-stu-id="762d2-176">eq</span></span>|
|<span data-ttu-id="762d2-177">riskDetail</span><span class="sxs-lookup"><span data-stu-id="762d2-177">riskDetail</span></span>| <span data-ttu-id="762d2-178">eq</span><span class="sxs-lookup"><span data-stu-id="762d2-178">eq</span></span>|
|<span data-ttu-id="762d2-179">riskLevelAggregated</span><span class="sxs-lookup"><span data-stu-id="762d2-179">riskLevelAggregated</span></span>| <span data-ttu-id="762d2-180">eq</span><span class="sxs-lookup"><span data-stu-id="762d2-180">eq</span></span>|
|<span data-ttu-id="762d2-181">riskLevelDuringSignIn</span><span class="sxs-lookup"><span data-stu-id="762d2-181">riskLevelDuringSignIn</span></span>| <span data-ttu-id="762d2-182">eq</span><span class="sxs-lookup"><span data-stu-id="762d2-182">eq</span></span>|
|<span data-ttu-id="762d2-183">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="762d2-183">riskEventTypes</span></span>| <span data-ttu-id="762d2-184">eq</span><span class="sxs-lookup"><span data-stu-id="762d2-184">eq</span></span>|
|<span data-ttu-id="762d2-185">riskState</span><span class="sxs-lookup"><span data-stu-id="762d2-185">riskState</span></span>| <span data-ttu-id="762d2-186">eq</span><span class="sxs-lookup"><span data-stu-id="762d2-186">eq</span></span>|
|<span data-ttu-id="762d2-187">originalRequestId</span><span class="sxs-lookup"><span data-stu-id="762d2-187">originalRequestId</span></span>| <span data-ttu-id="762d2-188">eq</span><span class="sxs-lookup"><span data-stu-id="762d2-188">eq</span></span>|
|<span data-ttu-id="762d2-189">tokenIssuerName</span><span class="sxs-lookup"><span data-stu-id="762d2-189">tokenIssuerName</span></span>| <span data-ttu-id="762d2-190">eq</span><span class="sxs-lookup"><span data-stu-id="762d2-190">eq</span></span>|
|<span data-ttu-id="762d2-191">tokenIssuerType</span><span class="sxs-lookup"><span data-stu-id="762d2-191">tokenIssuerType</span></span>| <span data-ttu-id="762d2-192">eq</span><span class="sxs-lookup"><span data-stu-id="762d2-192">eq</span></span>|
|<span data-ttu-id="762d2-193">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="762d2-193">resourceDisplayName</span></span>| <span data-ttu-id="762d2-194">eq</span><span class="sxs-lookup"><span data-stu-id="762d2-194">eq</span></span>|
|<span data-ttu-id="762d2-195">resourceId</span><span class="sxs-lookup"><span data-stu-id="762d2-195">resourceId</span></span>| <span data-ttu-id="762d2-196">eq</span><span class="sxs-lookup"><span data-stu-id="762d2-196">eq</span></span>|


## <a name="response"></a><span data-ttu-id="762d2-197">応答</span><span class="sxs-lookup"><span data-stu-id="762d2-197">Response</span></span>
<span data-ttu-id="762d2-198">成功した場合、このメソッドは `200 OK` 応答コードと、[signIn](../resources/signin.md) オブジェクトのコレクションを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="762d2-198">If successful, this method returns a `200 OK` response code and collection of [directoryAudit](../resources/signin.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="762d2-199">例</span><span class="sxs-lookup"><span data-stu-id="762d2-199">Example</span></span>
##### <a name="request"></a><span data-ttu-id="762d2-200">要求</span><span class="sxs-lookup"><span data-stu-id="762d2-200">Request</span></span>
<span data-ttu-id="762d2-201">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="762d2-201">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_signins"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
##### <a name="response"></a><span data-ttu-id="762d2-202">応答</span><span class="sxs-lookup"><span data-stu-id="762d2-202">Response</span></span>
<span data-ttu-id="762d2-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="762d2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
