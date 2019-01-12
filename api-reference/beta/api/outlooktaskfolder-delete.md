---
title: OutlookTaskFolder を削除します。
description: 指定した Outlook の仕事フォルダーを削除します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 2a43ad79edfee90ec32d45e6d91c619630c6bd9f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935326"
---
# <a name="delete-outlooktaskfolder"></a><span data-ttu-id="5ded1-103">OutlookTaskFolder を削除します。</span><span class="sxs-lookup"><span data-stu-id="5ded1-103">Delete outlookTaskFolder</span></span>

> <span data-ttu-id="5ded1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5ded1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5ded1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5ded1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5ded1-106">指定した Outlook の仕事フォルダーを削除します。</span><span class="sxs-lookup"><span data-stu-id="5ded1-106">Delete the specified Outlook task folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="5ded1-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5ded1-107">Permissions</span></span>
<span data-ttu-id="5ded1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5ded1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ded1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5ded1-110">Permission type</span></span>      | <span data-ttu-id="5ded1-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5ded1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ded1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5ded1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5ded1-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ded1-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="5ded1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5ded1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ded1-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ded1-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="5ded1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5ded1-116">Application</span></span> | <span data-ttu-id="5ded1-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5ded1-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ded1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5ded1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id|userPrincipalName}/outlook/taskFolders/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}

```
## <a name="request-headers"></a><span data-ttu-id="5ded1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5ded1-119">Request headers</span></span>
| <span data-ttu-id="5ded1-120">名前</span><span class="sxs-lookup"><span data-stu-id="5ded1-120">Name</span></span>       | <span data-ttu-id="5ded1-121">説明</span><span class="sxs-lookup"><span data-stu-id="5ded1-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5ded1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ded1-122">Authorization</span></span>  | <span data-ttu-id="5ded1-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5ded1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5ded1-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="5ded1-125">Request body</span></span>
<span data-ttu-id="5ded1-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5ded1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ded1-127">応答</span><span class="sxs-lookup"><span data-stu-id="5ded1-127">Response</span></span>

<span data-ttu-id="5ded1-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="5ded1-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ded1-130">例</span><span class="sxs-lookup"><span data-stu-id="5ded1-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5ded1-131">要求</span><span class="sxs-lookup"><span data-stu-id="5ded1-131">Request</span></span>
<span data-ttu-id="5ded1-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5ded1-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_outlooktaskfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/taskFolders('AAMkADIyAAAhrbPXAAA=')
```
##### <a name="response"></a><span data-ttu-id="5ded1-133">応答</span><span class="sxs-lookup"><span data-stu-id="5ded1-133">Response</span></span>
<span data-ttu-id="5ded1-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="5ded1-134">Here is an example of the response.</span></span> 
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
  "description": "Delete outlookTaskFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
