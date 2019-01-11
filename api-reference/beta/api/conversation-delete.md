---
title: Delete conversation
description: 会話を削除します。
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: a52735b7c67fb52906e9afcafb98629168f70f89
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829268"
---
# <a name="delete-conversation"></a><span data-ttu-id="16936-103">会話を削除する</span><span class="sxs-lookup"><span data-stu-id="16936-103">Delete conversation</span></span>

> <span data-ttu-id="16936-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="16936-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16936-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16936-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="16936-106">会話を削除します。</span><span class="sxs-lookup"><span data-stu-id="16936-106">Delete conversation.</span></span>
## <a name="permissions"></a><span data-ttu-id="16936-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="16936-107">Permissions</span></span>
<span data-ttu-id="16936-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="16936-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16936-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="16936-110">Permission type</span></span>      | <span data-ttu-id="16936-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="16936-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16936-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="16936-112">Delegated (work or school account)</span></span> | <span data-ttu-id="16936-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16936-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="16936-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="16936-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16936-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16936-115">Not supported.</span></span>    |
|<span data-ttu-id="16936-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="16936-116">Application</span></span> | <span data-ttu-id="16936-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16936-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="16936-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="16936-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```
## <a name="request-headers"></a><span data-ttu-id="16936-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="16936-119">Request headers</span></span>
| <span data-ttu-id="16936-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="16936-120">Header</span></span>       | <span data-ttu-id="16936-121">値</span><span class="sxs-lookup"><span data-stu-id="16936-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="16936-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="16936-122">Authorization</span></span>  | <span data-ttu-id="16936-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="16936-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="16936-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="16936-125">Request body</span></span>
<span data-ttu-id="16936-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="16936-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16936-127">応答</span><span class="sxs-lookup"><span data-stu-id="16936-127">Response</span></span>

<span data-ttu-id="16936-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="16936-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16936-130">例</span><span class="sxs-lookup"><span data-stu-id="16936-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="16936-131">要求</span><span class="sxs-lookup"><span data-stu-id="16936-131">Request</span></span>
<span data-ttu-id="16936-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="16936-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_conversation"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/conversations/{id}
```
##### <a name="response"></a><span data-ttu-id="16936-133">応答</span><span class="sxs-lookup"><span data-stu-id="16936-133">Response</span></span>
<span data-ttu-id="16936-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="16936-134">Here is an example of the response.</span></span> 
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
