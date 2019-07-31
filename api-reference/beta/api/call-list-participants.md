---
title: 参加者を一覧表示する
description: 呼び出し内の参加者のオブジェクトのリストを取得します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3c08172eaa30a53c29971d346853a3aa2002b93f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35944549"
---
# <a name="list-participants"></a><span data-ttu-id="53444-103">参加者を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="53444-103">List participants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53444-104">呼び出し内の参加者のオブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="53444-104">Retrieve a list of participant objects in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="53444-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="53444-105">Permissions</span></span>

<span data-ttu-id="53444-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="53444-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="53444-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="53444-108">Permission type</span></span> | <span data-ttu-id="53444-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="53444-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="53444-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="53444-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="53444-111">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="53444-111">Not Supported</span></span>        |
| <span data-ttu-id="53444-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="53444-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53444-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="53444-113">Not Supported</span></span>        |
| <span data-ttu-id="53444-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="53444-114">Application</span></span>     | <span data-ttu-id="53444-115">None</span><span class="sxs-lookup"><span data-stu-id="53444-115">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="53444-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="53444-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /app/calls/{id}/participants
GET /applications/{id}/calls/{id}/participants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="53444-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="53444-117">Optional query parameters</span></span>

<span data-ttu-id="53444-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="53444-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="53444-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="53444-119">Request headers</span></span>

| <span data-ttu-id="53444-120">名前</span><span class="sxs-lookup"><span data-stu-id="53444-120">Name</span></span>          | <span data-ttu-id="53444-121">説明</span><span class="sxs-lookup"><span data-stu-id="53444-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="53444-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="53444-122">Authorization</span></span> | <span data-ttu-id="53444-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="53444-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="53444-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="53444-125">Request body</span></span>

<span data-ttu-id="53444-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="53444-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53444-127">応答</span><span class="sxs-lookup"><span data-stu-id="53444-127">Response</span></span>

<span data-ttu-id="53444-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[参加者](../resources/participant.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="53444-128">If successful, this method returns a `200 OK` response code and collection of [participant](../resources/participant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="53444-129">例</span><span class="sxs-lookup"><span data-stu-id="53444-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="53444-130">要求</span><span class="sxs-lookup"><span data-stu-id="53444-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="53444-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="53444-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-participants"
}-->

```http
GET https://graph.microsoft.com/beta/app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants
Authorization: Bearer <TOKEN>
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="53444-132">C#</span><span class="sxs-lookup"><span data-stu-id="53444-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-participants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="53444-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="53444-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-participants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="53444-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="53444-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-participants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="53444-135">Java</span><span class="sxs-lookup"><span data-stu-id="53444-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-participants-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="53444-136">応答</span><span class="sxs-lookup"><span data-stu-id="53444-136">Response</span></span>

> <span data-ttu-id="53444-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="53444-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.participant",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

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
<!--
{
  "type": "#page.annotation",
  "description": "List participants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
