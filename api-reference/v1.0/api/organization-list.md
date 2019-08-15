---
title: 組織を一覧表示する
description: 組織オブジェクトのリストを取得します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 77338c81e01e49e69a03dbf9977e4e8a5aee1828
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36422190"
---
# <a name="list-organization"></a><span data-ttu-id="14b3f-103">組織を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="14b3f-103">List organization</span></span>



<span data-ttu-id="14b3f-104">組織オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="14b3f-104">Retrieve a list of organization objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="14b3f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="14b3f-105">Permissions</span></span>
<span data-ttu-id="14b3f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="14b3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14b3f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="14b3f-108">Permission type</span></span>      | <span data-ttu-id="14b3f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="14b3f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14b3f-110">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="14b3f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="14b3f-111">User.Read、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14b3f-111">User.Read, Directory.Read.All, Directory.ReadWrite.All</span></span>   |
|<span data-ttu-id="14b3f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="14b3f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14b3f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="14b3f-113">Not supported.</span></span>    |
|<span data-ttu-id="14b3f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="14b3f-114">Application</span></span> | <span data-ttu-id="14b3f-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14b3f-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="14b3f-116">注: User.Read アクセス許可を付与されたアプリケーションは、組織の *id*、*displayName*、および *verifiedDomains* プロパティのみを読み取ることができます。</span><span class="sxs-lookup"><span data-stu-id="14b3f-116">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="14b3f-117">他のすべてのプロパティは `null` 値を返します。</span><span class="sxs-lookup"><span data-stu-id="14b3f-117">All other properties will return with `null` values.</span></span> <span data-ttu-id="14b3f-118">すべてのプロパティを読み取るには、Directory.Read.All を使用します。</span><span class="sxs-lookup"><span data-stu-id="14b3f-118">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="14b3f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="14b3f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization
```
## <a name="optional-query-parameters"></a><span data-ttu-id="14b3f-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="14b3f-120">Optional query parameters</span></span>
<span data-ttu-id="14b3f-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="14b3f-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="14b3f-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="14b3f-122">Request headers</span></span>
| <span data-ttu-id="14b3f-123">名前</span><span class="sxs-lookup"><span data-stu-id="14b3f-123">Name</span></span>       | <span data-ttu-id="14b3f-124">型</span><span class="sxs-lookup"><span data-stu-id="14b3f-124">Type</span></span> | <span data-ttu-id="14b3f-125">説明</span><span class="sxs-lookup"><span data-stu-id="14b3f-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="14b3f-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="14b3f-126">Authorization</span></span>  | <span data-ttu-id="14b3f-127">string</span><span class="sxs-lookup"><span data-stu-id="14b3f-127">string</span></span>  | <span data-ttu-id="14b3f-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="14b3f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="14b3f-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="14b3f-130">Request body</span></span>
<span data-ttu-id="14b3f-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="14b3f-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14b3f-132">応答</span><span class="sxs-lookup"><span data-stu-id="14b3f-132">Response</span></span>

<span data-ttu-id="14b3f-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [organization](../resources/organization.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="14b3f-133">If successful, this method returns a `200 OK` response code and collection of [organization](../resources/organization.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="14b3f-134">例</span><span class="sxs-lookup"><span data-stu-id="14b3f-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="14b3f-135">要求</span><span class="sxs-lookup"><span data-stu-id="14b3f-135">Request</span></span>
<span data-ttu-id="14b3f-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="14b3f-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="14b3f-137">プロトコル</span><span class="sxs-lookup"><span data-stu-id="14b3f-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->
```http
GET https://graph.microsoft.com/beta/organization
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="14b3f-138">C#</span><span class="sxs-lookup"><span data-stu-id="14b3f-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="14b3f-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14b3f-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="14b3f-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="14b3f-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="14b3f-141">応答</span><span class="sxs-lookup"><span data-stu-id="14b3f-141">Response</span></span>
<span data-ttu-id="14b3f-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="14b3f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 500

{
  "value": [
    {
      "assignedPlans": [
        {
          "assignedDateTime": "2016-10-19T10:37:00Z",
          "capabilityStatus": "capabilityStatus-value",
          "service": "service-value",
          "servicePlanId": "servicePlanId-value"
        }
      ],
      "businessPhones": [
        "businessPhones-value"
      ],
      "city": "city-value",
      "country": "country-value",
      "countryLetterCode": "countryLetterCode-value",
      "displayName": "displayName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
