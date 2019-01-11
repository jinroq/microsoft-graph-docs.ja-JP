---
title: アプリケーションを削除します。
description: アプリケーションを削除します。
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 46c02d0fc1730f5741175e5ab99e2082e60c8f48
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838816"
---
# <a name="delete-application"></a><span data-ttu-id="65133-103">アプリケーションを削除します。</span><span class="sxs-lookup"><span data-stu-id="65133-103">Delete application</span></span>

> <span data-ttu-id="65133-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="65133-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65133-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65133-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="65133-106">アプリケーションを削除します。</span><span class="sxs-lookup"><span data-stu-id="65133-106">Deletes an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="65133-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="65133-107">Permissions</span></span>
<span data-ttu-id="65133-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="65133-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65133-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="65133-110">Permission type</span></span>      | <span data-ttu-id="65133-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="65133-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65133-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="65133-112">Delegated (work or school account)</span></span> | <span data-ttu-id="65133-113">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="65133-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="65133-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="65133-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65133-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65133-115">Not supported.</span></span>    |
|<span data-ttu-id="65133-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="65133-116">Application</span></span> | <span data-ttu-id="65133-117">Application.ReadWrite.OwnedBy、Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65133-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="65133-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="65133-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /applications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="65133-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="65133-119">Request headers</span></span>
| <span data-ttu-id="65133-120">名前</span><span class="sxs-lookup"><span data-stu-id="65133-120">Name</span></span>       | <span data-ttu-id="65133-121">種類</span><span class="sxs-lookup"><span data-stu-id="65133-121">Type</span></span> | <span data-ttu-id="65133-122">説明</span><span class="sxs-lookup"><span data-stu-id="65133-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="65133-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="65133-123">Authorization</span></span>  | <span data-ttu-id="65133-124">string</span><span class="sxs-lookup"><span data-stu-id="65133-124">string</span></span>  | <span data-ttu-id="65133-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="65133-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="65133-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="65133-127">Request body</span></span>
<span data-ttu-id="65133-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="65133-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65133-129">応答</span><span class="sxs-lookup"><span data-stu-id="65133-129">Response</span></span>

<span data-ttu-id="65133-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="65133-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65133-132">例</span><span class="sxs-lookup"><span data-stu-id="65133-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="65133-133">要求</span><span class="sxs-lookup"><span data-stu-id="65133-133">Request</span></span>
<span data-ttu-id="65133-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="65133-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_application"
}-->
```http
DELETE https://graph.microsoft.com/beta/applications/{id}
```
##### <a name="response"></a><span data-ttu-id="65133-135">応答</span><span class="sxs-lookup"><span data-stu-id="65133-135">Response</span></span>
<span data-ttu-id="65133-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="65133-136">Here is an example of the response.</span></span> 
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
  "description": "Delete application",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
