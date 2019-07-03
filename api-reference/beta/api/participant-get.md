---
title: 参加者を取得する
description: '**参加者**オブジェクトのプロパティと関係を取得します。'
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c6fc3457c6604997fc0264f6a61c24fb0e5f50ca
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35453972"
---
# <a name="get-participant"></a><span data-ttu-id="a2d9c-103">参加者を取得する</span><span class="sxs-lookup"><span data-stu-id="a2d9c-103">Get participant</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2d9c-104">**参加者**オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="a2d9c-104">Retrieve the properties and relationships of a **participant** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2d9c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a2d9c-105">Permissions</span></span>
<span data-ttu-id="a2d9c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2d9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a2d9c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a2d9c-108">Permission type</span></span> | <span data-ttu-id="a2d9c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a2d9c-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="a2d9c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a2d9c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a2d9c-111">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="a2d9c-111">Not Supported</span></span>        |
| <span data-ttu-id="a2d9c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a2d9c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2d9c-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="a2d9c-113">Not Supported</span></span>        |
| <span data-ttu-id="a2d9c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a2d9c-114">Application</span></span>     | <span data-ttu-id="a2d9c-115">None</span><span class="sxs-lookup"><span data-stu-id="a2d9c-115">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="a2d9c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a2d9c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/participants/{id}
GET /applications/{id}/calls/{id}/participants/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a2d9c-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a2d9c-117">Optional query parameters</span></span>
<span data-ttu-id="a2d9c-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a2d9c-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a2d9c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a2d9c-119">Request headers</span></span>
| <span data-ttu-id="a2d9c-120">名前</span><span class="sxs-lookup"><span data-stu-id="a2d9c-120">Name</span></span>          | <span data-ttu-id="a2d9c-121">説明</span><span class="sxs-lookup"><span data-stu-id="a2d9c-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="a2d9c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2d9c-122">Authorization</span></span> | <span data-ttu-id="a2d9c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a2d9c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2d9c-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a2d9c-125">Request body</span></span>
<span data-ttu-id="a2d9c-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a2d9c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2d9c-127">応答</span><span class="sxs-lookup"><span data-stu-id="a2d9c-127">Response</span></span>
<span data-ttu-id="a2d9c-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[参加者](../resources/participant.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a2d9c-128">If successful, this method returns a `200 OK` response code and a [participant](../resources/participant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2d9c-129">例</span><span class="sxs-lookup"><span data-stu-id="a2d9c-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a2d9c-130">要求</span><span class="sxs-lookup"><span data-stu-id="a2d9c-130">Request</span></span>
<span data-ttu-id="a2d9c-131">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="a2d9c-131">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a2d9c-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="a2d9c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-participant"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/participants/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a2d9c-133">C#</span><span class="sxs-lookup"><span data-stu-id="a2d9c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-participant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a2d9c-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="a2d9c-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-participant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a2d9c-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="a2d9c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-participant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a2d9c-136">応答</span><span class="sxs-lookup"><span data-stu-id="a2d9c-136">Response</span></span>

> <span data-ttu-id="a2d9c-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a2d9c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.participant"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 977

{
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "info": {
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "languageId-value",
    "region": "region-value"
  },
  "isInLobby": true,
  "isMuted": true,
  "mediaStreams": [
    {
      "sourceId": "1",
      "direction": "sendReceive",
      "label": "main-audio",
      "mediaType": "audio",
      "serverMuted": false
    }
  ],
  "metadata": "metadata-value",
  "recordingInfo": {
    "initiatedBy": {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "languageId": "languageId-value",
      "region": "region-value"
    },
    "status": "recordingCapable"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get participant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
