---
title: 会話の一覧表示
description: このグループの会話の一覧を取得します。
author: dkershaw10
ms.openlocfilehash: 81b5b8deb9389d5aff6be9e537bb65ef43d366b9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321400"
---
# <a name="list-conversations"></a><span data-ttu-id="d728d-103">会話の一覧表示</span><span class="sxs-lookup"><span data-stu-id="d728d-103">List conversations</span></span>
<span data-ttu-id="d728d-104">このグループの[会話](../resources/conversation.md)の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="d728d-104">Retrieve the list of [conversations](../resources/conversation.md) in this group.</span></span>

## <a name="permissions"></a><span data-ttu-id="d728d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d728d-105">Permissions</span></span>
<span data-ttu-id="d728d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d728d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d728d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d728d-108">Permission type</span></span>      | <span data-ttu-id="d728d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d728d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d728d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d728d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d728d-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d728d-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d728d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d728d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d728d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d728d-113">Not supported.</span></span>    |
|<span data-ttu-id="d728d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d728d-114">Application</span></span> | <span data-ttu-id="d728d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d728d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d728d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d728d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d728d-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d728d-117">Optional query parameters</span></span>
<span data-ttu-id="d728d-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d728d-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d728d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d728d-119">Request headers</span></span>
| <span data-ttu-id="d728d-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d728d-120">Header</span></span>       | <span data-ttu-id="d728d-121">値</span><span class="sxs-lookup"><span data-stu-id="d728d-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d728d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d728d-122">Authorization</span></span>  | <span data-ttu-id="d728d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d728d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d728d-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="d728d-125">Request body</span></span>
<span data-ttu-id="d728d-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d728d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d728d-127">応答</span><span class="sxs-lookup"><span data-stu-id="d728d-127">Response</span></span>
<span data-ttu-id="d728d-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Conversation](../resources/conversation.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="d728d-128">If successful, this method returns a `200 OK` response code and collection of [conversation](../resources/conversation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d728d-129">例</span><span class="sxs-lookup"><span data-stu-id="d728d-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d728d-130">要求</span><span class="sxs-lookup"><span data-stu-id="d728d-130">Request</span></span>
<span data-ttu-id="d728d-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d728d-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversations"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations
```
#### <a name="response"></a><span data-ttu-id="d728d-132">応答</span><span class="sxs-lookup"><span data-stu-id="d728d-132">Response</span></span>
<span data-ttu-id="d728d-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d728d-133">The following is an example of the response.</span></span>
><span data-ttu-id="d728d-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d728d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
    {
      "topic": "topic-value",
      "hasAttachments": true,
      "lastDeliveredDateTime": "datetime-value",
      "uniqueSenders": [
        "uniqueSenders-value"
      ],
      "preview": "preview-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List conversations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->