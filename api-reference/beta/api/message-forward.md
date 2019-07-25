---
title: 'メッセージ: forward'
description: 'メッセージを転送する、コメントを追加する、または更新可能なプロパティを変更する  '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: c2f229054ba8a6948aa948d82208581141a57d3b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879631"
---
# <a name="message-forward"></a><span data-ttu-id="32d41-103">メッセージ: forward</span><span class="sxs-lookup"><span data-stu-id="32d41-103">message: forward</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32d41-104">メッセージを転送する、コメントを追加する、または更新可能なプロパティを変更する</span><span class="sxs-lookup"><span data-stu-id="32d41-104">Forward a message, add a comment or modify any updateable properties</span></span>  
<span data-ttu-id="32d41-105">すべて1回の**転送**呼び出し。</span><span class="sxs-lookup"><span data-stu-id="32d41-105">all in one **forward** call.</span></span> <span data-ttu-id="32d41-106">メッセージは [送信済みアイテム] フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="32d41-106">The message is saved in the Sent Items folder.</span></span>

<span data-ttu-id="32d41-107">または、最初に[下書きの転送メッセージを作成して](../api/message-createforward.md)コメントを含めるか、メッセージのプロパティを更新し、転送メッセージを[送信](../api/message-send.md)します。</span><span class="sxs-lookup"><span data-stu-id="32d41-107">Alternatively, you can first [create a draft forward message](../api/message-createforward.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="32d41-108">**注**</span><span class="sxs-lookup"><span data-stu-id="32d41-108">**Note**</span></span>

- <span data-ttu-id="32d41-109">パラメーターには、comment または body プロパティのいずれかを指定できます。 \*\*\*\* `message`</span><span class="sxs-lookup"><span data-stu-id="32d41-109">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="32d41-110">両方を指定すると、「HTTP 400 要求が正しくありません」というエラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="32d41-110">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="32d41-111">パラメーターを指定するか`toRecipients` 、 `message`パラメーターの**トーラス**プロパティを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="32d41-111">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="32d41-112">両方を指定するか、どちらも指定しないと、「HTTP 400 要求が正しくありません」というエラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="32d41-112">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="32d41-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="32d41-113">Permissions</span></span>
<span data-ttu-id="32d41-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="32d41-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32d41-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="32d41-116">Permission type</span></span>      | <span data-ttu-id="32d41-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="32d41-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32d41-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="32d41-118">Delegated (work or school account)</span></span> | <span data-ttu-id="32d41-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="32d41-119">Mail.Send</span></span>    |
|<span data-ttu-id="32d41-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="32d41-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32d41-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="32d41-121">Mail.Send</span></span>    |
|<span data-ttu-id="32d41-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="32d41-122">Application</span></span> | <span data-ttu-id="32d41-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="32d41-123">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="32d41-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="32d41-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="32d41-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="32d41-125">Request headers</span></span>
| <span data-ttu-id="32d41-126">名前</span><span class="sxs-lookup"><span data-stu-id="32d41-126">Name</span></span>       | <span data-ttu-id="32d41-127">型</span><span class="sxs-lookup"><span data-stu-id="32d41-127">Type</span></span> | <span data-ttu-id="32d41-128">説明</span><span class="sxs-lookup"><span data-stu-id="32d41-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="32d41-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="32d41-129">Authorization</span></span>  | <span data-ttu-id="32d41-130">string</span><span class="sxs-lookup"><span data-stu-id="32d41-130">string</span></span>  | <span data-ttu-id="32d41-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="32d41-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="32d41-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="32d41-133">Content-Type</span></span> | <span data-ttu-id="32d41-134">string</span><span class="sxs-lookup"><span data-stu-id="32d41-134">string</span></span>  | <span data-ttu-id="32d41-p106">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="32d41-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="32d41-137">要求本文</span><span class="sxs-lookup"><span data-stu-id="32d41-137">Request body</span></span>
<span data-ttu-id="32d41-138">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="32d41-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="32d41-139">パラメーター</span><span class="sxs-lookup"><span data-stu-id="32d41-139">Parameter</span></span>    | <span data-ttu-id="32d41-140">型</span><span class="sxs-lookup"><span data-stu-id="32d41-140">Type</span></span>   |<span data-ttu-id="32d41-141">説明</span><span class="sxs-lookup"><span data-stu-id="32d41-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32d41-142">comment</span><span class="sxs-lookup"><span data-stu-id="32d41-142">comment</span></span>|<span data-ttu-id="32d41-143">String</span><span class="sxs-lookup"><span data-stu-id="32d41-143">String</span></span>|<span data-ttu-id="32d41-p107">含めるコメントです。空の文字列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="32d41-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="32d41-146">toRecipients</span><span class="sxs-lookup"><span data-stu-id="32d41-146">toRecipients</span></span>|<span data-ttu-id="32d41-147">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="32d41-147">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="32d41-148">受信者の一覧です。</span><span class="sxs-lookup"><span data-stu-id="32d41-148">The list of recipients.</span></span>|
|<span data-ttu-id="32d41-149">message</span><span class="sxs-lookup"><span data-stu-id="32d41-149">message</span></span>|[<span data-ttu-id="32d41-150">message</span><span class="sxs-lookup"><span data-stu-id="32d41-150">message</span></span>](../resources/message.md)|<span data-ttu-id="32d41-151">返信メッセージで更新する書き込み可能なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="32d41-151">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="32d41-152">応答</span><span class="sxs-lookup"><span data-stu-id="32d41-152">Response</span></span>

<span data-ttu-id="32d41-p108">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="32d41-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32d41-155">例</span><span class="sxs-lookup"><span data-stu-id="32d41-155">Example</span></span>
<span data-ttu-id="32d41-156">次の例では、 **isDeliveryReceiptRequested**プロパティを true に設定し、コメントを追加してメッセージを転送します。</span><span class="sxs-lookup"><span data-stu-id="32d41-156">The following example sets the **isDeliveryReceiptRequested** property to true, adds a comment and forwards the message.</span></span>
##### <a name="request"></a><span data-ttu-id="32d41-157">要求</span><span class="sxs-lookup"><span data-stu-id="32d41-157">Request</span></span>
<span data-ttu-id="32d41-158">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="32d41-158">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="32d41-159">プロトコル</span><span class="sxs-lookup"><span data-stu-id="32d41-159">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="32d41-160">C#</span><span class="sxs-lookup"><span data-stu-id="32d41-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-forward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="32d41-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="32d41-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-forward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="32d41-162">目的-C</span><span class="sxs-lookup"><span data-stu-id="32d41-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-forward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="32d41-163">Java</span><span class="sxs-lookup"><span data-stu-id="32d41-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-forward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="32d41-164">応答</span><span class="sxs-lookup"><span data-stu-id="32d41-164">Response</span></span>
<span data-ttu-id="32d41-165">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="32d41-165">Here is an example of the response.</span></span>
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
  "description": "message: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
