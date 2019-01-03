---
title: AcceptedSender の削除
description: 'AcceptedSenders リストからユーザーまたはグループを削除します。 '
author: dkershaw10
ms.openlocfilehash: 7028f2f63e340c9f5c3f300f6e3724a05f87d288
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313910"
---
# <a name="remove-acceptedsender"></a><span data-ttu-id="f5384-103">AcceptedSender の削除</span><span class="sxs-lookup"><span data-stu-id="f5384-103">Remove acceptedSender</span></span>

> <span data-ttu-id="f5384-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f5384-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5384-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f5384-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f5384-106">AcceptedSenders リストからユーザーまたはグループを削除します。</span><span class="sxs-lookup"><span data-stu-id="f5384-106">Remove a user or group from the acceptedSenders list.</span></span> 

## <a name="permissions"></a><span data-ttu-id="f5384-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f5384-107">Permissions</span></span>
<span data-ttu-id="f5384-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f5384-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f5384-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f5384-110">Permission type</span></span>                        | <span data-ttu-id="f5384-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f5384-111">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="f5384-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f5384-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f5384-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5384-113">Group.ReadWrite.All</span></span>    |
| <span data-ttu-id="f5384-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f5384-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5384-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f5384-115">Not supported.</span></span>|
| <span data-ttu-id="f5384-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f5384-116">Application</span></span>                            | <span data-ttu-id="f5384-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f5384-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5384-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f5384-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/acceptedSenders/$ref?$id=<id>
```

## <a name="request-headers"></a><span data-ttu-id="f5384-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f5384-119">Request headers</span></span>
| <span data-ttu-id="f5384-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f5384-120">Header</span></span>         | <span data-ttu-id="f5384-121">値</span><span class="sxs-lookup"><span data-stu-id="f5384-121">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="f5384-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5384-122">Authorization</span></span>  | <span data-ttu-id="f5384-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f5384-p103">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="f5384-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="f5384-125">Request body</span></span>
<span data-ttu-id="f5384-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f5384-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5384-127">応答</span><span class="sxs-lookup"><span data-stu-id="f5384-127">Response</span></span>
<span data-ttu-id="f5384-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="f5384-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5384-130">例</span><span class="sxs-lookup"><span data-stu-id="f5384-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f5384-131">要求</span><span class="sxs-lookup"><span data-stu-id="f5384-131">Request</span></span>
<span data-ttu-id="f5384-132">要求のいくつかの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f5384-132">The following are a couple of examples of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{id}

DELETE https://graph.microsoft.com/beta/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/beta/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="f5384-133">応答</span><span class="sxs-lookup"><span data-stu-id="f5384-133">Response</span></span>
<span data-ttu-id="f5384-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f5384-134">The following is an example of the response.</span></span> 

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
  "description": "Create acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->