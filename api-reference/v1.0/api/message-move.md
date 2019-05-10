---
title: 'メッセージ: move'
description: メッセージをフォルダーに移動します。 これにより、宛先フォルダーにメッセージの新しいコピーが作成され、元のメッセージが削除されます。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 6594510eaab6f94f2d1650eea167be99f68d995f
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33612480"
---
# <a name="message-move"></a><span data-ttu-id="18afa-104">メッセージ: move</span><span class="sxs-lookup"><span data-stu-id="18afa-104">message: move</span></span>

<span data-ttu-id="18afa-105">メッセージをフォルダーに移動します。</span><span class="sxs-lookup"><span data-stu-id="18afa-105">Move a message to a folder.</span></span> <span data-ttu-id="18afa-106">これにより、宛先フォルダーにメッセージの新しいコピーが作成され、元のメッセージが削除されます。</span><span class="sxs-lookup"><span data-stu-id="18afa-106">This creates a new copy of the message in the destination folder and removes the original message.</span></span>

## <a name="permissions"></a><span data-ttu-id="18afa-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="18afa-107">Permissions</span></span>

<span data-ttu-id="18afa-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="18afa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="18afa-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="18afa-110">Permission type</span></span> | <span data-ttu-id="18afa-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="18afa-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="18afa-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="18afa-112">Delegated (work or school account)</span></span> | <span data-ttu-id="18afa-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18afa-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="18afa-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="18afa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18afa-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18afa-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="18afa-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="18afa-116">Application</span></span> | <span data-ttu-id="18afa-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18afa-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="18afa-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="18afa-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/move
POST /users/{id | userPrincipalName}/messages/{id}/move
POST /me/mailFolders/{id}/messages/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="18afa-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18afa-119">Request headers</span></span>

| <span data-ttu-id="18afa-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18afa-120">Header</span></span> | <span data-ttu-id="18afa-121">値</span><span class="sxs-lookup"><span data-stu-id="18afa-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="18afa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="18afa-122">Authorization</span></span> | <span data-ttu-id="18afa-123">`Bearer {token}`</span><span class="sxs-lookup"><span data-stu-id="18afa-123">`Bearer {token}`.</span></span> <span data-ttu-id="18afa-124">必須です。</span><span class="sxs-lookup"><span data-stu-id="18afa-124">Required.</span></span> |
| <span data-ttu-id="18afa-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="18afa-125">Content-Type</span></span> | <span data-ttu-id="18afa-126">`application/json`</span><span class="sxs-lookup"><span data-stu-id="18afa-126">`application/json`.</span></span> <span data-ttu-id="18afa-127">必須です。</span><span class="sxs-lookup"><span data-stu-id="18afa-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="18afa-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="18afa-128">Request body</span></span>

<span data-ttu-id="18afa-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="18afa-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="18afa-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="18afa-130">Parameter</span></span>   | <span data-ttu-id="18afa-131">型</span><span class="sxs-lookup"><span data-stu-id="18afa-131">Type</span></span> |<span data-ttu-id="18afa-132">説明</span><span class="sxs-lookup"><span data-stu-id="18afa-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18afa-133">destinationId</span><span class="sxs-lookup"><span data-stu-id="18afa-133">destinationId</span></span>|<span data-ttu-id="18afa-134">String</span><span class="sxs-lookup"><span data-stu-id="18afa-134">String</span></span>|<span data-ttu-id="18afa-135">宛先フォルダーの ID または既知のフォルダー名です。</span><span class="sxs-lookup"><span data-stu-id="18afa-135">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="18afa-136">サポートされている既知のフォルダー名の一覧については、「[mailFolder リソースの種類](../resources/mailfolder.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="18afa-136">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="18afa-137">応答</span><span class="sxs-lookup"><span data-stu-id="18afa-137">Response</span></span>

