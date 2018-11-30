---
title: 会話を削除する
description: conversation オブジェクトを削除します。
ms.openlocfilehash: df770b3782b727542571f308c32d9c654c53f169
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023616"
---
# <a name="delete-conversation"></a><span data-ttu-id="0bdc5-103">会話を削除する</span><span class="sxs-lookup"><span data-stu-id="0bdc5-103">Delete conversation</span></span>
<span data-ttu-id="0bdc5-104">[conversation](../resources/conversation.md) オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="0bdc5-104">Delete a [conversation](../resources/conversation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0bdc5-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0bdc5-105">Permissions</span></span>
<span data-ttu-id="0bdc5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0bdc5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0bdc5-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0bdc5-108">Permission type</span></span>      | <span data-ttu-id="0bdc5-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0bdc5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0bdc5-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0bdc5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0bdc5-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bdc5-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0bdc5-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0bdc5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0bdc5-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0bdc5-113">Not supported.</span></span>    |
|<span data-ttu-id="0bdc5-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0bdc5-114">Application</span></span> | <span data-ttu-id="0bdc5-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0bdc5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0bdc5-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0bdc5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0bdc5-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0bdc5-117">Request headers</span></span>
| <span data-ttu-id="0bdc5-118">名前</span><span class="sxs-lookup"><span data-stu-id="0bdc5-118">Name</span></span>       | <span data-ttu-id="0bdc5-119">型</span><span class="sxs-lookup"><span data-stu-id="0bdc5-119">Type</span></span> | <span data-ttu-id="0bdc5-120">説明</span><span class="sxs-lookup"><span data-stu-id="0bdc5-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0bdc5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0bdc5-121">Authorization</span></span>  | <span data-ttu-id="0bdc5-122">string</span><span class="sxs-lookup"><span data-stu-id="0bdc5-122">string</span></span>  | <span data-ttu-id="0bdc5-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0bdc5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0bdc5-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="0bdc5-125">Request body</span></span>
<span data-ttu-id="0bdc5-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0bdc5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0bdc5-127">応答</span><span class="sxs-lookup"><span data-stu-id="0bdc5-127">Response</span></span>
<span data-ttu-id="0bdc5-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="0bdc5-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bdc5-130">例</span><span class="sxs-lookup"><span data-stu-id="0bdc5-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0bdc5-131">要求</span><span class="sxs-lookup"><span data-stu-id="0bdc5-131">Request</span></span>
<span data-ttu-id="0bdc5-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0bdc5-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU="],
  "name": "delete_group_conversation"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```

#### <a name="response"></a><span data-ttu-id="0bdc5-133">応答</span><span class="sxs-lookup"><span data-stu-id="0bdc5-133">Response</span></span>
<span data-ttu-id="0bdc5-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0bdc5-134">The following is an example of the response.</span></span> 
><span data-ttu-id="0bdc5-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0bdc5-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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