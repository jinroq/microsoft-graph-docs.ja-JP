---
title: スレッドを一覧表示する
description: グループの会話のすべてのスレッドを取得します。
author: dkershaw10
ms.openlocfilehash: e9203fce8d2b6b5b216d051bcb00193ced3da4a7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333006"
---
# <a name="list-threads"></a><span data-ttu-id="cfe8b-103">スレッドを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="cfe8b-103">List threads</span></span>

<span data-ttu-id="cfe8b-104">グループの会話のすべてのスレッドを取得します。</span><span class="sxs-lookup"><span data-stu-id="cfe8b-104">Get all the threads in a group conversation.</span></span>

<span data-ttu-id="cfe8b-105">注:[グループのすべてのスレッドを取得する](group-list-threads.md)ことも可能です。</span><span class="sxs-lookup"><span data-stu-id="cfe8b-105">Note: You can also [get all the threads of a group](group-list-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cfe8b-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cfe8b-106">Permissions</span></span>
<span data-ttu-id="cfe8b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cfe8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfe8b-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cfe8b-109">Permission type</span></span>      | <span data-ttu-id="cfe8b-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cfe8b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cfe8b-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cfe8b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cfe8b-112">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="cfe8b-112">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="cfe8b-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cfe8b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cfe8b-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cfe8b-114">Not supported.</span></span>    |
|<span data-ttu-id="cfe8b-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cfe8b-115">Application</span></span> | <span data-ttu-id="cfe8b-116">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="cfe8b-116">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cfe8b-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cfe8b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}/threads
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cfe8b-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="cfe8b-118">Optional query parameters</span></span>
<span data-ttu-id="cfe8b-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="cfe8b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cfe8b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cfe8b-120">Request headers</span></span>
| <span data-ttu-id="cfe8b-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cfe8b-121">Header</span></span>       | <span data-ttu-id="cfe8b-122">値</span><span class="sxs-lookup"><span data-stu-id="cfe8b-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cfe8b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cfe8b-123">Authorization</span></span>  | <span data-ttu-id="cfe8b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cfe8b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cfe8b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="cfe8b-126">Request body</span></span>
<span data-ttu-id="cfe8b-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="cfe8b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cfe8b-128">応答</span><span class="sxs-lookup"><span data-stu-id="cfe8b-128">Response</span></span>

<span data-ttu-id="cfe8b-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [conversationThread](../resources/conversationthread.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="cfe8b-129">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cfe8b-130">例</span><span class="sxs-lookup"><span data-stu-id="cfe8b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cfe8b-131">要求</span><span class="sxs-lookup"><span data-stu-id="cfe8b-131">Request</span></span>
<span data-ttu-id="cfe8b-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cfe8b-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_threads"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}/threads
```
##### <a name="response"></a><span data-ttu-id="cfe8b-133">応答</span><span class="sxs-lookup"><span data-stu-id="cfe8b-133">Response</span></span>
<span data-ttu-id="cfe8b-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cfe8b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 536

{
  "value": [
    {
      "toRecipients": [
        {
          "emailAddress": {
            "name": "name-value",
            "address": "address-value"
          }
        }
      ],
      "topic": "topic-value",
      "hasAttachments": true,
      "lastDeliveredDateTime": "datetime-value",
      "uniqueSenders": [
        "uniqueSenders-value"
      ],
      "ccRecipients": [
        {
          "emailAddress": {
            "name": "name-value",
            "address": "address-value"
          }
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List threads",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->