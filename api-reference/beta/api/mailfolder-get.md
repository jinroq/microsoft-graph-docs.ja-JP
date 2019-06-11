---
title: mailFolder を取得する
description: メッセージ フォルダー オブジェクトのプロパティとリレーションシップを取得します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 310456f05e0a853a9a0ec78d83f4fdbdca51e236
ms.sourcegitcommit: b742da101a3a232356bf748c42da3ba08a7539d3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/10/2019
ms.locfileid: "34812860"
---
# <a name="get-mailfolder"></a><span data-ttu-id="8c10e-103">mailFolder を取得する</span><span class="sxs-lookup"><span data-stu-id="8c10e-103">Get mailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c10e-104">メッセージ フォルダー オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="8c10e-104">Retrieve the properties and relationships of a message folder object.</span></span>

<span data-ttu-id="8c10e-105">アプリで別のユーザーのメール フォルダーを取得するシナリオは 2 つあります。</span><span class="sxs-lookup"><span data-stu-id="8c10e-105">There are two scenarios where an app can get another user's mail folder:</span></span>

* <span data-ttu-id="8c10e-106">アプリにアプリケーションのアクセス許可がある場合。または</span><span class="sxs-lookup"><span data-stu-id="8c10e-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="8c10e-107">あるユーザーからアプリに適切な代理[アクセス許可](#permissions)が与えられ、別のユーザーがそのユーザーとメール フォルダーを共有しているか、そのユーザーに代理アクセスを付与している場合。</span><span class="sxs-lookup"><span data-stu-id="8c10e-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="8c10e-108">[詳細と例](/graph/outlook-share-messages-folders)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8c10e-108">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

## <a name="permissions"></a><span data-ttu-id="8c10e-109">権限</span><span class="sxs-lookup"><span data-stu-id="8c10e-109">Permissions</span></span>

<span data-ttu-id="8c10e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8c10e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c10e-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8c10e-112">Permission type</span></span>      | <span data-ttu-id="8c10e-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8c10e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c10e-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8c10e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="8c10e-115">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c10e-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8c10e-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8c10e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c10e-117">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c10e-117">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8c10e-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8c10e-118">Application</span></span> | <span data-ttu-id="8c10e-119">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c10e-119">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c10e-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8c10e-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8c10e-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8c10e-121">Optional query parameters</span></span>

<span data-ttu-id="8c10e-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8c10e-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8c10e-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8c10e-123">Request headers</span></span>

| <span data-ttu-id="8c10e-124">名前</span><span class="sxs-lookup"><span data-stu-id="8c10e-124">Name</span></span>          | <span data-ttu-id="8c10e-125">型</span><span class="sxs-lookup"><span data-stu-id="8c10e-125">Type</span></span>   | <span data-ttu-id="8c10e-126">説明</span><span class="sxs-lookup"><span data-stu-id="8c10e-126">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="8c10e-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c10e-127">Authorization</span></span> | <span data-ttu-id="8c10e-128">string</span><span class="sxs-lookup"><span data-stu-id="8c10e-128">string</span></span> | <span data-ttu-id="8c10e-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8c10e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c10e-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="8c10e-131">Request body</span></span>

<span data-ttu-id="8c10e-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8c10e-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c10e-133">応答</span><span class="sxs-lookup"><span data-stu-id="8c10e-133">Response</span></span>

<span data-ttu-id="8c10e-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [mailFolder](../resources/mailfolder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8c10e-134">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8c10e-135">例</span><span class="sxs-lookup"><span data-stu-id="8c10e-135">Examples</span></span>

### <a name="example-1-get-a-mail-folder"></a><span data-ttu-id="8c10e-136">例 1: メールフォルダーを取得する</span><span class="sxs-lookup"><span data-stu-id="8c10e-136">Example 1: Get a mail folder</span></span>

#### <a name="request"></a><span data-ttu-id="8c10e-137">要求</span><span class="sxs-lookup"><span data-stu-id="8c10e-137">Request</span></span>

<span data-ttu-id="8c10e-138">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8c10e-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEzM"],
  "name": "get_mailfolder"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="8c10e-139">応答</span><span class="sxs-lookup"><span data-stu-id="8c10e-139">Response</span></span>

<span data-ttu-id="8c10e-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8c10e-140">The following is an example of the response.</span></span>

> <span data-ttu-id="8c10e-141">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="8c10e-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8c10e-142">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8c10e-142">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "AAMkAGVmMDEzM",
  "displayName": "Inbox",
  "parentFolderId": "AAMkAGVmMDEzI",
  "childFolderCount": 2,
  "unreadItemCount": 59,
  "totalItemCount": 60,
  "wellKnownName": "inbox"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="8c10e-143">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="8c10e-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8c10e-144">C#</span><span class="sxs-lookup"><span data-stu-id="8c10e-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_mailfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8c10e-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="8c10e-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_mailfolder-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-get-a-mail-search-folder"></a><span data-ttu-id="8c10e-146">例 2: メール検索フォルダーを取得する</span><span class="sxs-lookup"><span data-stu-id="8c10e-146">Example 2: Get a mail search folder</span></span>

#### <a name="request"></a><span data-ttu-id="8c10e-147">要求</span><span class="sxs-lookup"><span data-stu-id="8c10e-147">Request</span></span>

<span data-ttu-id="8c10e-148">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8c10e-148">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEzM"],
  "name": "get_mailSearchfolder"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzN
```

#### <a name="response"></a><span data-ttu-id="8c10e-149">応答</span><span class="sxs-lookup"><span data-stu-id="8c10e-149">Response</span></span>

<span data-ttu-id="8c10e-150">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8c10e-150">The following is an example of the response.</span></span>

> <span data-ttu-id="8c10e-151">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="8c10e-151">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8c10e-152">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8c10e-152">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.mailSearchFolder",
  "id": "AAMkAGVmMDEzN",
  "displayName": "Get MyAnalytics",
  "parentFolderId": "AAMkAGVmMDEzI",
  "childFolderCount": 0,
  "unreadItemCount": 6,
  "totalItemCount": 6,
  "wellKnownName": null,
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIds": [
    "AAMkAGVmMDEzM"
  ],
  "filterQuery": "contains(subject, 'MyAnalytics')"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="8c10e-153">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="8c10e-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8c10e-154">C#</span><span class="sxs-lookup"><span data-stu-id="8c10e-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_mailSearchfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8c10e-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="8c10e-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_mailSearchfolder-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailfolder-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/mailfolder-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/mailfolder-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/mailfolder-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
