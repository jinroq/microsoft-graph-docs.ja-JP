---
title: outlooktask の削除
description: ユーザーのメールボックス内の指定された Outlook タスクを削除します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 45660f5bb4a2c74fccb5b618dc30f7d331f558bc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32539761"
---
# <a name="delete-outlooktask"></a><span data-ttu-id="56eb3-103">outlooktask の削除</span><span class="sxs-lookup"><span data-stu-id="56eb3-103">Delete outlookTask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56eb3-104">ユーザーのメールボックス内の指定された Outlook タスクを削除します。</span><span class="sxs-lookup"><span data-stu-id="56eb3-104">Delete the specified Outlook task in the user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="56eb3-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="56eb3-105">Permissions</span></span>

<span data-ttu-id="56eb3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="56eb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56eb3-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="56eb3-108">Permission type</span></span>      | <span data-ttu-id="56eb3-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="56eb3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56eb3-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="56eb3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="56eb3-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56eb3-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="56eb3-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="56eb3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56eb3-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56eb3-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="56eb3-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="56eb3-114">Application</span></span> | <span data-ttu-id="56eb3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="56eb3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="56eb3-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="56eb3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/outlook/tasks/{id}
DELETE /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="56eb3-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="56eb3-117">Request headers</span></span>

| <span data-ttu-id="56eb3-118">名前</span><span class="sxs-lookup"><span data-stu-id="56eb3-118">Name</span></span>       | <span data-ttu-id="56eb3-119">説明</span><span class="sxs-lookup"><span data-stu-id="56eb3-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="56eb3-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="56eb3-120">Authorization</span></span>  | <span data-ttu-id="56eb3-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="56eb3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="56eb3-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="56eb3-123">Request body</span></span>

<span data-ttu-id="56eb3-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="56eb3-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56eb3-125">応答</span><span class="sxs-lookup"><span data-stu-id="56eb3-125">Response</span></span>

<span data-ttu-id="56eb3-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="56eb3-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56eb3-128">例</span><span class="sxs-lookup"><span data-stu-id="56eb3-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="56eb3-129">要求</span><span class="sxs-lookup"><span data-stu-id="56eb3-129">Request</span></span>

<span data-ttu-id="56eb3-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="56eb3-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_outlooktask"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADIyAAAhrb_QAAA=')
```

### <a name="response"></a><span data-ttu-id="56eb3-131">応答</span><span class="sxs-lookup"><span data-stu-id="56eb3-131">Response</span></span>

<span data-ttu-id="56eb3-132">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="56eb3-132">Here is an example of the response.</span></span>
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
  "description": "Delete outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktask-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
