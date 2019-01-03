---
title: オーディオのルーティング グループを削除します。
description: 指定されたオーディオのルーティング グループを削除します。
author: VinodRavichandran
ms.openlocfilehash: a21c90722b63d582f3c76ff518bcc68837135593
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380374"
---
# <a name="delete-audio-routing-group"></a><span data-ttu-id="0a55e-103">オーディオのルーティング グループを削除します。</span><span class="sxs-lookup"><span data-stu-id="0a55e-103">Delete audio routing group</span></span>

> <span data-ttu-id="0a55e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0a55e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a55e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a55e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0a55e-106">指定した[audioRoutingGroup](../resources/audioroutinggroup.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="0a55e-106">Delete the specified [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0a55e-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0a55e-107">Permissions</span></span>
<span data-ttu-id="0a55e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0a55e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0a55e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0a55e-110">Permission type</span></span> | <span data-ttu-id="0a55e-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0a55e-111">Permissions (from least to most privileged)</span></span>  |
| :-------------- | :------------------------------------------- |
| <span data-ttu-id="0a55e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0a55e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="0a55e-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="0a55e-113">Not Supported</span></span>        |
| <span data-ttu-id="0a55e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0a55e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a55e-115">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="0a55e-115">Not Supported</span></span>        |
| <span data-ttu-id="0a55e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0a55e-116">Application</span></span>     | <span data-ttu-id="0a55e-117">Calls.JoinGroupCalls.All、Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="0a55e-117">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a55e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0a55e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}/audioRoutingGroups/{id}
DELETE /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0a55e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0a55e-119">Request headers</span></span>
| <span data-ttu-id="0a55e-120">名前</span><span class="sxs-lookup"><span data-stu-id="0a55e-120">Name</span></span>          | <span data-ttu-id="0a55e-121">説明</span><span class="sxs-lookup"><span data-stu-id="0a55e-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="0a55e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a55e-122">Authorization</span></span> | <span data-ttu-id="0a55e-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0a55e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0a55e-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="0a55e-125">Request body</span></span>
<span data-ttu-id="0a55e-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0a55e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a55e-127">応答</span><span class="sxs-lookup"><span data-stu-id="0a55e-127">Response</span></span>
<span data-ttu-id="0a55e-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="0a55e-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a55e-130">例</span><span class="sxs-lookup"><span data-stu-id="0a55e-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0a55e-131">要求</span><span class="sxs-lookup"><span data-stu-id="0a55e-131">Request</span></span>
<span data-ttu-id="0a55e-132">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="0a55e-132">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete-audioRoutingGroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="0a55e-133">応答</span><span class="sxs-lookup"><span data-stu-id="0a55e-133">Response</span></span>

> <span data-ttu-id="0a55e-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0a55e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Delete audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->