---
title: 構成要素を取得します。
description: プロパティと関係の**構成要素**オブジェクトを取得します。
author: VinodRavichandran
ms.openlocfilehash: 8a306c3397a10222692022999194fe12c9501f87
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380192"
---
# <a name="get-participant"></a><span data-ttu-id="705ed-103">構成要素を取得します。</span><span class="sxs-lookup"><span data-stu-id="705ed-103">Get participant</span></span>

> <span data-ttu-id="705ed-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="705ed-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="705ed-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="705ed-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="705ed-106">プロパティと関係の**構成要素**オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="705ed-106">Retrieve the properties and relationships of a **participant** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="705ed-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="705ed-107">Permissions</span></span>
<span data-ttu-id="705ed-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="705ed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="705ed-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="705ed-110">Permission type</span></span> | <span data-ttu-id="705ed-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="705ed-111">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="705ed-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="705ed-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="705ed-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="705ed-113">Not Supported</span></span>        |
| <span data-ttu-id="705ed-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="705ed-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="705ed-115">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="705ed-115">Not Supported</span></span>        |
| <span data-ttu-id="705ed-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="705ed-116">Application</span></span>     | <span data-ttu-id="705ed-117">なし</span><span class="sxs-lookup"><span data-stu-id="705ed-117">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="705ed-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="705ed-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/participants/{id}
GET /applications/{id}/calls/{id}/participants/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="705ed-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="705ed-119">Optional query parameters</span></span>
<span data-ttu-id="705ed-120">このメソッドは、応答をカスタマイズするために[OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="705ed-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="705ed-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="705ed-121">Request headers</span></span>
| <span data-ttu-id="705ed-122">名前</span><span class="sxs-lookup"><span data-stu-id="705ed-122">Name</span></span>          | <span data-ttu-id="705ed-123">説明</span><span class="sxs-lookup"><span data-stu-id="705ed-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="705ed-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="705ed-124">Authorization</span></span> | <span data-ttu-id="705ed-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="705ed-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="705ed-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="705ed-127">Request body</span></span>
<span data-ttu-id="705ed-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="705ed-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="705ed-129">応答</span><span class="sxs-lookup"><span data-stu-id="705ed-129">Response</span></span>
<span data-ttu-id="705ed-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の[構成要素](../resources/participant.md)オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="705ed-130">If successful, this method returns a `200 OK` response code and a [participant](../resources/participant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="705ed-131">例</span><span class="sxs-lookup"><span data-stu-id="705ed-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="705ed-132">要求</span><span class="sxs-lookup"><span data-stu-id="705ed-132">Request</span></span>
<span data-ttu-id="705ed-133">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="705ed-133">The following example shows the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get-participant"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/participants/{id}
```

##### <a name="response"></a><span data-ttu-id="705ed-134">応答</span><span class="sxs-lookup"><span data-stu-id="705ed-134">Response</span></span>

> <span data-ttu-id="705ed-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="705ed-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Get participant",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->