---
title: メッセージを一覧表示する
description: サインイン中のユーザーのメールボックス内のメッセージを取得します (削除済みアイテムと低優先メール フォルダーを含む)。
localization_priority: Priority
ms.openlocfilehash: 5ded8cef8142bdeeaa17eabc1f78a8bfa0f0d019
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862707"
---
# <a name="list-messages"></a><span data-ttu-id="0aeac-103">メッセージを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="0aeac-103">List messages</span></span>

<span data-ttu-id="0aeac-104">サインイン中のユーザーのメールボックス内のメッセージを取得します (削除済みアイテムと低優先メール フォルダーを含む)。</span><span class="sxs-lookup"><span data-stu-id="0aeac-104">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span>

<span data-ttu-id="0aeac-105">現在、この操作によって返されるメッセージの本文は HTML 形式のみです。</span><span class="sxs-lookup"><span data-stu-id="0aeac-105">Currently, this operation returns message bodies in only HTML format.</span></span>

<span data-ttu-id="0aeac-106">2 つシナリオは、アプリケーションが別のユーザーのメール フォルダーにメッセージを取得する場所です。</span><span class="sxs-lookup"><span data-stu-id="0aeac-106">There are two scenarios where an app can get messages in another user's mail folder:</span></span>

* <span data-ttu-id="0aeac-107">アプリケーションは、アプリケーションの権限を持つ場合、または、</span><span class="sxs-lookup"><span data-stu-id="0aeac-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="0aeac-108">アプリケーションがある場合、適切な 1 人のユーザーから[アクセス許可](#permissions)を委任を実行し、別のユーザーは、そのユーザーのメール フォルダーを共有するにはまたは、そのユーザーに代理アクセスを与えを実行します。</span><span class="sxs-lookup"><span data-stu-id="0aeac-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="0aeac-109">[詳細と例](/graph/outlook-share-messages-folders)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0aeac-109">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

## <a name="permissions"></a><span data-ttu-id="0aeac-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0aeac-110">Permissions</span></span>
<span data-ttu-id="0aeac-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0aeac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0aeac-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0aeac-113">Permission type</span></span>      | <span data-ttu-id="0aeac-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0aeac-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0aeac-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0aeac-115">Delegated (work or school account)</span></span> | <span data-ttu-id="0aeac-116">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0aeac-116">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0aeac-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0aeac-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0aeac-118">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0aeac-118">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0aeac-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0aeac-119">Application</span></span> | <span data-ttu-id="0aeac-120">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0aeac-120">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0aeac-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0aeac-121">HTTP request</span></span>

<span data-ttu-id="0aeac-122">ユーザーのメールボックス内のすべてのメッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="0aeac-122">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="0aeac-123">ユーザーのメールボックス内の特定のフォルダーにあるメッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="0aeac-123">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0aeac-124">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="0aeac-124">Optional query parameters</span></span>
<span data-ttu-id="0aeac-125">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="0aeac-125">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0aeac-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0aeac-126">Request headers</span></span>
| <span data-ttu-id="0aeac-127">名前</span><span class="sxs-lookup"><span data-stu-id="0aeac-127">Name</span></span>       | <span data-ttu-id="0aeac-128">種類</span><span class="sxs-lookup"><span data-stu-id="0aeac-128">Type</span></span> | <span data-ttu-id="0aeac-129">説明</span><span class="sxs-lookup"><span data-stu-id="0aeac-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0aeac-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="0aeac-130">Authorization</span></span>  | <span data-ttu-id="0aeac-131">string</span><span class="sxs-lookup"><span data-stu-id="0aeac-131">string</span></span>  | <span data-ttu-id="0aeac-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0aeac-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0aeac-134">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="0aeac-134">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="0aeac-135">文字列</span><span class="sxs-lookup"><span data-stu-id="0aeac-135">string</span></span> | <span data-ttu-id="0aeac-136">**body** プロパティと **uniqueBody** プロパティが返されるときの形式です。</span><span class="sxs-lookup"><span data-stu-id="0aeac-136">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="0aeac-137">値は、"text" または "html" になります。</span><span class="sxs-lookup"><span data-stu-id="0aeac-137">Values can be "text" or "html".</span></span> <span data-ttu-id="0aeac-138">ヘッダーが指定されていない場合は、**body** プロパティと **uniqueBody** プロパティは HTML 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="0aeac-138">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="0aeac-139">省略可能。</span><span class="sxs-lookup"><span data-stu-id="0aeac-139">Optional.</span></span> |


## <a name="request-body"></a><span data-ttu-id="0aeac-140">要求本文</span><span class="sxs-lookup"><span data-stu-id="0aeac-140">Request body</span></span>
<span data-ttu-id="0aeac-141">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0aeac-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0aeac-142">応答</span><span class="sxs-lookup"><span data-stu-id="0aeac-142">Response</span></span>

<span data-ttu-id="0aeac-143">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Message](../resources/message.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="0aeac-143">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>

<span data-ttu-id="0aeac-144">この要求の既定のページ サイズは、メッセージ 10 個です。</span><span class="sxs-lookup"><span data-stu-id="0aeac-144">The default page size for this request is 10 messages.</span></span>

## <a name="example"></a><span data-ttu-id="0aeac-145">例</span><span class="sxs-lookup"><span data-stu-id="0aeac-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0aeac-146">要求</span><span class="sxs-lookup"><span data-stu-id="0aeac-146">Request</span></span>
<span data-ttu-id="0aeac-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0aeac-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages
```
##### <a name="response"></a><span data-ttu-id="0aeac-148">応答</span><span class="sxs-lookup"><span data-stu-id="0aeac-148">Response</span></span>
<span data-ttu-id="0aeac-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0aeac-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 317

{
  "value": [
    {
      "receivedDateTime": "datetime-value",
      "sentDateTime": "datetime-value",
      "hasAttachments": true,
      "subject": "subject-value",
      "body": {
        "contentType": "",
        "content": "content-value"
      },
      "bodyPreview": "bodyPreview-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
