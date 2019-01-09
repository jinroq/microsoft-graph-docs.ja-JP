---
title: OutlookTask を削除します。
description: ユーザーのメールボックスに指定された Outlook タスクを削除します。
ms.openlocfilehash: cab78b8fea63c5044cc6faa6a1e4f09dd960bfd6
ms.sourcegitcommit: 6b1ba9b3be038cd6247de54a255bad560034fe42
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/08/2019
ms.locfileid: "27771780"
---
# <a name="delete-outlooktask"></a><span data-ttu-id="a7ffe-103">OutlookTask を削除します。</span><span class="sxs-lookup"><span data-stu-id="a7ffe-103">Delete outlookTask</span></span>

> <span data-ttu-id="a7ffe-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a7ffe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a7ffe-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a7ffe-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a7ffe-106">ユーザーのメールボックスに指定された Outlook タスクを削除します。</span><span class="sxs-lookup"><span data-stu-id="a7ffe-106">Delete the specified Outlook task in the user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7ffe-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a7ffe-107">Permissions</span></span>

<span data-ttu-id="a7ffe-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a7ffe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7ffe-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a7ffe-110">Permission type</span></span>      | <span data-ttu-id="a7ffe-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a7ffe-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7ffe-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a7ffe-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a7ffe-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a7ffe-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="a7ffe-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a7ffe-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7ffe-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a7ffe-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="a7ffe-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a7ffe-116">Application</span></span> | <span data-ttu-id="a7ffe-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a7ffe-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7ffe-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a7ffe-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/outlook/tasks/{id}
DELETE /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a7ffe-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a7ffe-119">Request headers</span></span>

| <span data-ttu-id="a7ffe-120">名前</span><span class="sxs-lookup"><span data-stu-id="a7ffe-120">Name</span></span>       | <span data-ttu-id="a7ffe-121">説明</span><span class="sxs-lookup"><span data-stu-id="a7ffe-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a7ffe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7ffe-122">Authorization</span></span>  | <span data-ttu-id="a7ffe-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a7ffe-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a7ffe-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a7ffe-125">Request body</span></span>

<span data-ttu-id="a7ffe-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a7ffe-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7ffe-127">応答</span><span class="sxs-lookup"><span data-stu-id="a7ffe-127">Response</span></span>

<span data-ttu-id="a7ffe-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="a7ffe-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7ffe-130">例</span><span class="sxs-lookup"><span data-stu-id="a7ffe-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7ffe-131">要求</span><span class="sxs-lookup"><span data-stu-id="a7ffe-131">Request</span></span>

<span data-ttu-id="a7ffe-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a7ffe-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_outlooktask"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADIyAAAhrb_QAAA=')
```

### <a name="response"></a><span data-ttu-id="a7ffe-133">応答</span><span class="sxs-lookup"><span data-stu-id="a7ffe-133">Response</span></span>

<span data-ttu-id="a7ffe-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="a7ffe-134">Here is an example of the response.</span></span>
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
  "description": "Delete outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->