---
title: 会話を削除する
description: conversation オブジェクトを削除します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: d5e736de924ebcfadac37f267d9ba154383f3b91
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329578"
---
# <a name="delete-conversation"></a><span data-ttu-id="95972-103">会話を削除する</span><span class="sxs-lookup"><span data-stu-id="95972-103">Delete conversation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95972-104">[conversation](../resources/conversation.md) オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="95972-104">Delete a [conversation](../resources/conversation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="95972-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="95972-105">Permissions</span></span>
<span data-ttu-id="95972-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="95972-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95972-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="95972-108">Permission type</span></span>      | <span data-ttu-id="95972-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="95972-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95972-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="95972-110">Delegated (work or school account)</span></span> | <span data-ttu-id="95972-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95972-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="95972-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="95972-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95972-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95972-113">Not supported.</span></span>    |
|<span data-ttu-id="95972-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="95972-114">Application</span></span> | <span data-ttu-id="95972-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95972-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="95972-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="95972-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="95972-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95972-117">Request headers</span></span>
| <span data-ttu-id="95972-118">名前</span><span class="sxs-lookup"><span data-stu-id="95972-118">Name</span></span>       | <span data-ttu-id="95972-119">型</span><span class="sxs-lookup"><span data-stu-id="95972-119">Type</span></span> | <span data-ttu-id="95972-120">説明</span><span class="sxs-lookup"><span data-stu-id="95972-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="95972-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="95972-121">Authorization</span></span>  | <span data-ttu-id="95972-122">string</span><span class="sxs-lookup"><span data-stu-id="95972-122">string</span></span>  | <span data-ttu-id="95972-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="95972-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="95972-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="95972-125">Request body</span></span>
<span data-ttu-id="95972-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="95972-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95972-127">応答</span><span class="sxs-lookup"><span data-stu-id="95972-127">Response</span></span>
<span data-ttu-id="95972-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="95972-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95972-130">例</span><span class="sxs-lookup"><span data-stu-id="95972-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="95972-131">要求</span><span class="sxs-lookup"><span data-stu-id="95972-131">Request</span></span>
<span data-ttu-id="95972-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="95972-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group_conversation"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```

#### <a name="response"></a><span data-ttu-id="95972-133">応答</span><span class="sxs-lookup"><span data-stu-id="95972-133">Response</span></span>
<span data-ttu-id="95972-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="95972-134">The following is an example of the response.</span></span> 
><span data-ttu-id="95972-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="95972-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
