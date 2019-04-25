---
title: Delete conversationThread
description: conversationThread を削除します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 486752a88a3d9b632b430e46a7fd9d155ab989fa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566144"
---
# <a name="delete-conversationthread"></a><span data-ttu-id="ba132-103">Delete conversationThread</span><span class="sxs-lookup"><span data-stu-id="ba132-103">Delete conversationThread</span></span>

<span data-ttu-id="ba132-104">conversationThread を削除します。</span><span class="sxs-lookup"><span data-stu-id="ba132-104">Delete conversationThread.</span></span>
## <a name="permissions"></a><span data-ttu-id="ba132-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ba132-105">Permissions</span></span>
<span data-ttu-id="ba132-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ba132-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba132-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ba132-108">Permission type</span></span>      | <span data-ttu-id="ba132-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ba132-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba132-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ba132-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ba132-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba132-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ba132-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ba132-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba132-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ba132-113">Not supported.</span></span>    |
|<span data-ttu-id="ba132-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ba132-114">Application</span></span> | <span data-ttu-id="ba132-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba132-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba132-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ba132-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="ba132-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ba132-117">Request headers</span></span>
| <span data-ttu-id="ba132-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ba132-118">Header</span></span>       | <span data-ttu-id="ba132-119">値</span><span class="sxs-lookup"><span data-stu-id="ba132-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ba132-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba132-120">Authorization</span></span>  | <span data-ttu-id="ba132-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ba132-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ba132-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ba132-123">Request body</span></span>
<span data-ttu-id="ba132-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ba132-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba132-125">応答</span><span class="sxs-lookup"><span data-stu-id="ba132-125">Response</span></span>

<span data-ttu-id="ba132-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="ba132-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba132-128">例</span><span class="sxs-lookup"><span data-stu-id="ba132-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ba132-129">要求</span><span class="sxs-lookup"><span data-stu-id="ba132-129">Request</span></span>
<span data-ttu-id="ba132-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ba132-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_conversationthread"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}
```
##### <a name="response"></a><span data-ttu-id="ba132-131">応答</span><span class="sxs-lookup"><span data-stu-id="ba132-131">Response</span></span>
<span data-ttu-id="ba132-132">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="ba132-132">Here is an example of the response.</span></span> 
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
  "description": "Delete conversationThread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
