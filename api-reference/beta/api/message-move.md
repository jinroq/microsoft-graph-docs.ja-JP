---
title: 'メッセージ: move'
description: メッセージをフォルダーに移動します。 これにより、宛先フォルダーにメッセージの新しいコピーが作成され、元のメッセージが削除されます。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e0c96d5a921b4e9a7e3e051ccac9d3678a2b259a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35983923"
---
# <a name="message-move"></a><span data-ttu-id="4c24c-104">メッセージ: move</span><span class="sxs-lookup"><span data-stu-id="4c24c-104">message: move</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c24c-105">メッセージをフォルダーに移動します。</span><span class="sxs-lookup"><span data-stu-id="4c24c-105">Move a message to a folder.</span></span> <span data-ttu-id="4c24c-106">これにより、宛先フォルダーにメッセージの新しいコピーが作成され、元のメッセージが削除されます。</span><span class="sxs-lookup"><span data-stu-id="4c24c-106">This creates a new copy of the message in the destination folder and removes the original message.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c24c-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4c24c-107">Permissions</span></span>

<span data-ttu-id="4c24c-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4c24c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4c24c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4c24c-110">Permission type</span></span> | <span data-ttu-id="4c24c-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4c24c-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="4c24c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4c24c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4c24c-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4c24c-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4c24c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4c24c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c24c-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4c24c-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4c24c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4c24c-116">Application</span></span> | <span data-ttu-id="4c24c-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4c24c-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c24c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4c24c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/move
POST /users/{id | userPrincipalName}/messages/{id}/move
POST /me/mailFolders/{id}/messages/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="4c24c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4c24c-119">Request headers</span></span>

| <span data-ttu-id="4c24c-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4c24c-120">Header</span></span> | <span data-ttu-id="4c24c-121">値</span><span class="sxs-lookup"><span data-stu-id="4c24c-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="4c24c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c24c-122">Authorization</span></span> | <span data-ttu-id="4c24c-123">`Bearer {token}`</span><span class="sxs-lookup"><span data-stu-id="4c24c-123">`Bearer {token}`.</span></span> <span data-ttu-id="4c24c-124">必須です。</span><span class="sxs-lookup"><span data-stu-id="4c24c-124">Required.</span></span> |
| <span data-ttu-id="4c24c-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4c24c-125">Content-Type</span></span> | <span data-ttu-id="4c24c-126">`application/json`</span><span class="sxs-lookup"><span data-stu-id="4c24c-126">`application/json`.</span></span> <span data-ttu-id="4c24c-127">必須です。</span><span class="sxs-lookup"><span data-stu-id="4c24c-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c24c-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="4c24c-128">Request body</span></span>

<span data-ttu-id="4c24c-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="4c24c-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4c24c-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="4c24c-130">Parameter</span></span>   | <span data-ttu-id="4c24c-131">型</span><span class="sxs-lookup"><span data-stu-id="4c24c-131">Type</span></span> |<span data-ttu-id="4c24c-132">説明</span><span class="sxs-lookup"><span data-stu-id="4c24c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c24c-133">DestinationId</span><span class="sxs-lookup"><span data-stu-id="4c24c-133">DestinationId</span></span>|<span data-ttu-id="4c24c-134">String</span><span class="sxs-lookup"><span data-stu-id="4c24c-134">String</span></span>|<span data-ttu-id="4c24c-135">宛先フォルダーの ID または既知のフォルダー名です。</span><span class="sxs-lookup"><span data-stu-id="4c24c-135">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="4c24c-136">サポートされている既知のフォルダー名の一覧については、「[mailFolder リソースの種類](../resources/mailfolder.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4c24c-136">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="4c24c-137">応答</span><span class="sxs-lookup"><span data-stu-id="4c24c-137">Response</span></span>

<span data-ttu-id="4c24c-138">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [message](../resources/message.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="4c24c-138">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c24c-139">例</span><span class="sxs-lookup"><span data-stu-id="4c24c-139">Example</span></span>

<span data-ttu-id="4c24c-140">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="4c24c-140">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="4c24c-141">要求</span><span class="sxs-lookup"><span data-stu-id="4c24c-141">Request</span></span>

<span data-ttu-id="4c24c-142">次の要求は、指定されたメッセージを既知のフォルダー名 `deleteditems` で識別される削除済みアイテム フォルダーに移動します。</span><span class="sxs-lookup"><span data-stu-id="4c24c-142">The following request moves the specified message to the Deleted Items folder, identified by its well-known folder name `deleteditems`.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4c24c-143">プロトコル</span><span class="sxs-lookup"><span data-stu-id="4c24c-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhAAATs28OAAA="],
  "name": "message_move"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADhAAATs28OAAA=/move
Content-type: application/json

{
  "destinationId": "deleteditems"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4c24c-144">C#</span><span class="sxs-lookup"><span data-stu-id="4c24c-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-move-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4c24c-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="4c24c-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-move-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4c24c-146">目的-C</span><span class="sxs-lookup"><span data-stu-id="4c24c-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-move-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4c24c-147">Java</span><span class="sxs-lookup"><span data-stu-id="4c24c-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-move-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4c24c-148">応答</span><span class="sxs-lookup"><span data-stu-id="4c24c-148">Response</span></span>

<span data-ttu-id="4c24c-149">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="4c24c-149">Here is an example of the response.</span></span>

> <span data-ttu-id="4c24c-150">**注:**  ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="4c24c-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4c24c-151">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="4c24c-151">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#message",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
