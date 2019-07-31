---
title: オーディオルーティンググループの一覧表示
description: '**AudioRoutingGroup**オブジェクトのリストを取得します。'
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: dad1e79bafc478691618d8834ccc8873904613fb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35944516"
---
# <a name="list-audio-routing-groups"></a><span data-ttu-id="37b7e-103">オーディオルーティンググループの一覧表示</span><span class="sxs-lookup"><span data-stu-id="37b7e-103">List audio routing groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37b7e-104">**AudioRoutingGroup**オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="37b7e-104">Retrieve a list of **audioRoutingGroup** objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="37b7e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="37b7e-105">Permissions</span></span>
<span data-ttu-id="37b7e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="37b7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="37b7e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="37b7e-108">Permission type</span></span>                        | <span data-ttu-id="37b7e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="37b7e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="37b7e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="37b7e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="37b7e-111">サポートされません。</span><span class="sxs-lookup"><span data-stu-id="37b7e-111">Not Supported.</span></span>                               |
| <span data-ttu-id="37b7e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="37b7e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37b7e-113">サポートされません。</span><span class="sxs-lookup"><span data-stu-id="37b7e-113">Not Supported.</span></span>                               |
| <span data-ttu-id="37b7e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="37b7e-114">Application</span></span>     | <span data-ttu-id="37b7e-115">JoinGroupCalls を呼び出します。すべて、InitiateGroupCalls を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="37b7e-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="37b7e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="37b7e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/audioRoutingGroups
GET /applications/{id}/calls/{id}/audioRoutingGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="37b7e-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="37b7e-117">Optional query parameters</span></span>
<span data-ttu-id="37b7e-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="37b7e-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="37b7e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="37b7e-119">Request headers</span></span>
| <span data-ttu-id="37b7e-120">名前</span><span class="sxs-lookup"><span data-stu-id="37b7e-120">Name</span></span>          | <span data-ttu-id="37b7e-121">説明</span><span class="sxs-lookup"><span data-stu-id="37b7e-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="37b7e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="37b7e-122">Authorization</span></span> | <span data-ttu-id="37b7e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="37b7e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="37b7e-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="37b7e-125">Request body</span></span>
<span data-ttu-id="37b7e-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="37b7e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37b7e-127">応答</span><span class="sxs-lookup"><span data-stu-id="37b7e-127">Response</span></span>
<span data-ttu-id="37b7e-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[audioRoutingGroup](../resources/audioroutinggroup.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="37b7e-128">If successful, this method returns a `200 OK` response code and a collection of [audioRoutingGroup](../resources/audioroutinggroup.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37b7e-129">例</span><span class="sxs-lookup"><span data-stu-id="37b7e-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="37b7e-130">要求</span><span class="sxs-lookup"><span data-stu-id="37b7e-130">Request</span></span>
<span data-ttu-id="37b7e-131">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="37b7e-131">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="37b7e-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="37b7e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-audioRoutingGroups"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="37b7e-133">C#</span><span class="sxs-lookup"><span data-stu-id="37b7e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-audioroutinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="37b7e-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="37b7e-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-audioroutinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="37b7e-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="37b7e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-audioroutinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="37b7e-136">Java</span><span class="sxs-lookup"><span data-stu-id="37b7e-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-audioroutinggroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="37b7e-137">応答</span><span class="sxs-lookup"><span data-stu-id="37b7e-137">Response</span></span>

> <span data-ttu-id="37b7e-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="37b7e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  ]
}
-->
