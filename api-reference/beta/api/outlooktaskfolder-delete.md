---
title: outlooktaskfolder の削除
description: 指定された Outlook タスクフォルダーを削除します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: a961c0016bc3a321418404997a95aa551ee775ec
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338039"
---
# <a name="delete-outlooktaskfolder"></a><span data-ttu-id="96a58-103">outlooktaskfolder の削除</span><span class="sxs-lookup"><span data-stu-id="96a58-103">Delete outlookTaskFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96a58-104">指定された Outlook タスクフォルダーを削除します。</span><span class="sxs-lookup"><span data-stu-id="96a58-104">Delete the specified Outlook task folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="96a58-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="96a58-105">Permissions</span></span>
<span data-ttu-id="96a58-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="96a58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96a58-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="96a58-108">Permission type</span></span>      | <span data-ttu-id="96a58-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="96a58-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96a58-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="96a58-110">Delegated (work or school account)</span></span> | <span data-ttu-id="96a58-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96a58-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="96a58-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="96a58-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96a58-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96a58-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="96a58-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="96a58-114">Application</span></span> | <span data-ttu-id="96a58-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96a58-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="96a58-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="96a58-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/taskFolders/{id}
DELETE /me/outlook/taskGroups/{id}/taskFolders/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskFolders/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="96a58-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="96a58-117">Request headers</span></span>
| <span data-ttu-id="96a58-118">名前</span><span class="sxs-lookup"><span data-stu-id="96a58-118">Name</span></span>       | <span data-ttu-id="96a58-119">説明</span><span class="sxs-lookup"><span data-stu-id="96a58-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="96a58-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="96a58-120">Authorization</span></span>  | <span data-ttu-id="96a58-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="96a58-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="96a58-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="96a58-123">Request body</span></span>
<span data-ttu-id="96a58-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="96a58-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96a58-125">応答</span><span class="sxs-lookup"><span data-stu-id="96a58-125">Response</span></span>

<span data-ttu-id="96a58-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="96a58-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96a58-128">例</span><span class="sxs-lookup"><span data-stu-id="96a58-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="96a58-129">要求</span><span class="sxs-lookup"><span data-stu-id="96a58-129">Request</span></span>
<span data-ttu-id="96a58-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="96a58-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_outlooktaskfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/taskFolders/AAMkADIyAAAhrbPXAAA=
```
##### <a name="response"></a><span data-ttu-id="96a58-131">応答</span><span class="sxs-lookup"><span data-stu-id="96a58-131">Response</span></span>
<span data-ttu-id="96a58-132">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="96a58-132">Here is an example of the response.</span></span> 
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
  "description": "Delete outlookTaskFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
