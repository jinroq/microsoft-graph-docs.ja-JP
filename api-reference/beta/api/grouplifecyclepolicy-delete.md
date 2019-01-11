---
title: Delete groupLifecyclePolicy
description: groupLifecyclePolicy を削除します。
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: f92a8fbfd0a45abfdfbb1705f99eaa2d7335bc08
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882580"
---
# <a name="delete-grouplifecyclepolicy"></a><span data-ttu-id="13eb4-103">Delete groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="13eb4-103">Delete groupLifecyclePolicy</span></span>

> <span data-ttu-id="13eb4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="13eb4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13eb4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13eb4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="13eb4-106">[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="13eb4-106">Deletes a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="13eb4-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="13eb4-107">Permissions</span></span>

<span data-ttu-id="13eb4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="13eb4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13eb4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="13eb4-110">Permission type</span></span>      | <span data-ttu-id="13eb4-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="13eb4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13eb4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="13eb4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="13eb4-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13eb4-113">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="13eb4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="13eb4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13eb4-115">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="13eb4-115">Not supported</span></span> |
|<span data-ttu-id="13eb4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="13eb4-116">Application</span></span> | <span data-ttu-id="13eb4-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13eb4-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="13eb4-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="13eb4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupLifecyclePolicies/{id}

```

## <a name="request-headers"></a><span data-ttu-id="13eb4-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="13eb4-119">Request headers</span></span>

| <span data-ttu-id="13eb4-120">名前</span><span class="sxs-lookup"><span data-stu-id="13eb4-120">Name</span></span> | <span data-ttu-id="13eb4-121">説明</span><span class="sxs-lookup"><span data-stu-id="13eb4-121">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="13eb4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="13eb4-122">Authorization</span></span> | <span data-ttu-id="13eb4-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="13eb4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="13eb4-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="13eb4-125">Content-Type</span></span>  | <span data-ttu-id="13eb4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="13eb4-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="13eb4-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="13eb4-127">Request body</span></span>
<span data-ttu-id="13eb4-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="13eb4-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="13eb4-129">応答</span><span class="sxs-lookup"><span data-stu-id="13eb4-129">Response</span></span>

<span data-ttu-id="13eb4-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="13eb4-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13eb4-132">例</span><span class="sxs-lookup"><span data-stu-id="13eb4-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="13eb4-133">要求</span><span class="sxs-lookup"><span data-stu-id="13eb4-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_grouplifecyclepolicy"
}-->
```http
DELETE https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="13eb4-134">応答</span><span class="sxs-lookup"><span data-stu-id="13eb4-134">Response</span></span>

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
  "description": "Delete groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
