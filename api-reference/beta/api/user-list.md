---
title: ユーザーを一覧表示する
description: ユーザー オブジェクトのリストを取得します。
author: dkershaw10
ms.openlocfilehash: 6d80bde11d5370a87432394c191519bc9a1780ab
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361937"
---
# <a name="list-users"></a><span data-ttu-id="0cd88-103">ユーザーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="0cd88-103">List users</span></span>

> <span data-ttu-id="0cd88-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中で、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0cd88-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0cd88-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0cd88-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0cd88-106">ユーザー オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="0cd88-106">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="0cd88-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0cd88-107">Permissions</span></span>

<span data-ttu-id="0cd88-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0cd88-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cd88-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0cd88-110">Permission type</span></span>      | <span data-ttu-id="0cd88-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0cd88-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0cd88-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0cd88-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0cd88-113">User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0cd88-113">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0cd88-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0cd88-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0cd88-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0cd88-115">Not supported.</span></span>    |
|<span data-ttu-id="0cd88-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0cd88-116">Application</span></span> | <span data-ttu-id="0cd88-117">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cd88-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0cd88-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0cd88-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0cd88-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="0cd88-119">Optional query parameters</span></span>

<span data-ttu-id="0cd88-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="0cd88-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0cd88-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0cd88-121">Request headers</span></span>
| <span data-ttu-id="0cd88-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0cd88-122">Header</span></span>        | <span data-ttu-id="0cd88-123">値</span><span class="sxs-lookup"><span data-stu-id="0cd88-123">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="0cd88-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0cd88-124">Authorization</span></span> | <span data-ttu-id="0cd88-125">Bearer {トークン} (必須)</span><span class="sxs-lookup"><span data-stu-id="0cd88-125">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="0cd88-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0cd88-126">Content-Type</span></span>  | <span data-ttu-id="0cd88-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0cd88-127">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="0cd88-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="0cd88-128">Request body</span></span>

<span data-ttu-id="0cd88-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0cd88-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0cd88-130">応答</span><span class="sxs-lookup"><span data-stu-id="0cd88-130">Response</span></span>

<span data-ttu-id="0cd88-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [user](../resources/user.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="0cd88-131">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cd88-132">例</span><span class="sxs-lookup"><span data-stu-id="0cd88-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0cd88-133">要求</span><span class="sxs-lookup"><span data-stu-id="0cd88-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/beta/users
```

##### <a name="response"></a><span data-ttu-id="0cd88-134">応答</span><span class="sxs-lookup"><span data-stu-id="0cd88-134">Response</span></span>

<span data-ttu-id="0cd88-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="0cd88-135">Here is an example of the response.</span></span> <span data-ttu-id="0cd88-136">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="0cd88-136">Note: The response object shown here may be truncated for brevity.</span></span> 

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->