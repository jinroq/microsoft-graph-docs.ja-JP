---
title: ownedDevices を一覧表示する
description: ユーザーが所有しているデバイスの一覧を取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9080c0eeb8a1967dd28990aa37f6b4783f4733e3
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36362184"
---
# <a name="list-owneddevices"></a><span data-ttu-id="430f3-103">ownedDevices を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="430f3-103">List ownedDevices</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="430f3-104">ユーザーが所有しているデバイスの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="430f3-104">Get the list of devices that are owned by the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="430f3-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="430f3-105">Permissions</span></span>
<span data-ttu-id="430f3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="430f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="430f3-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="430f3-108">Permission type</span></span>      | <span data-ttu-id="430f3-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="430f3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="430f3-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="430f3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="430f3-111">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="430f3-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="430f3-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="430f3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="430f3-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="430f3-113">Not supported.</span></span>    |
|<span data-ttu-id="430f3-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="430f3-114">Application</span></span> | <span data-ttu-id="430f3-115">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="430f3-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="430f3-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="430f3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/ownedDevices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="430f3-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="430f3-117">Optional query parameters</span></span>
<span data-ttu-id="430f3-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="430f3-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="430f3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="430f3-119">Request headers</span></span>
| <span data-ttu-id="430f3-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="430f3-120">Header</span></span>       | <span data-ttu-id="430f3-121">値</span><span class="sxs-lookup"><span data-stu-id="430f3-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="430f3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="430f3-122">Authorization</span></span>  | <span data-ttu-id="430f3-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="430f3-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="430f3-125">承諾</span><span class="sxs-lookup"><span data-stu-id="430f3-125">Accept</span></span>  | <span data-ttu-id="430f3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="430f3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="430f3-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="430f3-127">Request body</span></span>
<span data-ttu-id="430f3-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="430f3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="430f3-129">応答</span><span class="sxs-lookup"><span data-stu-id="430f3-129">Response</span></span>

<span data-ttu-id="430f3-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="430f3-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="430f3-131">例</span><span class="sxs-lookup"><span data-stu-id="430f3-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="430f3-132">要求</span><span class="sxs-lookup"><span data-stu-id="430f3-132">Request</span></span>
<span data-ttu-id="430f3-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="430f3-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="430f3-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="430f3-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_owneddevices"
}-->
```http
GET https://graph.microsoft.com/beta/me/ownedDevices
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="430f3-135">C#</span><span class="sxs-lookup"><span data-stu-id="430f3-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-owneddevices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="430f3-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="430f3-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-owneddevices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="430f3-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="430f3-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-owneddevices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="430f3-138">Java</span><span class="sxs-lookup"><span data-stu-id="430f3-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-owneddevices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="430f3-139">応答</span><span class="sxs-lookup"><span data-stu-id="430f3-139">Response</span></span>
<span data-ttu-id="430f3-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="430f3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List ownedDevices",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
