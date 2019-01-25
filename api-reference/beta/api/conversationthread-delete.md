---
title: Delete conversationThread
description: conversationThread を削除します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: b4f2cde17e48a4a55f2059ba35aac892d77754ef
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525403"
---
# <a name="delete-conversationthread"></a><span data-ttu-id="ab0f2-103">Delete conversationThread</span><span class="sxs-lookup"><span data-stu-id="ab0f2-103">Delete conversationThread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab0f2-104">conversationThread を削除します。</span><span class="sxs-lookup"><span data-stu-id="ab0f2-104">Delete conversationThread.</span></span>
## <a name="permissions"></a><span data-ttu-id="ab0f2-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ab0f2-105">Permissions</span></span>
<span data-ttu-id="ab0f2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ab0f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab0f2-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ab0f2-108">Permission type</span></span>      | <span data-ttu-id="ab0f2-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ab0f2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab0f2-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ab0f2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ab0f2-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab0f2-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ab0f2-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ab0f2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab0f2-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ab0f2-113">Not supported.</span></span>    |
|<span data-ttu-id="ab0f2-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ab0f2-114">Application</span></span> | <span data-ttu-id="ab0f2-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab0f2-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab0f2-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ab0f2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="ab0f2-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ab0f2-117">Request headers</span></span>
| <span data-ttu-id="ab0f2-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ab0f2-118">Header</span></span>       | <span data-ttu-id="ab0f2-119">値</span><span class="sxs-lookup"><span data-stu-id="ab0f2-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ab0f2-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab0f2-120">Authorization</span></span>  | <span data-ttu-id="ab0f2-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ab0f2-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ab0f2-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ab0f2-123">Request body</span></span>
<span data-ttu-id="ab0f2-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ab0f2-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab0f2-125">応答</span><span class="sxs-lookup"><span data-stu-id="ab0f2-125">Response</span></span>

<span data-ttu-id="ab0f2-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="ab0f2-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab0f2-128">例</span><span class="sxs-lookup"><span data-stu-id="ab0f2-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ab0f2-129">要求</span><span class="sxs-lookup"><span data-stu-id="ab0f2-129">Request</span></span>
<span data-ttu-id="ab0f2-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ab0f2-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_conversationthread"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/threads/{id}
```
##### <a name="response"></a><span data-ttu-id="ab0f2-131">応答</span><span class="sxs-lookup"><span data-stu-id="ab0f2-131">Response</span></span>
<span data-ttu-id="ab0f2-132">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="ab0f2-132">Here is an example of the response.</span></span> 
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
  "description": "Delete conversationThread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/conversationthread-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
