---
title: ディレクトリ ロールのメンバーを削除する
description: directoryRole からメンバーを削除します。
author: lleonard-msft
ms.openlocfilehash: c2b0f8896ca2cc13ebb9f53900638875ade365bd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302416"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="486ef-103">ディレクトリ ロールのメンバーを削除する</span><span class="sxs-lookup"><span data-stu-id="486ef-103">Remove directory role member</span></span>

> <span data-ttu-id="486ef-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="486ef-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="486ef-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="486ef-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="486ef-106">directoryRole からメンバーを削除します。</span><span class="sxs-lookup"><span data-stu-id="486ef-106">Remove a member from a directoryRole.</span></span>

## <a name="permissions"></a><span data-ttu-id="486ef-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="486ef-107">Permissions</span></span>

<span data-ttu-id="486ef-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="486ef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="486ef-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="486ef-110">Permission type</span></span>      | <span data-ttu-id="486ef-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="486ef-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="486ef-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="486ef-112">Delegated (work or school account)</span></span> | <span data-ttu-id="486ef-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="486ef-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="486ef-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="486ef-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="486ef-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="486ef-115">Not supported.</span></span>    |
|<span data-ttu-id="486ef-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="486ef-116">Application</span></span> | <span data-ttu-id="486ef-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="486ef-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="486ef-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="486ef-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryroles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="486ef-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="486ef-119">Request headers</span></span>

| <span data-ttu-id="486ef-120">名前</span><span class="sxs-lookup"><span data-stu-id="486ef-120">Name</span></span>       | <span data-ttu-id="486ef-121">種類</span><span class="sxs-lookup"><span data-stu-id="486ef-121">Type</span></span> | <span data-ttu-id="486ef-122">説明</span><span class="sxs-lookup"><span data-stu-id="486ef-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="486ef-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="486ef-123">Authorization</span></span>  | <span data-ttu-id="486ef-124">string</span><span class="sxs-lookup"><span data-stu-id="486ef-124">string</span></span>  | <span data-ttu-id="486ef-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="486ef-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="486ef-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="486ef-127">Request body</span></span>

<span data-ttu-id="486ef-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="486ef-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="486ef-129">応答</span><span class="sxs-lookup"><span data-stu-id="486ef-129">Response</span></span>

<span data-ttu-id="486ef-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="486ef-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="486ef-132">例</span><span class="sxs-lookup"><span data-stu-id="486ef-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="486ef-133">要求</span><span class="sxs-lookup"><span data-stu-id="486ef-133">Request</span></span>

<span data-ttu-id="486ef-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="486ef-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole"
}-->

```http
DELETE https://graph.microsoft.com/beta/directoryroles/{id}/members/{id}/$ref
```

##### <a name="response"></a><span data-ttu-id="486ef-135">応答</span><span class="sxs-lookup"><span data-stu-id="486ef-135">Response</span></span>

<span data-ttu-id="486ef-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="486ef-136">Here is an example of the response.</span></span> 
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
  "description": "Delete a member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->