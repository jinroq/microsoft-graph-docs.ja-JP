---
title: ユーザーを一覧表示する
description: ユーザー オブジェクトの一覧を取得します。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f8fcaff790c1069ee58b569b19adec4d432f7b8a
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637158"
---
# <a name="list-users"></a><span data-ttu-id="1c5b0-103">ユーザーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1c5b0-103">List users</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c5b0-104">ユーザー オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="1c5b0-104">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c5b0-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1c5b0-105">Permissions</span></span>

<span data-ttu-id="1c5b0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1c5b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c5b0-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1c5b0-108">Permission type</span></span>      | <span data-ttu-id="1c5b0-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1c5b0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c5b0-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1c5b0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1c5b0-111">User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1c5b0-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1c5b0-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1c5b0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c5b0-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1c5b0-113">Not supported.</span></span>    |
|<span data-ttu-id="1c5b0-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1c5b0-114">Application</span></span> | <span data-ttu-id="1c5b0-115">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c5b0-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c5b0-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1c5b0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1c5b0-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="1c5b0-117">Optional query parameters</span></span>

<span data-ttu-id="1c5b0-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="1c5b0-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1c5b0-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1c5b0-119">Request headers</span></span>
| <span data-ttu-id="1c5b0-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1c5b0-120">Header</span></span>        | <span data-ttu-id="1c5b0-121">値</span><span class="sxs-lookup"><span data-stu-id="1c5b0-121">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="1c5b0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c5b0-122">Authorization</span></span> | <span data-ttu-id="1c5b0-123">Bearer {トークン} (必須)</span><span class="sxs-lookup"><span data-stu-id="1c5b0-123">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="1c5b0-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1c5b0-124">Content-Type</span></span>  | <span data-ttu-id="1c5b0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1c5b0-125">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="1c5b0-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="1c5b0-126">Request body</span></span>

<span data-ttu-id="1c5b0-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1c5b0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c5b0-128">応答</span><span class="sxs-lookup"><span data-stu-id="1c5b0-128">Response</span></span>

<span data-ttu-id="1c5b0-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [user](../resources/user.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="1c5b0-129">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c5b0-130">例</span><span class="sxs-lookup"><span data-stu-id="1c5b0-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1c5b0-131">要求</span><span class="sxs-lookup"><span data-stu-id="1c5b0-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/beta/users
```

##### <a name="response"></a><span data-ttu-id="1c5b0-132">応答</span><span class="sxs-lookup"><span data-stu-id="1c5b0-132">Response</span></span>

<span data-ttu-id="1c5b0-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="1c5b0-133">Here is an example of the response.</span></span> <span data-ttu-id="1c5b0-134">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="1c5b0-134">Note: The response object shown here may be truncated for brevity.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 608

{
  "value": [
    {
      "businessPhones": [
        "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1c5b0-135">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="1c5b0-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1c5b0-136">C#</span><span class="sxs-lookup"><span data-stu-id="1c5b0-136">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_users-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1c5b0-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="1c5b0-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_users-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
