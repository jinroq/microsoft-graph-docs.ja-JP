---
title: アプリケーションを取得する
description: アプリケーション オブジェクトのプロパティと関係を取得します。
author: davidmu1
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 779eebd5cf283e237e25d7e9fb0b64e1cc8ed1eb
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408332"
---
# <a name="get-application"></a><span data-ttu-id="7aa6e-103">アプリケーションを取得する</span><span class="sxs-lookup"><span data-stu-id="7aa6e-103">Get application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7aa6e-104">アプリケーション オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="7aa6e-104">Retrieve the properties and relationships of application object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7aa6e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7aa6e-105">Permissions</span></span>
<span data-ttu-id="7aa6e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7aa6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7aa6e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7aa6e-108">Permission type</span></span>      | <span data-ttu-id="7aa6e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7aa6e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7aa6e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7aa6e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7aa6e-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7aa6e-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7aa6e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7aa6e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7aa6e-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7aa6e-113">Not supported.</span></span>    |
|<span data-ttu-id="7aa6e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7aa6e-114">Application</span></span> | <span data-ttu-id="7aa6e-115">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="7aa6e-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7aa6e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7aa6e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7aa6e-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7aa6e-117">Optional query parameters</span></span>
<span data-ttu-id="7aa6e-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7aa6e-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7aa6e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7aa6e-119">Request headers</span></span>
| <span data-ttu-id="7aa6e-120">名前</span><span class="sxs-lookup"><span data-stu-id="7aa6e-120">Name</span></span>       | <span data-ttu-id="7aa6e-121">種類</span><span class="sxs-lookup"><span data-stu-id="7aa6e-121">Type</span></span> | <span data-ttu-id="7aa6e-122">説明</span><span class="sxs-lookup"><span data-stu-id="7aa6e-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7aa6e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7aa6e-123">Authorization</span></span>  | <span data-ttu-id="7aa6e-124">string</span><span class="sxs-lookup"><span data-stu-id="7aa6e-124">string</span></span>  | <span data-ttu-id="7aa6e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7aa6e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7aa6e-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7aa6e-127">Request body</span></span>
<span data-ttu-id="7aa6e-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7aa6e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7aa6e-129">応答</span><span class="sxs-lookup"><span data-stu-id="7aa6e-129">Response</span></span>

<span data-ttu-id="7aa6e-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [application](../resources/application.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7aa6e-130">If successful, this method returns a `200 OK` response code and [application](../resources/application.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7aa6e-131">例</span><span class="sxs-lookup"><span data-stu-id="7aa6e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7aa6e-132">要求</span><span class="sxs-lookup"><span data-stu-id="7aa6e-132">Request</span></span>
<span data-ttu-id="7aa6e-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7aa6e-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7aa6e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="7aa6e-134">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_application"
}-->
```http
GET https://graph.microsoft.com/beta/applications/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7aa6e-135">C#</span><span class="sxs-lookup"><span data-stu-id="7aa6e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7aa6e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7aa6e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7aa6e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7aa6e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7aa6e-138">応答</span><span class="sxs-lookup"><span data-stu-id="7aa6e-138">Response</span></span>
<span data-ttu-id="7aa6e-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7aa6e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1044

{
  "api": {
    "acceptedAccessTokenVersion": 1,
    "publishedPermissionScopes": [
      {
        "adminConsentDescription": "adminConsentDescription-value",
        "adminConsentDisplayName": "adminConsentDisplayName-value",
        "id": "id-value",
        "isEnabled": true,
        "type": "type-value",
        "userConsentDescription": "userConsentDescription-value",
        "userConsentDisplayName": "userConsentDisplayName-value",
        "value": "value-value"
      }
    ]
  },
  "allowPublicClient": true,
  "applicationAliases": [
    "applicationAliases-value"
  ],
  "createdDateTime": "datetime-value",
  "installedClients": {
    "redirectUrls": [
      "redirectUrls-value"
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
