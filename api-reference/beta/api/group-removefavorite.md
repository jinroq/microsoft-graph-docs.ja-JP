---
title: 'グループ: removeFavorite'
description: 現在のユーザーのお気に入りのグループ一覧からグループを削除します。Office 365 のグループのみをサポートします。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 9ed755add4771b062d004aaa35c55b9afd23a390
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951020"
---
# <a name="group-removefavorite"></a><span data-ttu-id="449e5-104">グループ: removeFavorite</span><span class="sxs-lookup"><span data-stu-id="449e5-104">group: removeFavorite</span></span>

> <span data-ttu-id="449e5-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="449e5-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="449e5-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="449e5-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="449e5-p103">現在のユーザーのお気に入りのグループ一覧からグループを削除します。Office 365 のグループのみをサポートします。</span><span class="sxs-lookup"><span data-stu-id="449e5-p103">Remove the group from the list of the current user's favorite groups. Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="449e5-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="449e5-109">Permissions</span></span>
<span data-ttu-id="449e5-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="449e5-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="449e5-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="449e5-112">Permission type</span></span>      | <span data-ttu-id="449e5-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="449e5-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="449e5-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="449e5-114">Delegated (work or school account)</span></span> | <span data-ttu-id="449e5-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="449e5-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="449e5-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="449e5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="449e5-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="449e5-117">Not supported.</span></span>    |
|<span data-ttu-id="449e5-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="449e5-118">Application</span></span> | <span data-ttu-id="449e5-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="449e5-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="449e5-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="449e5-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/removeFavorite
```

## <a name="request-headers"></a><span data-ttu-id="449e5-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="449e5-121">Request headers</span></span>
| <span data-ttu-id="449e5-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="449e5-122">Header</span></span>       | <span data-ttu-id="449e5-123">値</span><span class="sxs-lookup"><span data-stu-id="449e5-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="449e5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="449e5-124">Authorization</span></span>  | <span data-ttu-id="449e5-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="449e5-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="449e5-127">Prefer</span><span class="sxs-lookup"><span data-stu-id="449e5-127">Prefer</span></span> | <span data-ttu-id="449e5-128">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="449e5-128">return=minimal.</span></span> <span data-ttu-id="449e5-129">最小応答ヘッダーが要求ヘッダーに含まれている場合、正常な応答で `204 No Content` コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="449e5-129">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="449e5-130">省略可能。</span><span class="sxs-lookup"><span data-stu-id="449e5-130">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="449e5-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="449e5-131">Request body</span></span>
<span data-ttu-id="449e5-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="449e5-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="449e5-133">応答</span><span class="sxs-lookup"><span data-stu-id="449e5-133">Response</span></span>
<span data-ttu-id="449e5-p107">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="449e5-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="449e5-136">例</span><span class="sxs-lookup"><span data-stu-id="449e5-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="449e5-137">要求</span><span class="sxs-lookup"><span data-stu-id="449e5-137">Request</span></span>
<span data-ttu-id="449e5-138">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="449e5-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_removefavorite"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/removeFavorite
```

#### <a name="response"></a><span data-ttu-id="449e5-139">応答</span><span class="sxs-lookup"><span data-stu-id="449e5-139">Response</span></span>
<span data-ttu-id="449e5-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="449e5-140">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: removeFavorite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
