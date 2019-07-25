---
title: 'メッセージ: createReply'
description: 指定したメッセージに対する返信の下書きを作成します。 下書きを更新して**本文**に返信のコンテンツを追加したり、その他のメッセージのプロパティを変更したりすることも、下書きをそのまま送信することもできます。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 409ca69cc1664cf486748ad0c39d888086e54a33
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889748"
---
# <a name="message-createreply"></a><span data-ttu-id="adf65-104">メッセージ: createReply</span><span class="sxs-lookup"><span data-stu-id="adf65-104">message: createReply</span></span>

<span data-ttu-id="adf65-105">指定した[メッセージ](../resources/message.md)に対する返信の下書きを作成します。</span><span class="sxs-lookup"><span data-stu-id="adf65-105">Create a draft of the reply to the specified [message](../resources/message.md).</span></span> <span data-ttu-id="adf65-106">下書きを[更新](../api/message-update.md)して**本文**に返信のコンテンツを追加したり、その他のメッセージのプロパティを変更したりすることも、下書きをそのまま[送信](../api/message-send.md)することもできます。</span><span class="sxs-lookup"><span data-stu-id="adf65-106">You can then [update](../api/message-update.md) the draft to add reply content to the **body** or change other message properties, or, simply [send](../api/message-send.md) the draft.</span></span>

## <a name="permissions"></a><span data-ttu-id="adf65-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="adf65-107">Permissions</span></span>
<span data-ttu-id="adf65-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="adf65-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="adf65-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="adf65-110">Permission type</span></span>      | <span data-ttu-id="adf65-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="adf65-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="adf65-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="adf65-112">Delegated (work or school account)</span></span> | <span data-ttu-id="adf65-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="adf65-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="adf65-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="adf65-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="adf65-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="adf65-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="adf65-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="adf65-116">Application</span></span> | <span data-ttu-id="adf65-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="adf65-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="adf65-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="adf65-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReply
POST /users/{id | userPrincipalName}/messages/{id}/createReply
POST /me/mailFolders/{id}/messages/{id}/createReply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReply
```
## <a name="request-headers"></a><span data-ttu-id="adf65-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="adf65-119">Request headers</span></span>
| <span data-ttu-id="adf65-120">名前</span><span class="sxs-lookup"><span data-stu-id="adf65-120">Name</span></span>       | <span data-ttu-id="adf65-121">型</span><span class="sxs-lookup"><span data-stu-id="adf65-121">Type</span></span> | <span data-ttu-id="adf65-122">説明</span><span class="sxs-lookup"><span data-stu-id="adf65-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="adf65-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="adf65-123">Authorization</span></span>  | <span data-ttu-id="adf65-124">string</span><span class="sxs-lookup"><span data-stu-id="adf65-124">string</span></span>  | <span data-ttu-id="adf65-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="adf65-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="adf65-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="adf65-127">Request body</span></span>
<span data-ttu-id="adf65-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="adf65-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="adf65-129">応答</span><span class="sxs-lookup"><span data-stu-id="adf65-129">Response</span></span>

<span data-ttu-id="adf65-130">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [Message](../resources/message.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="adf65-130">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="adf65-131">例</span><span class="sxs-lookup"><span data-stu-id="adf65-131">Example</span></span>
<span data-ttu-id="adf65-132">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="adf65-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="adf65-133">要求</span><span class="sxs-lookup"><span data-stu-id="adf65-133">Request</span></span>
<span data-ttu-id="adf65-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="adf65-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="adf65-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="adf65-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_createreply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/createReply
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="adf65-136">C#</span><span class="sxs-lookup"><span data-stu-id="adf65-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createreply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="adf65-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="adf65-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createreply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="adf65-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="adf65-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createreply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="adf65-139">Java</span><span class="sxs-lookup"><span data-stu-id="adf65-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-createreply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="adf65-140">応答</span><span class="sxs-lookup"><span data-stu-id="adf65-140">Response</span></span>
<span data-ttu-id="adf65-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="adf65-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
