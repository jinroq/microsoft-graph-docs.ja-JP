---
title: 'メッセージ: createReplyAll'
description: 指定したメッセージの差出人とすべの受信者に対して返信するための下書きを作成します。 **本文**への返信の内容を追加またはその他のメッセージのプロパティを変更するのには下書きを更新したり、単に下書きを送信できます。
localization_priority: Normal
ms.openlocfilehash: d09de032dc515173219a00b19a64d64ba0b72195
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804782"
---
# <a name="message-createreplyall"></a><span data-ttu-id="f2497-104">メッセージ: createReplyAll</span><span class="sxs-lookup"><span data-stu-id="f2497-104">message: createReplyAll</span></span>

<span data-ttu-id="f2497-105">指定した[メッセージ](../resources/message.md)の差出人とすべの受信者に対して返信するための下書きを作成します。</span><span class="sxs-lookup"><span data-stu-id="f2497-105">Create a draft to reply to the sender and all the recipients of the specified [message](../resources/message.md).</span></span> <span data-ttu-id="f2497-106">下書きを[更新](../api/message-update.md)して**本文**に返信のコンテンツを追加したり、その他のメッセージのプロパティを変更したりすることも、下書きをそのまま[送信](../api/message-send.md)することもできます。</span><span class="sxs-lookup"><span data-stu-id="f2497-106">You can then [update](../api/message-update.md) the draft to add reply content to the **body** or change other message properties, or, simply [send](../api/message-send.md) the draft.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2497-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f2497-107">Permissions</span></span>
<span data-ttu-id="f2497-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f2497-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2497-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f2497-110">Permission type</span></span>      | <span data-ttu-id="f2497-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f2497-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2497-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f2497-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f2497-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2497-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f2497-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f2497-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2497-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2497-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f2497-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f2497-116">Application</span></span> | <span data-ttu-id="f2497-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2497-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2497-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f2497-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/messages/{id}/createReplyAll
POST /me/mailFolders/{id}/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReplyAll
```
## <a name="request-headers"></a><span data-ttu-id="f2497-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f2497-119">Request headers</span></span>
| <span data-ttu-id="f2497-120">名前</span><span class="sxs-lookup"><span data-stu-id="f2497-120">Name</span></span>       | <span data-ttu-id="f2497-121">種類</span><span class="sxs-lookup"><span data-stu-id="f2497-121">Type</span></span> | <span data-ttu-id="f2497-122">説明</span><span class="sxs-lookup"><span data-stu-id="f2497-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f2497-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2497-123">Authorization</span></span>  | <span data-ttu-id="f2497-124">string</span><span class="sxs-lookup"><span data-stu-id="f2497-124">string</span></span>  | <span data-ttu-id="f2497-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f2497-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2497-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f2497-127">Request body</span></span>
<span data-ttu-id="f2497-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f2497-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2497-129">応答</span><span class="sxs-lookup"><span data-stu-id="f2497-129">Response</span></span>

<span data-ttu-id="f2497-130">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [Message](../resources/message.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f2497-130">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2497-131">例</span><span class="sxs-lookup"><span data-stu-id="f2497-131">Example</span></span>
<span data-ttu-id="f2497-132">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="f2497-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f2497-133">要求</span><span class="sxs-lookup"><span data-stu-id="f2497-133">Request</span></span>
<span data-ttu-id="f2497-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f2497-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_createreplyall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/createReplyAll
```

##### <a name="response"></a><span data-ttu-id="f2497-135">応答</span><span class="sxs-lookup"><span data-stu-id="f2497-135">Response</span></span>
<span data-ttu-id="f2497-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f2497-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: createReplyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
