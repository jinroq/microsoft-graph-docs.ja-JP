---
title: signIns を一覧表示する
description: Microsoft Graph API からのサインインリソース (エンティティ) の list メソッドについて説明します。
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9500ca9421f74247c86d9cb5f667ede3948833a0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36307771"
---
# <a name="list-signins"></a><span data-ttu-id="94ff1-103">signIn を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="94ff1-103">List signIns</span></span>

<span data-ttu-id="94ff1-104">テナントの Azure AD ユーザーのサインインを取得します。</span><span class="sxs-lookup"><span data-stu-id="94ff1-104">Retrieve the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="94ff1-105">ユーザー名とパスワードが認証トークンの一部として渡され、正常なフェデレーションサインインがサインインログに含まれているなど、本質的に対話型のサインインは現在ありません。</span><span class="sxs-lookup"><span data-stu-id="94ff1-105">Sign-ins that are interactive in nature (where a username/password is passed as part of auth token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>

## <a name="permissions"></a><span data-ttu-id="94ff1-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="94ff1-106">Permissions</span></span>

<span data-ttu-id="94ff1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions_reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="94ff1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="94ff1-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="94ff1-109">Permission type</span></span>      | <span data-ttu-id="94ff1-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="94ff1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94ff1-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="94ff1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="94ff1-112">監査ログ。 all および All を参照してください。</span><span class="sxs-lookup"><span data-stu-id="94ff1-112">AuditLog.Read.All and Directory.Read.All</span></span> |
|<span data-ttu-id="94ff1-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="94ff1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94ff1-114">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="94ff1-114">Not supported</span></span>   |
|<span data-ttu-id="94ff1-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="94ff1-115">Application</span></span> | <span data-ttu-id="94ff1-116">監査ログ。 all および All を参照してください。</span><span class="sxs-lookup"><span data-stu-id="94ff1-116">AuditLog.Read.All and Directory.Read.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="94ff1-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="94ff1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```

## <a name="optional-query-parameters"></a><span data-ttu-id="94ff1-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="94ff1-118">Optional query parameters</span></span>

<span data-ttu-id="94ff1-119">このメソッドは、応答をカスタマイズするために、次の OData クエリパラメーターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="94ff1-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="94ff1-120">これらのパラメーターを使用する方法の詳細については、[OData クエリ パラメーター](/graph/query_parameters)をご確認ください。</span><span class="sxs-lookup"><span data-stu-id="94ff1-120">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

|<span data-ttu-id="94ff1-121">Name</span><span class="sxs-lookup"><span data-stu-id="94ff1-121">Name</span></span>     |<span data-ttu-id="94ff1-122">説明</span><span class="sxs-lookup"><span data-stu-id="94ff1-122">Description</span></span>                            |<span data-ttu-id="94ff1-123">例</span><span class="sxs-lookup"><span data-stu-id="94ff1-123">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="94ff1-124">$filter</span><span class="sxs-lookup"><span data-stu-id="94ff1-124">$filter</span></span>](/graph/query_parameters#filter-parameter)|<span data-ttu-id="94ff1-125">結果 (行) をフィルターします。</span><span class="sxs-lookup"><span data-stu-id="94ff1-125">Filters results (rows).</span></span> |`/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24`
|[<span data-ttu-id="94ff1-126">$top</span><span class="sxs-lookup"><span data-stu-id="94ff1-126">$top</span></span>](/graph/query_parameters#top-parameter)|<span data-ttu-id="94ff1-127">結果のページ サイズを設定します。</span><span class="sxs-lookup"><span data-stu-id="94ff1-127">Sets the page size of results.</span></span>|`/auditLogs/signIns?$top=1`|
|[<span data-ttu-id="94ff1-128">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="94ff1-128">$skiptoken</span></span>](/graph/query_parameters#skiptoken-parameter)|<span data-ttu-id="94ff1-129">複数ページにわたる結果セットから、結果の次のページを取得します。</span><span class="sxs-lookup"><span data-stu-id="94ff1-129">Retrieves the next page of results from result sets that span multiple pages.</span></span>|`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="attributes-supported-by-filter-parameter"></a><span data-ttu-id="94ff1-130">$filter パラメーターでサポートされている属性</span><span class="sxs-lookup"><span data-stu-id="94ff1-130">Attributes supported by $filter parameter</span></span>

|<span data-ttu-id="94ff1-131">属性名</span><span class="sxs-lookup"><span data-stu-id="94ff1-131">Attribute name</span></span> |<span data-ttu-id="94ff1-132">サポートされる演算子</span><span class="sxs-lookup"><span data-stu-id="94ff1-132">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="94ff1-133">id</span><span class="sxs-lookup"><span data-stu-id="94ff1-133">id</span></span>|<span data-ttu-id="94ff1-134">eq</span><span class="sxs-lookup"><span data-stu-id="94ff1-134">eq</span></span>|
|<span data-ttu-id="94ff1-135">userId</span><span class="sxs-lookup"><span data-stu-id="94ff1-135">userId</span></span>|<span data-ttu-id="94ff1-136">eq</span><span class="sxs-lookup"><span data-stu-id="94ff1-136">eq</span></span>|
|<span data-ttu-id="94ff1-137">appId</span><span class="sxs-lookup"><span data-stu-id="94ff1-137">appId</span></span>|<span data-ttu-id="94ff1-138">eq</span><span class="sxs-lookup"><span data-stu-id="94ff1-138">eq</span></span>|
|<span data-ttu-id="94ff1-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="94ff1-139">createdDateTime</span></span>| <span data-ttu-id="94ff1-140">eq、le、ge</span><span class="sxs-lookup"><span data-stu-id="94ff1-140">eq, le, ge</span></span>|
|<span data-ttu-id="94ff1-141">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="94ff1-141">userDisplayName</span></span>| <span data-ttu-id="94ff1-142">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="94ff1-142">eq, startswith</span></span>|
|<span data-ttu-id="94ff1-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="94ff1-143">userPrincipalName</span></span>| <span data-ttu-id="94ff1-144">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="94ff1-144">eq, startswith</span></span>|
|<span data-ttu-id="94ff1-145">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="94ff1-145">appDisplayName</span></span>| <span data-ttu-id="94ff1-146">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="94ff1-146">eq, startswith</span></span>|
|<span data-ttu-id="94ff1-147">ipAddress</span><span class="sxs-lookup"><span data-stu-id="94ff1-147">ipAddress</span></span>| <span data-ttu-id="94ff1-148">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="94ff1-148">eq, startswith</span></span>|
|<span data-ttu-id="94ff1-149">location/city</span><span class="sxs-lookup"><span data-stu-id="94ff1-149">location/city</span></span>| <span data-ttu-id="94ff1-150">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="94ff1-150">eq, startswith</span></span>|
|<span data-ttu-id="94ff1-151">location/state</span><span class="sxs-lookup"><span data-stu-id="94ff1-151">location/state</span></span>| <span data-ttu-id="94ff1-152">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="94ff1-152">eq, startswith</span></span>|
|<span data-ttu-id="94ff1-153">location/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="94ff1-153">location/countryOrRegion</span></span>| <span data-ttu-id="94ff1-154">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="94ff1-154">eq, startswith</span></span>|
|<span data-ttu-id="94ff1-155">status/errorCode</span><span class="sxs-lookup"><span data-stu-id="94ff1-155">status/errorCode</span></span>|<span data-ttu-id="94ff1-156">eq</span><span class="sxs-lookup"><span data-stu-id="94ff1-156">eq</span></span>|
|<span data-ttu-id="94ff1-157">initiatedBy/user/id</span><span class="sxs-lookup"><span data-stu-id="94ff1-157">initiatedBy/user/id</span></span>|<span data-ttu-id="94ff1-158">eq</span><span class="sxs-lookup"><span data-stu-id="94ff1-158">eq</span></span>|
|<span data-ttu-id="94ff1-159">initiatedBy/user/displayName</span><span class="sxs-lookup"><span data-stu-id="94ff1-159">initiatedBy/user/displayName</span></span>| <span data-ttu-id="94ff1-160">eq</span><span class="sxs-lookup"><span data-stu-id="94ff1-160">eq</span></span>|
|<span data-ttu-id="94ff1-161">initiatedBy/user/userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="94ff1-161">initiatedBy/user/userPrincipalName</span></span>| <span data-ttu-id="94ff1-162">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="94ff1-162">eq, startswith</span></span>|
|<span data-ttu-id="94ff1-163">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="94ff1-163">clientAppUsed</span></span>| <span data-ttu-id="94ff1-164">eq</span><span class="sxs-lookup"><span data-stu-id="94ff1-164">eq</span></span>|
|<span data-ttu-id="94ff1-165">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="94ff1-165">conditionalAccessStatus</span></span> | <span data-ttu-id="94ff1-166">eq</span><span class="sxs-lookup"><span data-stu-id="94ff1-166">eq</span></span>|
|<span data-ttu-id="94ff1-167">deviceDetail/browser</span><span class="sxs-lookup"><span data-stu-id="94ff1-167">deviceDetail/browser</span></span>| <span data-ttu-id="94ff1-168">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="94ff1-168">eq, startswith</span></span>|
|<span data-ttu-id="94ff1-169">deviceDetail/operatingSystem</span><span class="sxs-lookup"><span data-stu-id="94ff1-169">deviceDetail/operatingSystem</span></span>| <span data-ttu-id="94ff1-170">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="94ff1-170">eq, startswith</span></span>|
|<span data-ttu-id="94ff1-171">correlationId</span><span class="sxs-lookup"><span data-stu-id="94ff1-171">correlationId</span></span>| <span data-ttu-id="94ff1-172">eq</span><span class="sxs-lookup"><span data-stu-id="94ff1-172">eq</span></span>|
|<span data-ttu-id="94ff1-173">isRisky</span><span class="sxs-lookup"><span data-stu-id="94ff1-173">isRisky</span></span>| <span data-ttu-id="94ff1-174">eq</span><span class="sxs-lookup"><span data-stu-id="94ff1-174">eq</span></span>|

## <a name="response"></a><span data-ttu-id="94ff1-175">応答</span><span class="sxs-lookup"><span data-stu-id="94ff1-175">Response</span></span>

<span data-ttu-id="94ff1-176">成功した場合、このメソッドは `200 OK` 応答コードと、[signIn](../resources/signin.md) オブジェクトのコレクションを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="94ff1-176">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94ff1-177">例</span><span class="sxs-lookup"><span data-stu-id="94ff1-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="94ff1-178">要求</span><span class="sxs-lookup"><span data-stu-id="94ff1-178">Request</span></span>

<span data-ttu-id="94ff1-179">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="94ff1-179">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="94ff1-180">プロトコル</span><span class="sxs-lookup"><span data-stu-id="94ff1-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_signins"
}-->
```http
GET https://graph.microsoft.com/v1.0/auditLogs/signIns
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="94ff1-181">C#</span><span class="sxs-lookup"><span data-stu-id="94ff1-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-signins-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="94ff1-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94ff1-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-signins-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="94ff1-183">目的-C</span><span class="sxs-lookup"><span data-stu-id="94ff1-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-signins-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="94ff1-184">Java</span><span class="sxs-lookup"><span data-stu-id="94ff1-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-signins-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="94ff1-185">応答</span><span class="sxs-lookup"><span data-stu-id="94ff1-185">Response</span></span>

<span data-ttu-id="94ff1-186">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="94ff1-186">Here is an example of the response.</span></span>
><span data-ttu-id="94ff1-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="94ff1-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  ]
}-->
