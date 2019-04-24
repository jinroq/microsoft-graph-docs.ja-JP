---
title: 音声ルーティング グループを削除する
description: 指定したオーディオルーティンググループを削除します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0c0e5c0cd58c867f7c69a3ac5d4f99a11af223ee
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459354"
---
# <a name="delete-audio-routing-group"></a><span data-ttu-id="4eeca-103">音声ルーティング グループを削除する</span><span class="sxs-lookup"><span data-stu-id="4eeca-103">Delete audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4eeca-104">指定した[audioRoutingGroup](../resources/audioroutinggroup.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="4eeca-104">Delete the specified [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4eeca-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4eeca-105">Permissions</span></span>
<span data-ttu-id="4eeca-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4eeca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4eeca-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4eeca-108">Permission type</span></span> | <span data-ttu-id="4eeca-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4eeca-109">Permissions (from least to most privileged)</span></span>  |
| :-------------- | :------------------------------------------- |
| <span data-ttu-id="4eeca-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4eeca-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4eeca-111">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="4eeca-111">Not Supported</span></span>        |
| <span data-ttu-id="4eeca-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4eeca-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4eeca-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="4eeca-113">Not Supported</span></span>        |
| <span data-ttu-id="4eeca-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4eeca-114">Application</span></span>     | <span data-ttu-id="4eeca-115">joingroupcalls を呼び出します。すべて、initiategroupcalls を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="4eeca-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4eeca-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4eeca-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}/audioRoutingGroups/{id}
DELETE /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4eeca-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4eeca-117">Request headers</span></span>
| <span data-ttu-id="4eeca-118">名前</span><span class="sxs-lookup"><span data-stu-id="4eeca-118">Name</span></span>          | <span data-ttu-id="4eeca-119">説明</span><span class="sxs-lookup"><span data-stu-id="4eeca-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="4eeca-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4eeca-120">Authorization</span></span> | <span data-ttu-id="4eeca-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4eeca-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4eeca-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="4eeca-123">Request body</span></span>
<span data-ttu-id="4eeca-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4eeca-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4eeca-125">応答</span><span class="sxs-lookup"><span data-stu-id="4eeca-125">Response</span></span>
<span data-ttu-id="4eeca-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="4eeca-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4eeca-128">例</span><span class="sxs-lookup"><span data-stu-id="4eeca-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4eeca-129">要求</span><span class="sxs-lookup"><span data-stu-id="4eeca-129">Request</span></span>
<span data-ttu-id="4eeca-130">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="4eeca-130">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete-audioRoutingGroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="4eeca-131">応答</span><span class="sxs-lookup"><span data-stu-id="4eeca-131">Response</span></span>

> <span data-ttu-id="4eeca-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="4eeca-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
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
  "description": "Delete audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/audioroutinggroup-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
