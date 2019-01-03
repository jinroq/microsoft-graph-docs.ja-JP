---
title: スレッドを一覧表示する
description: グループの会話のすべてのスレッドを取得します。
author: dkershaw10
ms.openlocfilehash: 1f19692f9c5a1510a901fa4c0cc5c60862625179
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334056"
---
# <a name="list-threads"></a><span data-ttu-id="bc58e-103">スレッドを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="bc58e-103">List threads</span></span>

> <span data-ttu-id="bc58e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bc58e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc58e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bc58e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bc58e-106">グループの会話のすべてのスレッドを取得します。</span><span class="sxs-lookup"><span data-stu-id="bc58e-106">Get all the threads in a group conversation.</span></span>
<span data-ttu-id="bc58e-107">注:[グループのすべてのスレッドを取得する](group-list-threads.md)ことも可能です。</span><span class="sxs-lookup"><span data-stu-id="bc58e-107">Note: You can also [get all the threads of a group](group-list-threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="bc58e-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bc58e-108">Permissions</span></span>
<span data-ttu-id="bc58e-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bc58e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc58e-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bc58e-111">Permission type</span></span>      | <span data-ttu-id="bc58e-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bc58e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc58e-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bc58e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="bc58e-114">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="bc58e-114">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="bc58e-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bc58e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc58e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bc58e-116">Not supported.</span></span>    |
|<span data-ttu-id="bc58e-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bc58e-117">Application</span></span> | <span data-ttu-id="bc58e-118">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="bc58e-118">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc58e-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bc58e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}/threads
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bc58e-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="bc58e-120">Optional query parameters</span></span>
<span data-ttu-id="bc58e-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="bc58e-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="bc58e-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bc58e-122">Request headers</span></span>
| <span data-ttu-id="bc58e-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bc58e-123">Header</span></span>       | <span data-ttu-id="bc58e-124">値</span><span class="sxs-lookup"><span data-stu-id="bc58e-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bc58e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc58e-125">Authorization</span></span>  | <span data-ttu-id="bc58e-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bc58e-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bc58e-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="bc58e-128">Request body</span></span>
<span data-ttu-id="bc58e-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="bc58e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc58e-130">応答</span><span class="sxs-lookup"><span data-stu-id="bc58e-130">Response</span></span>

<span data-ttu-id="bc58e-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [conversationThread](../resources/conversationthread.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="bc58e-131">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bc58e-132">例</span><span class="sxs-lookup"><span data-stu-id="bc58e-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bc58e-133">要求</span><span class="sxs-lookup"><span data-stu-id="bc58e-133">Request</span></span>
<span data-ttu-id="bc58e-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bc58e-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_threads"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/conversations/{id}/threads
```
##### <a name="response"></a><span data-ttu-id="bc58e-135">応答</span><span class="sxs-lookup"><span data-stu-id="bc58e-135">Response</span></span>
<span data-ttu-id="bc58e-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bc58e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
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