---
title: メッセージを作成する
description: この API を使用して、新しいメッセージを mailFolder 内に作成します。
author: angelgolfer-ms
ms.openlocfilehash: bb88a061a8e867f4cc15470073925c51fe6a3cf6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332544"
---
# <a name="create-message"></a><span data-ttu-id="9daa7-103">メッセージを作成する</span><span class="sxs-lookup"><span data-stu-id="9daa7-103">Create Message</span></span>

<span data-ttu-id="9daa7-104">この API を使用して、新しいメッセージを mailFolder 内に作成します。</span><span class="sxs-lookup"><span data-stu-id="9daa7-104">Use this API to create a new Message in a mailfolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="9daa7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9daa7-105">Permissions</span></span>
<span data-ttu-id="9daa7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9daa7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9daa7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9daa7-108">Permission type</span></span>      | <span data-ttu-id="9daa7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9daa7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9daa7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9daa7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9daa7-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9daa7-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9daa7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9daa7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9daa7-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9daa7-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9daa7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9daa7-114">Application</span></span> | <span data-ttu-id="9daa7-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9daa7-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9daa7-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9daa7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="9daa7-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9daa7-117">Request headers</span></span>
| <span data-ttu-id="9daa7-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9daa7-118">Header</span></span>       | <span data-ttu-id="9daa7-119">値</span><span class="sxs-lookup"><span data-stu-id="9daa7-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9daa7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9daa7-120">Authorization</span></span>  | <span data-ttu-id="9daa7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9daa7-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9daa7-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9daa7-123">Content-Type</span></span>  | <span data-ttu-id="9daa7-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="9daa7-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9daa7-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="9daa7-126">Request body</span></span>
<span data-ttu-id="9daa7-127">要求本文で、[メッセージ](../resources/message.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9daa7-127">In the request body, supply a JSON representation of [Message](../resources/message.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9daa7-128">応答</span><span class="sxs-lookup"><span data-stu-id="9daa7-128">Response</span></span>

<span data-ttu-id="9daa7-129">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [Message](../resources/message.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9daa7-129">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9daa7-130">例</span><span class="sxs-lookup"><span data-stu-id="9daa7-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9daa7-131">要求</span><span class="sxs-lookup"><span data-stu-id="9daa7-131">Request</span></span>
<span data-ttu-id="9daa7-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9daa7-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_message_from_mailfolder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages
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
<span data-ttu-id="9daa7-133">要求本文で、[メッセージ](../resources/message.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9daa7-133">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="9daa7-134">応答</span><span class="sxs-lookup"><span data-stu-id="9daa7-134">Response</span></span>
<span data-ttu-id="9daa7-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9daa7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create Message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->