---
title: グループ設定の削除
description: グループ設定を削除します。
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 55a9c1d51e03eaea785d351c0700803915b2fe33
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839068"
---
# <a name="delete-a-group-setting"></a><span data-ttu-id="71013-103">グループ設定の削除</span><span class="sxs-lookup"><span data-stu-id="71013-103">Delete a group setting</span></span>

<span data-ttu-id="71013-104">グループ設定を削除します。</span><span class="sxs-lookup"><span data-stu-id="71013-104">Delete a group setting.</span></span>

## <a name="permissions"></a><span data-ttu-id="71013-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="71013-105">Permissions</span></span>

<span data-ttu-id="71013-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="71013-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="71013-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="71013-108">Permission type</span></span>      | <span data-ttu-id="71013-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="71013-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71013-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="71013-110">Delegated (work or school account)</span></span> | <span data-ttu-id="71013-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="71013-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="71013-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="71013-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71013-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="71013-113">Not supported.</span></span>    |
|<span data-ttu-id="71013-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="71013-114">Application</span></span> | <span data-ttu-id="71013-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71013-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="71013-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="71013-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupSettings/{id}
DELETE /groups/{id}/settings/{id}

```

## <a name="request-headers"></a><span data-ttu-id="71013-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="71013-117">Request headers</span></span>

| <span data-ttu-id="71013-118">名前</span><span class="sxs-lookup"><span data-stu-id="71013-118">Name</span></span> | <span data-ttu-id="71013-119">説明</span><span class="sxs-lookup"><span data-stu-id="71013-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="71013-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="71013-120">Authorization</span></span>  | <span data-ttu-id="71013-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="71013-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="71013-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="71013-123">Content-Type</span></span>  | <span data-ttu-id="71013-124">application/json</span><span class="sxs-lookup"><span data-stu-id="71013-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="71013-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="71013-125">Request body</span></span>
<span data-ttu-id="71013-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="71013-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71013-127">応答</span><span class="sxs-lookup"><span data-stu-id="71013-127">Response</span></span>

<span data-ttu-id="71013-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="71013-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71013-130">例</span><span class="sxs-lookup"><span data-stu-id="71013-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="71013-131">要求</span><span class="sxs-lookup"><span data-stu-id="71013-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_groupsetting"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupSettings/{id}
```
##### <a name="response"></a><span data-ttu-id="71013-132">応答</span><span class="sxs-lookup"><span data-stu-id="71013-132">Response</span></span>
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
  "description": "Delete groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
