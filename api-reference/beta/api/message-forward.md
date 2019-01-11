---
title: 'メッセージ: forward'
description: 'メッセージを転送する、コメントを追加または更新可能なプロパティを変更します。  '
localization_priority: Normal
ms.openlocfilehash: b601ea1152e9f5b0c5796779967393b956fd2da0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864681"
---
# <a name="message-forward"></a><span data-ttu-id="24c96-103">メッセージ: forward</span><span class="sxs-lookup"><span data-stu-id="24c96-103">message: forward</span></span>

> <span data-ttu-id="24c96-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="24c96-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="24c96-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24c96-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="24c96-106">メッセージを転送する、コメントを追加または更新可能なプロパティを変更します。</span><span class="sxs-lookup"><span data-stu-id="24c96-106">Forward a message, add a comment or modify any updateable properties</span></span>  
<span data-ttu-id="24c96-107">1 つ**前方**にすべてを呼び出します。</span><span class="sxs-lookup"><span data-stu-id="24c96-107">all in one **forward** call.</span></span> <span data-ttu-id="24c96-108">メッセージは、送信済みアイテム フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="24c96-108">The message is saved in the Sent Items folder.</span></span>

<span data-ttu-id="24c96-109">または、最初に[下書きの転送メッセージを作成して](../api/message-createforward.md)コメントを含めるか、メッセージのプロパティを更新し、転送メッセージを[送信](../api/message-send.md)します。</span><span class="sxs-lookup"><span data-stu-id="24c96-109">Alternatively, you can first [create a draft forward message](../api/message-createforward.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="24c96-110">**注**</span><span class="sxs-lookup"><span data-stu-id="24c96-110">**Note**</span></span>

- <span data-ttu-id="24c96-111">**Body**プロパティまたはコメントのいずれかを指定することができます、`message`のパラメーターです。</span><span class="sxs-lookup"><span data-stu-id="24c96-111">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="24c96-112">両方を指定すると、「HTTP 400 要求が正しくありません」というエラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="24c96-112">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="24c96-113">どちらかを指定する必要があります、`toRecipients`の**toRecipients**プロパティは、パラメーター、または、`message`パラメーター。</span><span class="sxs-lookup"><span data-stu-id="24c96-113">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="24c96-114">両方を指定するか、どちらも指定しないと、「HTTP 400 要求が正しくありません」というエラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="24c96-114">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="24c96-115">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="24c96-115">Permissions</span></span>
<span data-ttu-id="24c96-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="24c96-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24c96-118">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="24c96-118">Permission type</span></span>      | <span data-ttu-id="24c96-119">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="24c96-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24c96-120">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="24c96-120">Delegated (work or school account)</span></span> | <span data-ttu-id="24c96-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="24c96-121">Mail.Send</span></span>    |
|<span data-ttu-id="24c96-122">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="24c96-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24c96-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="24c96-123">Mail.Send</span></span>    |
|<span data-ttu-id="24c96-124">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="24c96-124">Application</span></span> | <span data-ttu-id="24c96-125">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="24c96-125">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="24c96-126">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="24c96-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="24c96-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="24c96-127">Request headers</span></span>
| <span data-ttu-id="24c96-128">名前</span><span class="sxs-lookup"><span data-stu-id="24c96-128">Name</span></span>       | <span data-ttu-id="24c96-129">種類</span><span class="sxs-lookup"><span data-stu-id="24c96-129">Type</span></span> | <span data-ttu-id="24c96-130">説明</span><span class="sxs-lookup"><span data-stu-id="24c96-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="24c96-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="24c96-131">Authorization</span></span>  | <span data-ttu-id="24c96-132">string</span><span class="sxs-lookup"><span data-stu-id="24c96-132">string</span></span>  | <span data-ttu-id="24c96-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="24c96-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="24c96-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="24c96-135">Content-Type</span></span> | <span data-ttu-id="24c96-136">string</span><span class="sxs-lookup"><span data-stu-id="24c96-136">string</span></span>  | <span data-ttu-id="24c96-p107">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="24c96-p107">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="24c96-139">要求本文</span><span class="sxs-lookup"><span data-stu-id="24c96-139">Request body</span></span>
<span data-ttu-id="24c96-140">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="24c96-140">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="24c96-141">パラメーター</span><span class="sxs-lookup"><span data-stu-id="24c96-141">Parameter</span></span>    | <span data-ttu-id="24c96-142">Type</span><span class="sxs-lookup"><span data-stu-id="24c96-142">Type</span></span>   |<span data-ttu-id="24c96-143">説明</span><span class="sxs-lookup"><span data-stu-id="24c96-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="24c96-144">comment</span><span class="sxs-lookup"><span data-stu-id="24c96-144">comment</span></span>|<span data-ttu-id="24c96-145">String</span><span class="sxs-lookup"><span data-stu-id="24c96-145">String</span></span>|<span data-ttu-id="24c96-p108">含めるコメントです。空の文字列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="24c96-p108">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="24c96-148">toRecipients</span><span class="sxs-lookup"><span data-stu-id="24c96-148">toRecipients</span></span>|<span data-ttu-id="24c96-149">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="24c96-149">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="24c96-150">受信者の一覧です。</span><span class="sxs-lookup"><span data-stu-id="24c96-150">The list of recipients.</span></span>|
|<span data-ttu-id="24c96-151">message</span><span class="sxs-lookup"><span data-stu-id="24c96-151">message</span></span>|[<span data-ttu-id="24c96-152">message</span><span class="sxs-lookup"><span data-stu-id="24c96-152">message</span></span>](../resources/message.md)|<span data-ttu-id="24c96-153">返信メッセージで更新する書き込み可能なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="24c96-153">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="24c96-154">応答</span><span class="sxs-lookup"><span data-stu-id="24c96-154">Response</span></span>

<span data-ttu-id="24c96-p109">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="24c96-p109">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24c96-157">例</span><span class="sxs-lookup"><span data-stu-id="24c96-157">Example</span></span>
<span data-ttu-id="24c96-158">次の使用例は、 **isDeliveryReceiptRequested**プロパティを true に設定、コメントを追加し、メッセージを転送します。</span><span class="sxs-lookup"><span data-stu-id="24c96-158">The following example sets the **isDeliveryReceiptRequested** property to true, adds a comment and forwards the message.</span></span>
##### <a name="request"></a><span data-ttu-id="24c96-159">要求</span><span class="sxs-lookup"><span data-stu-id="24c96-159">Request</span></span>
<span data-ttu-id="24c96-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="24c96-160">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_forward"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaLAAA=/forward
Content-Type: application/json

{
  "message":{  
    "isDeliveryReceiptRequested": true,
    "toRecipients":[
      {
        "emailAddress": {
          "address":"danas@contoso.onmicrosoft.com",
          "name":"Dana Swope"
        }
      }
     ]
  },
  "comment": "Dana, just want to make sure you get this." 
}
```

##### <a name="response"></a><span data-ttu-id="24c96-161">応答</span><span class="sxs-lookup"><span data-stu-id="24c96-161">Response</span></span>
<span data-ttu-id="24c96-162">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="24c96-162">Here is an example of the response.</span></span>
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
  "description": "message: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
