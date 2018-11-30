---
title: リスト favoritePlans
description: ユーザーがお気に入りとしてマークされている plannerPlans の一覧を取得します。 お気に入りとして計画をマークするには、plannerUser リソースを更新します。
ms.openlocfilehash: e9e3cf3cd348430a3512d15ac2e0cdc68d24d258
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068700"
---
# <a name="list-favoriteplans"></a><span data-ttu-id="101db-104">リスト favoritePlans</span><span class="sxs-lookup"><span data-stu-id="101db-104">List favoritePlans</span></span>

> <span data-ttu-id="101db-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="101db-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="101db-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="101db-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="101db-107">ユーザーがお気に入りとしてマークされている[plannerPlans](../resources/plannerplan.md)の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="101db-107">Retrieve a list of [plannerPlans](../resources/plannerplan.md) that are marked as favorite by a user.</span></span> <span data-ttu-id="101db-108">お気に入りとして計画をマークするには、 [plannerUser リソースを更新](planneruser-update.md)します。</span><span class="sxs-lookup"><span data-stu-id="101db-108">You can mark a plan as favorite by [updating the plannerUser resource](planneruser-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="101db-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="101db-109">Permissions</span></span>
<span data-ttu-id="101db-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="101db-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="101db-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="101db-112">Permission type</span></span>      | <span data-ttu-id="101db-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="101db-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="101db-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="101db-114">Delegated (work or school account)</span></span> | <span data-ttu-id="101db-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="101db-115">Group.Read.All</span></span>    |
|<span data-ttu-id="101db-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="101db-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="101db-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="101db-117">Not supported.</span></span>    |
|<span data-ttu-id="101db-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="101db-118">Application</span></span> | <span data-ttu-id="101db-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="101db-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="101db-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="101db-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/favoritePlans
GET /users/<id>/planner/favoritePlans
```
## <a name="optional-query-parameters"></a><span data-ttu-id="101db-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="101db-121">Optional query parameters</span></span>
<span data-ttu-id="101db-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="101db-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="101db-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="101db-123">Request headers</span></span>
| <span data-ttu-id="101db-124">名前</span><span class="sxs-lookup"><span data-stu-id="101db-124">Name</span></span>      |<span data-ttu-id="101db-125">説明</span><span class="sxs-lookup"><span data-stu-id="101db-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="101db-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="101db-126">Authorization</span></span>  | <span data-ttu-id="101db-p105">Bearer {code}。必須。</span><span class="sxs-lookup"><span data-stu-id="101db-p105">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="101db-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="101db-129">Request body</span></span>
<span data-ttu-id="101db-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="101db-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="101db-131">応答</span><span class="sxs-lookup"><span data-stu-id="101db-131">Response</span></span>
<span data-ttu-id="101db-132">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[plannerPlan](../resources/plannerplan.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="101db-132">If successful, this method returns a `200 OK` response code and a collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="101db-133">例</span><span class="sxs-lookup"><span data-stu-id="101db-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="101db-134">要求</span><span class="sxs-lookup"><span data-stu-id="101db-134">Request</span></span>
<span data-ttu-id="101db-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="101db-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_favoriteplans"
}-->
```http
GET https://graph.microsoft.com/beta/me/planner/favoritePlans
```
##### <a name="response"></a><span data-ttu-id="101db-136">応答</span><span class="sxs-lookup"><span data-stu-id="101db-136">Response</span></span>
<span data-ttu-id="101db-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="101db-137">The following is an example of the response.</span></span> 

><span data-ttu-id="101db-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="101db-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 979

{
  "value": [
    {
      "@odata.etag": "W/\"JzEtUGxhbiAgQEBAQEBAQEBAQEBAQEBDXCc=\"",
      "createdBy": {
        "user": {
          "id": "dd8a8379-1ac1-4eee-861d-ec15f6fa3611"
        },
        "application": {
          "id": "09abbdfd-ed23-44ee-a2d9-a627aa1c90f3"
        }
      },
      "createdDateTime": "2015-10-14T00:57:28.4698344Z",
      "owner": "eacd01dd-84cc-4c12-bd8a-9a33e5aeed11",
      "title": "Budget Planning (2016)",
      "id": "uZWtCtli30CGoWLIWSat1mQAC0ai"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List favoritePlans",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
