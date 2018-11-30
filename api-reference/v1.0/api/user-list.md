---
title: ユーザーを一覧表示する
description: ユーザー オブジェクトのリストを取得します。
ms.openlocfilehash: 3ab6d2a663233bcb26b31abee33b430039ac8d25
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021366"
---
# <a name="list-users"></a><span data-ttu-id="fd219-103">ユーザーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="fd219-103">List users</span></span>

<span data-ttu-id="fd219-104">ユーザー オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="fd219-104">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd219-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fd219-105">Permissions</span></span>

<span data-ttu-id="fd219-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fd219-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd219-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fd219-108">Permission type</span></span>      | <span data-ttu-id="fd219-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fd219-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd219-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fd219-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fd219-111">User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fd219-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fd219-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fd219-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd219-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fd219-113">Not supported.</span></span>    |
|<span data-ttu-id="fd219-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fd219-114">Application</span></span> | <span data-ttu-id="fd219-115">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd219-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd219-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fd219-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fd219-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="fd219-117">Optional query parameters</span></span>

<span data-ttu-id="fd219-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="fd219-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="fd219-119">既定では、限定的なプロパティのセットのみが返されます (_businessPhones、displayName、givenName、id、jobTitle、mail、mobilePhone、officeLocation、preferredLanguage、surname、userPrincipalName_)。</span><span class="sxs-lookup"><span data-stu-id="fd219-119">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> 

<span data-ttu-id="fd219-120">別のプロパティ セットを返すには、OData `$select` クエリ パラメーターを使用して、目的の [user](../resources/user.md) プロパティのセットを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="fd219-120">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="fd219-121">たとえば、_displayName_、_givenName_、_postalCode_ を返すには、クエリに `$select=displayName,givenName,postalCode` を追加します。</span><span class="sxs-lookup"><span data-stu-id="fd219-121">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

> <span data-ttu-id="fd219-p103">注意: 特定のプロパティは、ユーザー コレクションでは返すことができません。[単一のユーザーを取得する](./user-get.md)場合にのみ、_aboutMe、birthday、hireDate、interests、mySite、pastProjects, preferredName、responsibilities、schools、skills、mailboxSettings_ の各プロパティがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="fd219-p103">Note: Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving an single user](./user-get.md): _aboutMe, birthday, hireDate, interests, mySite, pastProjects, preferredName, responsibilities, schools, skills, mailboxSettings_</span></span>

## <a name="request-headers"></a><span data-ttu-id="fd219-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fd219-124">Request headers</span></span>

| <span data-ttu-id="fd219-125">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fd219-125">Header</span></span>        | <span data-ttu-id="fd219-126">値</span><span class="sxs-lookup"><span data-stu-id="fd219-126">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="fd219-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd219-127">Authorization</span></span> | <span data-ttu-id="fd219-128">Bearer {トークン} (必須)</span><span class="sxs-lookup"><span data-stu-id="fd219-128">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="fd219-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fd219-129">Content-Type</span></span>  | <span data-ttu-id="fd219-130">application/json</span><span class="sxs-lookup"><span data-stu-id="fd219-130">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="fd219-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="fd219-131">Request body</span></span>

<span data-ttu-id="fd219-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fd219-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd219-133">応答</span><span class="sxs-lookup"><span data-stu-id="fd219-133">Response</span></span>

<span data-ttu-id="fd219-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [user](../resources/user.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="fd219-134">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fd219-135">例</span><span class="sxs-lookup"><span data-stu-id="fd219-135">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="fd219-136">例 1:標準的なユーザーの要求</span><span class="sxs-lookup"><span data-stu-id="fd219-136">Example 1: Standard users request</span></span>

<span data-ttu-id="fd219-137">既定では、限定的なプロパティのセットのみが返されます (_businessPhones、displayName、givenName、id、jobTitle、mail、mobilePhone、officeLocation、preferredLanguage、surname、userPrincipalName_)。</span><span class="sxs-lookup"><span data-stu-id="fd219-137">By default, only a limited set of properties are returned (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span></span> <span data-ttu-id="fd219-138">この例では、既定の要求と応答を示します。</span><span class="sxs-lookup"><span data-stu-id="fd219-138">This example illustrates the default request and response.</span></span> 

##### <a name="request"></a><span data-ttu-id="fd219-139">要求</span><span class="sxs-lookup"><span data-stu-id="fd219-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/users
```

##### <a name="response"></a><span data-ttu-id="fd219-140">応答</span><span class="sxs-lookup"><span data-stu-id="fd219-140">Response</span></span>

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

### <a name="example-2-users-request-using-select"></a><span data-ttu-id="fd219-141">例 2:$select を使用したユーザーの要求</span><span class="sxs-lookup"><span data-stu-id="fd219-141">Example 2: Users request using $select</span></span>

<span data-ttu-id="fd219-142">別のプロパティ セットを必要とする場合、OData `$select` クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="fd219-142">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="fd219-143">たとえば、_displayName_、_givenName_、_postalCode_ を返すには、クエリに `$select=displayName,givenName,postalCode` を追加します。</span><span class="sxs-lookup"><span data-stu-id="fd219-143">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

##### <a name="request"></a><span data-ttu-id="fd219-144">要求</span><span class="sxs-lookup"><span data-stu-id="fd219-144">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/users?$select=displayName,givenName,postalCode
```

##### <a name="response"></a><span data-ttu-id="fd219-145">応答</span><span class="sxs-lookup"><span data-stu-id="fd219-145">Response</span></span>

<span data-ttu-id="fd219-146">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="fd219-146">Note: The response object shown here may be truncated for brevity.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 159

{
  "value": [
    {
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "postalCode": "postalCode-value"
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
