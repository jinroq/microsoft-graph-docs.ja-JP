---
title: オーディオルーティンググループの一覧表示
description: '**audioRoutingGroup**オブジェクトのリストを取得します。'
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 02a782af2bb7690cc55dd3a4632aeb0cf93734da
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461261"
---
# <a name="list-audio-routing-groups"></a><span data-ttu-id="cc50c-103">オーディオルーティンググループの一覧表示</span><span class="sxs-lookup"><span data-stu-id="cc50c-103">List audio routing groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc50c-104">**audioRoutingGroup**オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="cc50c-104">Retrieve a list of **audioRoutingGroup** objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc50c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cc50c-105">Permissions</span></span>
<span data-ttu-id="cc50c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cc50c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cc50c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cc50c-108">Permission type</span></span>                        | <span data-ttu-id="cc50c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cc50c-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cc50c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cc50c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="cc50c-111">サポートされません。</span><span class="sxs-lookup"><span data-stu-id="cc50c-111">Not Supported.</span></span>                               |
| <span data-ttu-id="cc50c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cc50c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc50c-113">サポートされません。</span><span class="sxs-lookup"><span data-stu-id="cc50c-113">Not Supported.</span></span>                               |
| <span data-ttu-id="cc50c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cc50c-114">Application</span></span>     | <span data-ttu-id="cc50c-115">joingroupcalls を呼び出します。すべて、initiategroupcalls を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="cc50c-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc50c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cc50c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/audioRoutingGroups
GET /applications/{id}/calls/{id}/audioRoutingGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cc50c-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="cc50c-117">Optional query parameters</span></span>
<span data-ttu-id="cc50c-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="cc50c-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cc50c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cc50c-119">Request headers</span></span>
| <span data-ttu-id="cc50c-120">名前</span><span class="sxs-lookup"><span data-stu-id="cc50c-120">Name</span></span>          | <span data-ttu-id="cc50c-121">説明</span><span class="sxs-lookup"><span data-stu-id="cc50c-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="cc50c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc50c-122">Authorization</span></span> | <span data-ttu-id="cc50c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cc50c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc50c-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="cc50c-125">Request body</span></span>
<span data-ttu-id="cc50c-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="cc50c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc50c-127">応答</span><span class="sxs-lookup"><span data-stu-id="cc50c-127">Response</span></span>
<span data-ttu-id="cc50c-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[audioRoutingGroup](../resources/audioroutinggroup.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="cc50c-128">If successful, this method returns a `200 OK` response code and a collection of [audioRoutingGroup](../resources/audioroutinggroup.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc50c-129">例</span><span class="sxs-lookup"><span data-stu-id="cc50c-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="cc50c-130">要求</span><span class="sxs-lookup"><span data-stu-id="cc50c-130">Request</span></span>
<span data-ttu-id="cc50c-131">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="cc50c-131">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-audioRoutingGroups"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups
```

##### <a name="response"></a><span data-ttu-id="cc50c-132">応答</span><span class="sxs-lookup"><span data-stu-id="cc50c-132">Response</span></span>

> <span data-ttu-id="cc50c-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="cc50c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.audioRoutingGroup",
  "isCollection": true 
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 302

{
  "value": [
    {
      "id": "oneToOne",
      "routingMode": "oneToOne",
      "sources": [
        "632899f8-2ea1-4604-8413-27bd2892079f"
      ],
      "receivers": [
        "550fae72-d251-43ec-868c-373732c2704f",
        "72f988bf-86f1-41af-91ab-2d7cd011db47"
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List audioRoutingGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-list-audioroutinggroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
