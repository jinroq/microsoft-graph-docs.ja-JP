---
title: childFolders を一覧表示する
description: '指定したフォルダーの下のフォルダー コレクションを取得します。 `.../me/MailFolders`ショートカットを使用して、最上位レベルを取得することができます。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 50b5a36d2529e295a4876e851cf89459cc386a77
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35445297"
---
# <a name="list-childfolders"></a><span data-ttu-id="cb3c7-104">childFolders を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="cb3c7-104">List childFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb3c7-p102">指定したフォルダーの下のフォルダーのコレクションを取得します。`.../me/mailFolders` ショートカットを使用して、最上位フォルダーのコレクションを取得して、別のフォルダーに移動することができます。</span><span class="sxs-lookup"><span data-stu-id="cb3c7-p102">Get the folder collection under the specified folder. You can use the `.../me/mailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb3c7-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cb3c7-107">Permissions</span></span>

<span data-ttu-id="cb3c7-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cb3c7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cb3c7-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cb3c7-110">Permission type</span></span>                        | <span data-ttu-id="cb3c7-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cb3c7-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="cb3c7-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cb3c7-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="cb3c7-113">メール ReadBasic、Mail. 読み取り、ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cb3c7-113">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="cb3c7-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cb3c7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb3c7-115">メール ReadBasic、Mail. 読み取り、ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cb3c7-115">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="cb3c7-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cb3c7-116">Application</span></span>                            | <span data-ttu-id="cb3c7-117">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cb3c7-117">Mail.Read, Mail.ReadWrite</span></span>           |

## <a name="http-request"></a><span data-ttu-id="cb3c7-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cb3c7-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cb3c7-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="cb3c7-119">Optional query parameters</span></span>

<span data-ttu-id="cb3c7-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="cb3c7-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cb3c7-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cb3c7-121">Request headers</span></span>

| <span data-ttu-id="cb3c7-122">名前</span><span class="sxs-lookup"><span data-stu-id="cb3c7-122">Name</span></span>          | <span data-ttu-id="cb3c7-123">型</span><span class="sxs-lookup"><span data-stu-id="cb3c7-123">Type</span></span>   | <span data-ttu-id="cb3c7-124">説明</span><span class="sxs-lookup"><span data-stu-id="cb3c7-124">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="cb3c7-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb3c7-125">Authorization</span></span> | <span data-ttu-id="cb3c7-126">string</span><span class="sxs-lookup"><span data-stu-id="cb3c7-126">string</span></span> | <span data-ttu-id="cb3c7-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cb3c7-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb3c7-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="cb3c7-129">Request body</span></span>

<span data-ttu-id="cb3c7-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="cb3c7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb3c7-131">応答</span><span class="sxs-lookup"><span data-stu-id="cb3c7-131">Response</span></span>

<span data-ttu-id="cb3c7-132">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[mailfolder](../resources/mailfolder.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="cb3c7-132">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cb3c7-133">例</span><span class="sxs-lookup"><span data-stu-id="cb3c7-133">Examples</span></span>

### <a name="example-1-list-mail-folders"></a><span data-ttu-id="cb3c7-134">例 1: メールフォルダーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="cb3c7-134">Example 1: List mail folders</span></span>

#### <a name="request"></a><span data-ttu-id="cb3c7-135">要求</span><span class="sxs-lookup"><span data-stu-id="cb3c7-135">Request</span></span>

<span data-ttu-id="cb3c7-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cb3c7-136">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="cb3c7-137">プロトコル</span><span class="sxs-lookup"><span data-stu-id="cb3c7-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/childFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cb3c7-138">C#</span><span class="sxs-lookup"><span data-stu-id="cb3c7-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-childfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cb3c7-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="cb3c7-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-childfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cb3c7-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="cb3c7-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-childfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="cb3c7-141">応答</span><span class="sxs-lookup"><span data-stu-id="cb3c7-141">Response</span></span>

<span data-ttu-id="cb3c7-142">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cb3c7-142">The following is an example of the response.</span></span>

> <span data-ttu-id="cb3c7-143">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="cb3c7-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cb3c7-144">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="cb3c7-144">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "AAMkAGVmMDEzA",
      "displayName": "Internal Screens",
      "parentFolderId": "AAMkAGVmMDEzM",
      "childFolderCount": 0,
      "unreadItemCount": 2,
      "totalItemCount": 2,
      "wellKnownName": null
    },
    {
      "id": "AAMkAGVmMDEzB",
      "displayName": "Project Falcon",
      "parentFolderId": "AAMkAGVmMDEzM",
      "childFolderCount": 0,
      "unreadItemCount": 5,
      "totalItemCount": 5,
      "wellKnownName": null
    },
    {
      "id": "AAMkAGVmMDEzMA",
      "displayName": "Finder",
      "parentFolderId": "AAMkAGVmMDEzM",
      "childFolderCount": 4,
      "unreadItemCount": 0,
      "totalItemCount": 0,
      "wellKnownName": "searchfolders"
    }
  ]
}
```

### <a name="example-2-list-mail-search-folders"></a><span data-ttu-id="cb3c7-145">例 2: メール検索フォルダーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="cb3c7-145">Example 2: List mail search folders</span></span>

#### <a name="request"></a><span data-ttu-id="cb3c7-146">要求</span><span class="sxs-lookup"><span data-stu-id="cb3c7-146">Request</span></span>

<span data-ttu-id="cb3c7-147">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cb3c7-147">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="cb3c7-148">プロトコル</span><span class="sxs-lookup"><span data-stu-id="cb3c7-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_childfolders_of_searchfolders"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cb3c7-149">C#</span><span class="sxs-lookup"><span data-stu-id="cb3c7-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-childfolders-of-searchfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cb3c7-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="cb3c7-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-childfolders-of-searchfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cb3c7-151">目的-C</span><span class="sxs-lookup"><span data-stu-id="cb3c7-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-childfolders-of-searchfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cb3c7-152">応答</span><span class="sxs-lookup"><span data-stu-id="cb3c7-152">Response</span></span>

<span data-ttu-id="cb3c7-153">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cb3c7-153">The following is an example of the response.</span></span>

> <span data-ttu-id="cb3c7-154">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="cb3c7-154">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cb3c7-155">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="cb3c7-155">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mailSearchFolder",
      "id": "AAMkAGE1NWMz",
      "displayName": "Get MyAnalytics",
      "parentFolderId": "AAMkAGE1NWMx",
      "childFolderCount": 0,
      "unreadItemCount": 6,
      "totalItemCount": 6,
      "wellKnownName": null,
      "isSupported": true,
      "filterQuery": "contains(subject, 'MyAnalytics')"
    },
    {
      "@odata.type": "#microsoft.graph.mailSearchFolder",
      "id": "AAMkAGE1NWMy",
      "displayName": "Action Required",
      "parentFolderId": "AAMkAGE1NWMx",
      "childFolderCount": 0,
      "unreadItemCount": 2,
      "totalItemCount": 4,
      "wellKnownName": null,
      "isSupported": true,
      "filterQuery": "contains(subject, 'ACTION REQUIRED')"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
