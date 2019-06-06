---
title: ユーザーを一覧表示する
description: ユーザー オブジェクトの一覧を取得します。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fb519c1fa613b420581576099687096ec6aaa6f0
ms.sourcegitcommit: 624ac42e74533a9bf0d0d22b3b15adbb258fd594
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/05/2019
ms.locfileid: "34709440"
---
# <a name="list-users"></a><span data-ttu-id="53be4-103">ユーザーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="53be4-103">List users</span></span>

<span data-ttu-id="53be4-104">ユーザー オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="53be4-104">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="53be4-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="53be4-105">Permissions</span></span>

<span data-ttu-id="53be4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="53be4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53be4-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="53be4-108">Permission type</span></span>      | <span data-ttu-id="53be4-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="53be4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53be4-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="53be4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="53be4-111">User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="53be4-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="53be4-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="53be4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53be4-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="53be4-113">Not supported.</span></span>    |
|<span data-ttu-id="53be4-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="53be4-114">Application</span></span> | <span data-ttu-id="53be4-115">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53be4-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="53be4-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="53be4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="53be4-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="53be4-117">Optional query parameters</span></span>

<span data-ttu-id="53be4-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="53be4-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="53be4-119">既定では、限定的なプロパティのセットのみが返されます (**businessPhones**、**displayName**、**givenName**、**id**、**jobTitle**、**mail**、**mobilePhone**、**officeLocation**、**preferredLanguage**、**surname**、および **userPrincipalName**)。</span><span class="sxs-lookup"><span data-stu-id="53be4-119">By default, only a limited set of properties are returned (**businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName**).</span></span> 

<span data-ttu-id="53be4-120">別のプロパティ セットを返すには、OData `$select` クエリ パラメーターを使用して、目的の [user](../resources/user.md) プロパティのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="53be4-120">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="53be4-121">たとえば、**displayName**、**givenName**、**postalCode** を返すには、クエリ `$select=displayName,givenName,postalCode` に次を追加します。</span><span class="sxs-lookup"><span data-stu-id="53be4-121">For example, to return **displayName**, **givenName**, and **postalCode**, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

<span data-ttu-id="53be4-p103">特定のプロパティは、ユーザー コレクションでは返すことができません。[単一のユーザーを取得する](./user-get.md)場合にのみ、**aboutMe**、**birthday**、**hireDate**、**interests**、**mySite**、**pastProjects**、**preferredName**、**responsibilities**、**schools**、**skills**、**mailboxSettings** の各プロパティがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="53be4-p103">Note: Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving an single user](./user-get.md): **aboutMe, birthday, hireDate, interests, mySite, pastProjects, preferredName, responsibilities, schools, skills, mailboxSettings**</span></span>

## <a name="request-headers"></a><span data-ttu-id="53be4-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="53be4-124">Request headers</span></span>

| <span data-ttu-id="53be4-125">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="53be4-125">Header</span></span>        | <span data-ttu-id="53be4-126">値</span><span class="sxs-lookup"><span data-stu-id="53be4-126">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="53be4-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="53be4-127">Authorization</span></span> | <span data-ttu-id="53be4-128">Bearer {トークン} (必須)</span><span class="sxs-lookup"><span data-stu-id="53be4-128">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="53be4-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="53be4-129">Content-Type</span></span>  | <span data-ttu-id="53be4-130">application/json</span><span class="sxs-lookup"><span data-stu-id="53be4-130">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="53be4-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="53be4-131">Request body</span></span>

<span data-ttu-id="53be4-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="53be4-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53be4-133">応答</span><span class="sxs-lookup"><span data-stu-id="53be4-133">Response</span></span>

<span data-ttu-id="53be4-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [user](../resources/user.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="53be4-134">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span> <span data-ttu-id="53be4-135">大きいユーザー コレクションが返された場合は、[アプリでページング](/graph/paging)を使用することができます。</span><span class="sxs-lookup"><span data-stu-id="53be4-135">If a large user collection is returned, you can use [paging in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="53be4-136">例</span><span class="sxs-lookup"><span data-stu-id="53be4-136">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="53be4-137">例 1:標準的なユーザーの要求</span><span class="sxs-lookup"><span data-stu-id="53be4-137">Example 1: Standard users request</span></span>

<span data-ttu-id="53be4-138">既定では、限定的なプロパティのセットのみが返されます (**businessPhones**、**displayName**、**givenName**、**id**、**jobTitle**、**mail**、**mobilePhone**、**officeLocation**、**preferredLanguage**、**surname**、**userPrincipalName**)。</span><span class="sxs-lookup"><span data-stu-id="53be4-138">By default, only a limited set of properties are returned (**businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName**).</span></span> <span data-ttu-id="53be4-139">この例では、既定の要求と応答を示します。</span><span class="sxs-lookup"><span data-stu-id="53be4-139">This example illustrates the default request and response.</span></span> 

##### <a name="request"></a><span data-ttu-id="53be4-140">要求</span><span class="sxs-lookup"><span data-stu-id="53be4-140">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/users
```

##### <a name="response"></a><span data-ttu-id="53be4-141">応答</span><span class="sxs-lookup"><span data-stu-id="53be4-141">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="53be4-142">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="53be4-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="53be4-143">C#</span><span class="sxs-lookup"><span data-stu-id="53be4-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_users-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="53be4-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="53be4-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_users-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-users-request-using-select"></a><span data-ttu-id="53be4-145">例 2:$select を使用したユーザーの要求</span><span class="sxs-lookup"><span data-stu-id="53be4-145">Example 2: Users request using $select</span></span>

<span data-ttu-id="53be4-146">別のプロパティ セットを必要とする場合、OData `$select` クエリ パラメーターを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="53be4-146">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="53be4-147">たとえば、**displayName**、**givenName**、**postalCode** を返すには、クエリに `$select=displayName,givenName,postalCode` を追加します。</span><span class="sxs-lookup"><span data-stu-id="53be4-147">For example, to return **displayName**, **givenName**, and **postalCode**, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

##### <a name="request"></a><span data-ttu-id="53be4-148">要求</span><span class="sxs-lookup"><span data-stu-id="53be4-148">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_users_properties"
}-->
```http
GET https://graph.microsoft.com/v1.0/users?$select=displayName,givenName,postalCode
```

##### <a name="response"></a><span data-ttu-id="53be4-149">応答</span><span class="sxs-lookup"><span data-stu-id="53be4-149">Response</span></span>

<span data-ttu-id="53be4-150">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="53be4-150">Note: The response object shown here may be truncated for brevity.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="53be4-151">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="53be4-151">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="53be4-152">C#</span><span class="sxs-lookup"><span data-stu-id="53be4-152">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_users_properties-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="53be4-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="53be4-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_users_properties-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/user-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
