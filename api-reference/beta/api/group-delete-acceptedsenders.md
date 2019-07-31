---
title: AcceptedSender の削除
description: '承認済み送信者リストからユーザーまたはグループを削除します。 '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 341f887de0252dd6ae1ebc9f899263c67716658f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954031"
---
# <a name="remove-acceptedsender"></a><span data-ttu-id="15549-103">AcceptedSender の削除</span><span class="sxs-lookup"><span data-stu-id="15549-103">Remove acceptedSender</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15549-104">指定したグループの承認済み送信者リストからユーザーまたはグループを削除します。</span><span class="sxs-lookup"><span data-stu-id="15549-104">Remove a user or group from the accepted-senders list of the specified group.</span></span> 

## <a name="permissions"></a><span data-ttu-id="15549-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="15549-105">Permissions</span></span>
<span data-ttu-id="15549-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="15549-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="15549-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="15549-108">Permission type</span></span>                        | <span data-ttu-id="15549-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="15549-109">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="15549-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="15549-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="15549-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15549-111">Group.ReadWrite.All</span></span>    |
| <span data-ttu-id="15549-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="15549-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15549-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15549-113">Not supported.</span></span>|
| <span data-ttu-id="15549-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="15549-114">Application</span></span>                            | <span data-ttu-id="15549-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15549-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15549-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="15549-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/acceptedSenders/$ref?$id={id}
```

## <a name="request-headers"></a><span data-ttu-id="15549-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="15549-117">Request headers</span></span>
| <span data-ttu-id="15549-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="15549-118">Header</span></span>         | <span data-ttu-id="15549-119">値</span><span class="sxs-lookup"><span data-stu-id="15549-119">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="15549-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="15549-120">Authorization</span></span>  | <span data-ttu-id="15549-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="15549-p102">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="15549-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="15549-123">Request body</span></span>
<span data-ttu-id="15549-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="15549-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15549-125">応答</span><span class="sxs-lookup"><span data-stu-id="15549-125">Response</span></span>
<span data-ttu-id="15549-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="15549-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="15549-128">例</span><span class="sxs-lookup"><span data-stu-id="15549-128">Examples</span></span>
### <a name="example-1-remove-a-user-from-the-accepted-senders-list-for-the-group"></a><span data-ttu-id="15549-129">例 1: グループの承認済み送信者リストからユーザーを削除します。</span><span class="sxs-lookup"><span data-stu-id="15549-129">Example 1: Remove a user from the accepted-senders list for the group.</span></span>
#### <a name="request"></a><span data-ttu-id="15549-130">要求</span><span class="sxs-lookup"><span data-stu-id="15549-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_user_from_acceptedsenderslist_of_group"
}-->
```http
DELETE https://graph/microsoft.com/beta/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{user-id}
```

#### <a name="response"></a><span data-ttu-id="15549-131">応答</span><span class="sxs-lookup"><span data-stu-id="15549-131">Response</span></span>
<span data-ttu-id="15549-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="15549-132">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "name": "remove_user_from_acceptedsenderslist_of_group",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-remove-a-group-from-the-accepted-senders-list-for-the-group"></a><span data-ttu-id="15549-133">例 2: グループの承認済み送信者リストからグループを削除します。</span><span class="sxs-lookup"><span data-stu-id="15549-133">Example 2: Remove a group from the accepted-senders list for the group.</span></span>
#### <a name="request"></a><span data-ttu-id="15549-134">要求</span><span class="sxs-lookup"><span data-stu-id="15549-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_group_from_acceptedsenderslist_of_group"
}-->
```http
DELETE https://graph/microsoft.com/beta/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/beta/groups/{other-group-id}
```

#### <a name="response"></a><span data-ttu-id="15549-135">応答</span><span class="sxs-lookup"><span data-stu-id="15549-135">Response</span></span>
<span data-ttu-id="15549-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="15549-136">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "name": "remove_group_from_acceptedsenderslist_of_group",
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
  "description": "Remove acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
