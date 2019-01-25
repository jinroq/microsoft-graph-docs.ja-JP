---
title: リスト favoritePlans
description: ユーザーがお気に入りとしてマークされている plannerPlans の一覧を取得します。 お気に入りとして計画をマークするには、plannerUser リソースを更新します。
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: c189b3a3a7ed6d36272c05e9614fd6d0327600d4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519123"
---
# <a name="list-favoriteplans"></a><span data-ttu-id="3d73c-104">リスト favoritePlans</span><span class="sxs-lookup"><span data-stu-id="3d73c-104">List favoritePlans</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d73c-105">ユーザーがお気に入りとしてマークされている[plannerPlans](../resources/plannerplan.md)の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="3d73c-105">Retrieve a list of [plannerPlans](../resources/plannerplan.md) that are marked as favorite by a user.</span></span> <span data-ttu-id="3d73c-106">お気に入りとして計画をマークするには、 [plannerUser リソースを更新](planneruser-update.md)します。</span><span class="sxs-lookup"><span data-stu-id="3d73c-106">You can mark a plan as favorite by [updating the plannerUser resource](planneruser-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3d73c-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3d73c-107">Permissions</span></span>
<span data-ttu-id="3d73c-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3d73c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d73c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3d73c-110">Permission type</span></span>      | <span data-ttu-id="3d73c-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3d73c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d73c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3d73c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3d73c-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d73c-113">Group.Read.All</span></span>    |
|<span data-ttu-id="3d73c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3d73c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d73c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3d73c-115">Not supported.</span></span>    |
|<span data-ttu-id="3d73c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3d73c-116">Application</span></span> | <span data-ttu-id="3d73c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3d73c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d73c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3d73c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/favoritePlans
GET /users/<id>/planner/favoritePlans
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3d73c-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3d73c-119">Optional query parameters</span></span>
<span data-ttu-id="3d73c-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="3d73c-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3d73c-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3d73c-121">Request headers</span></span>
| <span data-ttu-id="3d73c-122">名前</span><span class="sxs-lookup"><span data-stu-id="3d73c-122">Name</span></span>      |<span data-ttu-id="3d73c-123">説明</span><span class="sxs-lookup"><span data-stu-id="3d73c-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3d73c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d73c-124">Authorization</span></span>  | <span data-ttu-id="3d73c-p104">Bearer {code}。必須。</span><span class="sxs-lookup"><span data-stu-id="3d73c-p104">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d73c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="3d73c-127">Request body</span></span>
<span data-ttu-id="3d73c-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3d73c-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3d73c-129">応答</span><span class="sxs-lookup"><span data-stu-id="3d73c-129">Response</span></span>
<span data-ttu-id="3d73c-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[plannerPlan](../resources/plannerplan.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="3d73c-130">If successful, this method returns a `200 OK` response code and a collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3d73c-131">例</span><span class="sxs-lookup"><span data-stu-id="3d73c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3d73c-132">要求</span><span class="sxs-lookup"><span data-stu-id="3d73c-132">Request</span></span>
<span data-ttu-id="3d73c-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3d73c-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_favoriteplans"
}-->
```http
GET https://graph.microsoft.com/beta/me/planner/favoritePlans
```
##### <a name="response"></a><span data-ttu-id="3d73c-134">応答</span><span class="sxs-lookup"><span data-stu-id="3d73c-134">Response</span></span>
<span data-ttu-id="3d73c-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3d73c-135">The following is an example of the response.</span></span> 

><span data-ttu-id="3d73c-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="3d73c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "List favoritePlans",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/planneruser-list-favoriteplans.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
