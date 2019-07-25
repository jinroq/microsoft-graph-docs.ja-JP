---
title: Get directoryRole
description: directoryrole オブジェクトのプロパティを取得します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7ae26075004d940ad522425d7665bfbb6abc4750
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865943"
---
# <a name="get-directoryrole"></a><span data-ttu-id="6836a-103">Get directoryRole</span><span class="sxs-lookup"><span data-stu-id="6836a-103">Get directoryRole</span></span>

<span data-ttu-id="6836a-104">directoryrole オブジェクトのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="6836a-104">Retrieve the properties of a directoryRole object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6836a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6836a-105">Permissions</span></span>
<span data-ttu-id="6836a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6836a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6836a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6836a-108">Permission type</span></span>      | <span data-ttu-id="6836a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6836a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6836a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6836a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6836a-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6836a-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6836a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6836a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6836a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6836a-113">Not supported.</span></span>    |
|<span data-ttu-id="6836a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6836a-114">Application</span></span> | <span data-ttu-id="6836a-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6836a-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6836a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6836a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6836a-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6836a-117">Optional query parameters</span></span>
<span data-ttu-id="6836a-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポート**していません** (例: $filter はここではサポートされていません)。</span><span class="sxs-lookup"><span data-stu-id="6836a-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6836a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6836a-119">Request headers</span></span>
| <span data-ttu-id="6836a-120">名前</span><span class="sxs-lookup"><span data-stu-id="6836a-120">Name</span></span>       | <span data-ttu-id="6836a-121">型</span><span class="sxs-lookup"><span data-stu-id="6836a-121">Type</span></span> | <span data-ttu-id="6836a-122">説明</span><span class="sxs-lookup"><span data-stu-id="6836a-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6836a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6836a-123">Authorization</span></span>  | <span data-ttu-id="6836a-124">string</span><span class="sxs-lookup"><span data-stu-id="6836a-124">string</span></span>  | <span data-ttu-id="6836a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6836a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6836a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="6836a-127">Request body</span></span>
<span data-ttu-id="6836a-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6836a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6836a-129">応答</span><span class="sxs-lookup"><span data-stu-id="6836a-129">Response</span></span>

<span data-ttu-id="6836a-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryRole](../resources/directoryrole.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6836a-130">If successful, this method returns a `200 OK` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6836a-131">例</span><span class="sxs-lookup"><span data-stu-id="6836a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6836a-132">要求</span><span class="sxs-lookup"><span data-stu-id="6836a-132">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6836a-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="6836a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoles/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6836a-134">C#</span><span class="sxs-lookup"><span data-stu-id="6836a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6836a-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="6836a-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6836a-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="6836a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6836a-137">Java</span><span class="sxs-lookup"><span data-stu-id="6836a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6836a-138">応答</span><span class="sxs-lookup"><span data-stu-id="6836a-138">Response</span></span>
<span data-ttu-id="6836a-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6836a-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
