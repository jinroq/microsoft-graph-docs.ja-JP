---
title: List ownedObjects
description: ユーザーが所有しているディレクトリ オブジェクトの一覧を取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9175de1a96b23a1d86075be8e28765111f1899ea
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35456800"
---
# <a name="list-ownedobjects"></a><span data-ttu-id="492bc-103">List ownedObjects</span><span class="sxs-lookup"><span data-stu-id="492bc-103">List ownedObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="492bc-104">ユーザーが所有しているディレクトリ オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="492bc-104">Get the list of directory objects that are owned by the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="492bc-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="492bc-105">Permissions</span></span>
<span data-ttu-id="492bc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="492bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="492bc-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="492bc-108">Permission type</span></span>      | <span data-ttu-id="492bc-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="492bc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="492bc-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="492bc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="492bc-111">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="492bc-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="492bc-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="492bc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="492bc-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="492bc-113">Not supported.</span></span>    |
|<span data-ttu-id="492bc-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="492bc-114">Application</span></span> | <span data-ttu-id="492bc-115">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="492bc-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="492bc-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="492bc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/ownedObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="492bc-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="492bc-117">Optional query parameters</span></span>
<span data-ttu-id="492bc-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="492bc-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="492bc-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="492bc-119">Request headers</span></span>
| <span data-ttu-id="492bc-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="492bc-120">Header</span></span>       | <span data-ttu-id="492bc-121">値</span><span class="sxs-lookup"><span data-stu-id="492bc-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="492bc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="492bc-122">Authorization</span></span>  | <span data-ttu-id="492bc-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="492bc-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="492bc-125">承諾</span><span class="sxs-lookup"><span data-stu-id="492bc-125">Accept</span></span>  | <span data-ttu-id="492bc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="492bc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="492bc-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="492bc-127">Request body</span></span>
<span data-ttu-id="492bc-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="492bc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="492bc-129">応答</span><span class="sxs-lookup"><span data-stu-id="492bc-129">Response</span></span>

<span data-ttu-id="492bc-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="492bc-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="492bc-131">例</span><span class="sxs-lookup"><span data-stu-id="492bc-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="492bc-132">要求</span><span class="sxs-lookup"><span data-stu-id="492bc-132">Request</span></span>
<span data-ttu-id="492bc-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="492bc-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="492bc-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="492bc-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_ownedobjects"
}-->
```http
GET https://graph.microsoft.com/beta/me/ownedObjects
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="492bc-135">C#</span><span class="sxs-lookup"><span data-stu-id="492bc-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-ownedobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="492bc-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="492bc-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-ownedobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="492bc-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="492bc-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-ownedobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="492bc-138">応答</span><span class="sxs-lookup"><span data-stu-id="492bc-138">Response</span></span>
<span data-ttu-id="492bc-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="492bc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List ownedObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
