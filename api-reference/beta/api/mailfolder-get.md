---
title: mailFolder を取得する
description: メッセージ フォルダー オブジェクトのプロパティとリレーションシップを取得します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: f997ebe701ce55b16415b0f87d52e0b7fadd2f51
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880098"
---
# <a name="get-mailfolder"></a><span data-ttu-id="659e3-103">mailFolder を取得する</span><span class="sxs-lookup"><span data-stu-id="659e3-103">Get mailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="659e3-104">メッセージ フォルダー オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="659e3-104">Retrieve the properties and relationships of a message folder object.</span></span>

<span data-ttu-id="659e3-105">アプリで別のユーザーのメール フォルダーを取得するシナリオは 2 つあります。</span><span class="sxs-lookup"><span data-stu-id="659e3-105">There are two scenarios where an app can get another user's mail folder:</span></span>

* <span data-ttu-id="659e3-106">アプリにアプリケーションのアクセス許可がある場合。または</span><span class="sxs-lookup"><span data-stu-id="659e3-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="659e3-107">あるユーザーからアプリに適切な代理[アクセス許可](#permissions)が与えられ、別のユーザーがそのユーザーとメール フォルダーを共有しているか、そのユーザーに代理アクセスを付与している場合。</span><span class="sxs-lookup"><span data-stu-id="659e3-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="659e3-108">[詳細と例](/graph/outlook-share-messages-folders)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="659e3-108">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

## <a name="permissions"></a><span data-ttu-id="659e3-109">権限</span><span class="sxs-lookup"><span data-stu-id="659e3-109">Permissions</span></span>

<span data-ttu-id="659e3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="659e3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="659e3-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="659e3-112">Permission type</span></span>      | <span data-ttu-id="659e3-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="659e3-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="659e3-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="659e3-114">Delegated (work or school account)</span></span> | <span data-ttu-id="659e3-115">メール ReadBasic、Mail. 読み取り、ReadWrite</span><span class="sxs-lookup"><span data-stu-id="659e3-115">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="659e3-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="659e3-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="659e3-117">メール ReadBasic、Mail. 読み取り、ReadWrite</span><span class="sxs-lookup"><span data-stu-id="659e3-117">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="659e3-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="659e3-118">Application</span></span> | <span data-ttu-id="659e3-119">-ReadBasic、mail. 読み取り、および書き込み</span><span class="sxs-lookup"><span data-stu-id="659e3-119">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="659e3-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="659e3-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="659e3-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="659e3-121">Optional query parameters</span></span>

<span data-ttu-id="659e3-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="659e3-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="659e3-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="659e3-123">Request headers</span></span>

| <span data-ttu-id="659e3-124">名前</span><span class="sxs-lookup"><span data-stu-id="659e3-124">Name</span></span>          | <span data-ttu-id="659e3-125">型</span><span class="sxs-lookup"><span data-stu-id="659e3-125">Type</span></span>   | <span data-ttu-id="659e3-126">説明</span><span class="sxs-lookup"><span data-stu-id="659e3-126">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="659e3-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="659e3-127">Authorization</span></span> | <span data-ttu-id="659e3-128">string</span><span class="sxs-lookup"><span data-stu-id="659e3-128">string</span></span> | <span data-ttu-id="659e3-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="659e3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="659e3-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="659e3-131">Request body</span></span>

<span data-ttu-id="659e3-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="659e3-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="659e3-133">応答</span><span class="sxs-lookup"><span data-stu-id="659e3-133">Response</span></span>

<span data-ttu-id="659e3-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [mailFolder](../resources/mailfolder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="659e3-134">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="659e3-135">例</span><span class="sxs-lookup"><span data-stu-id="659e3-135">Examples</span></span>

### <a name="example-1-get-a-mail-folder"></a><span data-ttu-id="659e3-136">例 1: メールフォルダーを取得する</span><span class="sxs-lookup"><span data-stu-id="659e3-136">Example 1: Get a mail folder</span></span>

#### <a name="request"></a><span data-ttu-id="659e3-137">要求</span><span class="sxs-lookup"><span data-stu-id="659e3-137">Request</span></span>

<span data-ttu-id="659e3-138">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="659e3-138">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="659e3-139">プロトコル</span><span class="sxs-lookup"><span data-stu-id="659e3-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEzM"],
  "name": "get_mailfolder"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="659e3-140">C#</span><span class="sxs-lookup"><span data-stu-id="659e3-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="659e3-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="659e3-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="659e3-142">目的-C</span><span class="sxs-lookup"><span data-stu-id="659e3-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="659e3-143">Java</span><span class="sxs-lookup"><span data-stu-id="659e3-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="659e3-144">応答</span><span class="sxs-lookup"><span data-stu-id="659e3-144">Response</span></span>

<span data-ttu-id="659e3-145">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="659e3-145">The following is an example of the response.</span></span>

> <span data-ttu-id="659e3-146">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="659e3-146">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="659e3-147">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="659e3-147">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-mail-search-folder"></a><span data-ttu-id="659e3-148">例 2: メール検索フォルダーを取得する</span><span class="sxs-lookup"><span data-stu-id="659e3-148">Example 2: Get a mail search folder</span></span>

#### <a name="request"></a><span data-ttu-id="659e3-149">要求</span><span class="sxs-lookup"><span data-stu-id="659e3-149">Request</span></span>

<span data-ttu-id="659e3-150">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="659e3-150">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="659e3-151">プロトコル</span><span class="sxs-lookup"><span data-stu-id="659e3-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEzM"],
  "name": "get_mailSearchfolder"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzN
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="659e3-152">C#</span><span class="sxs-lookup"><span data-stu-id="659e3-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailsearchfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="659e3-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="659e3-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailsearchfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="659e3-154">目的-C</span><span class="sxs-lookup"><span data-stu-id="659e3-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailsearchfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="659e3-155">Java</span><span class="sxs-lookup"><span data-stu-id="659e3-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailsearchfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="659e3-156">応答</span><span class="sxs-lookup"><span data-stu-id="659e3-156">Response</span></span>

<span data-ttu-id="659e3-157">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="659e3-157">The following is an example of the response.</span></span>

> <span data-ttu-id="659e3-158">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="659e3-158">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="659e3-159">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="659e3-159">All the properties will be returned from an actual call.</span></span>

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
  ]
}
-->
