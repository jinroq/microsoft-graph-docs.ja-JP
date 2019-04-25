---
title: 'メッセージ: 購読取り消し'
description: サイン インユーザーに代わって電子メール要求を送信し、電子メール配布リストから登録を解除します。 `List-Unsubscribe` ヘッダー内の情報を使用します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 69d14315fc0732ed12db357f9aa9a0c837f48f29
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32540369"
---
# <a name="message-unsubscribe"></a><span data-ttu-id="addc2-104">メッセージ: 購読取り消し</span><span class="sxs-lookup"><span data-stu-id="addc2-104">message: unsubscribe</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="addc2-p102">サイン インユーザーに代わって電子メール要求を送信し、電子メール配布リストから登録を解除します。 `List-Unsubscribe` ヘッダー内の情報を使用します。</span><span class="sxs-lookup"><span data-stu-id="addc2-p102">Submits a email request on behalf of the signed-in user to unsubscribe from an email distribution list. Uses the information in the `List-Unsubscribe` header.</span></span>

<span data-ttu-id="addc2-107">メッセージの送信者は、受信者がオプトアウトするオプションを指定することにより、ユーザーフレンドリな方法でメーリングリストを使用できます。これを行うには、 `List-Unsubscribe` [RFC-2369](https://www.faqs.org/rfcs/rfc2369.html)の後に各メッセージのヘッダーを指定します。</span><span class="sxs-lookup"><span data-stu-id="addc2-107">Message senders can use mailing lists in a user-friendly way by including an option for recipients to opt out. They can do so by specifying the `List-Unsubscribe` header in each message following [RFC-2369](https://www.faqs.org/rfcs/rfc2369.html).</span></span>

<span data-ttu-id="addc2-108">**メモ**特に、登録**解除**アクションが機能するには、送信者`mailto:`が URL ベースの登録解除情報ではなく、を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="addc2-108">**Note** In particular, for the **unsubscribe** action to work, the sender must specify `mailto:` and not URL-based unsubscribe information.</span></span>

<span data-ttu-id="addc2-109">また、そのヘッダーを設定すると、[メッセージ](../resources/message.md)インスタンスの**unsubscribeEnabled**プロパティ`true`がに設定され、 **unsubscribeData**プロパティがヘッダーデータに設定されます。</span><span class="sxs-lookup"><span data-stu-id="addc2-109">Setting that header would also set the **unsubscribeEnabled** property of the [message](../resources/message.md) instance to `true`, and the **unsubscribeData** property to the header data.</span></span>

<span data-ttu-id="addc2-110">メッセージの**unsubscribeEnabled**プロパティがの場合は`true`、**購読取り消し**アクションを使用して、メッセージ送信者によって管理されているような、同様の今後のメッセージからユーザーを登録解除することができます。</span><span class="sxs-lookup"><span data-stu-id="addc2-110">If the **unsubscribeEnabled** property of a message is `true`, you can use the **unsubscribe** action to unsubscribe the user from similar future messages as managed by the message sender.</span></span>

<span data-ttu-id="addc2-111">登録**解除**が正常に完了すると、メッセージは [**削除済みアイテム**] フォルダーに移動されます。</span><span class="sxs-lookup"><span data-stu-id="addc2-111">A successful **unsubscribe** action moves the message to the **Deleted Items** folder.</span></span> <span data-ttu-id="addc2-112">将来のメール配布からのユーザーの実際の除外は、送信者によって管理されます。</span><span class="sxs-lookup"><span data-stu-id="addc2-112">The actual exclusion of the user from future mail distribution is managed by the sender.</span></span>

## <a name="permissions"></a><span data-ttu-id="addc2-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="addc2-113">Permissions</span></span>
<span data-ttu-id="addc2-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="addc2-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="addc2-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="addc2-116">Permission type</span></span>      | <span data-ttu-id="addc2-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="addc2-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="addc2-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="addc2-118">Delegated (work or school account)</span></span> | <span data-ttu-id="addc2-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="addc2-119">Mail.Send</span></span>    |
|<span data-ttu-id="addc2-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="addc2-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="addc2-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="addc2-121">Mail.Send</span></span>    |
|<span data-ttu-id="addc2-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="addc2-122">Application</span></span> | <span data-ttu-id="addc2-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="addc2-123">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="addc2-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="addc2-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/messages/{id}/unsubscribe
```
## <a name="request-headers"></a><span data-ttu-id="addc2-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="addc2-125">Request headers</span></span>
| <span data-ttu-id="addc2-126">名前</span><span class="sxs-lookup"><span data-stu-id="addc2-126">Name</span></span>       | <span data-ttu-id="addc2-127">型</span><span class="sxs-lookup"><span data-stu-id="addc2-127">Type</span></span> | <span data-ttu-id="addc2-128">説明</span><span class="sxs-lookup"><span data-stu-id="addc2-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="addc2-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="addc2-129">Authorization</span></span>  | <span data-ttu-id="addc2-130">string</span><span class="sxs-lookup"><span data-stu-id="addc2-130">string</span></span>  | <span data-ttu-id="addc2-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="addc2-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="addc2-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="addc2-133">Request body</span></span>
<span data-ttu-id="addc2-134">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="addc2-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="addc2-135">応答</span><span class="sxs-lookup"><span data-stu-id="addc2-135">Response</span></span>

<span data-ttu-id="addc2-p106">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="addc2-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="addc2-138">例</span><span class="sxs-lookup"><span data-stu-id="addc2-138">Example</span></span>
<span data-ttu-id="addc2-139">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="addc2-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="addc2-140">要求</span><span class="sxs-lookup"><span data-stu-id="addc2-140">Request</span></span>
<span data-ttu-id="addc2-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="addc2-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_unsubscribe"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/{id}/unsubscribe
```

##### <a name="response"></a><span data-ttu-id="addc2-142">応答</span><span class="sxs-lookup"><span data-stu-id="addc2-142">Response</span></span>
<span data-ttu-id="addc2-143">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="addc2-143">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: unsubscribe",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-unsubscribe.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
