---
title: AcceptedSender の作成
description: AcceptedSender リストに新しいユーザーやグループを追加します。
ms.openlocfilehash: 7f58f1919ca592fd2ba00e091d714f020e81a6bc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071974"
---
# <a name="create-acceptedsender"></a><span data-ttu-id="e388f-103">AcceptedSender の作成</span><span class="sxs-lookup"><span data-stu-id="e388f-103">Create acceptedSender</span></span>

> <span data-ttu-id="e388f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e388f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e388f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e388f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e388f-106">AcceptedSender リストに新しいユーザーやグループを追加します。</span><span class="sxs-lookup"><span data-stu-id="e388f-106">Add a new user or group to the acceptedSender list.</span></span>

<span data-ttu-id="e388f-p102">`@odata.id` 内のユーザーやグループを要求の本文で指定します。承諾済み送信者リスト内のユーザーは、グループに会話を投稿できません。承認送信者と拒否送信者のリストに同一のユーザーやグループを指定すると、エラーになるので注意してください。</span><span class="sxs-lookup"><span data-stu-id="e388f-p102">Specify the user or group in `@odata.id` in the request body. Users in the accepted senders list can post to conversations of the group . Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="e388f-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e388f-110">Permissions</span></span>
<span data-ttu-id="e388f-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e388f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e388f-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e388f-113">Permission type</span></span>      | <span data-ttu-id="e388f-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e388f-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e388f-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e388f-115">Delegated (work or school account)</span></span> | <span data-ttu-id="e388f-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e388f-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e388f-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e388f-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e388f-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e388f-118">Not supported.</span></span>    |
|<span data-ttu-id="e388f-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e388f-119">Application</span></span> | <span data-ttu-id="e388f-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e388f-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e388f-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e388f-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/acceptedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="e388f-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e388f-122">Request headers</span></span>
| <span data-ttu-id="e388f-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e388f-123">Header</span></span>       | <span data-ttu-id="e388f-124">値</span><span class="sxs-lookup"><span data-stu-id="e388f-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e388f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e388f-125">Authorization</span></span>  | <span data-ttu-id="e388f-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e388f-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e388f-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="e388f-128">Request body</span></span>
<span data-ttu-id="e388f-129">要求の本文で、ユーザーまたはグループのオブジェクトの id を指定します。</span><span class="sxs-lookup"><span data-stu-id="e388f-129">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="e388f-130">応答</span><span class="sxs-lookup"><span data-stu-id="e388f-130">Response</span></span>
<span data-ttu-id="e388f-131">このメソッドは `204 No Content` 応答コードを返し、応答の本文は返しません。</span><span class="sxs-lookup"><span data-stu-id="e388f-131">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="e388f-132">例</span><span class="sxs-lookup"><span data-stu-id="e388f-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e388f-133">要求</span><span class="sxs-lookup"><span data-stu-id="e388f-133">Request</span></span>
<span data-ttu-id="e388f-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e388f-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_acceptedsender"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/acceptedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/beta/users/alexd@contoso.com"
}
```

#### <a name="response"></a><span data-ttu-id="e388f-135">応答</span><span class="sxs-lookup"><span data-stu-id="e388f-135">Response</span></span>
<span data-ttu-id="e388f-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e388f-136">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
