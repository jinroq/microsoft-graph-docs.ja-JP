---
title: メンバーを一覧表示する
description: ディレクトリ ロールに割り当てられているユーザーの一覧を取得します。  ディレクトリに割り当てることができるのはユーザーのみです。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5bc68b6a0a70a99c24e2f4cedd4ae909f201a13e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35459329"
---
# <a name="list-members"></a><span data-ttu-id="41cb0-104">メンバーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="41cb0-104">List members</span></span>

<span data-ttu-id="41cb0-105">ディレクトリ ロールに割り当てられているユーザーの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="41cb0-105">Retrieve a list of the users that are assigned to the directory role.</span></span>  <span data-ttu-id="41cb0-106">ディレクトリに割り当てることができるのはユーザーのみです。</span><span class="sxs-lookup"><span data-stu-id="41cb0-106">Only users can be assigned to a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="41cb0-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="41cb0-107">Permissions</span></span>
<span data-ttu-id="41cb0-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="41cb0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="41cb0-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="41cb0-110">Permission type</span></span>      | <span data-ttu-id="41cb0-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="41cb0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41cb0-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="41cb0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="41cb0-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="41cb0-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="41cb0-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="41cb0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41cb0-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="41cb0-115">Not supported.</span></span>    |
|<span data-ttu-id="41cb0-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="41cb0-116">Application</span></span> | <span data-ttu-id="41cb0-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41cb0-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="41cb0-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="41cb0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="41cb0-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="41cb0-119">Optional query parameters</span></span>
<span data-ttu-id="41cb0-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="41cb0-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="41cb0-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="41cb0-121">Request headers</span></span>
| <span data-ttu-id="41cb0-122">名前</span><span class="sxs-lookup"><span data-stu-id="41cb0-122">Name</span></span>       | <span data-ttu-id="41cb0-123">型</span><span class="sxs-lookup"><span data-stu-id="41cb0-123">Type</span></span> | <span data-ttu-id="41cb0-124">説明</span><span class="sxs-lookup"><span data-stu-id="41cb0-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="41cb0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="41cb0-125">Authorization</span></span>  | <span data-ttu-id="41cb0-126">string</span><span class="sxs-lookup"><span data-stu-id="41cb0-126">string</span></span>  | <span data-ttu-id="41cb0-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="41cb0-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="41cb0-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="41cb0-129">Request body</span></span>
<span data-ttu-id="41cb0-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="41cb0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41cb0-131">応答</span><span class="sxs-lookup"><span data-stu-id="41cb0-131">Response</span></span>

<span data-ttu-id="41cb0-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="41cb0-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="41cb0-133">例</span><span class="sxs-lookup"><span data-stu-id="41cb0-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="41cb0-134">要求</span><span class="sxs-lookup"><span data-stu-id="41cb0-134">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="41cb0-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="41cb0-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoles/{id}/members
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="41cb0-136">C#</span><span class="sxs-lookup"><span data-stu-id="41cb0-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="41cb0-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="41cb0-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="41cb0-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="41cb0-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="41cb0-139">応答</span><span class="sxs-lookup"><span data-stu-id="41cb0-139">Response</span></span>
<span data-ttu-id="41cb0-p105">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="41cb0-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "businessPhones":["000-000-0000"],
      "displayName":"First Last",
      "givenName":"First",
      "jobTitle":null,
      "mail":"first@example.com",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Last",
      "userPrincipalName":"first@example.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
