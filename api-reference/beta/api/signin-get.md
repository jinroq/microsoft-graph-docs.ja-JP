---
title: サインインを取得します。
description: テナントの Azure AD ユーザーのサインインを取得します。 インタラクティブ (ユーザー名とパスワードは認証トークンの一部として渡す) 性質およびフェデレーション サインインが成功には、サインインの問題は現在、サインインがログに含まれます。
localization_priority: Priority
ms.openlocfilehash: 5d2d0513f44196d48aa863ac19838af13d960f85
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894496"
---
# <a name="get-signin"></a><span data-ttu-id="84017-104">サインインを取得します。</span><span class="sxs-lookup"><span data-stu-id="84017-104">Get signIn</span></span>
<span data-ttu-id="84017-105">テナントの Azure AD ユーザーのサインインを取得します。</span><span class="sxs-lookup"><span data-stu-id="84017-105">Retrieves the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="84017-106">インタラクティブ (ユーザー名とパスワードは認証トークンの一部として渡す) 性質およびフェデレーション サインインが成功には、サインインの問題は現在、サインインがログに含まれます。</span><span class="sxs-lookup"><span data-stu-id="84017-106">Sign-ins that are interactive in nature (where a username/password is passed as part of authorization token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>


## <a name="permissions"></a><span data-ttu-id="84017-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="84017-107">Permissions</span></span>
<span data-ttu-id="84017-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="84017-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84017-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="84017-110">Permission type</span></span>      | <span data-ttu-id="84017-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="84017-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84017-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="84017-112">Delegated (work or school account)</span></span> | <span data-ttu-id="84017-113">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="84017-113">AuditLog.Read.All</span></span> |
|<span data-ttu-id="84017-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="84017-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84017-115">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="84017-115">Not supported</span></span>   |
|<span data-ttu-id="84017-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="84017-116">Application</span></span> | <span data-ttu-id="84017-117">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="84017-117">AuditLog.Read.All</span></span> | 

<span data-ttu-id="84017-118">さらに、アプリケーションでは、Azure AD に[適切に登録](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)をする必要があります。</span><span class="sxs-lookup"><span data-stu-id="84017-118">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="84017-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="84017-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="84017-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="84017-120">Optional query parameters</span></span>
<span data-ttu-id="84017-121">このメソッドは、応答をカスタマイズするための以下の OData クエリ パラメーターをサポートします。</span><span class="sxs-lookup"><span data-stu-id="84017-121">This method supports the following OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="84017-122">これらのパラメーターを使用する方法については、 [OData クエリのパラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)を確認してください。</span><span class="sxs-lookup"><span data-stu-id="84017-122">Check [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) for how to use these parameters.</span></span>

## <a name="request-headers"></a><span data-ttu-id="84017-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="84017-123">Request headers</span></span>
| <span data-ttu-id="84017-124">名前</span><span class="sxs-lookup"><span data-stu-id="84017-124">Name</span></span>      |<span data-ttu-id="84017-125">説明</span><span class="sxs-lookup"><span data-stu-id="84017-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="84017-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="84017-126">Authorization</span></span>  | <span data-ttu-id="84017-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="84017-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="84017-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="84017-128">Request body</span></span>
<span data-ttu-id="84017-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="84017-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="84017-130">応答</span><span class="sxs-lookup"><span data-stu-id="84017-130">Response</span></span>
<span data-ttu-id="84017-131">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[サイン](../resources/signin.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="84017-131">If successful, this method returns a `200 OK` response code and [signIn](../resources/signin.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="84017-132">例</span><span class="sxs-lookup"><span data-stu-id="84017-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="84017-133">要求</span><span class="sxs-lookup"><span data-stu-id="84017-133">Request</span></span>
<span data-ttu-id="84017-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="84017-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "reque|location/city| eq, startswith|
st",
  "name": "get_signin"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/signIns/{id}
```
##### <a name="response"></a><span data-ttu-id="84017-135">応答</span><span class="sxs-lookup"><span data-stu-id="84017-135">Response</span></span>
<span data-ttu-id="84017-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="84017-136">Here is an example of the response.</span></span> 
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
            "additionalDetails": "SignIn Success & CA Sucess"
        },
        "clientAppUsed": null,
        "deviceDetail": {
            "deviceId": "34390ed6-52b3-4102-aeff-aad2292abac3",
            "displayName": "DeviceName",
            "operatingSystem": "Windows 10",
            "browser": "Rich Client v1.0.2016.0",
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
  "tocPath": ""
}-->
