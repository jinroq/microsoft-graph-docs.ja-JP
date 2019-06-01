---
title: サインインを取得する
description: テナントの特定の Azure AD ユーザーのサインイン イベントを取得します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4b1a6aad8847bfaf2b30439c86c841a85005a3d2
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657372"
---
# <a name="get-signin"></a><span data-ttu-id="96601-103">signIn を取得する</span><span class="sxs-lookup"><span data-stu-id="96601-103">Get signIn</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96601-104">テナントの特定の Azure AD ユーザーのサインイン イベントを取得します。</span><span class="sxs-lookup"><span data-stu-id="96601-104">Retrieve a specific Azure AD user sign-in event for your tenant.</span></span> <span data-ttu-id="96601-105">本来対話型のサイイン (ユーザー名とパスワードが認証トークンの一部として渡される場合) と、成功したフェデレーション サインインは、現在サインイン ログに含まれています。</span><span class="sxs-lookup"><span data-stu-id="96601-105">Sign-ins that are interactive in nature (where a username/password is passed as part of authorization token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>


## <a name="permissions"></a><span data-ttu-id="96601-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="96601-106">Permissions</span></span>

<span data-ttu-id="96601-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="96601-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96601-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="96601-109">Permission type</span></span>      | <span data-ttu-id="96601-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="96601-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96601-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="96601-111">Delegated (work or school account)</span></span> | <span data-ttu-id="96601-112">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="96601-112">AuditLog.Read.All</span></span> |
|<span data-ttu-id="96601-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="96601-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96601-114">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="96601-114">Not supported</span></span>   |
|<span data-ttu-id="96601-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="96601-115">Application</span></span> | <span data-ttu-id="96601-116">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="96601-116">AuditLog.Read.All</span></span> | 

<span data-ttu-id="96601-117">また、アプリは Azure AD に[正しく登録されている](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)必要があります。</span><span class="sxs-lookup"><span data-stu-id="96601-117">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="96601-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="96601-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="96601-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="96601-119">Optional query parameters</span></span>

<span data-ttu-id="96601-120">このメソッドは、応答をカスタマイズするための OData クエリ パラメーターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="96601-120">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="96601-121">これらのパラメーターを使用する方法の詳細については、[OData クエリ パラメーター](/graph/query_parameters)をご確認ください。</span><span class="sxs-lookup"><span data-stu-id="96601-121">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="96601-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="96601-122">Request headers</span></span>

| <span data-ttu-id="96601-123">名前</span><span class="sxs-lookup"><span data-stu-id="96601-123">Name</span></span>      |<span data-ttu-id="96601-124">説明</span><span class="sxs-lookup"><span data-stu-id="96601-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="96601-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="96601-125">Authorization</span></span>  | <span data-ttu-id="96601-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="96601-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="96601-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="96601-127">Request body</span></span>

<span data-ttu-id="96601-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="96601-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96601-129">応答</span><span class="sxs-lookup"><span data-stu-id="96601-129">Response</span></span>

<span data-ttu-id="96601-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [signIn](../resources/signin.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="96601-130">If successful, this method returns a `200 OK` response code and [signIn](../resources/signin.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96601-131">例</span><span class="sxs-lookup"><span data-stu-id="96601-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="96601-132">要求</span><span class="sxs-lookup"><span data-stu-id="96601-132">Request</span></span>

<span data-ttu-id="96601-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="96601-133">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_signin"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/signIns/{id}
```

### <a name="response"></a><span data-ttu-id="96601-134">応答</span><span class="sxs-lookup"><span data-stu-id="96601-134">Response</span></span>

<span data-ttu-id="96601-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="96601-135">Here is an example of the response.</span></span> 

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="96601-136">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="96601-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="96601-137">C#</span><span class="sxs-lookup"><span data-stu-id="96601-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_signin-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="96601-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="96601-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_signin-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get signIn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/signin-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/signin-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
