---
title: 'メッセージ: replyAll'
description: メッセージの受信者すべてに返信します。その後、メッセージは送信済みアイテム フォルダーに保存されます。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a5a285becea0fd351011e8d74cfbcb5d70fd2e84
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36022860"
---
# <a name="message-replyall"></a><span data-ttu-id="1e948-104">メッセージ: replyAll</span><span class="sxs-lookup"><span data-stu-id="1e948-104">message: replyAll</span></span>

<span data-ttu-id="1e948-p102">メッセージの受信者すべてに返信します。その後、メッセージは送信済みアイテム フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="1e948-p102">Reply to all recipients of a message. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e948-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1e948-107">Permissions</span></span>
<span data-ttu-id="1e948-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1e948-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e948-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1e948-110">Permission type</span></span>      | <span data-ttu-id="1e948-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1e948-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e948-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1e948-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1e948-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="1e948-113">Mail.Send</span></span>    |
|<span data-ttu-id="1e948-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1e948-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e948-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="1e948-115">Mail.Send</span></span>    |
|<span data-ttu-id="1e948-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1e948-116">Application</span></span> | <span data-ttu-id="1e948-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="1e948-117">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e948-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1e948-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="1e948-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1e948-119">Request headers</span></span>
| <span data-ttu-id="1e948-120">名前</span><span class="sxs-lookup"><span data-stu-id="1e948-120">Name</span></span>       | <span data-ttu-id="1e948-121">型</span><span class="sxs-lookup"><span data-stu-id="1e948-121">Type</span></span> | <span data-ttu-id="1e948-122">説明</span><span class="sxs-lookup"><span data-stu-id="1e948-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1e948-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e948-123">Authorization</span></span>  | <span data-ttu-id="1e948-124">string</span><span class="sxs-lookup"><span data-stu-id="1e948-124">string</span></span>  | <span data-ttu-id="1e948-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1e948-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1e948-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1e948-127">Content-Type</span></span> | <span data-ttu-id="1e948-128">string</span><span class="sxs-lookup"><span data-stu-id="1e948-128">string</span></span>  | <span data-ttu-id="1e948-p105">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="1e948-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e948-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="1e948-131">Request body</span></span>
<span data-ttu-id="1e948-132">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="1e948-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1e948-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="1e948-133">Parameter</span></span>    | <span data-ttu-id="1e948-134">型</span><span class="sxs-lookup"><span data-stu-id="1e948-134">Type</span></span>   |<span data-ttu-id="1e948-135">説明</span><span class="sxs-lookup"><span data-stu-id="1e948-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e948-136">comment</span><span class="sxs-lookup"><span data-stu-id="1e948-136">comment</span></span>|<span data-ttu-id="1e948-137">String</span><span class="sxs-lookup"><span data-stu-id="1e948-137">String</span></span>|<span data-ttu-id="1e948-p106">含めるコメントです。空の文字列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="1e948-p106">A comment to include. Can be an empty string.</span></span>|

## <a name="response"></a><span data-ttu-id="1e948-140">応答</span><span class="sxs-lookup"><span data-stu-id="1e948-140">Response</span></span>

<span data-ttu-id="1e948-p107">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="1e948-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e948-143">例</span><span class="sxs-lookup"><span data-stu-id="1e948-143">Example</span></span>
<span data-ttu-id="1e948-144">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="1e948-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1e948-145">要求</span><span class="sxs-lookup"><span data-stu-id="1e948-145">Request</span></span>
<span data-ttu-id="1e948-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1e948-146">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1e948-147">プロトコル</span><span class="sxs-lookup"><span data-stu-id="1e948-147">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="1e948-148">C#</span><span class="sxs-lookup"><span data-stu-id="1e948-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-replyall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1e948-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="1e948-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-replyall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1e948-150">目的-C</span><span class="sxs-lookup"><span data-stu-id="1e948-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-replyall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1e948-151">Java</span><span class="sxs-lookup"><span data-stu-id="1e948-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-replyall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a><span data-ttu-id="1e948-152">応答</span><span class="sxs-lookup"><span data-stu-id="1e948-152">Response</span></span>
<span data-ttu-id="1e948-153">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="1e948-153">Here is an example of the response.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
