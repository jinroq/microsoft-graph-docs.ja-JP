---
title: Get conversation
description: 会話オブジェクトのプロパティとリレーションシップを取得します。
ms.openlocfilehash: 33e38e321ff948f55213646cb9349db85176e989
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071028"
---
# <a name="get-conversation"></a><span data-ttu-id="b208c-103">Get conversation</span><span class="sxs-lookup"><span data-stu-id="b208c-103">Get conversation</span></span>

> <span data-ttu-id="b208c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b208c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b208c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b208c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b208c-106">会話オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="b208c-106">Retrieve the properties and relationships of conversation object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b208c-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b208c-107">Permissions</span></span>
<span data-ttu-id="b208c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b208c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b208c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b208c-110">Permission type</span></span>      | <span data-ttu-id="b208c-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b208c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b208c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b208c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b208c-113">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b208c-113">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="b208c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b208c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b208c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b208c-115">Not supported.</span></span>    |
|<span data-ttu-id="b208c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b208c-116">Application</span></span> | <span data-ttu-id="b208c-117">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b208c-117">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b208c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b208c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="b208c-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b208c-119">Optional query parameters</span></span>
<span data-ttu-id="b208c-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b208c-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b208c-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b208c-121">Request headers</span></span>
| <span data-ttu-id="b208c-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b208c-122">Header</span></span>       | <span data-ttu-id="b208c-123">値</span><span class="sxs-lookup"><span data-stu-id="b208c-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b208c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b208c-124">Authorization</span></span>  | <span data-ttu-id="b208c-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b208c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b208c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b208c-127">Request body</span></span>
<span data-ttu-id="b208c-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b208c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b208c-129">応答</span><span class="sxs-lookup"><span data-stu-id="b208c-129">Response</span></span>

<span data-ttu-id="b208c-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[会話](../resources/conversation.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b208c-130">If successful, this method returns a `200 OK` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b208c-131">例</span><span class="sxs-lookup"><span data-stu-id="b208c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b208c-132">要求</span><span class="sxs-lookup"><span data-stu-id="b208c-132">Request</span></span>
<span data-ttu-id="b208c-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b208c-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversation"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/conversations/{id}
```
##### <a name="response"></a><span data-ttu-id="b208c-134">応答</span><span class="sxs-lookup"><span data-stu-id="b208c-134">Response</span></span>
<span data-ttu-id="b208c-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b208c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "preview": "preview-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
