---
title: rejectedSender の削除
description: rejectedSenders リストからユーザーまたはグループを削除します。
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 6033b1991807aac1b3edfff10ff407f0b667df7f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830528"
---
# <a name="remove-rejectedsender"></a><span data-ttu-id="93add-103">rejectedSender の削除</span><span class="sxs-lookup"><span data-stu-id="93add-103">Remove rejectedSender</span></span>
<span data-ttu-id="93add-104">rejectedSenders リストからユーザーまたはグループを削除します。</span><span class="sxs-lookup"><span data-stu-id="93add-104">Remove a user or group from the rejectedSenders list.</span></span>

## <a name="permissions"></a><span data-ttu-id="93add-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="93add-105">Permissions</span></span>
<span data-ttu-id="93add-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="93add-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="93add-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="93add-108">Permission type</span></span>                        | <span data-ttu-id="93add-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="93add-109">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="93add-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="93add-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="93add-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93add-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="93add-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="93add-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93add-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="93add-113">Not supported.</span></span> |
| <span data-ttu-id="93add-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="93add-114">Application</span></span>                            | <span data-ttu-id="93add-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="93add-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="93add-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="93add-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/v1.0/users/{user-id}
DELETE /groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/v1.0/groups/{other-group-id}
```

## <a name="request-headers"></a><span data-ttu-id="93add-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="93add-117">Request headers</span></span>

| <span data-ttu-id="93add-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="93add-118">Header</span></span>         | <span data-ttu-id="93add-119">値</span><span class="sxs-lookup"><span data-stu-id="93add-119">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="93add-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="93add-120">Authorization</span></span>  | <span data-ttu-id="93add-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="93add-p102">Bearer {token}. Required.</span></span> 

## <a name="request-body"></a><span data-ttu-id="93add-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="93add-123">Request body</span></span>
<span data-ttu-id="93add-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="93add-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93add-125">応答</span><span class="sxs-lookup"><span data-stu-id="93add-125">Response</span></span>
<span data-ttu-id="93add-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="93add-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93add-128">例</span><span class="sxs-lookup"><span data-stu-id="93add-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="93add-129">要求</span><span class="sxs-lookup"><span data-stu-id="93add-129">Request</span></span>
<span data-ttu-id="93add-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="93add-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "remove_rejectedSender_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/v1.0/users/{user-id}
```

#### <a name="response"></a><span data-ttu-id="93add-131">応答</span><span class="sxs-lookup"><span data-stu-id="93add-131">Response</span></span>
<span data-ttu-id="93add-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="93add-132">The following is an example of the response.</span></span> 
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
  "description": "Remove rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
