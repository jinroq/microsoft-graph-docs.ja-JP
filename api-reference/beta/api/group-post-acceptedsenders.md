---
title: AcceptedSender の作成
description: AcceptedSender リストに新しいユーザーやグループを追加します。
author: dkershaw10
ms.openlocfilehash: bdf7eee53c16089685991334ce839abb4b3cadc0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338746"
---
# <a name="create-acceptedsender"></a><span data-ttu-id="68325-103">AcceptedSender の作成</span><span class="sxs-lookup"><span data-stu-id="68325-103">Create acceptedSender</span></span>

> <span data-ttu-id="68325-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="68325-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="68325-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="68325-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="68325-106">AcceptedSender リストに新しいユーザーやグループを追加します。</span><span class="sxs-lookup"><span data-stu-id="68325-106">Add a new user or group to the acceptedSender list.</span></span>

<span data-ttu-id="68325-p102">`@odata.id` 内のユーザーやグループを要求の本文で指定します。承諾済み送信者リスト内のユーザーは、グループに会話を投稿できません。承認送信者と拒否送信者のリストに同一のユーザーやグループを指定すると、エラーになるので注意してください。</span><span class="sxs-lookup"><span data-stu-id="68325-p102">Specify the user or group in `@odata.id` in the request body. Users in the accepted senders list can post to conversations of the group . Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="68325-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="68325-110">Permissions</span></span>
<span data-ttu-id="68325-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="68325-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68325-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="68325-113">Permission type</span></span>      | <span data-ttu-id="68325-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="68325-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68325-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="68325-115">Delegated (work or school account)</span></span> | <span data-ttu-id="68325-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68325-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="68325-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="68325-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68325-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="68325-118">Not supported.</span></span>    |
|<span data-ttu-id="68325-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="68325-119">Application</span></span> | <span data-ttu-id="68325-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="68325-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="68325-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="68325-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/acceptedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="68325-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="68325-122">Request headers</span></span>
| <span data-ttu-id="68325-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="68325-123">Header</span></span>       | <span data-ttu-id="68325-124">値</span><span class="sxs-lookup"><span data-stu-id="68325-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="68325-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="68325-125">Authorization</span></span>  | <span data-ttu-id="68325-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="68325-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="68325-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="68325-128">Request body</span></span>
<span data-ttu-id="68325-129">要求の本文で、ユーザーまたはグループのオブジェクトの id を指定します。</span><span class="sxs-lookup"><span data-stu-id="68325-129">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="68325-130">応答</span><span class="sxs-lookup"><span data-stu-id="68325-130">Response</span></span>
<span data-ttu-id="68325-131">このメソッドは `204 No Content` 応答コードを返し、応答の本文は返しません。</span><span class="sxs-lookup"><span data-stu-id="68325-131">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="68325-132">例</span><span class="sxs-lookup"><span data-stu-id="68325-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="68325-133">要求</span><span class="sxs-lookup"><span data-stu-id="68325-133">Request</span></span>
<span data-ttu-id="68325-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="68325-134">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="68325-135">応答</span><span class="sxs-lookup"><span data-stu-id="68325-135">Response</span></span>
<span data-ttu-id="68325-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="68325-136">The following is an example of the response.</span></span>
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