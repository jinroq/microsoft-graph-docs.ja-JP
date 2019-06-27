---
title: mailFolders を一覧表示する　
description: サインインしているユーザーのメールボックス内のすべてのメールフォルダーを取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 86e2ef795db5eb3fd2973854d982cb2d7742927a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270192"
---
# <a name="list-mailfolders"></a><span data-ttu-id="d28c8-103">mailFolders を一覧表示する　</span><span class="sxs-lookup"><span data-stu-id="d28c8-103">List mailFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d28c8-104">サインインしているユーザーのメールボックス内のすべてのメールフォルダーを取得します (すべてのメール[検索フォルダー](../resources/mailsearchfolder.md)を含みます)。</span><span class="sxs-lookup"><span data-stu-id="d28c8-104">Get all the mail folders in the signed-in user's mailbox, including any [mail search folders](../resources/mailsearchfolder.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d28c8-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d28c8-105">Permissions</span></span>
<span data-ttu-id="d28c8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d28c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d28c8-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d28c8-108">Permission type</span></span>      | <span data-ttu-id="d28c8-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d28c8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d28c8-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d28c8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d28c8-111">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d28c8-111">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d28c8-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d28c8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d28c8-113">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d28c8-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d28c8-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d28c8-114">Application</span></span> | <span data-ttu-id="d28c8-115">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d28c8-115">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d28c8-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d28c8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders
GET /users/{id | userPrincipalName}/mailFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d28c8-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d28c8-117">Optional query parameters</span></span>
<span data-ttu-id="d28c8-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d28c8-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d28c8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d28c8-119">Request headers</span></span>
| <span data-ttu-id="d28c8-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d28c8-120">Header</span></span>       | <span data-ttu-id="d28c8-121">値</span><span class="sxs-lookup"><span data-stu-id="d28c8-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d28c8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d28c8-122">Authorization</span></span>  | <span data-ttu-id="d28c8-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d28c8-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d28c8-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d28c8-125">Content-Type</span></span>   | <span data-ttu-id="d28c8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d28c8-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d28c8-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d28c8-127">Request body</span></span>
<span data-ttu-id="d28c8-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d28c8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d28c8-129">応答</span><span class="sxs-lookup"><span data-stu-id="d28c8-129">Response</span></span>

<span data-ttu-id="d28c8-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[mailfolder](../resources/mailfolder.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="d28c8-130">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d28c8-131">例</span><span class="sxs-lookup"><span data-stu-id="d28c8-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d28c8-132">要求</span><span class="sxs-lookup"><span data-stu-id="d28c8-132">Request</span></span>
<span data-ttu-id="d28c8-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d28c8-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders
```
##### <a name="response"></a><span data-ttu-id="d28c8-134">応答</span><span class="sxs-lookup"><span data-stu-id="d28c8-134">Response</span></span>
<span data-ttu-id="d28c8-135">受信トレイの下の子フォルダーである**Mailsearchfolder**を含む応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d28c8-135">Here is an example of the response which includes a **mailSearchFolder** that is a child folder under the Inbox.</span></span> <span data-ttu-id="d28c8-136">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="d28c8-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d28c8-137">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d28c8-137">All of the properties will be returned from an actual call.</span></span>
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
            "@odata.type": "#microsoft.graph.mailSearchFolder",
            "id": "AAMkADYRAAAZg1yTAAA=",
            "displayName": "Weekly digests",
            "parentFolderId": "AQMkADYAAAIBDAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 4,
            "totalItemCount": 5,
            "wellKnownName": null,
            "isSupported": true,
            "filterQuery": "contains(subject, 'weekly digest')"
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d28c8-138">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="d28c8-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d28c8-139">C#</span><span class="sxs-lookup"><span data-stu-id="d28c8-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_mailfolders-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d28c8-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="d28c8-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_mailfolders-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d28c8-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="d28c8-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_mailfolders-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List mailFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-mailfolders.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-list-mailfolders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-list-mailfolders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
