---
title: 組織を一覧表示する
description: 組織オブジェクトのリストを取得します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e62157fe7fec29df4afd1e4d931a28fa6e3b77f8
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33611670"
---
# <a name="list-organization"></a><span data-ttu-id="a5397-103">組織を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="a5397-103">List organization</span></span>



<span data-ttu-id="a5397-104">組織オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="a5397-104">Retrieve a list of organization objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="a5397-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a5397-105">Permissions</span></span>
<span data-ttu-id="a5397-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a5397-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5397-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a5397-108">Permission type</span></span>      | <span data-ttu-id="a5397-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a5397-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5397-110">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="a5397-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a5397-111">User.Read、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5397-111">User.Read, Directory.Read.All, Directory.ReadWrite.All</span></span>   |
|<span data-ttu-id="a5397-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a5397-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5397-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5397-113">Not supported.</span></span>    |
|<span data-ttu-id="a5397-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a5397-114">Application</span></span> | <span data-ttu-id="a5397-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5397-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="a5397-116">注: User.Read アクセス許可を付与されたアプリケーションは、組織の *id*、*displayName*、および *verifiedDomains* プロパティのみを読み取ることができます。</span><span class="sxs-lookup"><span data-stu-id="a5397-116">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="a5397-117">他のすべてのプロパティは `null` 値を返します。</span><span class="sxs-lookup"><span data-stu-id="a5397-117">All other properties will return with `null` values.</span></span> <span data-ttu-id="a5397-118">すべてのプロパティを読み取るには、Directory.Read.All を使用します。</span><span class="sxs-lookup"><span data-stu-id="a5397-118">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="a5397-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a5397-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a5397-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a5397-120">Optional query parameters</span></span>
<span data-ttu-id="a5397-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a5397-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a5397-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a5397-122">Request headers</span></span>
| <span data-ttu-id="a5397-123">名前</span><span class="sxs-lookup"><span data-stu-id="a5397-123">Name</span></span>       | <span data-ttu-id="a5397-124">型</span><span class="sxs-lookup"><span data-stu-id="a5397-124">Type</span></span> | <span data-ttu-id="a5397-125">説明</span><span class="sxs-lookup"><span data-stu-id="a5397-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a5397-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5397-126">Authorization</span></span>  | <span data-ttu-id="a5397-127">string</span><span class="sxs-lookup"><span data-stu-id="a5397-127">string</span></span>  | <span data-ttu-id="a5397-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a5397-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5397-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="a5397-130">Request body</span></span>
<span data-ttu-id="a5397-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a5397-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5397-132">応答</span><span class="sxs-lookup"><span data-stu-id="a5397-132">Response</span></span>

<span data-ttu-id="a5397-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [organization](../resources/organization.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="a5397-133">If successful, this method returns a `200 OK` response code and collection of [organization](../resources/organization.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a5397-134">例</span><span class="sxs-lookup"><span data-stu-id="a5397-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a5397-135">要求</span><span class="sxs-lookup"><span data-stu-id="a5397-135">Request</span></span>
<span data-ttu-id="a5397-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a5397-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->
```http
GET https://graph.microsoft.com/beta/organization
```
##### <a name="response"></a><span data-ttu-id="a5397-137">応答</span><span class="sxs-lookup"><span data-stu-id="a5397-137">Response</span></span>
<span data-ttu-id="a5397-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a5397-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="a5397-141">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="a5397-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a5397-142">Visual</span><span class="sxs-lookup"><span data-stu-id="a5397-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_organization-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a5397-143">Java</span><span class="sxs-lookup"><span data-stu-id="a5397-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_organization-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/organization-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/organization-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
