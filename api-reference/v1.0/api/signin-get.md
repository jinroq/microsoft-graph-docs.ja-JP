---
title: サインインを取得する
description: Microsoft Graph API からのサインインリソース (エンティティ) の get メソッドについて説明します。
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5abfdd96004e9aeb792e64713696326bb5b067d8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36307827"
---
# <a name="get-signin"></a><span data-ttu-id="eb357-103">signIn を取得する</span><span class="sxs-lookup"><span data-stu-id="eb357-103">Get signIn</span></span>

<span data-ttu-id="eb357-104">テナントの特定の Azure AD ユーザーのサインイン イベントを取得します。</span><span class="sxs-lookup"><span data-stu-id="eb357-104">Retrieve a specific Azure AD user sign-in event for your tenant.</span></span> <span data-ttu-id="eb357-105">ユーザー名とパスワードが認証トークンの一部として渡され、正常なフェデレーションサインインがサインインログに含まれているなど、本質的に対話型のサインインは現在ありません。</span><span class="sxs-lookup"><span data-stu-id="eb357-105">Sign-ins that are interactive in nature (where a username/password is passed as part of auth token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb357-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="eb357-106">Permissions</span></span>

<span data-ttu-id="eb357-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions_reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eb357-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="eb357-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="eb357-109">Permission type</span></span>      | <span data-ttu-id="eb357-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="eb357-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb357-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="eb357-111">Delegated (work or school account)</span></span> | <span data-ttu-id="eb357-112">監査ログ。 all および All を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eb357-112">AuditLog.Read.All and Directory.Read.All</span></span> |
|<span data-ttu-id="eb357-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="eb357-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb357-114">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="eb357-114">Not supported</span></span>   |
|<span data-ttu-id="eb357-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="eb357-115">Application</span></span> | <span data-ttu-id="eb357-116">監査ログ。 all および All を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eb357-116">AuditLog.Read.All and Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb357-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="eb357-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eb357-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="eb357-118">Optional query parameters</span></span>

<span data-ttu-id="eb357-119">このメソッドは、応答をカスタマイズするための OData クエリ パラメーターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="eb357-119">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="eb357-120">これらのパラメーターを使用する方法の詳細については、[OData クエリ パラメーター](/graph/query_parameters)をご確認ください。</span><span class="sxs-lookup"><span data-stu-id="eb357-120">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="eb357-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eb357-121">Request headers</span></span>

| <span data-ttu-id="eb357-122">名前</span><span class="sxs-lookup"><span data-stu-id="eb357-122">Name</span></span>      |<span data-ttu-id="eb357-123">説明</span><span class="sxs-lookup"><span data-stu-id="eb357-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="eb357-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb357-124">Authorization</span></span>  | <span data-ttu-id="eb357-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="eb357-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb357-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="eb357-126">Request body</span></span>

<span data-ttu-id="eb357-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="eb357-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb357-128">応答</span><span class="sxs-lookup"><span data-stu-id="eb357-128">Response</span></span>

<span data-ttu-id="eb357-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [signIn](../resources/signin.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="eb357-129">If successful, this method returns a `200 OK` response code and [signIn](../resources/signin.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb357-130">例</span><span class="sxs-lookup"><span data-stu-id="eb357-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb357-131">要求</span><span class="sxs-lookup"><span data-stu-id="eb357-131">Request</span></span>

<span data-ttu-id="eb357-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="eb357-132">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="eb357-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="eb357-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin"
}-->

```http
GET https://graph.microsoft.com/v1.0/auditLogs/signIns/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="eb357-134">C#</span><span class="sxs-lookup"><span data-stu-id="eb357-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eb357-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb357-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="eb357-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="eb357-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="eb357-137">Java</span><span class="sxs-lookup"><span data-stu-id="eb357-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="eb357-138">応答</span><span class="sxs-lookup"><span data-stu-id="eb357-138">Response</span></span>

<span data-ttu-id="eb357-139">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="eb357-139">Here is an example of the response.</span></span>
><span data-ttu-id="eb357-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="eb357-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#auditLogs/signIns",
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
