---
title: rejectedSender の作成
description: rejectedSender リストに新しいユーザーやグループを追加します。
author: dkershaw10
ms.openlocfilehash: 26965d41c2f5f688303a19f94d717b62713e6482
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354867"
---
# <a name="create-rejectedsender"></a><span data-ttu-id="5c569-103">rejectedSender の作成</span><span class="sxs-lookup"><span data-stu-id="5c569-103">Create rejectedSender</span></span>
<span data-ttu-id="5c569-104">rejectedSender リストに新しいユーザーやグループを追加します。</span><span class="sxs-lookup"><span data-stu-id="5c569-104">Add a new user or group to the rejectedSender list.</span></span>

<span data-ttu-id="5c569-p101">`@odata.id` 内のユーザーやグループを要求の本文で指定します。拒否送信者リスト内のユーザーは、グループの会話に投稿できません (POST 要求 URL で識別)。拒否送信者と承認送信者のリストに同一のユーザーやグループを指定すると、エラーになるので注意してください。</span><span class="sxs-lookup"><span data-stu-id="5c569-p101">Specify the user or group in `@odata.id` in the request body. Users in the rejected senders list cannot post to conversations of the group (identified in the POST request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c569-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5c569-108">Permissions</span></span>
<span data-ttu-id="5c569-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5c569-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c569-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5c569-111">Permission type</span></span>      | <span data-ttu-id="5c569-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5c569-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c569-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5c569-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5c569-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c569-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5c569-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5c569-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c569-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5c569-116">Not supported.</span></span>    |
|<span data-ttu-id="5c569-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5c569-117">Application</span></span> | <span data-ttu-id="5c569-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5c569-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c569-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5c569-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/rejectedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="5c569-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5c569-120">Request headers</span></span>
| <span data-ttu-id="5c569-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5c569-121">Header</span></span>       | <span data-ttu-id="5c569-122">値</span><span class="sxs-lookup"><span data-stu-id="5c569-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5c569-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c569-123">Authorization</span></span>  | <span data-ttu-id="5c569-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5c569-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5c569-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="5c569-126">Request body</span></span>
<span data-ttu-id="5c569-127">要求の本文で、ユーザーまたはグループのオブジェクトの id を指定します。</span><span class="sxs-lookup"><span data-stu-id="5c569-127">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="5c569-128">応答</span><span class="sxs-lookup"><span data-stu-id="5c569-128">Response</span></span>
<span data-ttu-id="5c569-129">このメソッドは `204 No Content` 応答コードを返し、応答の本文は返しません。</span><span class="sxs-lookup"><span data-stu-id="5c569-129">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c569-130">例</span><span class="sxs-lookup"><span data-stu-id="5c569-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="5c569-131">要求</span><span class="sxs-lookup"><span data-stu-id="5c569-131">Request</span></span>
<span data-ttu-id="5c569-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5c569-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/v1.0/users/alexd@contoso.com"
}
```
#### <a name="response"></a><span data-ttu-id="5c569-133">応答</span><span class="sxs-lookup"><span data-stu-id="5c569-133">Response</span></span>
<span data-ttu-id="5c569-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5c569-134">The following is an example of the response.</span></span>
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
  "description": "Create rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->