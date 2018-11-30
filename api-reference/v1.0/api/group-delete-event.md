---
title: イベントを削除する
description: event オブジェクトを削除します。
ms.openlocfilehash: ad3e8657c522c04eebbfc08c2e74d3d7ff4a8120
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024108"
---
# <a name="delete-event"></a><span data-ttu-id="dffab-103">イベントを削除する</span><span class="sxs-lookup"><span data-stu-id="dffab-103">Delete event</span></span>
<span data-ttu-id="dffab-104">[event](../resources/event.md) オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="dffab-104">Delete an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dffab-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="dffab-105">Permissions</span></span>
<span data-ttu-id="dffab-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dffab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dffab-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dffab-108">Permission type</span></span>      | <span data-ttu-id="dffab-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="dffab-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dffab-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dffab-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dffab-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dffab-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="dffab-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dffab-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dffab-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dffab-113">Not supported.</span></span>    |
|<span data-ttu-id="dffab-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dffab-114">Application</span></span> | <span data-ttu-id="dffab-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dffab-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dffab-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dffab-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/events/{id}
DELETE /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="dffab-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dffab-117">Request headers</span></span>
| <span data-ttu-id="dffab-118">名前</span><span class="sxs-lookup"><span data-stu-id="dffab-118">Name</span></span>       | <span data-ttu-id="dffab-119">型</span><span class="sxs-lookup"><span data-stu-id="dffab-119">Type</span></span> | <span data-ttu-id="dffab-120">説明</span><span class="sxs-lookup"><span data-stu-id="dffab-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dffab-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="dffab-121">Authorization</span></span>  | <span data-ttu-id="dffab-122">string</span><span class="sxs-lookup"><span data-stu-id="dffab-122">string</span></span>  | <span data-ttu-id="dffab-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="dffab-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dffab-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="dffab-125">Request body</span></span>
<span data-ttu-id="dffab-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="dffab-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dffab-127">応答</span><span class="sxs-lookup"><span data-stu-id="dffab-127">Response</span></span>
<span data-ttu-id="dffab-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="dffab-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dffab-130">例</span><span class="sxs-lookup"><span data-stu-id="dffab-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="dffab-131">要求</span><span class="sxs-lookup"><span data-stu-id="dffab-131">Request</span></span>
<span data-ttu-id="dffab-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dffab-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA=="],
  "name": "delete_group_event"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events/AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==
```

#### <a name="response"></a><span data-ttu-id="dffab-133">応答</span><span class="sxs-lookup"><span data-stu-id="dffab-133">Response</span></span>
<span data-ttu-id="dffab-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dffab-134">The following is an example of the response.</span></span> 
><span data-ttu-id="dffab-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="dffab-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->