---
title: Get conversation
description: 会話オブジェクトのプロパティと関係を取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 7661ceba1ef5719e2cc1711b1126771c40a4ebec
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36003113"
---
# <a name="get-conversation"></a><span data-ttu-id="8c906-103">会話を取得する</span><span class="sxs-lookup"><span data-stu-id="8c906-103">Get conversation</span></span>

<span data-ttu-id="8c906-104">会話オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="8c906-104">Retrieve the properties and relationships of conversation object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8c906-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8c906-105">Permissions</span></span>
<span data-ttu-id="8c906-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8c906-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c906-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8c906-108">Permission type</span></span>      | <span data-ttu-id="8c906-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8c906-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c906-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8c906-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8c906-111">グループ読み取り。すべてを取得します。</span><span class="sxs-lookup"><span data-stu-id="8c906-111">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="8c906-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8c906-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c906-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8c906-113">Not supported.</span></span>    |
|<span data-ttu-id="8c906-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8c906-114">Application</span></span> | <span data-ttu-id="8c906-115">グループ読み取り。すべてを取得します。</span><span class="sxs-lookup"><span data-stu-id="8c906-115">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c906-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8c906-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="8c906-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8c906-117">Optional query parameters</span></span>
<span data-ttu-id="8c906-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8c906-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8c906-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8c906-119">Request headers</span></span>
| <span data-ttu-id="8c906-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8c906-120">Header</span></span>       | <span data-ttu-id="8c906-121">値</span><span class="sxs-lookup"><span data-stu-id="8c906-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8c906-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c906-122">Authorization</span></span>  | <span data-ttu-id="8c906-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8c906-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8c906-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="8c906-125">Request body</span></span>
<span data-ttu-id="8c906-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8c906-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c906-127">応答</span><span class="sxs-lookup"><span data-stu-id="8c906-127">Response</span></span>

<span data-ttu-id="8c906-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[会話](../resources/conversation.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8c906-128">If successful, this method returns a `200 OK` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8c906-129">例</span><span class="sxs-lookup"><span data-stu-id="8c906-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8c906-130">要求</span><span class="sxs-lookup"><span data-stu-id="8c906-130">Request</span></span>
<span data-ttu-id="8c906-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8c906-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8c906-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="8c906-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversation"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8c906-133">C#</span><span class="sxs-lookup"><span data-stu-id="8c906-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8c906-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="8c906-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8c906-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="8c906-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8c906-136">Java</span><span class="sxs-lookup"><span data-stu-id="8c906-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8c906-137">応答</span><span class="sxs-lookup"><span data-stu-id="8c906-137">Response</span></span>
<span data-ttu-id="8c906-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8c906-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "lastDeliveredDateTime": "datetime-value",
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
