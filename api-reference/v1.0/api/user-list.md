---
title: ユーザーを一覧表示する
description: ユーザー オブジェクトの一覧を取得します。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 235411d1b323bbacc5ffb3f86cf68242b8a41861
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36316287"
---
# <a name="list-users"></a><span data-ttu-id="abc19-103">ユーザーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="abc19-103">List users</span></span>

<span data-ttu-id="abc19-104">ユーザー オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="abc19-104">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="abc19-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="abc19-105">Permissions</span></span>

<span data-ttu-id="abc19-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="abc19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abc19-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="abc19-108">Permission type</span></span>      | <span data-ttu-id="abc19-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="abc19-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="abc19-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="abc19-110">Delegated (work or school account)</span></span> | <span data-ttu-id="abc19-111">User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="abc19-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="abc19-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="abc19-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="abc19-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="abc19-113">Not supported.</span></span>    |
|<span data-ttu-id="abc19-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="abc19-114">Application</span></span> | <span data-ttu-id="abc19-115">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abc19-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="abc19-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="abc19-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="abc19-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="abc19-117">Optional query parameters</span></span>

<span data-ttu-id="abc19-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="abc19-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="abc19-119">既定では、限定的なプロパティのセットのみが返されます (**businessPhones**、**displayName**、**givenName**、**id**、**jobTitle**、**mail**、**mobilePhone**、**officeLocation**、**preferredLanguage**、**surname**、および **userPrincipalName**)。</span><span class="sxs-lookup"><span data-stu-id="abc19-119">By default, only a limited set of properties are returned (**businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName**).</span></span> 

<span data-ttu-id="abc19-120">別のプロパティ セットを返すには、OData `$select` クエリ パラメーターを使用して、目的の [user](../resources/user.md) プロパティのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="abc19-120">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="abc19-121">たとえば、**displayName**、**givenName**、**postalCode** を返すには、クエリ `$select=displayName,givenName,postalCode` に次を追加します。</span><span class="sxs-lookup"><span data-stu-id="abc19-121">For example, to return **displayName**, **givenName**, and **postalCode**, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

<span data-ttu-id="abc19-p103">特定のプロパティは、ユーザー コレクションでは返すことができません。[単一のユーザーを取得する](./user-get.md)場合にのみ、**aboutMe**、**birthday**、**hireDate**、**interests**、**mySite**、**pastProjects**、**preferredName**、**responsibilities**、**schools**、**skills**、**mailboxSettings** の各プロパティがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="abc19-p103">Note: Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving an single user](./user-get.md): **aboutMe, birthday, hireDate, interests, mySite, pastProjects, preferredName, responsibilities, schools, skills, mailboxSettings**</span></span>

## <a name="request-headers"></a><span data-ttu-id="abc19-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="abc19-124">Request headers</span></span>

| <span data-ttu-id="abc19-125">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="abc19-125">Header</span></span>        | <span data-ttu-id="abc19-126">値</span><span class="sxs-lookup"><span data-stu-id="abc19-126">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="abc19-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="abc19-127">Authorization</span></span> | <span data-ttu-id="abc19-128">Bearer {トークン} (必須)</span><span class="sxs-lookup"><span data-stu-id="abc19-128">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="abc19-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="abc19-129">Content-Type</span></span>  | <span data-ttu-id="abc19-130">application/json</span><span class="sxs-lookup"><span data-stu-id="abc19-130">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="abc19-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="abc19-131">Request body</span></span>

<span data-ttu-id="abc19-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="abc19-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="abc19-133">応答</span><span class="sxs-lookup"><span data-stu-id="abc19-133">Response</span></span>

<span data-ttu-id="abc19-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [user](../resources/user.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="abc19-134">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span> <span data-ttu-id="abc19-135">大きいユーザー コレクションが返された場合は、[アプリでページング](/graph/paging)を使用することができます。</span><span class="sxs-lookup"><span data-stu-id="abc19-135">If a large user collection is returned, you can use [paging in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="abc19-136">例</span><span class="sxs-lookup"><span data-stu-id="abc19-136">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="abc19-137">例 1:標準的なユーザーの要求</span><span class="sxs-lookup"><span data-stu-id="abc19-137">Example 1: Standard users request</span></span>

<span data-ttu-id="abc19-138">既定では、限定的なプロパティのセットのみが返されます (**businessPhones**、**displayName**、**givenName**、**id**、**jobTitle**、**mail**、**mobilePhone**、**officeLocation**、**preferredLanguage**、**surname**、**userPrincipalName**)。</span><span class="sxs-lookup"><span data-stu-id="abc19-138">By default, only a limited set of properties are returned (**businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName**).</span></span> <span data-ttu-id="abc19-139">この例では、既定の要求と応答を示します。</span><span class="sxs-lookup"><span data-stu-id="abc19-139">This example illustrates the default request and response.</span></span> 

##### <a name="request"></a><span data-ttu-id="abc19-140">要求</span><span class="sxs-lookup"><span data-stu-id="abc19-140">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="abc19-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="abc19-141">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/users
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="abc19-142">C#</span><span class="sxs-lookup"><span data-stu-id="abc19-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="abc19-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="abc19-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="abc19-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="abc19-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="abc19-145">Java</span><span class="sxs-lookup"><span data-stu-id="abc19-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="abc19-146">応答</span><span class="sxs-lookup"><span data-stu-id="abc19-146">Response</span></span>

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

### <a name="example-2-users-request-using-select"></a><span data-ttu-id="abc19-147">例 2:$select を使用したユーザーの要求</span><span class="sxs-lookup"><span data-stu-id="abc19-147">Example 2: Users request using $select</span></span>

<span data-ttu-id="abc19-148">別のプロパティ セットを必要とする場合、OData `$select` クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="abc19-148">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="abc19-149">たとえば、**displayName**、**givenName**、**postalCode** を返すには、クエリに `$select=displayName,givenName,postalCode` を追加します。</span><span class="sxs-lookup"><span data-stu-id="abc19-149">For example, to return **displayName**, **givenName**, and **postalCode**, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

##### <a name="request"></a><span data-ttu-id="abc19-150">要求</span><span class="sxs-lookup"><span data-stu-id="abc19-150">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="abc19-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="abc19-151">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users_properties"
}-->
```http
GET https://graph.microsoft.com/v1.0/users?$select=displayName,givenName,postalCode
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="abc19-152">C#</span><span class="sxs-lookup"><span data-stu-id="abc19-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-properties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="abc19-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="abc19-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-properties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="abc19-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="abc19-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-properties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="abc19-155">Java</span><span class="sxs-lookup"><span data-stu-id="abc19-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-properties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="abc19-156">応答</span><span class="sxs-lookup"><span data-stu-id="abc19-156">Response</span></span>

<span data-ttu-id="abc19-157">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="abc19-157">Note: The response object shown here may be truncated for brevity.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
