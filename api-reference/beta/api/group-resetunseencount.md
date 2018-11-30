---
title: 'グループ: resetUnseenCount'
description: 最後の訪問から現在のユーザーが認識されていないすべての投稿の unseenCount をリセットします。 Office 365 のグループのみをサポートします。
ms.openlocfilehash: b6218176f097759870aad4a3a2908759862002e2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073756"
---
# <a name="group-resetunseencount"></a><span data-ttu-id="a3008-104">グループ: resetUnseenCount</span><span class="sxs-lookup"><span data-stu-id="a3008-104">group: resetUnseenCount</span></span>

> <span data-ttu-id="a3008-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a3008-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a3008-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3008-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a3008-107">最後の訪問から現在のユーザーが認識されていないすべての投稿の unseenCount をリセットします。</span><span class="sxs-lookup"><span data-stu-id="a3008-107">Reset the unseenCount of all the posts that the current user has not seen since their last visit.</span></span> <span data-ttu-id="a3008-108">Office 365 のグループのみをサポートします。</span><span class="sxs-lookup"><span data-stu-id="a3008-108">Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3008-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a3008-109">Permissions</span></span>
<span data-ttu-id="a3008-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a3008-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3008-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a3008-112">Permission type</span></span>      | <span data-ttu-id="a3008-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a3008-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3008-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a3008-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a3008-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3008-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a3008-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a3008-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3008-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3008-117">Not supported.</span></span>    |
|<span data-ttu-id="a3008-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a3008-118">Application</span></span> | <span data-ttu-id="a3008-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3008-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3008-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a3008-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/resetUnseenCount
```
## <a name="request-headers"></a><span data-ttu-id="a3008-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a3008-121">Request headers</span></span>
| <span data-ttu-id="a3008-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a3008-122">Header</span></span>       | <span data-ttu-id="a3008-123">値</span><span class="sxs-lookup"><span data-stu-id="a3008-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a3008-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3008-124">Authorization</span></span>  | <span data-ttu-id="a3008-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a3008-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a3008-127">Prefer</span><span class="sxs-lookup"><span data-stu-id="a3008-127">Prefer</span></span> | <span data-ttu-id="a3008-128">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="a3008-128">return=minimal.</span></span> <span data-ttu-id="a3008-129">最小応答ヘッダーが要求ヘッダーに含まれている場合、正常な応答で `204 No Content` コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="a3008-129">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="a3008-130">省略可能。</span><span class="sxs-lookup"><span data-stu-id="a3008-130">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="a3008-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="a3008-131">Request body</span></span>
<span data-ttu-id="a3008-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a3008-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3008-133">応答</span><span class="sxs-lookup"><span data-stu-id="a3008-133">Response</span></span>
<span data-ttu-id="a3008-p107">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="a3008-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3008-136">例</span><span class="sxs-lookup"><span data-stu-id="a3008-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a3008-137">要求</span><span class="sxs-lookup"><span data-stu-id="a3008-137">Request</span></span>
<span data-ttu-id="a3008-138">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a3008-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_resetunseencount"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/resetUnseenCount
```

#### <a name="response"></a><span data-ttu-id="a3008-139">応答</span><span class="sxs-lookup"><span data-stu-id="a3008-139">Response</span></span>
<span data-ttu-id="a3008-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a3008-140">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: resetUnseenCount",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->