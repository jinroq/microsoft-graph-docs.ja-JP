---
title: 'メッセージ: replyAll'
description: メッセージの受信者すべてに返信します。その後、メッセージは送信済みアイテム フォルダーに保存されます。
ms.openlocfilehash: ce6ee75912834b14b4a3b5e1d3b03b929f209dfa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022914"
---
# <a name="message-replyall"></a><span data-ttu-id="fa943-104">メッセージ: replyAll</span><span class="sxs-lookup"><span data-stu-id="fa943-104">message: replyAll</span></span>

<span data-ttu-id="fa943-p102">メッセージの受信者すべてに返信します。その後、メッセージは送信済みアイテム フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="fa943-p102">Reply to all recipients of a message. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa943-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fa943-107">Permissions</span></span>
<span data-ttu-id="fa943-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fa943-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa943-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fa943-110">Permission type</span></span>      | <span data-ttu-id="fa943-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fa943-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa943-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fa943-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fa943-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="fa943-113">Mail.Send</span></span>    |
|<span data-ttu-id="fa943-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fa943-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa943-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="fa943-115">Mail.Send</span></span>    |
|<span data-ttu-id="fa943-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fa943-116">Application</span></span> | <span data-ttu-id="fa943-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="fa943-117">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa943-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fa943-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="fa943-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fa943-119">Request headers</span></span>
| <span data-ttu-id="fa943-120">名前</span><span class="sxs-lookup"><span data-stu-id="fa943-120">Name</span></span>       | <span data-ttu-id="fa943-121">型</span><span class="sxs-lookup"><span data-stu-id="fa943-121">Type</span></span> | <span data-ttu-id="fa943-122">説明</span><span class="sxs-lookup"><span data-stu-id="fa943-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fa943-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa943-123">Authorization</span></span>  | <span data-ttu-id="fa943-124">string</span><span class="sxs-lookup"><span data-stu-id="fa943-124">string</span></span>  | <span data-ttu-id="fa943-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fa943-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fa943-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fa943-127">Content-Type</span></span> | <span data-ttu-id="fa943-128">string</span><span class="sxs-lookup"><span data-stu-id="fa943-128">string</span></span>  | <span data-ttu-id="fa943-p105">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="fa943-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa943-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="fa943-131">Request body</span></span>
<span data-ttu-id="fa943-132">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="fa943-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fa943-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="fa943-133">Parameter</span></span>    | <span data-ttu-id="fa943-134">型</span><span class="sxs-lookup"><span data-stu-id="fa943-134">Type</span></span>   |<span data-ttu-id="fa943-135">説明</span><span class="sxs-lookup"><span data-stu-id="fa943-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa943-136">comment</span><span class="sxs-lookup"><span data-stu-id="fa943-136">comment</span></span>|<span data-ttu-id="fa943-137">String</span><span class="sxs-lookup"><span data-stu-id="fa943-137">String</span></span>|<span data-ttu-id="fa943-p106">含めるコメントです。空の文字列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="fa943-p106">A comment to include. Can be an empty string.</span></span>|

## <a name="response"></a><span data-ttu-id="fa943-140">応答</span><span class="sxs-lookup"><span data-stu-id="fa943-140">Response</span></span>

<span data-ttu-id="fa943-p107">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="fa943-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa943-143">例</span><span class="sxs-lookup"><span data-stu-id="fa943-143">Example</span></span>
<span data-ttu-id="fa943-144">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="fa943-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fa943-145">要求</span><span class="sxs-lookup"><span data-stu-id="fa943-145">Request</span></span>
<span data-ttu-id="fa943-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fa943-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_replyall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/replyAll
Content-type: application/json
Content-length: 32

{
  "comment": "comment-value"
}
```


##### <a name="response"></a><span data-ttu-id="fa943-147">応答</span><span class="sxs-lookup"><span data-stu-id="fa943-147">Response</span></span>
<span data-ttu-id="fa943-148">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="fa943-148">Here is an example of the response.</span></span>
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
  "description": "message: replyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
