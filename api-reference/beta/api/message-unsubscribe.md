---
title: 'メッセージ: 購読の取り消し'
description: サイン インユーザーに代わって電子メール要求を送信し、電子メール配布リストから登録を解除します。`List-Unsubscribe` ヘッダー内の情報を使用します。
ms.openlocfilehash: b4f72a0b629fb59074acbbd58f09a3c16118cc8c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070701"
---
# <a name="message-unsubscribe"></a><span data-ttu-id="c3849-104">メッセージ: 購読の取り消し</span><span class="sxs-lookup"><span data-stu-id="c3849-104">message: unsubscribe</span></span>

> <span data-ttu-id="c3849-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c3849-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c3849-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3849-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c3849-p103">サイン インユーザーに代わって電子メール要求を送信し、電子メール配布リストから登録を解除します。`List-Unsubscribe` ヘッダー内の情報を使用します。</span><span class="sxs-lookup"><span data-stu-id="c3849-p103">Submits a email request on behalf of the signed-in user to unsubscribe from an email distribution list. Uses the information in the `List-Unsubscribe` header.</span></span>

<span data-ttu-id="c3849-109">メッセージの送信者使用できますメーリング リスト ユーザー フレンドリな方法で受信者のオプションを含めることによって脱退します。ように指定することにより、`List-Unsubscribe`次の[RFC 2369](https://www.faqs.org/rfcs/rfc2369.html)各メッセージのメッセージ ヘッダー。</span><span class="sxs-lookup"><span data-stu-id="c3849-109">Message senders can use mailing lists in a user-friendly way by including an option for recipients to opt out. They can do so by specifying the `List-Unsubscribe` header in each message following [RFC-2369](https://www.faqs.org/rfcs/rfc2369.html).</span></span>

<span data-ttu-id="c3849-110">**メモ**具体的には、**購読の取り消し**操作をするため動作、送信者を指定してください`mailto:`し、URL ベースではない情報の購読を解除します。</span><span class="sxs-lookup"><span data-stu-id="c3849-110">**Note** In particular, for the **unsubscribe** action to work, the sender must specify `mailto:` and not URL-based unsubscribe information.</span></span>

<span data-ttu-id="c3849-111">そのヘッダーを設定する[メッセージ](../resources/message.md)のインスタンスの**unsubscribeEnabled**プロパティを設定します`true`、 **unsubscribeData**プロパティは、ヘッダーのデータをします。</span><span class="sxs-lookup"><span data-stu-id="c3849-111">Setting that header would also set the **unsubscribeEnabled** property of the [message](../resources/message.md) instance to `true`, and the **unsubscribeData** property to the header data.</span></span>

<span data-ttu-id="c3849-112">かどうか、メッセージの**unsubscribeEnabled**プロパティは、 `true`、メッセージの送信者によって管理のようなメッセージからユーザーの購読を解除する**購読を解除**アクションを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="c3849-112">If the **unsubscribeEnabled** property of a message is `true`, you can use the **unsubscribe** action to unsubscribe the user from similar future messages as managed by the message sender.</span></span>

<span data-ttu-id="c3849-113">成功を**登録解除**の操作は、メッセージを**削除済みアイテム**フォルダーに移動します。</span><span class="sxs-lookup"><span data-stu-id="c3849-113">A successful **unsubscribe** action moves the message to the **Deleted Items** folder.</span></span> <span data-ttu-id="c3849-114">将来のメールの配信から、ユーザーの実際の除外は、送信者によって管理されます。</span><span class="sxs-lookup"><span data-stu-id="c3849-114">The actual exclusion of the user from future mail distribution is managed by the sender.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3849-115">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c3849-115">Permissions</span></span>
<span data-ttu-id="c3849-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c3849-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3849-118">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c3849-118">Permission type</span></span>      | <span data-ttu-id="c3849-119">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c3849-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3849-120">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c3849-120">Delegated (work or school account)</span></span> | <span data-ttu-id="c3849-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="c3849-121">Mail.Send</span></span>    |
|<span data-ttu-id="c3849-122">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c3849-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3849-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="c3849-123">Mail.Send</span></span>    |
|<span data-ttu-id="c3849-124">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c3849-124">Application</span></span> | <span data-ttu-id="c3849-125">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="c3849-125">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3849-126">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c3849-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/messages/{id}/unsubscribe
```
## <a name="request-headers"></a><span data-ttu-id="c3849-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c3849-127">Request headers</span></span>
| <span data-ttu-id="c3849-128">名前</span><span class="sxs-lookup"><span data-stu-id="c3849-128">Name</span></span>       | <span data-ttu-id="c3849-129">型</span><span class="sxs-lookup"><span data-stu-id="c3849-129">Type</span></span> | <span data-ttu-id="c3849-130">説明</span><span class="sxs-lookup"><span data-stu-id="c3849-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c3849-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3849-131">Authorization</span></span>  | <span data-ttu-id="c3849-132">string</span><span class="sxs-lookup"><span data-stu-id="c3849-132">string</span></span>  | <span data-ttu-id="c3849-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c3849-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c3849-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="c3849-135">Request body</span></span>
<span data-ttu-id="c3849-136">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c3849-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3849-137">応答</span><span class="sxs-lookup"><span data-stu-id="c3849-137">Response</span></span>

<span data-ttu-id="c3849-p107">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="c3849-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3849-140">例</span><span class="sxs-lookup"><span data-stu-id="c3849-140">Example</span></span>
<span data-ttu-id="c3849-141">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="c3849-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c3849-142">要求</span><span class="sxs-lookup"><span data-stu-id="c3849-142">Request</span></span>
<span data-ttu-id="c3849-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c3849-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_unsubscribe"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/{id}/unsubscribe
```

##### <a name="response"></a><span data-ttu-id="c3849-144">応答</span><span class="sxs-lookup"><span data-stu-id="c3849-144">Response</span></span>
<span data-ttu-id="c3849-145">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="c3849-145">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: unsubscribe",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
