---
title: memberOf を一覧表示する
description: 'ユーザーがダイレクト メンバーになっているグループとディレクトリの役割を取得します。 '
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0a7ac90a4d8dcdb74234e80d2e0b70d4011792bf
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35460267"
---
# <a name="list-memberof"></a><span data-ttu-id="8aad3-103">memberOf を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="8aad3-103">List memberOf</span></span>

<span data-ttu-id="8aad3-104">ユーザーがダイレクト メンバーになっている[グループ](../resources/group.md)と[ディレクトリ ロール](../resources/directoryrole.md)を取得します。</span><span class="sxs-lookup"><span data-stu-id="8aad3-104">Get [groups](../resources/group.md) and [directory roles](../resources/directoryrole.md) that the user is a direct member of.</span></span> 

## <a name="permissions"></a><span data-ttu-id="8aad3-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8aad3-105">Permissions</span></span>
<span data-ttu-id="8aad3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8aad3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8aad3-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8aad3-108">Permission type</span></span>      | <span data-ttu-id="8aad3-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8aad3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8aad3-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8aad3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8aad3-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8aad3-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8aad3-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8aad3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8aad3-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8aad3-113">Not supported.</span></span>    |
|<span data-ttu-id="8aad3-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8aad3-114">Application</span></span> | <span data-ttu-id="8aad3-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8aad3-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8aad3-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8aad3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/memberOf
or
GET /users/{id | userPrincipalName}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8aad3-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8aad3-117">Optional query parameters</span></span>
<span data-ttu-id="8aad3-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8aad3-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="8aad3-119">$filter はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8aad3-119">$filter is not supported.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="8aad3-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8aad3-120">Request headers</span></span>
| <span data-ttu-id="8aad3-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8aad3-121">Header</span></span>       | <span data-ttu-id="8aad3-122">値</span><span class="sxs-lookup"><span data-stu-id="8aad3-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8aad3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8aad3-123">Authorization</span></span>  | <span data-ttu-id="8aad3-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8aad3-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8aad3-126">承諾</span><span class="sxs-lookup"><span data-stu-id="8aad3-126">Accept</span></span>  | <span data-ttu-id="8aad3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8aad3-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8aad3-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="8aad3-128">Request body</span></span>
<span data-ttu-id="8aad3-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8aad3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8aad3-130">応答</span><span class="sxs-lookup"><span data-stu-id="8aad3-130">Response</span></span>

<span data-ttu-id="8aad3-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="8aad3-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8aad3-132">例</span><span class="sxs-lookup"><span data-stu-id="8aad3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8aad3-133">要求</span><span class="sxs-lookup"><span data-stu-id="8aad3-133">Request</span></span>
<span data-ttu-id="8aad3-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8aad3-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8aad3-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="8aad3-135">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/memberOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8aad3-136">C#</span><span class="sxs-lookup"><span data-stu-id="8aad3-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8aad3-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="8aad3-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8aad3-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8aad3-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8aad3-139">応答</span><span class="sxs-lookup"><span data-stu-id="8aad3-139">Response</span></span>
<span data-ttu-id="8aad3-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8aad3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
