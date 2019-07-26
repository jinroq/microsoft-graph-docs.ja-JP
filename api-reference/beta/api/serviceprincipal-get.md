---
title: servicePrincipal を取得する
description: serviceprincipal オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Priority
ms.openlocfilehash: 00e437f0e80a59b51571e8871484b3b069f12f06
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870203"
---
# <a name="get-serviceprincipal"></a><span data-ttu-id="941c1-103">servicePrincipal を取得する</span><span class="sxs-lookup"><span data-stu-id="941c1-103">Get servicePrincipal</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="941c1-104">serviceprincipal オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="941c1-104">Retrieve the properties and relationships of serviceprincipal object.</span></span>
## <a name="permissions"></a><span data-ttu-id="941c1-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="941c1-105">Permissions</span></span>
<span data-ttu-id="941c1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="941c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="941c1-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="941c1-108">Permission type</span></span>      | <span data-ttu-id="941c1-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="941c1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="941c1-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="941c1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="941c1-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="941c1-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="941c1-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="941c1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="941c1-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="941c1-113">Not supported.</span></span>    |
|<span data-ttu-id="941c1-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="941c1-114">Application</span></span> | <span data-ttu-id="941c1-115">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="941c1-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="941c1-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="941c1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="941c1-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="941c1-117">Optional query parameters</span></span>
<span data-ttu-id="941c1-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="941c1-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="941c1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="941c1-119">Request headers</span></span>
| <span data-ttu-id="941c1-120">名前</span><span class="sxs-lookup"><span data-stu-id="941c1-120">Name</span></span>       | <span data-ttu-id="941c1-121">型</span><span class="sxs-lookup"><span data-stu-id="941c1-121">Type</span></span> | <span data-ttu-id="941c1-122">説明</span><span class="sxs-lookup"><span data-stu-id="941c1-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="941c1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="941c1-123">Authorization</span></span>  | <span data-ttu-id="941c1-124">string</span><span class="sxs-lookup"><span data-stu-id="941c1-124">string</span></span>  | <span data-ttu-id="941c1-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="941c1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="941c1-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="941c1-127">Request body</span></span>
<span data-ttu-id="941c1-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="941c1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="941c1-129">応答</span><span class="sxs-lookup"><span data-stu-id="941c1-129">Response</span></span>

<span data-ttu-id="941c1-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [servicePrincipal](../resources/serviceprincipal.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="941c1-130">If successful, this method returns a `200 OK` response code and [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="941c1-131">例</span><span class="sxs-lookup"><span data-stu-id="941c1-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="941c1-132">要求</span><span class="sxs-lookup"><span data-stu-id="941c1-132">Request</span></span>
<span data-ttu-id="941c1-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="941c1-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="941c1-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="941c1-134">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="941c1-135">C#</span><span class="sxs-lookup"><span data-stu-id="941c1-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="941c1-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="941c1-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="941c1-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="941c1-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="941c1-138">Java</span><span class="sxs-lookup"><span data-stu-id="941c1-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="941c1-139">応答</span><span class="sxs-lookup"><span data-stu-id="941c1-139">Response</span></span>
<span data-ttu-id="941c1-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="941c1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 391

{
  "accountEnabled": true,
  "addIns": [
    {
      "id": "id-value",
      "type": "type-value",
      "properties": [
        {
          "key": "key-value",
          "value": "value-value"
        }
      ]
    }
  ],
  "appDisplayName": "appDisplayName-value",
  "appId": "appId-value",
  "appOwnerOrganizationId": "appOwnerOrganizationId-value",
  "appRoleAssignmentRequired": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get servicePrincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
