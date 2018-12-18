---
title: チャットのスレッドを作成します。
description: ルート メッセージを指定することによって、指定されたチャネルでチャットの新しいスレッドを作成します。
author: nkramer
ms.openlocfilehash: fcd1c08c05b29d2150f4c436eac7765f40900920
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325614"
---
# <a name="create-chat-thread"></a><span data-ttu-id="177aa-103">チャットのスレッドを作成します。</span><span class="sxs-lookup"><span data-stu-id="177aa-103">Create chat thread</span></span>

> <span data-ttu-id="177aa-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="177aa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="177aa-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="177aa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="177aa-106">ルート メッセージを指定することによって、指定された[チャネル](../resources/channel.md)でチャットの新しいスレッドを作成します。</span><span class="sxs-lookup"><span data-stu-id="177aa-106">Create a new chat thread in the specified [channel](../resources/channel.md) by supplying the root messages.</span></span>

## <a name="permissions"></a><span data-ttu-id="177aa-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="177aa-107">Permissions</span></span>
<span data-ttu-id="177aa-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="177aa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="177aa-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="177aa-110">Permission type</span></span>      | <span data-ttu-id="177aa-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="177aa-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="177aa-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="177aa-112">Delegated (work or school account)</span></span> | <span data-ttu-id="177aa-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="177aa-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="177aa-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="177aa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="177aa-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="177aa-115">Not supported.</span></span>    |
|<span data-ttu-id="177aa-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="177aa-116">Application</span></span> | <span data-ttu-id="177aa-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="177aa-117">Not supported.</span></span> |

> <span data-ttu-id="177aa-118">現在、[委任されたアクセス許可](/graph/permissions-reference)をのみがこの操作に対してサポートされています。</span><span class="sxs-lookup"><span data-stu-id="177aa-118">Currently, only [delegated permissions](/graph/permissions-reference) are supported for this operation.</span></span>  <span data-ttu-id="177aa-119">将来のリリースでは、アプリケーションのアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="177aa-119">Future releases will support application permissions.</span></span> 

## <a name="http-request"></a><span data-ttu-id="177aa-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="177aa-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/chatThreads
```
## <a name="request-headers"></a><span data-ttu-id="177aa-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="177aa-121">Request headers</span></span>
| <span data-ttu-id="177aa-122">名前</span><span class="sxs-lookup"><span data-stu-id="177aa-122">Name</span></span>       | <span data-ttu-id="177aa-123">種類</span><span class="sxs-lookup"><span data-stu-id="177aa-123">Type</span></span> | <span data-ttu-id="177aa-124">説明</span><span class="sxs-lookup"><span data-stu-id="177aa-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="177aa-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="177aa-125">Authorization</span></span>  | <span data-ttu-id="177aa-126">string</span><span class="sxs-lookup"><span data-stu-id="177aa-126">string</span></span>  | <span data-ttu-id="177aa-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="177aa-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="177aa-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="177aa-129">Request body</span></span>
<span data-ttu-id="177aa-130">要求の本文に rootMessage プロパティが含まれている[chatThread](../resources/chatthread.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="177aa-130">In the request body, supply a JSON representation of a [chatThread](../resources/chatthread.md) object that contains the rootMessage property.</span></span>

## <a name="response"></a><span data-ttu-id="177aa-131">応答</span><span class="sxs-lookup"><span data-stu-id="177aa-131">Response</span></span>

<span data-ttu-id="177aa-132">かどうかは成功すると、このメソッドを返します`201 Created`、空の応答の本体を含む応答コード。</span><span class="sxs-lookup"><span data-stu-id="177aa-132">If successful, this method returns `201 Created` response code with an empty reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="177aa-133">例</span><span class="sxs-lookup"><span data-stu-id="177aa-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="177aa-134">要求</span><span class="sxs-lookup"><span data-stu-id="177aa-134">Request</span></span>
<span data-ttu-id="177aa-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="177aa-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chatthread_from_channel"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/chatThreads
Content-type: application/json

{
  "rootMessage": {
      "body": {
        "contentType": 1,
        "content": "<h1>Hello world</h1>"
      }
  }
}
```

> <span data-ttu-id="177aa-136">現時点では、文字列ではなく整数として、コンテンツ タイプを指定する必要があります:"text"または"html"の場合は 1 の場合は 0 です。</span><span class="sxs-lookup"><span data-stu-id="177aa-136">Currently, the contentType must be specified as an integer rather than a string: 0 for "text" or 1 for "html".</span></span>  <span data-ttu-id="177aa-137">API の将来のリリースには、これを修正します。</span><span class="sxs-lookup"><span data-stu-id="177aa-137">Future API releases will fix this.</span></span>

##### <a name="response"></a><span data-ttu-id="177aa-138">応答</span><span class="sxs-lookup"><span data-stu-id="177aa-138">Response</span></span>

<span data-ttu-id="177aa-139">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="177aa-139">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatThread"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 160

{
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
