---
title: ユーザーの取得
description: ユーザー オブジェクトのプロパティとリレーションシップを取得します。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ecbd6a5bba80b8e04aff5c7004ebb8cce2f792fc
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867678"
---
# <a name="get-a-user"></a><span data-ttu-id="66faf-103">ユーザーの取得</span><span class="sxs-lookup"><span data-stu-id="66faf-103">Get a user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66faf-104">ユーザー オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="66faf-104">Retrieve the properties and relationships of user object.</span></span>

<span data-ttu-id="66faf-105">**ユーザー** リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため、`GET` 操作を使用して、**ユーザー** インスタンスでカスタム プロパティと拡張機能データを取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="66faf-105">Since the **user** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **user** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="66faf-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="66faf-106">Permissions</span></span>
<span data-ttu-id="66faf-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="66faf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66faf-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="66faf-109">Permission type</span></span>      | <span data-ttu-id="66faf-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="66faf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66faf-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="66faf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="66faf-112">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="66faf-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="66faf-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="66faf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66faf-114">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66faf-114">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="66faf-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="66faf-115">Application</span></span> | <span data-ttu-id="66faf-116">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66faf-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="66faf-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="66faf-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="66faf-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="66faf-118">Optional query parameters</span></span>
<span data-ttu-id="66faf-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="66faf-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="66faf-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="66faf-120">Request headers</span></span>
| <span data-ttu-id="66faf-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="66faf-121">Header</span></span>       | <span data-ttu-id="66faf-122">値</span><span class="sxs-lookup"><span data-stu-id="66faf-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="66faf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="66faf-123">Authorization</span></span>  | <span data-ttu-id="66faf-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="66faf-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="66faf-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="66faf-126">Content-Type</span></span>   | <span data-ttu-id="66faf-127">application/json</span><span class="sxs-lookup"><span data-stu-id="66faf-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="66faf-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="66faf-128">Request body</span></span>
<span data-ttu-id="66faf-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="66faf-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66faf-130">応答</span><span class="sxs-lookup"><span data-stu-id="66faf-130">Response</span></span>

<span data-ttu-id="66faf-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [user](../resources/user.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="66faf-131">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

<span data-ttu-id="66faf-132">このメソッドは、要求が正常に処理されたが、サーバーが関連するバックグラウンド処理を完了するのにさらに時間を必要とする場合に `202 Accepted` を返します。</span><span class="sxs-lookup"><span data-stu-id="66faf-132">This method returns `202 Accepted` when the request has been processed successfully but the server requires more time to complete related background operations.</span></span>

## <a name="example"></a><span data-ttu-id="66faf-133">例</span><span class="sxs-lookup"><span data-stu-id="66faf-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="66faf-134">要求</span><span class="sxs-lookup"><span data-stu-id="66faf-134">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="66faf-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="66faf-135">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/beta/me
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="66faf-136">C#</span><span class="sxs-lookup"><span data-stu-id="66faf-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="66faf-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="66faf-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="66faf-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66faf-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="66faf-139">Java</span><span class="sxs-lookup"><span data-stu-id="66faf-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="66faf-140">応答</span><span class="sxs-lookup"><span data-stu-id="66faf-140">Response</span></span>
<span data-ttu-id="66faf-141">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="66faf-141">Here is an example of the response.</span></span> <span data-ttu-id="66faf-142">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="66faf-142">Note: The response object shown here may be truncated for brevity.</span></span> 

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

## <a name="see-also"></a><span data-ttu-id="66faf-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="66faf-143">See also</span></span>

- [<span data-ttu-id="66faf-144">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="66faf-144">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="66faf-145">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="66faf-145">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="66faf-146">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="66faf-146">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
