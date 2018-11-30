---
title: ディレクトリ ロールのメンバーを削除する
description: directoryRole からメンバーを削除します。
ms.openlocfilehash: 9ef64e3aa1833fe78e5a035f7bd8ef4692fa371b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069581"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="27bfc-103">ディレクトリ ロールのメンバーを削除する</span><span class="sxs-lookup"><span data-stu-id="27bfc-103">Remove directory role member</span></span>

> <span data-ttu-id="27bfc-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="27bfc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="27bfc-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27bfc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="27bfc-106">directoryRole からメンバーを削除します。</span><span class="sxs-lookup"><span data-stu-id="27bfc-106">Remove a member from a directoryRole.</span></span>

## <a name="permissions"></a><span data-ttu-id="27bfc-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="27bfc-107">Permissions</span></span>

<span data-ttu-id="27bfc-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="27bfc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="27bfc-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="27bfc-110">Permission type</span></span>      | <span data-ttu-id="27bfc-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="27bfc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27bfc-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="27bfc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="27bfc-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="27bfc-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="27bfc-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="27bfc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27bfc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27bfc-115">Not supported.</span></span>    |
|<span data-ttu-id="27bfc-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="27bfc-116">Application</span></span> | <span data-ttu-id="27bfc-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27bfc-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="27bfc-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="27bfc-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryroles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="27bfc-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="27bfc-119">Request headers</span></span>

| <span data-ttu-id="27bfc-120">名前</span><span class="sxs-lookup"><span data-stu-id="27bfc-120">Name</span></span>       | <span data-ttu-id="27bfc-121">型</span><span class="sxs-lookup"><span data-stu-id="27bfc-121">Type</span></span> | <span data-ttu-id="27bfc-122">説明</span><span class="sxs-lookup"><span data-stu-id="27bfc-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="27bfc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="27bfc-123">Authorization</span></span>  | <span data-ttu-id="27bfc-124">string</span><span class="sxs-lookup"><span data-stu-id="27bfc-124">string</span></span>  | <span data-ttu-id="27bfc-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="27bfc-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="27bfc-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="27bfc-127">Request body</span></span>

<span data-ttu-id="27bfc-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="27bfc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27bfc-129">応答</span><span class="sxs-lookup"><span data-stu-id="27bfc-129">Response</span></span>

<span data-ttu-id="27bfc-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="27bfc-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27bfc-132">例</span><span class="sxs-lookup"><span data-stu-id="27bfc-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="27bfc-133">要求</span><span class="sxs-lookup"><span data-stu-id="27bfc-133">Request</span></span>

<span data-ttu-id="27bfc-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="27bfc-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole"
}-->

```http
DELETE https://graph.microsoft.com/beta/directoryroles/{id}/members/{id}/$ref
```

##### <a name="response"></a><span data-ttu-id="27bfc-135">応答</span><span class="sxs-lookup"><span data-stu-id="27bfc-135">Response</span></span>

<span data-ttu-id="27bfc-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="27bfc-136">Here is an example of the response.</span></span> 
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