---
title: ユーザー推移的な memberOf を一覧表示する
description: ユーザーがメンバーになっているグループ、ディレクトリロールを取得します。 この API 要求は推移的なので、ユーザーがネストされたメンバーであるすべてのグループも返します。
author: anchanda
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 3c2a8f06b02870d2a1f0d021d77883ab7acf1d70
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36316261"
---
# <a name="list-user-transitive-memberof"></a><span data-ttu-id="07620-104">ユーザー推移的な memberOf を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="07620-104">List user transitive memberOf</span></span>

<span data-ttu-id="07620-105">ユーザーがメンバーになっているグループ、ディレクトリロールを取得します。</span><span class="sxs-lookup"><span data-stu-id="07620-105">Get groups, directory roles that the user is a member of.</span></span> <span data-ttu-id="07620-106">この API 要求は推移的なので、ユーザーがネストされたメンバーであるすべてのグループも返します。</span><span class="sxs-lookup"><span data-stu-id="07620-106">This API request is transitive, and will also return all groups the user is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="07620-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="07620-107">Permissions</span></span>

<span data-ttu-id="07620-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="07620-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07620-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="07620-110">Permission type</span></span>      | <span data-ttu-id="07620-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="07620-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07620-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="07620-112">Delegated (work or school account)</span></span> | <span data-ttu-id="07620-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="07620-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="07620-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="07620-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07620-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="07620-115">Not supported.</span></span>    |
|<span data-ttu-id="07620-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="07620-116">Application</span></span> | <span data-ttu-id="07620-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07620-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="07620-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="07620-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="07620-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="07620-119">Optional query parameters</span></span>

<span data-ttu-id="07620-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="07620-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="07620-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="07620-121">Request headers</span></span>

| <span data-ttu-id="07620-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="07620-122">Header</span></span>       | <span data-ttu-id="07620-123">値</span><span class="sxs-lookup"><span data-stu-id="07620-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="07620-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="07620-124">Authorization</span></span>  | <span data-ttu-id="07620-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="07620-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="07620-127">承諾</span><span class="sxs-lookup"><span data-stu-id="07620-127">Accept</span></span>  | <span data-ttu-id="07620-128">application/json</span><span class="sxs-lookup"><span data-stu-id="07620-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07620-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="07620-129">Request body</span></span>

<span data-ttu-id="07620-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="07620-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07620-131">応答</span><span class="sxs-lookup"><span data-stu-id="07620-131">Response</span></span>

<span data-ttu-id="07620-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="07620-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07620-133">例</span><span class="sxs-lookup"><span data-stu-id="07620-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="07620-134">要求</span><span class="sxs-lookup"><span data-stu-id="07620-134">Request</span></span>

<span data-ttu-id="07620-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="07620-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="07620-136">プロトコル</span><span class="sxs-lookup"><span data-stu-id="07620-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/transitiveMemberOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="07620-137">C#</span><span class="sxs-lookup"><span data-stu-id="07620-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="07620-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="07620-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="07620-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="07620-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="07620-140">Java</span><span class="sxs-lookup"><span data-stu-id="07620-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="07620-141">応答</span><span class="sxs-lookup"><span data-stu-id="07620-141">Response</span></span>

<span data-ttu-id="07620-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="07620-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
