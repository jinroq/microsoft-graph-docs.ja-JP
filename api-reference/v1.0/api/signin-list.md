---
title: signIns を一覧表示する
description: Microsoft Graph API からのサインインリソース (エンティティ) の list メソッドについて説明します。
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1c5d4f2d7bc4e60eb0b1d1d876e4c9bf5000a35c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33951421"
---
# <a name="list-signins"></a><span data-ttu-id="6c986-103">signIn を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="6c986-103">List signIns</span></span>

<span data-ttu-id="6c986-104">テナントの Azure AD ユーザーのサインインを取得します。</span><span class="sxs-lookup"><span data-stu-id="6c986-104">Retrieve the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="6c986-105">ユーザー名とパスワードが認証トークンの一部として渡され、正常なフェデレーションサインインがサインインログに含まれているなど、本質的に対話型のサインインは現在ありません。</span><span class="sxs-lookup"><span data-stu-id="6c986-105">Sign-ins that are interactive in nature (where a username/password is passed as part of auth token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c986-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6c986-106">Permissions</span></span>

<span data-ttu-id="6c986-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions_reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6c986-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="6c986-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6c986-109">Permission type</span></span>      | <span data-ttu-id="6c986-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6c986-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6c986-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6c986-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6c986-112">監査ログ。 all および All を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6c986-112">AuditLog.Read.All and Directory.Read.All</span></span> |
|<span data-ttu-id="6c986-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6c986-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c986-114">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="6c986-114">Not supported</span></span>   |
|<span data-ttu-id="6c986-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6c986-115">Application</span></span> | <span data-ttu-id="6c986-116">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c986-116">AuditLog.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c986-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6c986-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6c986-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6c986-118">Optional query parameters</span></span>

<span data-ttu-id="6c986-119">このメソッドは、応答をカスタマイズするために、次の OData クエリパラメーターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="6c986-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="6c986-120">これらのパラメーターを使用する方法の詳細については、[OData クエリ パラメーター](/graph/query_parameters)をご確認ください。</span><span class="sxs-lookup"><span data-stu-id="6c986-120">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

|<span data-ttu-id="6c986-121">Name</span><span class="sxs-lookup"><span data-stu-id="6c986-121">Name</span></span>     |<span data-ttu-id="6c986-122">説明</span><span class="sxs-lookup"><span data-stu-id="6c986-122">Description</span></span>                            |<span data-ttu-id="6c986-123">例</span><span class="sxs-lookup"><span data-stu-id="6c986-123">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="6c986-124">$filter</span><span class="sxs-lookup"><span data-stu-id="6c986-124">$filter</span></span>](/graph/query_parameters#filter-parameter)|<span data-ttu-id="6c986-125">結果 (行) をフィルターします。</span><span class="sxs-lookup"><span data-stu-id="6c986-125">Filters results (rows).</span></span> |`/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24`
|[<span data-ttu-id="6c986-126">$top</span><span class="sxs-lookup"><span data-stu-id="6c986-126">$top</span></span>](/graph/query_parameters#top-parameter)|<span data-ttu-id="6c986-127">結果のページ サイズを設定します。</span><span class="sxs-lookup"><span data-stu-id="6c986-127">Sets the page size of results.</span></span>|`/auditLogs/signIns?$top=1`|
|[<span data-ttu-id="6c986-128">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="6c986-128">$skiptoken</span></span>](/graph/query_parameters#skiptoken-parameter)|<span data-ttu-id="6c986-129">複数ページにわたる結果セットから、結果の次のページを取得します。</span><span class="sxs-lookup"><span data-stu-id="6c986-129">Retrieves the next page of results from result sets that span multiple pages.</span></span>|`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="attributes-supported-by-filter-parameter"></a><span data-ttu-id="6c986-130">$Filter パラメーターでサポートされている属性</span><span class="sxs-lookup"><span data-stu-id="6c986-130">Attributes supported by $filter parameter</span></span>

|<span data-ttu-id="6c986-131">属性名</span><span class="sxs-lookup"><span data-stu-id="6c986-131">Attribute name</span></span> |<span data-ttu-id="6c986-132">サポートされる演算子</span><span class="sxs-lookup"><span data-stu-id="6c986-132">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="6c986-133">id</span><span class="sxs-lookup"><span data-stu-id="6c986-133">id</span></span>|<span data-ttu-id="6c986-134">eq</span><span class="sxs-lookup"><span data-stu-id="6c986-134">eq</span></span>|
|<span data-ttu-id="6c986-135">userId</span><span class="sxs-lookup"><span data-stu-id="6c986-135">userId</span></span>|<span data-ttu-id="6c986-136">eq</span><span class="sxs-lookup"><span data-stu-id="6c986-136">eq</span></span>|
|<span data-ttu-id="6c986-137">appId</span><span class="sxs-lookup"><span data-stu-id="6c986-137">appId</span></span>|<span data-ttu-id="6c986-138">eq</span><span class="sxs-lookup"><span data-stu-id="6c986-138">eq</span></span>|
|<span data-ttu-id="6c986-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c986-139">createdDateTime</span></span>| <span data-ttu-id="6c986-140">eq、le、ge</span><span class="sxs-lookup"><span data-stu-id="6c986-140">eq, le, ge</span></span>|
|<span data-ttu-id="6c986-141">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="6c986-141">userDisplayName</span></span>| <span data-ttu-id="6c986-142">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="6c986-142">eq, startswith</span></span>|
|<span data-ttu-id="6c986-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6c986-143">userPrincipalName</span></span>| <span data-ttu-id="6c986-144">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="6c986-144">eq, startswith</span></span>|
|<span data-ttu-id="6c986-145">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="6c986-145">appDisplayName</span></span>| <span data-ttu-id="6c986-146">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="6c986-146">eq, startswith</span></span>|
|<span data-ttu-id="6c986-147">ipAddress</span><span class="sxs-lookup"><span data-stu-id="6c986-147">ipAddress</span></span>| <span data-ttu-id="6c986-148">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="6c986-148">eq, startswith</span></span>|
|<span data-ttu-id="6c986-149">location/city</span><span class="sxs-lookup"><span data-stu-id="6c986-149">location/city</span></span>| <span data-ttu-id="6c986-150">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="6c986-150">eq, startswith</span></span>|
|<span data-ttu-id="6c986-151">location/state</span><span class="sxs-lookup"><span data-stu-id="6c986-151">location/state</span></span>| <span data-ttu-id="6c986-152">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="6c986-152">eq, startswith</span></span>|
|<span data-ttu-id="6c986-153">location/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="6c986-153">location/countryOrRegion</span></span>| <span data-ttu-id="6c986-154">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="6c986-154">eq, startswith</span></span>|
|<span data-ttu-id="6c986-155">status/errorCode</span><span class="sxs-lookup"><span data-stu-id="6c986-155">status/errorCode</span></span>|<span data-ttu-id="6c986-156">eq</span><span class="sxs-lookup"><span data-stu-id="6c986-156">eq</span></span>|
|<span data-ttu-id="6c986-157">initiatedBy/user/id</span><span class="sxs-lookup"><span data-stu-id="6c986-157">initiatedBy/user/id</span></span>|<span data-ttu-id="6c986-158">eq</span><span class="sxs-lookup"><span data-stu-id="6c986-158">eq</span></span>|
|<span data-ttu-id="6c986-159">initiatedBy/user/displayName</span><span class="sxs-lookup"><span data-stu-id="6c986-159">initiatedBy/user/displayName</span></span>| <span data-ttu-id="6c986-160">eq</span><span class="sxs-lookup"><span data-stu-id="6c986-160">eq</span></span>|
|<span data-ttu-id="6c986-161">initiatedBy/user/userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6c986-161">initiatedBy/user/userPrincipalName</span></span>| <span data-ttu-id="6c986-162">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="6c986-162">eq, startswith</span></span>|
|<span data-ttu-id="6c986-163">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="6c986-163">clientAppUsed</span></span>| <span data-ttu-id="6c986-164">eq</span><span class="sxs-lookup"><span data-stu-id="6c986-164">eq</span></span>|
|<span data-ttu-id="6c986-165">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="6c986-165">conditionalAccessStatus</span></span> | <span data-ttu-id="6c986-166">eq</span><span class="sxs-lookup"><span data-stu-id="6c986-166">eq</span></span>|
|<span data-ttu-id="6c986-167">deviceDetails/browser</span><span class="sxs-lookup"><span data-stu-id="6c986-167">deviceDetails/browser</span></span>| <span data-ttu-id="6c986-168">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="6c986-168">eq, startswith</span></span>|
|<span data-ttu-id="6c986-169">deviceDetails/operatingSystem</span><span class="sxs-lookup"><span data-stu-id="6c986-169">deviceDetails/operatingSystem</span></span>| <span data-ttu-id="6c986-170">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="6c986-170">eq, startswith</span></span>|
|<span data-ttu-id="6c986-171">correlationId</span><span class="sxs-lookup"><span data-stu-id="6c986-171">correlationId</span></span>| <span data-ttu-id="6c986-172">eq</span><span class="sxs-lookup"><span data-stu-id="6c986-172">eq</span></span>|
|<span data-ttu-id="6c986-173">isRisky</span><span class="sxs-lookup"><span data-stu-id="6c986-173">isRisky</span></span>| <span data-ttu-id="6c986-174">eq</span><span class="sxs-lookup"><span data-stu-id="6c986-174">eq</span></span>|

## <a name="response"></a><span data-ttu-id="6c986-175">応答</span><span class="sxs-lookup"><span data-stu-id="6c986-175">Response</span></span>

<span data-ttu-id="6c986-176">成功した場合、このメソッドは `200 OK` 応答コードと、[signIn](../resources/signin.md) オブジェクトのコレクションを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="6c986-176">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c986-177">例</span><span class="sxs-lookup"><span data-stu-id="6c986-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c986-178">要求</span><span class="sxs-lookup"><span data-stu-id="6c986-178">Request</span></span>

<span data-ttu-id="6c986-179">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6c986-179">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_signins"
}-->
```http
GET https://graph.microsoft.com/v1.0/auditLogs/signIns
```

### <a name="response"></a><span data-ttu-id="6c986-180">応答</span><span class="sxs-lookup"><span data-stu-id="6c986-180">Response</span></span>

<span data-ttu-id="6c986-181">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="6c986-181">Here is an example of the response.</span></span>
><span data-ttu-id="6c986-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6c986-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="6c986-184">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="6c986-184">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6c986-185">C#</span><span class="sxs-lookup"><span data-stu-id="6c986-185">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/list_signins-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6c986-186">Javascript</span><span class="sxs-lookup"><span data-stu-id="6c986-186">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/list_signins-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

```json
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#auditLogs/signIns",
    "value": [{
        "id": "id",
        "appId": "d3590ed6-52b3-4102-aeff-aad2292ab01c",
        "appDisplayName": "Azure",
        "createdDateTime": "2018-01-09T21:17:21.5077253Z",
        "clientAppUsed": null,
        "conditionalAccessApplied": true,
        "conditionalAccessPolicies": [{
            "id": "26490ed6-52b3-4102-aeff-aad2292abacf",
            "displayName": "capPolicy",
            "enforcedAccessControls": ["MFA", "TOU"],
            "enforcedSessionControls": ["CloudAppSecurity"],
            "result": "success"
        }],
        "correlationId": "17444d3c-563d-4b08-ac20-815892b87e42",
        "deviceDetail": {
            "deviceId": "34390ed6-52b3-4102-aeff-aad2292abac3",
            "displayName": "DeviceName",
            "operatingSystem": "Windows 10",
            "browser": "Rich Client v3.14.1592.7",
            "isCompliant": true,
            "isManaged": true,
            "trustType": ""
        },
        "ipAddress": "127.0.0.1",
        "location": {
            "city": "Redmond",
            "state": "WA",
            "countryOrRegion": "USA",
            "geoCoordinates": {
                "altitude": 41.589,
                "latitude": 41.589,
                "longitude": -93.6151
            }
        },
        "status": {
            "errorCode": 0,
            "failureReason": null,
            "additionalDetails": "SignIn Success & CA Success"
        },
        "userDisplayName": "Jamie Doe",
        "userPrincipalName": "jdoe@wingtiptoys.com",
        "userId": "bbb3b4b5-e6e6-f7f5-f7f5-090805040302"
    }]
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
    "Error: /api-reference/v1.0/api/signin-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/signin-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
