---
title: ユーザーの所属を一覧表示する
description: ユーザーが直接メンバーであるグループ、ディレクトリロール、および管理単位を取得します。 この操作は推移的ではありません。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d09fc1f9b969c45c4b8db592cd45d066e2ff2caa
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35457717"
---
# <a name="list-user-memberof"></a><span data-ttu-id="b0617-104">ユーザーの所属を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="b0617-104">List user memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0617-105">ユーザーが直接メンバーであるグループ、ディレクトリロール、および管理単位を取得します。</span><span class="sxs-lookup"><span data-stu-id="b0617-105">Get groups, directory roles and administrative units that the user is a direct member of.</span></span> <span data-ttu-id="b0617-106">この操作は推移的ではありません。</span><span class="sxs-lookup"><span data-stu-id="b0617-106">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0617-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b0617-107">Permissions</span></span>

<span data-ttu-id="b0617-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b0617-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0617-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b0617-110">Permission type</span></span>      | <span data-ttu-id="b0617-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b0617-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0617-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b0617-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b0617-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b0617-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b0617-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b0617-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0617-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b0617-115">Not supported.</span></span>    |
|<span data-ttu-id="b0617-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b0617-116">Application</span></span> | <span data-ttu-id="b0617-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0617-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0617-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b0617-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/memberOf
or
GET /users/{id | userPrincipalName}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b0617-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b0617-119">Optional query parameters</span></span>

<span data-ttu-id="b0617-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b0617-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b0617-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b0617-121">Request headers</span></span>
| <span data-ttu-id="b0617-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b0617-122">Header</span></span>       | <span data-ttu-id="b0617-123">値</span><span class="sxs-lookup"><span data-stu-id="b0617-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b0617-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0617-124">Authorization</span></span>  | <span data-ttu-id="b0617-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b0617-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b0617-127">承諾</span><span class="sxs-lookup"><span data-stu-id="b0617-127">Accept</span></span>  | <span data-ttu-id="b0617-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b0617-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0617-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="b0617-129">Request body</span></span>

<span data-ttu-id="b0617-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b0617-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0617-131">応答</span><span class="sxs-lookup"><span data-stu-id="b0617-131">Response</span></span>

<span data-ttu-id="b0617-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="b0617-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0617-133">例</span><span class="sxs-lookup"><span data-stu-id="b0617-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0617-134">要求</span><span class="sxs-lookup"><span data-stu-id="b0617-134">Request</span></span>

<span data-ttu-id="b0617-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b0617-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b0617-136">プロトコル</span><span class="sxs-lookup"><span data-stu-id="b0617-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/me/memberOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b0617-137">C#</span><span class="sxs-lookup"><span data-stu-id="b0617-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b0617-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="b0617-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b0617-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="b0617-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b0617-140">応答</span><span class="sxs-lookup"><span data-stu-id="b0617-140">Response</span></span>

<span data-ttu-id="b0617-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b0617-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
