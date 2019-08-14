---
title: ユーザーの取得
description: ユーザー オブジェクトのプロパティとリレーションシップを取得します。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 583e09548ed514c90fb541d264f31dc278324d1a
ms.sourcegitcommit: 3db93e28e215c0e09a65b4705ba956c6ac3b5426
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/14/2019
ms.locfileid: "36396752"
---
# <a name="get-a-user"></a><span data-ttu-id="614ca-103">ユーザーの取得</span><span class="sxs-lookup"><span data-stu-id="614ca-103">Get a user</span></span>

<span data-ttu-id="614ca-104">ユーザー オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="614ca-104">Retrieve the properties and relationships of user object.</span></span>

> <span data-ttu-id="614ca-p101">注:ユーザーを取得すると、プロパティの既定セットのみが返されます (*businessPhones、displayName、givenName、id、jobTitle、mail、mobilePhone、officeLocation、preferredLanguage、surname、userPrincipalName*)。`$select` を使用して、[ユーザー](../resources/user.md) オブジェクトの他のプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="614ca-p101">Note: Getting a user returns a default set of properties only (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). Use `$select` to get the other properties and relationships for the [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="614ca-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="614ca-107">Permissions</span></span>
<span data-ttu-id="614ca-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="614ca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="614ca-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="614ca-110">Permission type</span></span>      | <span data-ttu-id="614ca-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="614ca-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="614ca-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="614ca-112">Delegated (work or school account)</span></span> | <span data-ttu-id="614ca-113">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="614ca-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="614ca-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="614ca-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="614ca-115">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="614ca-115">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="614ca-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="614ca-116">Application</span></span> | <span data-ttu-id="614ca-117">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="614ca-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="614ca-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="614ca-118">HTTP request</span></span>
<span data-ttu-id="614ca-119">特定のユーザー:</span><span class="sxs-lookup"><span data-stu-id="614ca-119">For a specific user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```

<span data-ttu-id="614ca-120">サインイン ユーザー:</span><span class="sxs-lookup"><span data-stu-id="614ca-120">For the signed-in user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me
```

## <a name="optional-query-parameters"></a><span data-ttu-id="614ca-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="614ca-121">Optional query parameters</span></span>
<span data-ttu-id="614ca-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="614ca-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="614ca-123">既定では、限定的なプロパティのセットのみが返されます (_businessPhones、displayName、givenName、id、jobTitle、mail、mobilePhone、officeLocation、preferredLanguage、surname、userPrincipalName_)。</span><span class="sxs-lookup"><span data-stu-id="614ca-123">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> 

<span data-ttu-id="614ca-124">別のプロパティ セットを返すには、OData `$select` クエリ パラメーターを使用して、目的の [user](../resources/user.md) プロパティのセットを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="614ca-124">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="614ca-125">たとえば、_displayName_、_givenName_、_postalCode_ を返すには、クエリに `$select=displayName,givenName,postalCode` を追加します。</span><span class="sxs-lookup"><span data-stu-id="614ca-125">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

## <a name="request-headers"></a><span data-ttu-id="614ca-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="614ca-126">Request headers</span></span>
| <span data-ttu-id="614ca-127">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="614ca-127">Header</span></span>       | <span data-ttu-id="614ca-128">値</span><span class="sxs-lookup"><span data-stu-id="614ca-128">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="614ca-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="614ca-129">Authorization</span></span>  | <span data-ttu-id="614ca-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="614ca-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="614ca-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="614ca-132">Content-Type</span></span>   | <span data-ttu-id="614ca-133">application/json</span><span class="sxs-lookup"><span data-stu-id="614ca-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="614ca-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="614ca-134">Request body</span></span>
<span data-ttu-id="614ca-135">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="614ca-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="614ca-136">応答</span><span class="sxs-lookup"><span data-stu-id="614ca-136">Response</span></span>

<span data-ttu-id="614ca-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [user](../resources/user.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="614ca-137">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

<span data-ttu-id="614ca-138">このメソッドは、要求が正常に処理されたが、サーバーが関連するバックグラウンド処理を完了するのにさらに時間を必要とする場合に `202 Accepted` を返します。</span><span class="sxs-lookup"><span data-stu-id="614ca-138">This method returns `202 Accepted` when the request has been processed successfully but the server requires more time to complete related background operations.</span></span>

## <a name="examples"></a><span data-ttu-id="614ca-139">例</span><span class="sxs-lookup"><span data-stu-id="614ca-139">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="614ca-140">例 1:標準的なユーザーの要求</span><span class="sxs-lookup"><span data-stu-id="614ca-140">Example 1: Standard users request</span></span>

<span data-ttu-id="614ca-141">既定では、限定的なプロパティのセットのみが返されます (_businessPhones、displayName、givenName、id、jobTitle、mail、mobilePhone、officeLocation、preferredLanguage、surname、userPrincipalName_)。</span><span class="sxs-lookup"><span data-stu-id="614ca-141">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> <span data-ttu-id="614ca-142">この例では、既定の要求と応答を示します。</span><span class="sxs-lookup"><span data-stu-id="614ca-142">This example illustrates the default request and response.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}
```

##### <a name="response"></a><span data-ttu-id="614ca-143">応答</span><span class="sxs-lookup"><span data-stu-id="614ca-143">Response</span></span>

<!-- { "blockType": "ignored" } -->
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


### <a name="example-2-signed-in-user-request"></a><span data-ttu-id="614ca-144">例 2: サインインしているユーザーの要求</span><span class="sxs-lookup"><span data-stu-id="614ca-144">Example 2: Signed-in user request</span></span>

<span data-ttu-id="614ca-145">`/users/{id | userPrincipalName}` を `/me` に置き換えると、サインイン ユーザーのユーザー情報を取得できます。</span><span class="sxs-lookup"><span data-stu-id="614ca-145">You can get the user information for the signed-in user by replacing `/users/{id | userPrincipalName}` with `/me`.</span></span>

##### <a name="request"></a><span data-ttu-id="614ca-146">要求</span><span class="sxs-lookup"><span data-stu-id="614ca-146">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="614ca-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="614ca-147">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="614ca-148">C#</span><span class="sxs-lookup"><span data-stu-id="614ca-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="614ca-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="614ca-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="614ca-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="614ca-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="614ca-151">Java</span><span class="sxs-lookup"><span data-stu-id="614ca-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="614ca-152">応答</span><span class="sxs-lookup"><span data-stu-id="614ca-152">Response</span></span>

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

### <a name="example-3-users-request-using-select"></a><span data-ttu-id="614ca-153">例 3: $select を使用したユーザーの要求</span><span class="sxs-lookup"><span data-stu-id="614ca-153">Example 3: Users request using $select</span></span>

<span data-ttu-id="614ca-154">別のプロパティ セットを必要とする場合、OData `$select` クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="614ca-154">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="614ca-155">たとえば、_displayName_、_givenName_、_postalCode_ を返すには、クエリに `$select=displayName,givenName,postalCode` を追加します。</span><span class="sxs-lookup"><span data-stu-id="614ca-155">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

##### <a name="request"></a><span data-ttu-id="614ca-156">要求</span><span class="sxs-lookup"><span data-stu-id="614ca-156">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}?$select=displayName,givenName,postalCode
```
##### <a name="response"></a><span data-ttu-id="614ca-157">応答</span><span class="sxs-lookup"><span data-stu-id="614ca-157">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
   "displayName": "displayName-value",
   "givenName": "givenName-value",
   "postalCode": "postalCode-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
