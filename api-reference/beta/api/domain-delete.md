---
title: ドメインを削除する
description: テナントからドメインを削除します。
ms.openlocfilehash: 2ed3772d767099e8ccd7fd5453c7a8231c9ea96c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069886"
---
# <a name="delete-domain"></a><span data-ttu-id="888e1-103">ドメインを削除する</span><span class="sxs-lookup"><span data-stu-id="888e1-103">Delete domain</span></span>

> <span data-ttu-id="888e1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="888e1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="888e1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="888e1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="888e1-106">テナントからドメインを削除します。</span><span class="sxs-lookup"><span data-stu-id="888e1-106">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="888e1-107">**重要な:** 削除されたドメインは、回復可能ではありません。</span><span class="sxs-lookup"><span data-stu-id="888e1-107">**Important:** Deleted domains are not recoverable.</span></span>

## <a name="permissions"></a><span data-ttu-id="888e1-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="888e1-108">Permissions</span></span>

<span data-ttu-id="888e1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="888e1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="888e1-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="888e1-111">Permission type</span></span>      | <span data-ttu-id="888e1-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="888e1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="888e1-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="888e1-113">Delegated (work or school account)</span></span> | <span data-ttu-id="888e1-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="888e1-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="888e1-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="888e1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="888e1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="888e1-116">Not supported.</span></span>    |
|<span data-ttu-id="888e1-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="888e1-117">Application</span></span> | <span data-ttu-id="888e1-118">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="888e1-118">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="888e1-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="888e1-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="888e1-120">{Id} には、ドメインを完全修飾ドメイン名で指定します。</span><span class="sxs-lookup"><span data-stu-id="888e1-120">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="888e1-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="888e1-121">Request headers</span></span>

| <span data-ttu-id="888e1-122">名前</span><span class="sxs-lookup"><span data-stu-id="888e1-122">Name</span></span>       | <span data-ttu-id="888e1-123">説明</span><span class="sxs-lookup"><span data-stu-id="888e1-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="888e1-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="888e1-124">Authorization</span></span>  | <span data-ttu-id="888e1-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="888e1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="888e1-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="888e1-127">Content-Type</span></span>  | <span data-ttu-id="888e1-128">application/json</span><span class="sxs-lookup"><span data-stu-id="888e1-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="888e1-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="888e1-129">Request body</span></span>

<span data-ttu-id="888e1-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="888e1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="888e1-131">応答</span><span class="sxs-lookup"><span data-stu-id="888e1-131">Response</span></span>

<span data-ttu-id="888e1-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文は返されません。</span><span class="sxs-lookup"><span data-stu-id="888e1-p104">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="888e1-134">例</span><span class="sxs-lookup"><span data-stu-id="888e1-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="888e1-135">要求</span><span class="sxs-lookup"><span data-stu-id="888e1-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/beta/domains/contoso.com
```

##### <a name="response"></a><span data-ttu-id="888e1-136">応答</span><span class="sxs-lookup"><span data-stu-id="888e1-136">Response</span></span>

<span data-ttu-id="888e1-p105">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="888e1-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->