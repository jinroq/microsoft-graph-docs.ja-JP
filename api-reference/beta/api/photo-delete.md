---
title: 写真を削除する
description: 写真を削除します。
localization_priority: Normal
ms.openlocfilehash: 117f4acbf5a45d9db64ccc5d3fc0ccc4d1c64896
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829261"
---
# <a name="delete-photo"></a><span data-ttu-id="16b9a-103">写真を削除する</span><span class="sxs-lookup"><span data-stu-id="16b9a-103">Delete photo</span></span>

> <span data-ttu-id="16b9a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="16b9a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16b9a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16b9a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="16b9a-106">写真を削除します。</span><span class="sxs-lookup"><span data-stu-id="16b9a-106">Delete a photo.</span></span>
## <a name="permissions"></a><span data-ttu-id="16b9a-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="16b9a-107">Permissions</span></span>
<span data-ttu-id="16b9a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="16b9a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16b9a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="16b9a-110">Permission type</span></span>      | <span data-ttu-id="16b9a-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="16b9a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16b9a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="16b9a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="16b9a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16b9a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="16b9a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="16b9a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16b9a-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16b9a-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="16b9a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="16b9a-116">Application</span></span> | <span data-ttu-id="16b9a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16b9a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="16b9a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="16b9a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/photo
DELETE /groups/{id}/photo
DELETE /drive/root/createdByUser/photo

```
## <a name="request-headers"></a><span data-ttu-id="16b9a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="16b9a-119">Request headers</span></span>
| <span data-ttu-id="16b9a-120">名前</span><span class="sxs-lookup"><span data-stu-id="16b9a-120">Name</span></span>       | <span data-ttu-id="16b9a-121">種類</span><span class="sxs-lookup"><span data-stu-id="16b9a-121">Type</span></span> | <span data-ttu-id="16b9a-122">説明</span><span class="sxs-lookup"><span data-stu-id="16b9a-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="16b9a-123">if-match</span><span class="sxs-lookup"><span data-stu-id="16b9a-123">if-match</span></span>  | <span data-ttu-id="16b9a-124">文字列</span><span class="sxs-lookup"><span data-stu-id="16b9a-124">string</span></span>  | <span data-ttu-id="16b9a-125">この要求ヘッダーが含まれていて、指定された eTag (または cTag) が項目の現在のタグに一致しない場合には、`412 Precondition Failed` 応答が返され、項目は削除されません。</span><span class="sxs-lookup"><span data-stu-id="16b9a-125">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>|
| <span data-ttu-id="16b9a-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="16b9a-126">Authorization</span></span>  | <span data-ttu-id="16b9a-127">string</span><span class="sxs-lookup"><span data-stu-id="16b9a-127">string</span></span>  | <span data-ttu-id="16b9a-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="16b9a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="16b9a-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="16b9a-130">Request body</span></span>
<span data-ttu-id="16b9a-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="16b9a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16b9a-132">応答</span><span class="sxs-lookup"><span data-stu-id="16b9a-132">Response</span></span>

<span data-ttu-id="16b9a-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="16b9a-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16b9a-135">例</span><span class="sxs-lookup"><span data-stu-id="16b9a-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="16b9a-136">要求</span><span class="sxs-lookup"><span data-stu-id="16b9a-136">Request</span></span>
<span data-ttu-id="16b9a-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="16b9a-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_photo"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="16b9a-138">応答</span><span class="sxs-lookup"><span data-stu-id="16b9a-138">Response</span></span>
<span data-ttu-id="16b9a-139">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="16b9a-139">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
