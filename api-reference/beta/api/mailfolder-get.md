---
title: mailFolder を取得する
description: メッセージ フォルダー オブジェクトのプロパティとリレーションシップを取得します。
author: angelgolfer-ms
ms.openlocfilehash: e1394c6bf97a3c5d65bda0ee7b8f29d8a29643bb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357814"
---
# <a name="get-mailfolder"></a><span data-ttu-id="d9dfe-103">mailFolder を取得する</span><span class="sxs-lookup"><span data-stu-id="d9dfe-103">Get mailFolder</span></span>

> <span data-ttu-id="d9dfe-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d9dfe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d9dfe-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d9dfe-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d9dfe-106">メッセージ フォルダー オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="d9dfe-106">Retrieve the properties and relationships of a message folder object.</span></span>

<span data-ttu-id="d9dfe-107">2 つシナリオは、アプリケーションが別のユーザーのメール フォルダーを取得する場所です。</span><span class="sxs-lookup"><span data-stu-id="d9dfe-107">There are two scenarios where an app can get another user's mail folder:</span></span>

* <span data-ttu-id="d9dfe-108">アプリケーションは、アプリケーションの権限を持つ場合、または、</span><span class="sxs-lookup"><span data-stu-id="d9dfe-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="d9dfe-109">アプリケーションがある場合、適切な 1 人のユーザーから[アクセス許可](#permissions)を委任を実行し、別のユーザーは、そのユーザーのメール フォルダーを共有するにはまたは、そのユーザーに代理アクセスを与えを実行します。</span><span class="sxs-lookup"><span data-stu-id="d9dfe-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="d9dfe-110">[詳細と例](/graph/outlook-share-messages-folders)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d9dfe-110">See [details and an example](/graph/outlook-share-messages-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="d9dfe-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d9dfe-111">Permissions</span></span>
<span data-ttu-id="d9dfe-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d9dfe-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9dfe-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d9dfe-114">Permission type</span></span>      | <span data-ttu-id="d9dfe-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d9dfe-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9dfe-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d9dfe-116">Delegated (work or school account)</span></span> | <span data-ttu-id="d9dfe-117">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9dfe-117">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d9dfe-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d9dfe-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9dfe-119">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9dfe-119">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d9dfe-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d9dfe-120">Application</span></span> | <span data-ttu-id="d9dfe-121">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9dfe-121">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9dfe-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d9dfe-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d9dfe-123">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d9dfe-123">Optional query parameters</span></span>
<span data-ttu-id="d9dfe-124">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d9dfe-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d9dfe-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d9dfe-125">Request headers</span></span>
| <span data-ttu-id="d9dfe-126">名前</span><span class="sxs-lookup"><span data-stu-id="d9dfe-126">Name</span></span>       | <span data-ttu-id="d9dfe-127">種類</span><span class="sxs-lookup"><span data-stu-id="d9dfe-127">Type</span></span> | <span data-ttu-id="d9dfe-128">説明</span><span class="sxs-lookup"><span data-stu-id="d9dfe-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d9dfe-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9dfe-129">Authorization</span></span>  | <span data-ttu-id="d9dfe-130">string</span><span class="sxs-lookup"><span data-stu-id="d9dfe-130">string</span></span>  | <span data-ttu-id="d9dfe-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d9dfe-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9dfe-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="d9dfe-133">Request body</span></span>
<span data-ttu-id="d9dfe-134">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d9dfe-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9dfe-135">応答</span><span class="sxs-lookup"><span data-stu-id="d9dfe-135">Response</span></span>
<span data-ttu-id="d9dfe-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [mailFolder](../resources/mailfolder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d9dfe-136">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="d9dfe-137">例 1</span><span class="sxs-lookup"><span data-stu-id="d9dfe-137">Example 1</span></span>
#### <a name="request-1"></a><span data-ttu-id="d9dfe-138">要求 1</span><span class="sxs-lookup"><span data-stu-id="d9dfe-138">Request 1</span></span>
<span data-ttu-id="d9dfe-139">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d9dfe-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolder"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
```

#### <a name="response-1"></a><span data-ttu-id="d9dfe-140">応答 1</span><span class="sxs-lookup"><span data-stu-id="d9dfe-140">Response 1</span></span>
<span data-ttu-id="d9dfe-141">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d9dfe-141">The following is an example of the response.</span></span>
 ><span data-ttu-id="d9dfe-142">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="d9dfe-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d9dfe-143">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d9dfe-143">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

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

## <a name="example-2"></a><span data-ttu-id="d9dfe-144">例 2</span><span class="sxs-lookup"><span data-stu-id="d9dfe-144">Example 2</span></span>
#### <a name="request-2"></a><span data-ttu-id="d9dfe-145">要求 2</span><span class="sxs-lookup"><span data-stu-id="d9dfe-145">Request 2</span></span>
<span data-ttu-id="d9dfe-146">次に、要求の検索フォルダーの例を示します。</span><span class="sxs-lookup"><span data-stu-id="d9dfe-146">The following is a search folder example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailSearchfolder"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
```

#### <a name="response-2"></a><span data-ttu-id="d9dfe-147">応答 2</span><span class="sxs-lookup"><span data-stu-id="d9dfe-147">Response 2</span></span>
<span data-ttu-id="d9dfe-148">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d9dfe-148">The following is an example of the response.</span></span>
 ><span data-ttu-id="d9dfe-149">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="d9dfe-149">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d9dfe-150">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d9dfe-150">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->