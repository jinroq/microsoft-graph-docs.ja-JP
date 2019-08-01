---
title: 組織を取得する
description: 現在認証されている組織のプロパティとリレーションシップを取得します。
localization_priority: Priority
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 87b4284416e68b411bd772a86b9984f18848c6b9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36022685"
---
# <a name="get-organization"></a><span data-ttu-id="bda32-103">組織を取得する</span><span class="sxs-lookup"><span data-stu-id="bda32-103">Get organization</span></span>

<span data-ttu-id="bda32-104">現在認証されている組織のプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="bda32-104">Retrieve the properties and relationships of currently authenticated organization.</span></span>

<span data-ttu-id="bda32-105">**organization** リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため、`GET` 操作を使用して、**organization** インスタンスでカスタム プロパティと拡張機能データを取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="bda32-105">Since the **event** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **event** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="bda32-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bda32-106">Permissions</span></span>

<span data-ttu-id="bda32-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bda32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bda32-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bda32-109">Permission type</span></span>      | <span data-ttu-id="bda32-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bda32-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bda32-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bda32-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bda32-112">User.Read、Organization.Read.All、Directory.Read.All、Organization.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bda32-112">User.Read, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="bda32-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bda32-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bda32-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bda32-114">Not supported.</span></span>    |
|<span data-ttu-id="bda32-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bda32-115">Application</span></span> | <span data-ttu-id="bda32-116">Organization.Read.All、Directory.Read.All、Organization.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bda32-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="bda32-117">**注**: User.Read アクセス許可を付与されたアプリケーションは、組織の **id**、**displayName**、および **verifiedDomains** プロパティのみを読み取ることができます。</span><span class="sxs-lookup"><span data-stu-id="bda32-117">Note: Applications granted the User.Read permission are able to read only the id, displayName, and verifiedDomains properties of the organization.</span></span>  <span data-ttu-id="bda32-118">他のすべてのプロパティは `null` 値を返します。</span><span class="sxs-lookup"><span data-stu-id="bda32-118">All other properties will return with `null` values.</span></span> <span data-ttu-id="bda32-119">すべてのプロパティを読み取るには、Organization.Read.All を使用します。</span><span class="sxs-lookup"><span data-stu-id="bda32-119">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="bda32-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bda32-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bda32-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="bda32-121">Optional query parameters</span></span>

<span data-ttu-id="bda32-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="bda32-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bda32-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bda32-123">Request headers</span></span>

| <span data-ttu-id="bda32-124">名前</span><span class="sxs-lookup"><span data-stu-id="bda32-124">Name</span></span>       | <span data-ttu-id="bda32-125">説明</span><span class="sxs-lookup"><span data-stu-id="bda32-125">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="bda32-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="bda32-126">Authorization</span></span>  | <span data-ttu-id="bda32-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bda32-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bda32-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="bda32-129">Request body</span></span>

<span data-ttu-id="bda32-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="bda32-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bda32-131">応答</span><span class="sxs-lookup"><span data-stu-id="bda32-131">Response</span></span>

<span data-ttu-id="bda32-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で 1 つの [organization](../resources/organization.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="bda32-132">If successful, this method returns a `200 OK` response code and a collection of one [organization](../resources/organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bda32-133">例</span><span class="sxs-lookup"><span data-stu-id="bda32-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bda32-134">要求</span><span class="sxs-lookup"><span data-stu-id="bda32-134">Request</span></span>

<span data-ttu-id="bda32-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bda32-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bda32-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="bda32-136">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->

```http
GET https://graph.microsoft.com/v1.0/organization
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bda32-137">C#</span><span class="sxs-lookup"><span data-stu-id="bda32-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bda32-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="bda32-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bda32-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bda32-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bda32-140">Java</span><span class="sxs-lookup"><span data-stu-id="bda32-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bda32-141">応答</span><span class="sxs-lookup"><span data-stu-id="bda32-141">Response</span></span>

<span data-ttu-id="bda32-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bda32-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 411

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#organization",
  "value": [
    {
      "assignedPlans": [
        {
          "assignedDateTime": "datetime-value",
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
  "description": "Get organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
