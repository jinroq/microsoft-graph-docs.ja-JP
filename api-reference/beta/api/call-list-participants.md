---
title: 参加者の一覧
description: 呼び出し内の構成要素のオブジェクトの一覧を取得します。
author: VinodRavichandran
ms.openlocfilehash: c22e276f7b7bb1ddd0a082bd54f0b5b8d93226c1
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380444"
---
# <a name="list-participants"></a><span data-ttu-id="54d28-103">参加者の一覧</span><span class="sxs-lookup"><span data-stu-id="54d28-103">List participants</span></span>

> <span data-ttu-id="54d28-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="54d28-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="54d28-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="54d28-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="54d28-106">呼び出し内の構成要素のオブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="54d28-106">Retrieve a list of participant objects in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="54d28-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="54d28-107">Permissions</span></span>
<span data-ttu-id="54d28-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="54d28-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="54d28-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="54d28-110">Permission type</span></span> | <span data-ttu-id="54d28-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="54d28-111">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="54d28-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="54d28-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="54d28-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="54d28-113">Not Supported</span></span>        |
| <span data-ttu-id="54d28-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="54d28-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54d28-115">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="54d28-115">Not Supported</span></span>        |
| <span data-ttu-id="54d28-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="54d28-116">Application</span></span>     | <span data-ttu-id="54d28-117">なし</span><span class="sxs-lookup"><span data-stu-id="54d28-117">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="54d28-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="54d28-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/participants
GET /applications/{id}/calls/{id}/participants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="54d28-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="54d28-119">Optional query parameters</span></span>
<span data-ttu-id="54d28-120">このメソッドは、応答をカスタマイズするために[OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="54d28-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="54d28-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="54d28-121">Request headers</span></span>
| <span data-ttu-id="54d28-122">名前</span><span class="sxs-lookup"><span data-stu-id="54d28-122">Name</span></span>          | <span data-ttu-id="54d28-123">説明</span><span class="sxs-lookup"><span data-stu-id="54d28-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="54d28-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="54d28-124">Authorization</span></span> | <span data-ttu-id="54d28-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="54d28-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="54d28-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="54d28-127">Request body</span></span>
<span data-ttu-id="54d28-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="54d28-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54d28-129">応答</span><span class="sxs-lookup"><span data-stu-id="54d28-129">Response</span></span>
<span data-ttu-id="54d28-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の[構成要素](../resources/participant.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="54d28-130">If successful, this method returns a `200 OK` response code and collection of [participant](../resources/participant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="54d28-131">例</span><span class="sxs-lookup"><span data-stu-id="54d28-131">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="54d28-132">例 1</span><span class="sxs-lookup"><span data-stu-id="54d28-132">Example 1</span></span>

##### <a name="request"></a><span data-ttu-id="54d28-133">要求</span><span class="sxs-lookup"><span data-stu-id="54d28-133">Request</span></span>
<span data-ttu-id="54d28-134">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="54d28-134">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-participants"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/participants
```

##### <a name="response"></a><span data-ttu-id="54d28-135">応答</span><span class="sxs-lookup"><span data-stu-id="54d28-135">Response</span></span>

> <span data-ttu-id="54d28-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="54d28-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.participant",
  "isCollection": true,
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1152

{
  "value": [
    {
      "id": "id-value",
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
      "isInLobby": false,
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
      "metadata": "metadata-value"
    }
  ]
}
```

### <a name="example-2"></a><span data-ttu-id="54d28-138">例 2</span><span class="sxs-lookup"><span data-stu-id="54d28-138">Example 2</span></span>

##### <a name="request"></a><span data-ttu-id="54d28-139">要求</span><span class="sxs-lookup"><span data-stu-id="54d28-139">Request</span></span>

```http
GET /app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants
Authorization: Bearer <TOKEN>
```

##### <a name="response"></a><span data-ttu-id="54d28-140">応答</span><span class="sxs-lookup"><span data-stu-id="54d28-140">Response</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.participant",
  "isCollection": true,
  "truncated": true
}-->
```json
{
  "value": [
    {
      "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
      "info": {
        "identity" : {
          "user" : {
            "displayName": "Test User",
            "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
          }
        },
        "region": "westus",
        "languageId": "en-US"
      },
      "mediaStreams": [
        {
          "sourceId": "1",
          "mediaType": "audio",
          "label": "main-audio",
          "direction": "sendReceive",
          "serverMuted": false
        }
      ]
    },
    {
      "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
      "info": {
        "identity" : {
          "phone": {
            "displayName": "+12345678890",
            "id": "+12345678890"
          }
        }
      },
      "mediaStreams": [
        {
          "sourceId": "2",
          "mediaType": "audio",
          "label": "main-audio",
          "direction": "sendReceive",
          "serverMuted": false
        }
      ],
      "isMuted": true
    },
    {
      "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
      "info": {
        "identity" : {
          "application" : {
            "displayName": "Test BOT",
            "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
          }
        },
        "region": "westus",
        "languageId": "en-US"
      },
      "mediaStreams": [
        {
          "sourceId": "3",
          "mediaType": "audio",
          "label": "main-audio",
          "direction": "sendReceive",
          "serverMuted": false
        }
      ],
      "isMuted": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List participants",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
