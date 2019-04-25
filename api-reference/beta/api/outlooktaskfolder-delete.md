---
title: outlooktaskfolder の削除
description: 指定された Outlook タスクフォルダーを削除します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 4c526c937f7d92b6e2b0482193f6c0327f4870c1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32539877"
---
# <a name="delete-outlooktaskfolder"></a><span data-ttu-id="7a38d-103">outlooktaskfolder の削除</span><span class="sxs-lookup"><span data-stu-id="7a38d-103">Delete outlookTaskFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a38d-104">指定された Outlook タスクフォルダーを削除します。</span><span class="sxs-lookup"><span data-stu-id="7a38d-104">Delete the specified Outlook task folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="7a38d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7a38d-105">Permissions</span></span>
<span data-ttu-id="7a38d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7a38d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a38d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7a38d-108">Permission type</span></span>      | <span data-ttu-id="7a38d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7a38d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a38d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7a38d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7a38d-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7a38d-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="7a38d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7a38d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a38d-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7a38d-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="7a38d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7a38d-114">Application</span></span> | <span data-ttu-id="7a38d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7a38d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a38d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7a38d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/taskFolders/{id}
DELETE /me/outlook/taskGroups/{id}/taskFolders/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskFolders/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="7a38d-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7a38d-117">Request headers</span></span>
| <span data-ttu-id="7a38d-118">名前</span><span class="sxs-lookup"><span data-stu-id="7a38d-118">Name</span></span>       | <span data-ttu-id="7a38d-119">説明</span><span class="sxs-lookup"><span data-stu-id="7a38d-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7a38d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a38d-120">Authorization</span></span>  | <span data-ttu-id="7a38d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7a38d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7a38d-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="7a38d-123">Request body</span></span>
<span data-ttu-id="7a38d-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7a38d-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a38d-125">応答</span><span class="sxs-lookup"><span data-stu-id="7a38d-125">Response</span></span>

<span data-ttu-id="7a38d-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="7a38d-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a38d-128">例</span><span class="sxs-lookup"><span data-stu-id="7a38d-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7a38d-129">要求</span><span class="sxs-lookup"><span data-stu-id="7a38d-129">Request</span></span>
<span data-ttu-id="7a38d-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7a38d-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_outlooktaskfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/taskFolders('AAMkADIyAAAhrbPXAAA=')
```
##### <a name="response"></a><span data-ttu-id="7a38d-131">応答</span><span class="sxs-lookup"><span data-stu-id="7a38d-131">Response</span></span>
<span data-ttu-id="7a38d-132">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="7a38d-132">Here is an example of the response.</span></span> 
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
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktaskfolder-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