<span data-ttu-id="18afa-138">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [message](../resources/message.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="18afa-138">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18afa-139">例</span><span class="sxs-lookup"><span data-stu-id="18afa-139">Example</span></span>

<span data-ttu-id="18afa-140">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="18afa-140">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="18afa-141">要求</span><span class="sxs-lookup"><span data-stu-id="18afa-141">Request</span></span>

<span data-ttu-id="18afa-142">次の要求は、指定されたメッセージを既知のフォルダー名 `deleteditems` で識別される削除済みアイテム フォルダーに移動します。</span><span class="sxs-lookup"><span data-stu-id="18afa-142">The following request moves the specified message to the Deleted Items folder, identified by its well-known folder name `deleteditems`.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhAAATs28OAAA="],
  "name": "message_move"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkADhAAATs28OAAA=/move
Content-type: application/json

{
  "destinationId": "deleteditems"
}
```

##### <a name="response"></a><span data-ttu-id="18afa-143">応答</span><span class="sxs-lookup"><span data-stu-id="18afa-143">Response</span></span>

<span data-ttu-id="18afa-144">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="18afa-144">Here is an example of the response.</span></span>

> <span data-ttu-id="18afa-145">**注:**  ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="18afa-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="18afa-146">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="18afa-146">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#message",
    "@odata.type":"#microsoft.graph.message",
    "@odata.etag":"W/\"FwAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAW/0tB\"",
    "id":"AAMkADhAAAW-VPeAAA=",
    "createdDateTime":"2018-08-12T08:43:22Z",
    "lastModifiedDateTime":"2018-08-15T19:47:54Z",
    "changeKey":"FwAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAW/0tB",
    "categories":[

    ],
    "receivedDateTime":"2018-08-12T08:43:22Z",
    "sentDateTime":"2018-08-12T08:43:20Z",
    "hasAttachments":false,
    "internetMessageId":"<00535324-5988-4b6a-b9af-d44cf2d0b691@MWHPR2201MB1022.namprd22.prod.outlook.com>",
    "subject":"Undeliverable: Meet for lunch?",
    "bodyPreview":"Delivery has failed to these recipients or groups:\r\n\r\nfannyd@contoso.onmicrosoft.com (fannyd@contoso.onmicrosoft.com)\r\nYour message couldn't be delivered. Despite repeated attempts to deliver your message, querying the Domain Name System (DNS) for the rec",
    "importance":"normal",
    "parentFolderId":"AAMkADhAAAAAAEKAAA=",
    "conversationId":"AAQkADhJzfbkARFhe5kKhjihSA=",
    "isDeliveryReceiptRequested":null,
    "isReadReceiptRequested":false,
    "isRead":false,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADhAAAW%2FVPeAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "body":{
        "contentType":"html",
        "content":"<html></html>"
    },
    "sender":{
        "emailAddress":{
            "name":"Microsoft Outlook",
            "address":"MicrosoftExchange329e71ec88ae4615bbc36ab6ce41109e@contoso.onmicrosoft.com"
        }
    },
    "from":{
        "emailAddress":{
            "name":"Microsoft Outlook",
            "address":"MicrosoftExchange329e71ec88ae4615bbc36ab6ce41109e@contoso.onmicrosoft.com"
        }
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"fannyd@contoso.onmicrosoft.com",
                "address":"fannyd@contoso.onmicrosoft.com"
            }
        },
        {
            "emailAddress":{
                "name":"danas@contoso.onmicrosoft.com",
                "address":"danas@contoso.onmicrosoft.com"
            }
        }
    ],
    "ccRecipients":[

    ],
    "bccRecipients":[

    ],
    "replyTo":[

    ],
    "flag":{
        "flagStatus":"notFlagged"
    }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="18afa-147">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="18afa-147">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="18afa-148">C#</span><span class="sxs-lookup"><span data-stu-id="18afa-148">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/message_move-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="18afa-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="18afa-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/message_move-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/message-move.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/message-move.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
