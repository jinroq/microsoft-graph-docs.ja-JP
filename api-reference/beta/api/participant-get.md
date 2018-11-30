---
title: 構成要素を取得します。
description: プロパティと関係の**構成要素**オブジェクトを取得します。
ms.openlocfilehash: 4e97278b7ac93d784884c789f4da089e63e195ad
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067088"
---
# <a name="get-participant"></a><span data-ttu-id="fe6f3-103">構成要素を取得します。</span><span class="sxs-lookup"><span data-stu-id="fe6f3-103">Get participant</span></span>

> <span data-ttu-id="fe6f3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fe6f3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe6f3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe6f3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fe6f3-106">プロパティと関係の**構成要素**オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="fe6f3-106">Retrieve the properties and relationships of a **participant** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe6f3-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fe6f3-107">Permissions</span></span>
<span data-ttu-id="fe6f3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fe6f3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fe6f3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fe6f3-110">Permission type</span></span> | <span data-ttu-id="fe6f3-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fe6f3-111">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="fe6f3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fe6f3-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="fe6f3-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="fe6f3-113">Not Supported</span></span>        |
| <span data-ttu-id="fe6f3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fe6f3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe6f3-115">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="fe6f3-115">Not Supported</span></span>        |
| <span data-ttu-id="fe6f3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fe6f3-116">Application</span></span>     | <span data-ttu-id="fe6f3-117">なし</span><span class="sxs-lookup"><span data-stu-id="fe6f3-117">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="fe6f3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fe6f3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/participants/{id}
GET /applications/{id}/calls/{id}/participants/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fe6f3-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="fe6f3-119">Optional query parameters</span></span>
<span data-ttu-id="fe6f3-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="fe6f3-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fe6f3-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fe6f3-121">Request headers</span></span>
| <span data-ttu-id="fe6f3-122">名前</span><span class="sxs-lookup"><span data-stu-id="fe6f3-122">Name</span></span>          | <span data-ttu-id="fe6f3-123">説明</span><span class="sxs-lookup"><span data-stu-id="fe6f3-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="fe6f3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe6f3-124">Authorization</span></span> | <span data-ttu-id="fe6f3-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fe6f3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe6f3-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="fe6f3-127">Request body</span></span>
<span data-ttu-id="fe6f3-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fe6f3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe6f3-129">応答</span><span class="sxs-lookup"><span data-stu-id="fe6f3-129">Response</span></span>
<span data-ttu-id="fe6f3-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の[構成要素](../resources/participant.md)オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="fe6f3-130">If successful, this method returns a `200 OK` response code and a [participant](../resources/participant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe6f3-131">例</span><span class="sxs-lookup"><span data-stu-id="fe6f3-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fe6f3-132">要求</span><span class="sxs-lookup"><span data-stu-id="fe6f3-132">Request</span></span>
<span data-ttu-id="fe6f3-133">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="fe6f3-133">The following example shows the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_participant"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/participants/{id}
```

##### <a name="response"></a><span data-ttu-id="fe6f3-134">応答</span><span class="sxs-lookup"><span data-stu-id="fe6f3-134">Response</span></span>

> <span data-ttu-id="fe6f3-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="fe6f3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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