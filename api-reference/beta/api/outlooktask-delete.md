---
title: OutlookTask を削除します。
description: ユーザーのメールボックスに指定された Outlook タスクを削除します。
ms.openlocfilehash: 00c2c4d1e5b706b34b531380e32083be55c98776
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073980"
---
# <a name="delete-outlooktask"></a><span data-ttu-id="7db54-103">OutlookTask を削除します。</span><span class="sxs-lookup"><span data-stu-id="7db54-103">Delete outlookTask</span></span>

> <span data-ttu-id="7db54-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7db54-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7db54-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7db54-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7db54-106">ユーザーのメールボックスに指定された Outlook タスクを削除します。</span><span class="sxs-lookup"><span data-stu-id="7db54-106">Delete the specified Outlook task in the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="7db54-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7db54-107">Permissions</span></span>
<span data-ttu-id="7db54-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7db54-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7db54-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7db54-110">Permission type</span></span>      | <span data-ttu-id="7db54-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7db54-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7db54-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7db54-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7db54-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7db54-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="7db54-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7db54-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7db54-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7db54-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="7db54-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7db54-116">Application</span></span> | <span data-ttu-id="7db54-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7db54-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7db54-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7db54-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id|userPrincipalName}/outlook/tasks/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}

```
## <a name="request-headers"></a><span data-ttu-id="7db54-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7db54-119">Request headers</span></span>
| <span data-ttu-id="7db54-120">名前</span><span class="sxs-lookup"><span data-stu-id="7db54-120">Name</span></span>       | <span data-ttu-id="7db54-121">説明</span><span class="sxs-lookup"><span data-stu-id="7db54-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7db54-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7db54-122">Authorization</span></span>  | <span data-ttu-id="7db54-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7db54-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7db54-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="7db54-125">Request body</span></span>
<span data-ttu-id="7db54-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7db54-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7db54-127">応答</span><span class="sxs-lookup"><span data-stu-id="7db54-127">Response</span></span>

<span data-ttu-id="7db54-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="7db54-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7db54-130">例</span><span class="sxs-lookup"><span data-stu-id="7db54-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7db54-131">要求</span><span class="sxs-lookup"><span data-stu-id="7db54-131">Request</span></span>
<span data-ttu-id="7db54-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7db54-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_outlooktask"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADIyAAAhrb_QAAA=')
```
##### <a name="response"></a><span data-ttu-id="7db54-133">応答</span><span class="sxs-lookup"><span data-stu-id="7db54-133">Response</span></span>
<span data-ttu-id="7db54-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="7db54-134">Here is an example of the response.</span></span> 
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