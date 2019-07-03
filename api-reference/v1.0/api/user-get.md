---
title: ユーザーの取得
description: ユーザー オブジェクトのプロパティとリレーションシップを取得します。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4eb5d65de63d6996189c49023d5d9de106348c61
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35460470"
---
# <a name="get-a-user"></a><span data-ttu-id="36a02-103">ユーザーの取得</span><span class="sxs-lookup"><span data-stu-id="36a02-103">Get a user</span></span>

<span data-ttu-id="36a02-104">ユーザー オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="36a02-104">Retrieve the properties and relationships of user object.</span></span>

> <span data-ttu-id="36a02-p101">注:ユーザーを取得すると、プロパティの既定セットのみが返されます (*businessPhones、displayName、givenName、id、jobTitle、mail、mobilePhone、officeLocation、preferredLanguage、surname、userPrincipalName*)。`$select` を使用して、[ユーザー](../resources/user.md) オブジェクトの他のプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="36a02-p101">Note: Getting a user returns a default set of properties only (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). Use `$select` to get the other properties and relationships for the [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="36a02-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="36a02-107">Permissions</span></span>
<span data-ttu-id="36a02-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="36a02-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36a02-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="36a02-110">Permission type</span></span>      | <span data-ttu-id="36a02-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="36a02-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36a02-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="36a02-112">Delegated (work or school account)</span></span> | <span data-ttu-id="36a02-113">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="36a02-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="36a02-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="36a02-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36a02-115">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="36a02-115">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="36a02-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="36a02-116">Application</span></span> | <span data-ttu-id="36a02-117">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36a02-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="36a02-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="36a02-118">HTTP request</span></span>
<span data-ttu-id="36a02-119">特定のユーザー:</span><span class="sxs-lookup"><span data-stu-id="36a02-119">For a specific user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```

<span data-ttu-id="36a02-120">サインイン ユーザー:</span><span class="sxs-lookup"><span data-stu-id="36a02-120">For the signed-in user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me
```

## <a name="optional-query-parameters"></a><span data-ttu-id="36a02-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="36a02-121">Optional query parameters</span></span>
<span data-ttu-id="36a02-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="36a02-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="36a02-123">既定では、限定的なプロパティのセットのみが返されます (_businessPhones、displayName、givenName、id、jobTitle、mail、mobilePhone、officeLocation、preferredLanguage、surname、userPrincipalName_)。</span><span class="sxs-lookup"><span data-stu-id="36a02-123">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> 

<span data-ttu-id="36a02-124">別のプロパティ セットを返すには、OData `$select` クエリ パラメーターを使用して、目的の [user](../resources/user.md) プロパティのセットを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="36a02-124">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="36a02-125">たとえば、_displayName_、_givenName_、_postalCode_ を返すには、クエリに `$select=displayName,givenName,postalCode` を追加します。</span><span class="sxs-lookup"><span data-stu-id="36a02-125">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

## <a name="request-headers"></a><span data-ttu-id="36a02-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="36a02-126">Request headers</span></span>
| <span data-ttu-id="36a02-127">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="36a02-127">Header</span></span>       | <span data-ttu-id="36a02-128">値</span><span class="sxs-lookup"><span data-stu-id="36a02-128">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="36a02-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="36a02-129">Authorization</span></span>  | <span data-ttu-id="36a02-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="36a02-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="36a02-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="36a02-132">Content-Type</span></span>   | <span data-ttu-id="36a02-133">application/json</span><span class="sxs-lookup"><span data-stu-id="36a02-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="36a02-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="36a02-134">Request body</span></span>
<span data-ttu-id="36a02-135">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="36a02-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36a02-136">応答</span><span class="sxs-lookup"><span data-stu-id="36a02-136">Response</span></span>

<span data-ttu-id="36a02-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [user](../resources/user.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="36a02-137">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

<span data-ttu-id="36a02-138">このメソッドは、要求が正常に処理されたが、サーバーが関連するバックグラウンド処理を完了するのにさらに時間を必要とする場合に `202 Accepted` を返します。</span><span class="sxs-lookup"><span data-stu-id="36a02-138">This method returns `202 Accepted` when the request has been processed successfully but the server requires more time to complete related background operations.</span></span>

## <a name="examples"></a><span data-ttu-id="36a02-139">例</span><span class="sxs-lookup"><span data-stu-id="36a02-139">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="36a02-140">例 1:標準的なユーザーの要求</span><span class="sxs-lookup"><span data-stu-id="36a02-140">Example 1: Standard users request</span></span>

<span data-ttu-id="36a02-141">既定では、限定的なプロパティのセットのみが返されます (_businessPhones、displayName、givenName、id、jobTitle、mail、mobilePhone、officeLocation、preferredLanguage、surname、userPrincipalName_)。</span><span class="sxs-lookup"><span data-stu-id="36a02-141">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> <span data-ttu-id="36a02-142">この例では、既定の要求と応答を示します。</span><span class="sxs-lookup"><span data-stu-id="36a02-142">This example illustrates the default request and response.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}
```

##### <a name="response"></a><span data-ttu-id="36a02-143">応答</span><span class="sxs-lookup"><span data-stu-id="36a02-143">Response</span></span>

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


### <a name="example-2-signed-in-user-request"></a><span data-ttu-id="36a02-144">例 2: サインインしているユーザーの要求</span><span class="sxs-lookup"><span data-stu-id="36a02-144">Example 2: Signed-in user request</span></span>

<span data-ttu-id="36a02-145">`/users/{id | userPrincipalName}` を `/me` に置き換えると、サインイン ユーザーのユーザー情報を取得できます。</span><span class="sxs-lookup"><span data-stu-id="36a02-145">You can get the user information for the signed-in user by replacing `/users/{id | userPrincipalName}` with `/me`.</span></span>

##### <a name="request"></a><span data-ttu-id="36a02-146">要求</span><span class="sxs-lookup"><span data-stu-id="36a02-146">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="36a02-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="36a02-147">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/v1.0/me
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="36a02-148">C#</span><span class="sxs-lookup"><span data-stu-id="36a02-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="36a02-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="36a02-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="36a02-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36a02-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="36a02-151">応答</span><span class="sxs-lookup"><span data-stu-id="36a02-151">Response</span></span>

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

### <a name="example-3-users-request-using-select"></a><span data-ttu-id="36a02-152">例 3: $select を使用したユーザーの要求</span><span class="sxs-lookup"><span data-stu-id="36a02-152">Example 3: Users request using $select</span></span>

<span data-ttu-id="36a02-153">別のプロパティ セットを必要とする場合、OData `$select` クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="36a02-153">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="36a02-154">たとえば、_displayName_、_givenName_、_postalCode_ を返すには、クエリに `$select=displayName,givenName,postalCode` を追加します。</span><span class="sxs-lookup"><span data-stu-id="36a02-154">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

##### <a name="request"></a><span data-ttu-id="36a02-155">要求</span><span class="sxs-lookup"><span data-stu-id="36a02-155">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}?$select=displayName,givenName,postalCode
```
##### <a name="response"></a><span data-ttu-id="36a02-156">応答</span><span class="sxs-lookup"><span data-stu-id="36a02-156">Response</span></span>
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
