---
title: childFolders を一覧表示する
description: '指定したフォルダーの下のフォルダー コレクションを取得します。 `.../me/MailFolders`ショートカットを使用して、最上位レベルを取得することができます。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 275f7bcd771db43f5d091848d9be8c50c6ddb124
ms.sourcegitcommit: ee710ff556f4a7907181df5c323e345f52808ce2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35417732"
---
# <a name="list-childfolders"></a><span data-ttu-id="72fe5-104">childFolders を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="72fe5-104">List childFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72fe5-p102">指定したフォルダーの下のフォルダーのコレクションを取得します。`.../me/mailFolders` ショートカットを使用して、最上位フォルダーのコレクションを取得して、別のフォルダーに移動することができます。</span><span class="sxs-lookup"><span data-stu-id="72fe5-p102">Get the folder collection under the specified folder. You can use the `.../me/mailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="72fe5-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="72fe5-107">Permissions</span></span>

<span data-ttu-id="72fe5-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="72fe5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="72fe5-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="72fe5-110">Permission type</span></span>                        | <span data-ttu-id="72fe5-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="72fe5-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="72fe5-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="72fe5-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="72fe5-113">メール ReadBasic、Mail. 読み取り、ReadWrite</span><span class="sxs-lookup"><span data-stu-id="72fe5-113">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="72fe5-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="72fe5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72fe5-115">メール ReadBasic、Mail. 読み取り、ReadWrite</span><span class="sxs-lookup"><span data-stu-id="72fe5-115">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="72fe5-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="72fe5-116">Application</span></span>                            | <span data-ttu-id="72fe5-117">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="72fe5-117">Mail.Read, Mail.ReadWrite</span></span>           |

## <a name="http-request"></a><span data-ttu-id="72fe5-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="72fe5-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="72fe5-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="72fe5-119">Optional query parameters</span></span>

<span data-ttu-id="72fe5-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="72fe5-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="72fe5-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="72fe5-121">Request headers</span></span>

| <span data-ttu-id="72fe5-122">名前</span><span class="sxs-lookup"><span data-stu-id="72fe5-122">Name</span></span>          | <span data-ttu-id="72fe5-123">型</span><span class="sxs-lookup"><span data-stu-id="72fe5-123">Type</span></span>   | <span data-ttu-id="72fe5-124">説明</span><span class="sxs-lookup"><span data-stu-id="72fe5-124">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="72fe5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="72fe5-125">Authorization</span></span> | <span data-ttu-id="72fe5-126">string</span><span class="sxs-lookup"><span data-stu-id="72fe5-126">string</span></span> | <span data-ttu-id="72fe5-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="72fe5-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="72fe5-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="72fe5-129">Request body</span></span>

<span data-ttu-id="72fe5-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="72fe5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72fe5-131">応答</span><span class="sxs-lookup"><span data-stu-id="72fe5-131">Response</span></span>

<span data-ttu-id="72fe5-132">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[mailfolder](../resources/mailfolder.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="72fe5-132">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="72fe5-133">例</span><span class="sxs-lookup"><span data-stu-id="72fe5-133">Examples</span></span>

### <a name="example-1-list-mail-folders"></a><span data-ttu-id="72fe5-134">例 1: メールフォルダーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="72fe5-134">Example 1: List mail folders</span></span>

#### <a name="request"></a><span data-ttu-id="72fe5-135">要求</span><span class="sxs-lookup"><span data-stu-id="72fe5-135">Request</span></span>

<span data-ttu-id="72fe5-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="72fe5-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/childFolders
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="72fe5-137">応答</span><span class="sxs-lookup"><span data-stu-id="72fe5-137">Response</span></span>

<span data-ttu-id="72fe5-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="72fe5-138">The following is an example of the response.</span></span>

> <span data-ttu-id="72fe5-139">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="72fe5-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="72fe5-140">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="72fe5-140">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="72fe5-141">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="72fe5-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="72fe5-142">C#</span><span class="sxs-lookup"><span data-stu-id="72fe5-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_childfolders-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="72fe5-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="72fe5-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_childfolders-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="72fe5-144">目的-C</span><span class="sxs-lookup"><span data-stu-id="72fe5-144">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_childfolders-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-list-mail-search-folders"></a><span data-ttu-id="72fe5-145">例 2: メール検索フォルダーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="72fe5-145">Example 2: List mail search folders</span></span>

#### <a name="request"></a><span data-ttu-id="72fe5-146">要求</span><span class="sxs-lookup"><span data-stu-id="72fe5-146">Request</span></span>

<span data-ttu-id="72fe5-147">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="72fe5-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_childfolders_of_searchfolders"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childFolders
```

#### <a name="response"></a><span data-ttu-id="72fe5-148">応答</span><span class="sxs-lookup"><span data-stu-id="72fe5-148">Response</span></span>

<span data-ttu-id="72fe5-149">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="72fe5-149">The following is an example of the response.</span></span>

> <span data-ttu-id="72fe5-150">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="72fe5-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="72fe5-151">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="72fe5-151">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="72fe5-152">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="72fe5-152">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="72fe5-153">C#</span><span class="sxs-lookup"><span data-stu-id="72fe5-153">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_childfolders_of_searchfolders-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="72fe5-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="72fe5-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_childfolders_of_searchfolders-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="72fe5-155">目的-C</span><span class="sxs-lookup"><span data-stu-id="72fe5-155">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_childfolders_of_searchfolders-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/mailfolder-list-childfolders.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/mailfolder-list-childfolders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/mailfolder-list-childfolders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/mailfolder-list-childfolders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/mailfolder-list-childfolders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
