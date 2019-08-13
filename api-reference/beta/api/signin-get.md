---
title: サインインを取得する
doc_type: apiPageType
description: テナントの特定の Azure AD ユーザーのサインイン イベントを取得します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d56d5c9377c3f0252901977738cb1f9f480b979d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36363826"
---
# <a name="get-signin"></a><span data-ttu-id="e270a-103">signIn を取得する</span><span class="sxs-lookup"><span data-stu-id="e270a-103">Get signIn</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e270a-104">テナントの特定の Azure AD ユーザーのサインイン イベントを取得します。</span><span class="sxs-lookup"><span data-stu-id="e270a-104">Retrieve a specific Azure AD user sign-in event for your tenant.</span></span> <span data-ttu-id="e270a-105">本来対話型のサイイン (ユーザー名とパスワードが認証トークンの一部として渡される場合) と、成功したフェデレーション サインインは、現在サインイン ログに含まれています。</span><span class="sxs-lookup"><span data-stu-id="e270a-105">Sign-ins that are interactive in nature (where a username/password is passed as part of authorization token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>


## <a name="permissions"></a><span data-ttu-id="e270a-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e270a-106">Permissions</span></span>

<span data-ttu-id="e270a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e270a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e270a-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e270a-109">Permission type</span></span>      | <span data-ttu-id="e270a-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e270a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e270a-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e270a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e270a-112">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="e270a-112">AuditLog.Read.All</span></span> |
|<span data-ttu-id="e270a-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e270a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e270a-114">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e270a-114">Directory.Read.All</span></span> |
|<span data-ttu-id="e270a-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e270a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e270a-116">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="e270a-116">Not supported</span></span>   |
|<span data-ttu-id="e270a-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e270a-117">Application</span></span> | <span data-ttu-id="e270a-118">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="e270a-118">AuditLog.Read.All</span></span> | 
|<span data-ttu-id="e270a-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e270a-119">Application</span></span> | <span data-ttu-id="e270a-120">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e270a-120">Directory.Read.All</span></span> | 


<span data-ttu-id="e270a-121">また、アプリは Azure AD に[正しく登録されている](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)必要があります。</span><span class="sxs-lookup"><span data-stu-id="e270a-121">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="e270a-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e270a-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e270a-123">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e270a-123">Optional query parameters</span></span>

<span data-ttu-id="e270a-124">このメソッドは、応答をカスタマイズするための OData クエリ パラメーターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="e270a-124">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="e270a-125">これらのパラメーターを使用する方法の詳細については、[OData クエリ パラメーター](/graph/query_parameters)をご確認ください。</span><span class="sxs-lookup"><span data-stu-id="e270a-125">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e270a-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e270a-126">Request headers</span></span>

| <span data-ttu-id="e270a-127">名前</span><span class="sxs-lookup"><span data-stu-id="e270a-127">Name</span></span>      |<span data-ttu-id="e270a-128">説明</span><span class="sxs-lookup"><span data-stu-id="e270a-128">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e270a-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="e270a-129">Authorization</span></span>  | <span data-ttu-id="e270a-130">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="e270a-130">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="e270a-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="e270a-131">Request body</span></span>

<span data-ttu-id="e270a-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e270a-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e270a-133">応答</span><span class="sxs-lookup"><span data-stu-id="e270a-133">Response</span></span>

<span data-ttu-id="e270a-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [signIn](../resources/signin.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e270a-134">If successful, this method returns a `200 OK` response code and [signIn](../resources/signin.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e270a-135">例</span><span class="sxs-lookup"><span data-stu-id="e270a-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="e270a-136">要求</span><span class="sxs-lookup"><span data-stu-id="e270a-136">Request</span></span>

<span data-ttu-id="e270a-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e270a-137">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e270a-138">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e270a-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/signIns/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e270a-139">C#</span><span class="sxs-lookup"><span data-stu-id="e270a-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e270a-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e270a-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e270a-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="e270a-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e270a-142">Java</span><span class="sxs-lookup"><span data-stu-id="e270a-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e270a-143">応答</span><span class="sxs-lookup"><span data-stu-id="e270a-143">Response</span></span>

<span data-ttu-id="e270a-144">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="e270a-144">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 211
```

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/signIns",
    "value": [{
        "id": "id",
        "createdDateTime": "2018-01-09T21:17:21.5077253Z",
        "userDisplayName": "Jamie Doe",
        "userPrincipalName": "jdoe@contoso.com",
        "userId": "bbb3b4b5-e6e6-f7f5-f7f5-090805040302",
        "appId": "d3590ed6-52b3-4102-aeff-aad2292ab01c",
        "appDisplayName": "Azure",
        "ipAddress": "127.0.0.1",
        "status": {
            "errorCode": 0,
            "failureReason": null,
            "additionalDetails": "SignIn Success & CA Success"
        },
        "clientAppUsed": null,
        "deviceDetail": {
            "deviceId": "34390ed6-52b3-4102-aeff-aad2292abac3",
            "displayName": "DeviceName",
            "operatingSystem": "Windows 10",
            "browser": "Rich Client v3.14.1592.7",
            "isCompliant": true,
            "isManaged": true,
            "trustType": ""
        },
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
        "mfaDetail": {
            "mfaAuthMethod": "Phone Auth",
            "mfaAuthDetail": null
        },
        "correlationId": "17c47d3c-593d-4d08-ac20-813892b87e42",
        "conditionalAccessApplied": true,
        "conditionalAccessPolicies": [{
            "id": "26490ed6-52b3-4102-aeff-aad2292abacf",
            "displayName": "capPolicy",
            "enforcedAccessControls": ["MFA", "TOU"],
            "enforcedSessionControls": ["CloudAppSecurity"],
            "result": "success"
        }],
        "isRisky": false,
        "riskLevel": "low"
    }]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get signIn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
