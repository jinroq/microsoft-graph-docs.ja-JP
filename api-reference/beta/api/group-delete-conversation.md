---
title: 会話を削除する
description: conversation オブジェクトを削除します。
author: dkershaw10
ms.openlocfilehash: 856ef098e9ac7a3a94bb52301335a339d6d966ce
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318671"
---
# <a name="delete-conversation"></a><span data-ttu-id="2ab39-103">会話を削除する</span><span class="sxs-lookup"><span data-stu-id="2ab39-103">Delete conversation</span></span>

> <span data-ttu-id="2ab39-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2ab39-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2ab39-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ab39-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2ab39-106">[conversation](../resources/conversation.md) オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="2ab39-106">Delete a [conversation](../resources/conversation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ab39-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2ab39-107">Permissions</span></span>
<span data-ttu-id="2ab39-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2ab39-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ab39-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2ab39-110">Permission type</span></span>      | <span data-ttu-id="2ab39-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2ab39-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ab39-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2ab39-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2ab39-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ab39-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2ab39-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2ab39-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ab39-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ab39-115">Not supported.</span></span>    |
|<span data-ttu-id="2ab39-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2ab39-116">Application</span></span> | <span data-ttu-id="2ab39-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ab39-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ab39-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2ab39-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2ab39-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2ab39-119">Request headers</span></span>
| <span data-ttu-id="2ab39-120">名前</span><span class="sxs-lookup"><span data-stu-id="2ab39-120">Name</span></span>       | <span data-ttu-id="2ab39-121">種類</span><span class="sxs-lookup"><span data-stu-id="2ab39-121">Type</span></span> | <span data-ttu-id="2ab39-122">説明</span><span class="sxs-lookup"><span data-stu-id="2ab39-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2ab39-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ab39-123">Authorization</span></span>  | <span data-ttu-id="2ab39-124">string</span><span class="sxs-lookup"><span data-stu-id="2ab39-124">string</span></span>  | <span data-ttu-id="2ab39-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2ab39-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ab39-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="2ab39-127">Request body</span></span>
<span data-ttu-id="2ab39-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2ab39-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ab39-129">応答</span><span class="sxs-lookup"><span data-stu-id="2ab39-129">Response</span></span>
<span data-ttu-id="2ab39-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="2ab39-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ab39-132">例</span><span class="sxs-lookup"><span data-stu-id="2ab39-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2ab39-133">要求</span><span class="sxs-lookup"><span data-stu-id="2ab39-133">Request</span></span>
<span data-ttu-id="2ab39-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2ab39-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group_conversation"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```

#### <a name="response"></a><span data-ttu-id="2ab39-135">応答</span><span class="sxs-lookup"><span data-stu-id="2ab39-135">Response</span></span>
<span data-ttu-id="2ab39-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2ab39-136">The following is an example of the response.</span></span> 
><span data-ttu-id="2ab39-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="2ab39-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->