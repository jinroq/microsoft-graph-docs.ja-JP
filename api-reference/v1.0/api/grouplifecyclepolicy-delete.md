---
title: Delete groupLifecyclePolicy
description: groupLifecyclePolicy を削除します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 9d58eca82c72008cb30095fe4fbfacf5a382111a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567439"
---
# <a name="delete-grouplifecyclepolicy"></a><span data-ttu-id="a3bca-103">Delete groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="a3bca-103">Delete groupLifecyclePolicy</span></span>

<span data-ttu-id="a3bca-104">[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="a3bca-104">Deletes a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a3bca-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a3bca-105">Permissions</span></span>

<span data-ttu-id="a3bca-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a3bca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3bca-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a3bca-108">Permission type</span></span>      | <span data-ttu-id="a3bca-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a3bca-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3bca-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a3bca-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a3bca-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3bca-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="a3bca-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a3bca-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3bca-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3bca-113">Not supported.</span></span>    |
|<span data-ttu-id="a3bca-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a3bca-114">Application</span></span> | <span data-ttu-id="a3bca-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3bca-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3bca-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a3bca-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupLifecyclePolicies/{id}

```

## <a name="request-headers"></a><span data-ttu-id="a3bca-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a3bca-117">Request headers</span></span>

| <span data-ttu-id="a3bca-118">名前</span><span class="sxs-lookup"><span data-stu-id="a3bca-118">Name</span></span> | <span data-ttu-id="a3bca-119">説明</span><span class="sxs-lookup"><span data-stu-id="a3bca-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="a3bca-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3bca-120">Authorization</span></span> | <span data-ttu-id="a3bca-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a3bca-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a3bca-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a3bca-123">Content-Type</span></span>  | <span data-ttu-id="a3bca-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a3bca-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a3bca-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a3bca-125">Request body</span></span>
<span data-ttu-id="a3bca-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a3bca-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="a3bca-127">応答</span><span class="sxs-lookup"><span data-stu-id="a3bca-127">Response</span></span>

<span data-ttu-id="a3bca-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="a3bca-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3bca-130">例</span><span class="sxs-lookup"><span data-stu-id="a3bca-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a3bca-131">要求</span><span class="sxs-lookup"><span data-stu-id="a3bca-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_grouplifecyclepolicy"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="a3bca-132">応答</span><span class="sxs-lookup"><span data-stu-id="a3bca-132">Response</span></span>

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
