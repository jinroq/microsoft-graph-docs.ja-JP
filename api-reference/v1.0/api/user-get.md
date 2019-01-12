---
title: ユーザーの取得
description: ユーザー オブジェクトのプロパティと関係を取得します。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bc408abf60ad42f564c4c36a37151db122ad573d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984151"
---
# <a name="get-a-user"></a><span data-ttu-id="6e781-103">ユーザーの取得</span><span class="sxs-lookup"><span data-stu-id="6e781-103">Get a user</span></span>

<span data-ttu-id="6e781-104">ユーザー オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="6e781-104">Retrieve the properties and relationships of user object.</span></span>

> <span data-ttu-id="6e781-p101">注:ユーザーを取得すると、プロパティの既定セットのみが返されます (*businessPhones、displayName、givenName、id、jobTitle、mail、mobilePhone、officeLocation、preferredLanguage、surname、userPrincipalName*)。`$select` を使用して、[ユーザー](../resources/user.md) オブジェクトの他のプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="6e781-p101">Note: Getting a user returns a default set of properties only (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). Use `$select` to get the other properties and relationships for the [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e781-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6e781-107">Permissions</span></span>
<span data-ttu-id="6e781-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6e781-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e781-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6e781-110">Permission type</span></span>      | <span data-ttu-id="6e781-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6e781-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e781-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6e781-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6e781-113">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6e781-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6e781-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6e781-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e781-115">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e781-115">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="6e781-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6e781-116">Application</span></span> | <span data-ttu-id="6e781-117">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e781-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e781-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6e781-118">HTTP request</span></span>
<span data-ttu-id="6e781-119">: 特定のユーザーの<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="6e781-119">For a specific user: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /users/{id | userPrincipalName}
```

<span data-ttu-id="6e781-120">サインインしているユーザー。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="6e781-120">For the signed-in user: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6e781-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6e781-121">Optional query parameters</span></span>
<span data-ttu-id="6e781-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6e781-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="6e781-123">既定では、限定的なプロパティのセットのみが返されます (_businessPhones、displayName、givenName、id、jobTitle、mail、mobilePhone、officeLocation、preferredLanguage、surname、userPrincipalName_)。</span><span class="sxs-lookup"><span data-stu-id="6e781-123">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> 

<span data-ttu-id="6e781-124">別のプロパティ セットを返すには、OData `$select` クエリ パラメーターを使用して、目的の [user](../resources/user.md) プロパティのセットを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6e781-124">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="6e781-125">たとえば、_displayName_、_givenName_、_postalCode_ を返すには、クエリに `$select=displayName,givenName,postalCode` を追加します。</span><span class="sxs-lookup"><span data-stu-id="6e781-125">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

## <a name="request-headers"></a><span data-ttu-id="6e781-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6e781-126">Request headers</span></span>
| <span data-ttu-id="6e781-127">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6e781-127">Header</span></span>       | <span data-ttu-id="6e781-128">値</span><span class="sxs-lookup"><span data-stu-id="6e781-128">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="6e781-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e781-129">Authorization</span></span>  | <span data-ttu-id="6e781-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6e781-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6e781-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6e781-132">Content-Type</span></span>   | <span data-ttu-id="6e781-133">application/json</span><span class="sxs-lookup"><span data-stu-id="6e781-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e781-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="6e781-134">Request body</span></span>
<span data-ttu-id="6e781-135">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6e781-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e781-136">応答</span><span class="sxs-lookup"><span data-stu-id="6e781-136">Response</span></span>

<span data-ttu-id="6e781-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [user](../resources/user.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6e781-137">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6e781-138">例</span><span class="sxs-lookup"><span data-stu-id="6e781-138">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="6e781-139">例 1:標準的なユーザーの要求</span><span class="sxs-lookup"><span data-stu-id="6e781-139">Example 1: Standard users request</span></span>

<span data-ttu-id="6e781-140">既定では、限定的なプロパティのセットのみが返されます (_businessPhones、displayName、givenName、id、jobTitle、mail、mobilePhone、officeLocation、preferredLanguage、surname、userPrincipalName_)。</span><span class="sxs-lookup"><span data-stu-id="6e781-140">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> <span data-ttu-id="6e781-141">この例では、既定の要求と応答を示します。</span><span class="sxs-lookup"><span data-stu-id="6e781-141">This example illustrates the default request and response.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}
```

##### <a name="response"></a><span data-ttu-id="6e781-142">応答</span><span class="sxs-lookup"><span data-stu-id="6e781-142">Response</span></span>

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


### <a name="example-2-signed-in-user-request"></a><span data-ttu-id="6e781-143">例 2: サインインしているユーザーの要求</span><span class="sxs-lookup"><span data-stu-id="6e781-143">Example 2: Signed-in user request</span></span>

<span data-ttu-id="6e781-144">`/users/{id | userPrincipalName}` を `/me` に置き換えると、サインイン ユーザーのユーザー情報を取得できます。</span><span class="sxs-lookup"><span data-stu-id="6e781-144">You can get the user information for the signed-in user by replacing `/users/{id | userPrincipalName}` with `/me`.</span></span>

##### <a name="request"></a><span data-ttu-id="6e781-145">要求</span><span class="sxs-lookup"><span data-stu-id="6e781-145">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/v1.0/me
```
##### <a name="response"></a><span data-ttu-id="6e781-146">応答</span><span class="sxs-lookup"><span data-stu-id="6e781-146">Response</span></span>

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

### <a name="example-3-users-request-using-select"></a><span data-ttu-id="6e781-147">例 3: $select を使用したユーザーの要求</span><span class="sxs-lookup"><span data-stu-id="6e781-147">Example 3: Users request using $select</span></span>

<span data-ttu-id="6e781-148">別のプロパティ セットを必要とする場合、OData `$select` クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="6e781-148">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="6e781-149">たとえば、_displayName_、_givenName_、_postalCode_ を返すには、クエリに `$select=displayName,givenName,postalCode` を追加します。</span><span class="sxs-lookup"><span data-stu-id="6e781-149">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

##### <a name="request"></a><span data-ttu-id="6e781-150">要求</span><span class="sxs-lookup"><span data-stu-id="6e781-150">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}?$select=displayName,givenName,postalCode
```
##### <a name="response"></a><span data-ttu-id="6e781-151">応答</span><span class="sxs-lookup"><span data-stu-id="6e781-151">Response</span></span>
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
  "tocPath": ""
}-->
