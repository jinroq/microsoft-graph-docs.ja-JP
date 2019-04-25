---
title: Get conversation
description: conversation オブジェクトを取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: efbf93afabb95db00075ea780e3d6f6bc28b27eb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574660"
---
# <a name="get-conversation"></a><span data-ttu-id="ac228-103">Get conversation</span><span class="sxs-lookup"><span data-stu-id="ac228-103">Get conversation</span></span>
<span data-ttu-id="ac228-104">[conversation](../resources/conversation.md) オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="ac228-104">Get a [conversation](../resources/conversation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac228-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ac228-105">Permissions</span></span>
<span data-ttu-id="ac228-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ac228-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac228-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ac228-108">Permission type</span></span>      | <span data-ttu-id="ac228-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ac228-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac228-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ac228-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ac228-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac228-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ac228-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ac228-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac228-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ac228-113">Not supported.</span></span>    |
|<span data-ttu-id="ac228-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ac228-114">Application</span></span> | <span data-ttu-id="ac228-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ac228-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac228-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ac228-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ac228-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ac228-117">Optional query parameters</span></span>
<span data-ttu-id="ac228-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ac228-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ac228-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ac228-119">Request headers</span></span>
| <span data-ttu-id="ac228-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ac228-120">Header</span></span>       | <span data-ttu-id="ac228-121">値</span><span class="sxs-lookup"><span data-stu-id="ac228-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ac228-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac228-122">Authorization</span></span>  | <span data-ttu-id="ac228-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ac228-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ac228-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="ac228-125">Request body</span></span>
<span data-ttu-id="ac228-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ac228-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac228-127">応答</span><span class="sxs-lookup"><span data-stu-id="ac228-127">Response</span></span>
<span data-ttu-id="ac228-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [conversation](../resources/conversation.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ac228-128">If successful, this method returns a `200 OK` response code and a [conversation](../resources/conversation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac228-129">例</span><span class="sxs-lookup"><span data-stu-id="ac228-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ac228-130">要求</span><span class="sxs-lookup"><span data-stu-id="ac228-130">Request</span></span>
<span data-ttu-id="ac228-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ac228-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU="],
  "name": "get_group_conversation"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```

#### <a name="response"></a><span data-ttu-id="ac228-132">応答</span><span class="sxs-lookup"><span data-stu-id="ac228-132">Response</span></span>
<span data-ttu-id="ac228-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ac228-133">The following is an example of the response.</span></span>
><span data-ttu-id="ac228-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="ac228-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 644

{
    "id": "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=",
    "topic": "New Training Plans",
    "hasAttachments": false,
    "lastDeliveredDateTime": "2017-07-31T18:59:05Z",
    "uniqueSenders": [
        "HR Taskforce"
    ],
    "preview": "Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>"
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
