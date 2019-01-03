---
title: ユーザーの取得
description: ユーザー オブジェクトのプロパティと関係を取得します。
author: dkershaw10
ms.openlocfilehash: eb2b3efe96e3fd4e4608ae045addaf8a1fe6911a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341574"
---
# <a name="get-a-user"></a><span data-ttu-id="6000c-103">ユーザーの取得</span><span class="sxs-lookup"><span data-stu-id="6000c-103">Get a user</span></span>

> <span data-ttu-id="6000c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6000c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6000c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6000c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6000c-106">ユーザー オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="6000c-106">Retrieve the properties and relationships of user object.</span></span>

<span data-ttu-id="6000c-107">**ユーザー**のリソースは、[拡張機能](/graph/extensibility-overview)をサポートするため使用することも、 `GET` 、**ユーザー**インスタンスのカスタム プロパティと拡張機能のデータを取得する操作です。</span><span class="sxs-lookup"><span data-stu-id="6000c-107">Since the **user** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **user** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="6000c-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6000c-108">Permissions</span></span>
<span data-ttu-id="6000c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6000c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6000c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6000c-111">Permission type</span></span>      | <span data-ttu-id="6000c-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6000c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6000c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6000c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6000c-114">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6000c-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6000c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6000c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6000c-116">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6000c-116">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="6000c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6000c-117">Application</span></span> | <span data-ttu-id="6000c-118">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6000c-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6000c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6000c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6000c-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6000c-120">Optional query parameters</span></span>
<span data-ttu-id="6000c-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6000c-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6000c-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6000c-122">Request headers</span></span>
| <span data-ttu-id="6000c-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6000c-123">Header</span></span>       | <span data-ttu-id="6000c-124">値</span><span class="sxs-lookup"><span data-stu-id="6000c-124">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="6000c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6000c-125">Authorization</span></span>  | <span data-ttu-id="6000c-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6000c-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="6000c-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6000c-128">Content-Type</span></span>   | <span data-ttu-id="6000c-129">application/json</span><span class="sxs-lookup"><span data-stu-id="6000c-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="6000c-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="6000c-130">Request body</span></span>
<span data-ttu-id="6000c-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6000c-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6000c-132">応答</span><span class="sxs-lookup"><span data-stu-id="6000c-132">Response</span></span>

<span data-ttu-id="6000c-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[ユーザー](../resources/user.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6000c-133">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6000c-134">例</span><span class="sxs-lookup"><span data-stu-id="6000c-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6000c-135">要求</span><span class="sxs-lookup"><span data-stu-id="6000c-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/beta/me
```
##### <a name="response"></a><span data-ttu-id="6000c-136">応答</span><span class="sxs-lookup"><span data-stu-id="6000c-136">Response</span></span>
<span data-ttu-id="6000c-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="6000c-137">Here is an example of the response.</span></span> <span data-ttu-id="6000c-138">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="6000c-138">Note: The response object shown here may be truncated for brevity.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

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
```

## <a name="see-also"></a><span data-ttu-id="6000c-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="6000c-139">See also</span></span>

- [<span data-ttu-id="6000c-140">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="6000c-140">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="6000c-141">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="6000c-141">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="6000c-142">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="6000c-142">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->