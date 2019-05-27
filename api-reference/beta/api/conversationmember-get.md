---
title: conversationMember を取得する
description: チャットのメンバーを取得します。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: a2c539b7240060a6434f5ece01dc242ae948a5f4
ms.sourcegitcommit: afea19508ad74a3583b11b5f7b544c53eafb3740
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/22/2019
ms.locfileid: "34379296"
---
# <a name="get-conversationmember"></a><span data-ttu-id="c41bc-103">conversationMember を取得する</span><span class="sxs-lookup"><span data-stu-id="c41bc-103">Get conversationMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c41bc-104">[chat](../resources/chat.md) から [conversationMember](../resources/conversationmember.md) を取得します。</span><span class="sxs-lookup"><span data-stu-id="c41bc-104">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c41bc-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c41bc-105">Permissions</span></span>

<span data-ttu-id="c41bc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c41bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c41bc-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c41bc-108">Permission Type</span></span>|<span data-ttu-id="c41bc-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c41bc-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="c41bc-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c41bc-110">Delegated (work or school account)</span></span>|<span data-ttu-id="c41bc-111">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c41bc-111">Chat.Read, Chat.ReadWrite</span></span>|
|<span data-ttu-id="c41bc-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c41bc-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c41bc-113">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="c41bc-113">Not supported</span></span>|
|<span data-ttu-id="c41bc-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c41bc-114">Application</span></span> |<span data-ttu-id="c41bc-115">Chat.Read.All、Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c41bc-115">Chat.Read.All, Chat.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c41bc-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c41bc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members/{id}
GET /users/{id}/chats/{id}/members/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c41bc-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c41bc-117">Optional query parameters</span></span>

<span data-ttu-id="c41bc-118">この操作は、応答をカスタマイズする [OData クエリ パラメーター](/graph/query-parameters)をサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="c41bc-118">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c41bc-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c41bc-119">Request headers</span></span>

| <span data-ttu-id="c41bc-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c41bc-120">Header</span></span>       | <span data-ttu-id="c41bc-121">値</span><span class="sxs-lookup"><span data-stu-id="c41bc-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c41bc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c41bc-122">Authorization</span></span>  | <span data-ttu-id="c41bc-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c41bc-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c41bc-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="c41bc-125">Request body</span></span>

<span data-ttu-id="c41bc-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c41bc-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c41bc-127">応答</span><span class="sxs-lookup"><span data-stu-id="c41bc-127">Response</span></span>

<span data-ttu-id="c41bc-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[conversationMember](../resources/conversationmember.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c41bc-128">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c41bc-129">例</span><span class="sxs-lookup"><span data-stu-id="c41bc-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c41bc-130">要求</span><span class="sxs-lookup"><span data-stu-id="c41bc-130">Request</span></span>

<span data-ttu-id="c41bc-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c41bc-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->
```http
GET https://graph.microsoft.com/beta/chats/{id}/members/{id}
```

##### <a name="response"></a><span data-ttu-id="c41bc-132">応答</span><span class="sxs-lookup"><span data-stu-id="c41bc-132">Response</span></span>

<span data-ttu-id="c41bc-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="c41bc-133">Here is an example of the response.</span></span> 

><span data-ttu-id="c41bc-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c41bc-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "id": "id-value",
  "displayName": "display-name-value"
}
```