---
title: Delete groupLifecyclePolicy
description: groupLifecyclePolicy を削除します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: c78e59c010e9c449af665d0b67abb0efcad0d3cc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527788"
---
# <a name="delete-grouplifecyclepolicy"></a><span data-ttu-id="793c7-103">Delete groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="793c7-103">Delete groupLifecyclePolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="793c7-104">[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="793c7-104">Deletes a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="793c7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="793c7-105">Permissions</span></span>

<span data-ttu-id="793c7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="793c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="793c7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="793c7-108">Permission type</span></span>      | <span data-ttu-id="793c7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="793c7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="793c7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="793c7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="793c7-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="793c7-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="793c7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="793c7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="793c7-113">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="793c7-113">Not supported</span></span> |
|<span data-ttu-id="793c7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="793c7-114">Application</span></span> | <span data-ttu-id="793c7-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="793c7-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="793c7-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="793c7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupLifecyclePolicies/{id}

```

## <a name="request-headers"></a><span data-ttu-id="793c7-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="793c7-117">Request headers</span></span>

| <span data-ttu-id="793c7-118">名前</span><span class="sxs-lookup"><span data-stu-id="793c7-118">Name</span></span> | <span data-ttu-id="793c7-119">説明</span><span class="sxs-lookup"><span data-stu-id="793c7-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="793c7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="793c7-120">Authorization</span></span> | <span data-ttu-id="793c7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="793c7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="793c7-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="793c7-123">Content-Type</span></span>  | <span data-ttu-id="793c7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="793c7-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="793c7-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="793c7-125">Request body</span></span>
<span data-ttu-id="793c7-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="793c7-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="793c7-127">応答</span><span class="sxs-lookup"><span data-stu-id="793c7-127">Response</span></span>

<span data-ttu-id="793c7-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="793c7-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="793c7-130">例</span><span class="sxs-lookup"><span data-stu-id="793c7-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="793c7-131">要求</span><span class="sxs-lookup"><span data-stu-id="793c7-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_grouplifecyclepolicy"
}-->
```http
DELETE https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="793c7-132">応答</span><span class="sxs-lookup"><span data-stu-id="793c7-132">Response</span></span>

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
  "description": "Delete groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/grouplifecyclepolicy-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
