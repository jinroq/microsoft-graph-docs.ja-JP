---
title: OrgContact を削除します。
description: OrgContact を削除します。
ms.openlocfilehash: 3119fa26874e872961f7ee91681377537f855549
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073354"
---
# <a name="delete-orgcontact"></a><span data-ttu-id="d9379-103">OrgContact を削除します。</span><span class="sxs-lookup"><span data-stu-id="d9379-103">Delete orgContact</span></span>

> <span data-ttu-id="d9379-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d9379-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d9379-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d9379-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d9379-106">OrgContact を削除します。</span><span class="sxs-lookup"><span data-stu-id="d9379-106">Delete orgContact.</span></span>
## <a name="permissions"></a><span data-ttu-id="d9379-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d9379-107">Permissions</span></span>
<span data-ttu-id="d9379-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d9379-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9379-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d9379-110">Permission type</span></span>      | <span data-ttu-id="d9379-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d9379-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9379-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d9379-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d9379-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d9379-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d9379-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d9379-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9379-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d9379-115">Not supported.</span></span>    |
|<span data-ttu-id="d9379-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d9379-116">Application</span></span> | <span data-ttu-id="d9379-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d9379-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9379-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d9379-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /contacts/{id}

```
## <a name="request-headers"></a><span data-ttu-id="d9379-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d9379-119">Request headers</span></span>
| <span data-ttu-id="d9379-120">名前</span><span class="sxs-lookup"><span data-stu-id="d9379-120">Name</span></span>       | <span data-ttu-id="d9379-121">型</span><span class="sxs-lookup"><span data-stu-id="d9379-121">Type</span></span> | <span data-ttu-id="d9379-122">説明</span><span class="sxs-lookup"><span data-stu-id="d9379-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d9379-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9379-123">Authorization</span></span>  | <span data-ttu-id="d9379-124">string</span><span class="sxs-lookup"><span data-stu-id="d9379-124">string</span></span>  | <span data-ttu-id="d9379-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d9379-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9379-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d9379-127">Request body</span></span>
<span data-ttu-id="d9379-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d9379-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9379-129">応答</span><span class="sxs-lookup"><span data-stu-id="d9379-129">Response</span></span>

<span data-ttu-id="d9379-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="d9379-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9379-132">例</span><span class="sxs-lookup"><span data-stu-id="d9379-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d9379-133">要求</span><span class="sxs-lookup"><span data-stu-id="d9379-133">Request</span></span>
<span data-ttu-id="d9379-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d9379-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_orgcontact"
}-->
```http
DELETE https://graph.microsoft.com/beta/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="d9379-135">応答</span><span class="sxs-lookup"><span data-stu-id="d9379-135">Response</span></span>
<span data-ttu-id="d9379-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="d9379-136">Here is an example of the response.</span></span> 
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
  "description": "Delete orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->