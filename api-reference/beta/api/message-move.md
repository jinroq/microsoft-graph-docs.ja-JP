---
title: 'メッセージ: move'
description: メッセージをフォルダーに移動します。 これは、先のフォルダーにメッセージの新しいコピーを作成し、元のメッセージを削除します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: efe2bcf262ef91b4684bc812fa19bdbe52f12564
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526859"
---
# <a name="message-move"></a><span data-ttu-id="07363-104">メッセージ: move</span><span class="sxs-lookup"><span data-stu-id="07363-104">message: move</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07363-105">メッセージをフォルダーに移動します。</span><span class="sxs-lookup"><span data-stu-id="07363-105">Move a message to a folder.</span></span> <span data-ttu-id="07363-106">これは、先のフォルダーにメッセージの新しいコピーを作成し、元のメッセージを削除します。</span><span class="sxs-lookup"><span data-stu-id="07363-106">This creates a new copy of the message in the destination folder and removes the original message.</span></span>

## <a name="permissions"></a><span data-ttu-id="07363-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="07363-107">Permissions</span></span>

<span data-ttu-id="07363-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="07363-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="07363-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="07363-110">Permission type</span></span> | <span data-ttu-id="07363-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="07363-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="07363-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="07363-112">Delegated (work or school account)</span></span> | <span data-ttu-id="07363-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="07363-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="07363-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="07363-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07363-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="07363-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="07363-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="07363-116">Application</span></span> | <span data-ttu-id="07363-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="07363-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="07363-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="07363-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/move
POST /users/{id | userPrincipalName}/messages/{id}/move
POST /me/mailFolders/{id}/messages/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="07363-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="07363-119">Request headers</span></span>

| <span data-ttu-id="07363-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="07363-120">Header</span></span> | <span data-ttu-id="07363-121">値</span><span class="sxs-lookup"><span data-stu-id="07363-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="07363-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="07363-122">Authorization</span></span> | <span data-ttu-id="07363-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="07363-123"></span></span> <span data-ttu-id="07363-124">必須です。</span><span class="sxs-lookup"><span data-stu-id="07363-124">Required.</span></span> |
| <span data-ttu-id="07363-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="07363-125">Content-Type</span></span> | <span data-ttu-id="07363-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="07363-126"></span></span> <span data-ttu-id="07363-127">必須です。</span><span class="sxs-lookup"><span data-stu-id="07363-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="07363-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="07363-128">Request body</span></span>

<span data-ttu-id="07363-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="07363-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="07363-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="07363-130">Parameter</span></span>   | <span data-ttu-id="07363-131">型</span><span class="sxs-lookup"><span data-stu-id="07363-131">Type</span></span> |<span data-ttu-id="07363-132">説明</span><span class="sxs-lookup"><span data-stu-id="07363-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07363-133">DestinationId</span><span class="sxs-lookup"><span data-stu-id="07363-133">DestinationId</span></span>|<span data-ttu-id="07363-134">String</span><span class="sxs-lookup"><span data-stu-id="07363-134">String</span></span>|<span data-ttu-id="07363-135">移動先のフォルダー ID、またはよく知られているフォルダー名です。</span><span class="sxs-lookup"><span data-stu-id="07363-135">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="07363-136">サポートされている既知のフォルダー名の一覧については、「[mailFolder リソースの種類](../resources/mailfolder.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="07363-136">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="07363-137">応答</span><span class="sxs-lookup"><span data-stu-id="07363-137">Response</span></span>

<span data-ttu-id="07363-138">かどうかは成功すると、このメソッドを返します`201 Created`応答コードおよび応答の本文に[メッセージ](../resources/message.md)リソース。</span><span class="sxs-lookup"><span data-stu-id="07363-138">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07363-139">例</span><span class="sxs-lookup"><span data-stu-id="07363-139">Example</span></span>

<span data-ttu-id="07363-140">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="07363-140">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="07363-141">要求</span><span class="sxs-lookup"><span data-stu-id="07363-141">Request</span></span>

<span data-ttu-id="07363-142">次のような要求の既知のフォルダー名で識別される、[削除済みアイテム フォルダーに指定したメッセージを移動する`deleteditems`。</span><span class="sxs-lookup"><span data-stu-id="07363-142">The following request moves the specified message to the Deleted Items folder, identified by its well-known folder name `deleteditems`.</span></span>
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

##### <a name="response"></a><span data-ttu-id="07363-143">応答</span><span class="sxs-lookup"><span data-stu-id="07363-143">Response</span></span>

<span data-ttu-id="07363-144">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="07363-144">Here is an example of the response.</span></span>

> <span data-ttu-id="07363-145">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="07363-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="07363-146">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="07363-146">All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/message-move.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
