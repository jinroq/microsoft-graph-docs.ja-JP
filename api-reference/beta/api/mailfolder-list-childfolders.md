---
title: childFolders を一覧表示する
description: '指定したフォルダーの下のフォルダー コレクションを取得します。 `.../me/MailFolders`ショートカットを使用して、最上位レベルを取得することができます。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 783a2f4d11c814cc0d0c6f903476a3fa2043cce1
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33598601"
---
# <a name="list-childfolders"></a><span data-ttu-id="67bfc-104">childFolders を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="67bfc-104">List childFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67bfc-p102">指定したフォルダーの下のフォルダーのコレクションを取得します。`.../me/MailFolders` ショートカットを使用して、最上位フォルダーのコレクションを取得して、別のフォルダーに移動することができます。</span><span class="sxs-lookup"><span data-stu-id="67bfc-p102">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="67bfc-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="67bfc-107">Permissions</span></span>

<span data-ttu-id="67bfc-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="67bfc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="67bfc-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="67bfc-110">Permission type</span></span>                        | <span data-ttu-id="67bfc-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="67bfc-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="67bfc-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="67bfc-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="67bfc-113">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67bfc-113">Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="67bfc-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="67bfc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67bfc-115">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67bfc-115">Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="67bfc-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="67bfc-116">Application</span></span>                            | <span data-ttu-id="67bfc-117">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67bfc-117">Mail.Read, Mail.ReadWrite</span></span>           |

## <a name="http-request"></a><span data-ttu-id="67bfc-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="67bfc-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="67bfc-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="67bfc-119">Optional query parameters</span></span>

<span data-ttu-id="67bfc-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="67bfc-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="67bfc-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="67bfc-121">Request headers</span></span>

| <span data-ttu-id="67bfc-122">名前</span><span class="sxs-lookup"><span data-stu-id="67bfc-122">Name</span></span>          | <span data-ttu-id="67bfc-123">型</span><span class="sxs-lookup"><span data-stu-id="67bfc-123">Type</span></span>   | <span data-ttu-id="67bfc-124">説明</span><span class="sxs-lookup"><span data-stu-id="67bfc-124">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="67bfc-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="67bfc-125">Authorization</span></span> | <span data-ttu-id="67bfc-126">string</span><span class="sxs-lookup"><span data-stu-id="67bfc-126">string</span></span> | <span data-ttu-id="67bfc-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="67bfc-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="67bfc-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="67bfc-129">Request body</span></span>

<span data-ttu-id="67bfc-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="67bfc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67bfc-131">応答</span><span class="sxs-lookup"><span data-stu-id="67bfc-131">Response</span></span>

<span data-ttu-id="67bfc-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [MailFolder](../resources/mailfolder.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="67bfc-132">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="67bfc-133">例</span><span class="sxs-lookup"><span data-stu-id="67bfc-133">Examples</span></span>

### <a name="example-1-list-mail-folders"></a><span data-ttu-id="67bfc-134">例 1: メールフォルダーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="67bfc-134">Example 1: List mail folders</span></span>

#### <a name="request"></a><span data-ttu-id="67bfc-135">要求</span><span class="sxs-lookup"><span data-stu-id="67bfc-135">Request</span></span>

<span data-ttu-id="67bfc-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="67bfc-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/childFolders
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="67bfc-137">応答</span><span class="sxs-lookup"><span data-stu-id="67bfc-137">Response</span></span>

<span data-ttu-id="67bfc-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="67bfc-138">The following is an example of the response.</span></span>

> <span data-ttu-id="67bfc-139">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="67bfc-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="67bfc-140">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="67bfc-140">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="67bfc-141">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="67bfc-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="67bfc-142">Visual</span><span class="sxs-lookup"><span data-stu-id="67bfc-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_childfolders-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="67bfc-143">Java</span><span class="sxs-lookup"><span data-stu-id="67bfc-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_childfolders-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-list-mail-search-folders"></a><span data-ttu-id="67bfc-144">例 2: メール検索フォルダーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="67bfc-144">Example 2: List mail search folders</span></span>

#### <a name="request"></a><span data-ttu-id="67bfc-145">要求</span><span class="sxs-lookup"><span data-stu-id="67bfc-145">Request</span></span>

<span data-ttu-id="67bfc-146">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="67bfc-146">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_childfolders_of_searchfolders"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childFolders
```

#### <a name="response"></a><span data-ttu-id="67bfc-147">応答</span><span class="sxs-lookup"><span data-stu-id="67bfc-147">Response</span></span>

<span data-ttu-id="67bfc-148">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="67bfc-148">The following is an example of the response.</span></span>

> <span data-ttu-id="67bfc-149">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="67bfc-149">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="67bfc-150">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="67bfc-150">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="67bfc-151">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="67bfc-151">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="67bfc-152">Visual</span><span class="sxs-lookup"><span data-stu-id="67bfc-152">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_childfolders_of_searchfolders-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="67bfc-153">Java</span><span class="sxs-lookup"><span data-stu-id="67bfc-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_childfolders_of_searchfolders-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/mailfolder-list-childfolders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/mailfolder-list-childfolders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/mailfolder-list-childfolders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/mailfolder-list-childfolders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
