---
title: mailFolders を一覧表示する　
description: 'サインイン中のユーザーのルート フォルダーからメール フォルダー コレクションを取得します。 '
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: f069a7c3a014e0b1b3b9d936dc67fd85e6406736
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35460274"
---
# <a name="list-mailfolders"></a><span data-ttu-id="59996-103">mailFolders を一覧表示する　</span><span class="sxs-lookup"><span data-stu-id="59996-103">List mailFolders</span></span>

<span data-ttu-id="59996-104">サインイン中のユーザーのルート フォルダーからメール フォルダー コレクションを直接取得します。</span><span class="sxs-lookup"><span data-stu-id="59996-104">Get the mail folder collection under the root folder of the signed-in user.</span></span> <span data-ttu-id="59996-105">返されたコレクションには、ルート直下にある[メール検索フォルダー](../resources/mailsearchfolder.md)が含まれています。</span><span class="sxs-lookup"><span data-stu-id="59996-105">The returned collection includes any [mail search folders](../resources/mailsearchfolder.md) directly under the root.</span></span>

## <a name="permissions"></a><span data-ttu-id="59996-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="59996-106">Permissions</span></span>
<span data-ttu-id="59996-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="59996-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59996-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="59996-109">Permission type</span></span>      | <span data-ttu-id="59996-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="59996-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59996-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="59996-111">Delegated (work or school account)</span></span> | <span data-ttu-id="59996-112">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59996-112">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="59996-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="59996-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59996-114">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59996-114">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="59996-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="59996-115">Application</span></span> | <span data-ttu-id="59996-116">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59996-116">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="59996-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="59996-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders
GET /users/{id | userPrincipalName}/mailFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="59996-118">省略可能なクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="59996-118">Optional query parameters</span></span>
<span data-ttu-id="59996-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="59996-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="59996-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="59996-120">Request headers</span></span>
| <span data-ttu-id="59996-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="59996-121">Header</span></span>       | <span data-ttu-id="59996-122">値</span><span class="sxs-lookup"><span data-stu-id="59996-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="59996-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="59996-123">Authorization</span></span>  | <span data-ttu-id="59996-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="59996-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="59996-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="59996-126">Content-Type</span></span>   | <span data-ttu-id="59996-127">application/json</span><span class="sxs-lookup"><span data-stu-id="59996-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="59996-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="59996-128">Request body</span></span>
<span data-ttu-id="59996-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="59996-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59996-130">応答</span><span class="sxs-lookup"><span data-stu-id="59996-130">Response</span></span>

<span data-ttu-id="59996-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [mailFolder](../resources/mailfolder.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="59996-131">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="59996-132">例</span><span class="sxs-lookup"><span data-stu-id="59996-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59996-133">要求</span><span class="sxs-lookup"><span data-stu-id="59996-133">Request</span></span>
<span data-ttu-id="59996-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="59996-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="59996-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="59996-135">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="59996-136">C#</span><span class="sxs-lookup"><span data-stu-id="59996-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="59996-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="59996-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="59996-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="59996-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="59996-139">応答</span><span class="sxs-lookup"><span data-stu-id="59996-139">Response</span></span>
<span data-ttu-id="59996-140">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="59996-140">Here is an example of the response.</span></span> 

><span data-ttu-id="59996-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="59996-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('68ca8ec0-11f8-456b-a785-70d9936650d5')/mailFolders",
    "value": [
        {
            "id": "AQMkADYAAAIBXQAAAA==",
            "displayName": "Archive",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "archive"
        },
        {
            "id": "AQMkADYAAAIBFQAAAA==",
            "displayName": "Conversation History",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 1,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "conversationhistory"
        },
        {
            "id": "AQMkADYAAAIBCgAAAA==",
            "displayName": "Deleted Items",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "deleteditems"
        },
        {
            "id": "AQMkADYAAAIBDwAAAA==",
            "displayName": "Drafts",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "drafts"
        },
        {
            "id": "AQMkADYAAAIBDAAAAA==",
            "displayName": "Inbox",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 1,
            "unreadItemCount": 70,
            "totalItemCount": 71,
            "wellKnownName": "inbox"
        },
        {
            "id": "AQMkADYAAAIBGQAAAA==",
            "displayName": "Junk Email",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "junkemail"
        },
        {
            "id": "AQMkADYAAAIBCwAAAA==",
            "displayName": "Outbox",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "outbox"
        },
        {
            "id": "AQMkADYAAAIBCQAAAA==",
            "displayName": "Sent Items",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "sentitems"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List mailFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
