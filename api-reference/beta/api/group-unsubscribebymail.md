---
title: 'グループ: unsubscribeByMail'
description: 'このメソッドを呼び出すと、そのグループ内の新規投稿、イベント、およびファイルには、このグループの電子メール通知を受信する現在のユーザーが無効になります。 Office 365 のグループのみをサポートします。 '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 34f231c4b2daa3faf2dc8a375bf397dc32225f01
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916500"
---
# <a name="group-unsubscribebymail"></a><span data-ttu-id="5d2f4-104">グループ: unsubscribeByMail</span><span class="sxs-lookup"><span data-stu-id="5d2f4-104">group: unsubscribeByMail</span></span>

> <span data-ttu-id="5d2f4-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5d2f4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5d2f4-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5d2f4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5d2f4-107">このメソッドを呼び出すと、そのグループ内の新規投稿、イベント、およびファイルには、このグループの電子メール通知を受信する現在のユーザーが無効になります。</span><span class="sxs-lookup"><span data-stu-id="5d2f4-107">Calling this method will disable the current user to receive email notifications for this group about new posts, events, and files in that group.</span></span> <span data-ttu-id="5d2f4-108">Office 365 のグループのみをサポートします。</span><span class="sxs-lookup"><span data-stu-id="5d2f4-108">Supported for Office 365 groups only.</span></span> 

## <a name="permissions"></a><span data-ttu-id="5d2f4-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5d2f4-109">Permissions</span></span>
<span data-ttu-id="5d2f4-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5d2f4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d2f4-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5d2f4-112">Permission type</span></span>      | <span data-ttu-id="5d2f4-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5d2f4-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d2f4-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5d2f4-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5d2f4-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d2f4-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5d2f4-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5d2f4-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d2f4-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5d2f4-117">Not supported.</span></span>    |
|<span data-ttu-id="5d2f4-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5d2f4-118">Application</span></span> | <span data-ttu-id="5d2f4-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d2f4-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d2f4-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5d2f4-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/unsubscribeByMail
```

## <a name="request-headers"></a><span data-ttu-id="5d2f4-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5d2f4-121">Request headers</span></span>
| <span data-ttu-id="5d2f4-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5d2f4-122">Header</span></span>       | <span data-ttu-id="5d2f4-123">値</span><span class="sxs-lookup"><span data-stu-id="5d2f4-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5d2f4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d2f4-124">Authorization</span></span>  | <span data-ttu-id="5d2f4-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5d2f4-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5d2f4-127">Prefer</span><span class="sxs-lookup"><span data-stu-id="5d2f4-127">Prefer</span></span> | <span data-ttu-id="5d2f4-128">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="5d2f4-128">return=minimal.</span></span> <span data-ttu-id="5d2f4-129">最小応答ヘッダーが要求ヘッダーに含まれている場合、正常な応答で `204 No Content` コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="5d2f4-129">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="5d2f4-130">省略可能。</span><span class="sxs-lookup"><span data-stu-id="5d2f4-130">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="5d2f4-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="5d2f4-131">Request body</span></span>
 <span data-ttu-id="5d2f4-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5d2f4-132">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="5d2f4-133">応答</span><span class="sxs-lookup"><span data-stu-id="5d2f4-133">Response</span></span>
<span data-ttu-id="5d2f4-p107">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="5d2f4-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d2f4-136">例</span><span class="sxs-lookup"><span data-stu-id="5d2f4-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="5d2f4-137">要求</span><span class="sxs-lookup"><span data-stu-id="5d2f4-137">Request</span></span>
<span data-ttu-id="5d2f4-138">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5d2f4-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_unsubscribebymail"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/unsubscribeByMail
```

#### <a name="response"></a><span data-ttu-id="5d2f4-139">応答</span><span class="sxs-lookup"><span data-stu-id="5d2f4-139">Response</span></span>
<span data-ttu-id="5d2f4-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5d2f4-140">The following is an example of the response.</span></span> 
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
  "description": "group: unsubscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
