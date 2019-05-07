---
title: 音声ルーティング グループを削除する
description: 指定したオーディオルーティンググループを削除します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e4144a1701d7fe96d507911ebed0ca36e242ac47
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636472"
---
# <a name="delete-audio-routing-group"></a><span data-ttu-id="f78c7-103">音声ルーティング グループを削除する</span><span class="sxs-lookup"><span data-stu-id="f78c7-103">Delete audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f78c7-104">指定した[audioRoutingGroup](../resources/audioroutinggroup.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="f78c7-104">Delete the specified [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f78c7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f78c7-105">Permissions</span></span>
<span data-ttu-id="f78c7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f78c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f78c7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f78c7-108">Permission type</span></span> | <span data-ttu-id="f78c7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f78c7-109">Permissions (from least to most privileged)</span></span>  |
| :-------------- | :------------------------------------------- |
| <span data-ttu-id="f78c7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f78c7-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f78c7-111">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="f78c7-111">Not Supported</span></span>        |
| <span data-ttu-id="f78c7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f78c7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f78c7-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="f78c7-113">Not Supported</span></span>        |
| <span data-ttu-id="f78c7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f78c7-114">Application</span></span>     | <span data-ttu-id="f78c7-115">JoinGroupCalls を呼び出します。すべて、InitiateGroupCalls を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="f78c7-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f78c7-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f78c7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}/audioRoutingGroups/{id}
DELETE /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f78c7-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f78c7-117">Request headers</span></span>
| <span data-ttu-id="f78c7-118">名前</span><span class="sxs-lookup"><span data-stu-id="f78c7-118">Name</span></span>          | <span data-ttu-id="f78c7-119">説明</span><span class="sxs-lookup"><span data-stu-id="f78c7-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f78c7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f78c7-120">Authorization</span></span> | <span data-ttu-id="f78c7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f78c7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f78c7-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="f78c7-123">Request body</span></span>
<span data-ttu-id="f78c7-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f78c7-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f78c7-125">応答</span><span class="sxs-lookup"><span data-stu-id="f78c7-125">Response</span></span>
<span data-ttu-id="f78c7-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="f78c7-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f78c7-128">例</span><span class="sxs-lookup"><span data-stu-id="f78c7-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f78c7-129">要求</span><span class="sxs-lookup"><span data-stu-id="f78c7-129">Request</span></span>
<span data-ttu-id="f78c7-130">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="f78c7-130">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete-audioRoutingGroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="f78c7-131">応答</span><span class="sxs-lookup"><span data-stu-id="f78c7-131">Response</span></span>

> <span data-ttu-id="f78c7-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f78c7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f78c7-134">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="f78c7-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f78c7-135">Visual</span><span class="sxs-lookup"><span data-stu-id="f78c7-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete-audioRoutingGroup-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f78c7-136">Java</span><span class="sxs-lookup"><span data-stu-id="f78c7-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete-audioRoutingGroup-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/audioroutinggroup-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/audioroutinggroup-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
