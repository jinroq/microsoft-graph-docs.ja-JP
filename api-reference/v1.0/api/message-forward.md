---
title: 'メッセージ: forward'
description: メッセージを転送します。メッセージは [送信済みアイテム] フォルダーに保存されます。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 12409685e21b338a86b392f32449b006a0e958f7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960547"
---
# <a name="message-forward"></a><span data-ttu-id="fe981-104">メッセージ: forward</span><span class="sxs-lookup"><span data-stu-id="fe981-104">message: forward</span></span>

<span data-ttu-id="fe981-p102">メッセージを転送します。メッセージは [送信済みアイテム] フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="fe981-p102">Forward a message. The message is saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe981-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fe981-107">Permissions</span></span>
<span data-ttu-id="fe981-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fe981-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe981-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fe981-110">Permission type</span></span>      | <span data-ttu-id="fe981-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fe981-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe981-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fe981-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fe981-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="fe981-113">Mail.Send</span></span>    |
|<span data-ttu-id="fe981-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fe981-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe981-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="fe981-115">Mail.Send</span></span>    |
|<span data-ttu-id="fe981-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fe981-116">Application</span></span> | <span data-ttu-id="fe981-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="fe981-117">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe981-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fe981-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="fe981-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fe981-119">Request headers</span></span>
| <span data-ttu-id="fe981-120">名前</span><span class="sxs-lookup"><span data-stu-id="fe981-120">Name</span></span>       | <span data-ttu-id="fe981-121">種類</span><span class="sxs-lookup"><span data-stu-id="fe981-121">Type</span></span> | <span data-ttu-id="fe981-122">説明</span><span class="sxs-lookup"><span data-stu-id="fe981-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fe981-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe981-123">Authorization</span></span>  | <span data-ttu-id="fe981-124">string</span><span class="sxs-lookup"><span data-stu-id="fe981-124">string</span></span>  | <span data-ttu-id="fe981-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fe981-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fe981-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fe981-127">Content-Type</span></span> | <span data-ttu-id="fe981-128">string</span><span class="sxs-lookup"><span data-stu-id="fe981-128">string</span></span>  | <span data-ttu-id="fe981-p105">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="fe981-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe981-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="fe981-131">Request body</span></span>
<span data-ttu-id="fe981-132">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="fe981-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fe981-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="fe981-133">Parameter</span></span>    | <span data-ttu-id="fe981-134">Type</span><span class="sxs-lookup"><span data-stu-id="fe981-134">Type</span></span>   |<span data-ttu-id="fe981-135">説明</span><span class="sxs-lookup"><span data-stu-id="fe981-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe981-136">comment</span><span class="sxs-lookup"><span data-stu-id="fe981-136">comment</span></span>|<span data-ttu-id="fe981-137">String</span><span class="sxs-lookup"><span data-stu-id="fe981-137">String</span></span>|<span data-ttu-id="fe981-p106">含めるコメントです。空の文字列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="fe981-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="fe981-140">toRecipients</span><span class="sxs-lookup"><span data-stu-id="fe981-140">toRecipients</span></span>|<span data-ttu-id="fe981-141">[Recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="fe981-141">[Recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="fe981-142">受信者の一覧です。</span><span class="sxs-lookup"><span data-stu-id="fe981-142">The list of recipients.</span></span>|

## <a name="response"></a><span data-ttu-id="fe981-143">応答</span><span class="sxs-lookup"><span data-stu-id="fe981-143">Response</span></span>

<span data-ttu-id="fe981-p107">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="fe981-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe981-146">例</span><span class="sxs-lookup"><span data-stu-id="fe981-146">Example</span></span>
<span data-ttu-id="fe981-147">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="fe981-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fe981-148">要求</span><span class="sxs-lookup"><span data-stu-id="fe981-148">Request</span></span>
<span data-ttu-id="fe981-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fe981-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/forward
Content-type: application/json
Content-length: 166

{
  "comment": "comment-value",
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="fe981-150">応答</span><span class="sxs-lookup"><span data-stu-id="fe981-150">Response</span></span>
##### <a name="response"></a><span data-ttu-id="fe981-151">応答</span><span class="sxs-lookup"><span data-stu-id="fe981-151">Response</span></span>
<span data-ttu-id="fe981-152">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="fe981-152">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
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
