---
title: 'メッセージ: move'
description: メッセージをフォルダーに移動します。 これは、先のフォルダーにメッセージの新しいコピーを作成し、元のメッセージを削除します。
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 7ad9ac2b8f64d75950c9b2cac17a4c5dc5a9b3eb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843289"
---
# <a name="message-move"></a><span data-ttu-id="50661-104">メッセージ: move</span><span class="sxs-lookup"><span data-stu-id="50661-104">message: move</span></span>

> <span data-ttu-id="50661-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="50661-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="50661-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="50661-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="50661-107">メッセージをフォルダーに移動します。</span><span class="sxs-lookup"><span data-stu-id="50661-107">Move a message to a folder.</span></span> <span data-ttu-id="50661-108">これは、先のフォルダーにメッセージの新しいコピーを作成し、元のメッセージを削除します。</span><span class="sxs-lookup"><span data-stu-id="50661-108">This creates a new copy of the message in the destination folder and removes the original message.</span></span>

## <a name="permissions"></a><span data-ttu-id="50661-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="50661-109">Permissions</span></span>

<span data-ttu-id="50661-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="50661-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="50661-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="50661-112">Permission type</span></span> | <span data-ttu-id="50661-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="50661-113">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="50661-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="50661-114">Delegated (work or school account)</span></span> | <span data-ttu-id="50661-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50661-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="50661-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="50661-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50661-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50661-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="50661-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="50661-118">Application</span></span> | <span data-ttu-id="50661-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50661-119">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="50661-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="50661-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/move
POST /users/{id | userPrincipalName}/messages/{id}/move
POST /me/mailFolders/{id}/messages/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="50661-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="50661-121">Request headers</span></span>

| <span data-ttu-id="50661-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="50661-122">Header</span></span> | <span data-ttu-id="50661-123">値</span><span class="sxs-lookup"><span data-stu-id="50661-123">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="50661-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="50661-124">Authorization</span></span> | <span data-ttu-id="50661-125">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="50661-125"></span></span> <span data-ttu-id="50661-126">必須。</span><span class="sxs-lookup"><span data-stu-id="50661-126">Required.</span></span> |
| <span data-ttu-id="50661-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="50661-127">Content-Type</span></span> | <span data-ttu-id="50661-128">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="50661-128"></span></span> <span data-ttu-id="50661-129">必須。</span><span class="sxs-lookup"><span data-stu-id="50661-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="50661-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="50661-130">Request body</span></span>

<span data-ttu-id="50661-131">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="50661-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="50661-132">パラメーター</span><span class="sxs-lookup"><span data-stu-id="50661-132">Parameter</span></span>   | <span data-ttu-id="50661-133">Type</span><span class="sxs-lookup"><span data-stu-id="50661-133">Type</span></span> |<span data-ttu-id="50661-134">説明</span><span class="sxs-lookup"><span data-stu-id="50661-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50661-135">DestinationId</span><span class="sxs-lookup"><span data-stu-id="50661-135">DestinationId</span></span>|<span data-ttu-id="50661-136">String</span><span class="sxs-lookup"><span data-stu-id="50661-136">String</span></span>|<span data-ttu-id="50661-137">移動先のフォルダー ID、またはよく知られているフォルダー名です。</span><span class="sxs-lookup"><span data-stu-id="50661-137">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="50661-138">サポートされている既知のフォルダー名の一覧については、「[mailFolder リソースの種類](../resources/mailfolder.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="50661-138">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="50661-139">応答</span><span class="sxs-lookup"><span data-stu-id="50661-139">Response</span></span>

<span data-ttu-id="50661-140">かどうかは成功すると、このメソッドを返します`201 Created`応答コードおよび応答の本文に[メッセージ](../resources/message.md)リソース。</span><span class="sxs-lookup"><span data-stu-id="50661-140">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50661-141">例</span><span class="sxs-lookup"><span data-stu-id="50661-141">Example</span></span>

<span data-ttu-id="50661-142">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="50661-142">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="50661-143">要求</span><span class="sxs-lookup"><span data-stu-id="50661-143">Request</span></span>

<span data-ttu-id="50661-144">次のような要求の既知のフォルダー名で識別される、[削除済みアイテム フォルダーに指定したメッセージを移動する`deleteditems`。</span><span class="sxs-lookup"><span data-stu-id="50661-144">The following request moves the specified message to the Deleted Items folder, identified by its well-known folder name `deleteditems`.</span></span>
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

##### <a name="response"></a><span data-ttu-id="50661-145">応答</span><span class="sxs-lookup"><span data-stu-id="50661-145">Response</span></span>

<span data-ttu-id="50661-146">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="50661-146">Here is an example of the response.</span></span>

> <span data-ttu-id="50661-147">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="50661-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="50661-148">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="50661-148">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "message: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
