---
title: orgcontact の削除
description: orgcontact を削除します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8a76d68e53ea5de3aa71b1673dbbf6287ab1aa30
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338055"
---
# <a name="delete-orgcontact"></a><span data-ttu-id="66a0e-103">orgcontact の削除</span><span class="sxs-lookup"><span data-stu-id="66a0e-103">Delete orgContact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66a0e-104">orgcontact を削除します。</span><span class="sxs-lookup"><span data-stu-id="66a0e-104">Delete orgContact.</span></span>
## <a name="permissions"></a><span data-ttu-id="66a0e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="66a0e-105">Permissions</span></span>
<span data-ttu-id="66a0e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="66a0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66a0e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="66a0e-108">Permission type</span></span>      | <span data-ttu-id="66a0e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="66a0e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66a0e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="66a0e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="66a0e-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="66a0e-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="66a0e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="66a0e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66a0e-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66a0e-113">Not supported.</span></span>    |
|<span data-ttu-id="66a0e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="66a0e-114">Application</span></span> | <span data-ttu-id="66a0e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66a0e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="66a0e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="66a0e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /contacts/{id}

```
## <a name="request-headers"></a><span data-ttu-id="66a0e-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="66a0e-117">Request headers</span></span>
| <span data-ttu-id="66a0e-118">名前</span><span class="sxs-lookup"><span data-stu-id="66a0e-118">Name</span></span>       | <span data-ttu-id="66a0e-119">型</span><span class="sxs-lookup"><span data-stu-id="66a0e-119">Type</span></span> | <span data-ttu-id="66a0e-120">説明</span><span class="sxs-lookup"><span data-stu-id="66a0e-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="66a0e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="66a0e-121">Authorization</span></span>  | <span data-ttu-id="66a0e-122">string</span><span class="sxs-lookup"><span data-stu-id="66a0e-122">string</span></span>  | <span data-ttu-id="66a0e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="66a0e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66a0e-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="66a0e-125">Request body</span></span>
<span data-ttu-id="66a0e-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="66a0e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66a0e-127">応答</span><span class="sxs-lookup"><span data-stu-id="66a0e-127">Response</span></span>

<span data-ttu-id="66a0e-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="66a0e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66a0e-130">例</span><span class="sxs-lookup"><span data-stu-id="66a0e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="66a0e-131">要求</span><span class="sxs-lookup"><span data-stu-id="66a0e-131">Request</span></span>
<span data-ttu-id="66a0e-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="66a0e-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_orgcontact"
}-->
```http
DELETE https://graph.microsoft.com/beta/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="66a0e-133">応答</span><span class="sxs-lookup"><span data-stu-id="66a0e-133">Response</span></span>
<span data-ttu-id="66a0e-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="66a0e-134">Here is an example of the response.</span></span> 
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
  "description": "Delete orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
