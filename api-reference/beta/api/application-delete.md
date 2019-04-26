---
title: アプリケーションを削除する
description: アプリケーションを削除します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 58b27088e5fc53b1be5f015aa2f7b194ab9825d4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322643"
---
# <a name="delete-application"></a><span data-ttu-id="c64ac-103">アプリケーションを削除する</span><span class="sxs-lookup"><span data-stu-id="c64ac-103">Delete application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c64ac-104">アプリケーションを削除します。</span><span class="sxs-lookup"><span data-stu-id="c64ac-104">Deletes an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="c64ac-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c64ac-105">Permissions</span></span>
<span data-ttu-id="c64ac-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c64ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c64ac-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c64ac-108">Permission type</span></span>      | <span data-ttu-id="c64ac-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c64ac-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c64ac-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c64ac-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c64ac-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c64ac-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c64ac-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c64ac-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c64ac-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c64ac-113">Not supported.</span></span>    |
|<span data-ttu-id="c64ac-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c64ac-114">Application</span></span> | <span data-ttu-id="c64ac-115">application.readwrite.ownedby、アプリケーションの読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="c64ac-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c64ac-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c64ac-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /applications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c64ac-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c64ac-117">Request headers</span></span>
| <span data-ttu-id="c64ac-118">名前</span><span class="sxs-lookup"><span data-stu-id="c64ac-118">Name</span></span>       | <span data-ttu-id="c64ac-119">型</span><span class="sxs-lookup"><span data-stu-id="c64ac-119">Type</span></span> | <span data-ttu-id="c64ac-120">説明</span><span class="sxs-lookup"><span data-stu-id="c64ac-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c64ac-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c64ac-121">Authorization</span></span>  | <span data-ttu-id="c64ac-122">string</span><span class="sxs-lookup"><span data-stu-id="c64ac-122">string</span></span>  | <span data-ttu-id="c64ac-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c64ac-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c64ac-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="c64ac-125">Request body</span></span>
<span data-ttu-id="c64ac-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c64ac-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c64ac-127">応答</span><span class="sxs-lookup"><span data-stu-id="c64ac-127">Response</span></span>

<span data-ttu-id="c64ac-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="c64ac-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c64ac-130">例</span><span class="sxs-lookup"><span data-stu-id="c64ac-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c64ac-131">要求</span><span class="sxs-lookup"><span data-stu-id="c64ac-131">Request</span></span>
<span data-ttu-id="c64ac-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c64ac-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_application"
}-->
```http
DELETE https://graph.microsoft.com/beta/applications/{id}
```
##### <a name="response"></a><span data-ttu-id="c64ac-133">応答</span><span class="sxs-lookup"><span data-stu-id="c64ac-133">Response</span></span>
<span data-ttu-id="c64ac-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="c64ac-134">Here is an example of the response.</span></span> 
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
  "description": "Delete application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
