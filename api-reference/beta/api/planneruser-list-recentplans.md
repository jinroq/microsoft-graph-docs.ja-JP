---
title: リスト recentPlans
description: ユーザーが最近表示した plannerPlans の一覧を取得します。 PlannerUser リソースを更新することによって、最近表示した計画を更新できます。
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: b4a8e25a31ceb17f85aef139378fa3e3e9058ab4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528740"
---
# <a name="list-recentplans"></a><span data-ttu-id="ff526-104">リスト recentPlans</span><span class="sxs-lookup"><span data-stu-id="ff526-104">List recentPlans</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff526-105">ユーザーが最近表示した[plannerPlans](../resources/plannerplan.md)の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="ff526-105">Retrieve a list of [plannerPlans](../resources/plannerplan.md) recently viewed by a user.</span></span> <span data-ttu-id="ff526-106">[PlannerUser リソースを更新](planneruser-update.md)することによって、最近表示した計画を更新できます。</span><span class="sxs-lookup"><span data-stu-id="ff526-106">You can update recently viewed plans by [updating the plannerUser resource](planneruser-update.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="ff526-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ff526-107">Permissions</span></span>
<span data-ttu-id="ff526-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ff526-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff526-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ff526-110">Permission type</span></span>      | <span data-ttu-id="ff526-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ff526-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff526-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ff526-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ff526-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="ff526-113">Group.Read.All</span></span>    |
|<span data-ttu-id="ff526-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ff526-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff526-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff526-115">Not supported.</span></span>    |
|<span data-ttu-id="ff526-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ff526-116">Application</span></span> | <span data-ttu-id="ff526-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff526-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff526-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ff526-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/recentPlans
GET /users/<id>/planner/recentPlans
```

## <a name="request-headers"></a><span data-ttu-id="ff526-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ff526-119">Request headers</span></span>
| <span data-ttu-id="ff526-120">名前</span><span class="sxs-lookup"><span data-stu-id="ff526-120">Name</span></span>      |<span data-ttu-id="ff526-121">説明</span><span class="sxs-lookup"><span data-stu-id="ff526-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ff526-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff526-122">Authorization</span></span>  | <span data-ttu-id="ff526-p104">Bearer {code}。必須。</span><span class="sxs-lookup"><span data-stu-id="ff526-p104">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff526-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="ff526-125">Request body</span></span>
<span data-ttu-id="ff526-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ff526-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ff526-127">応答</span><span class="sxs-lookup"><span data-stu-id="ff526-127">Response</span></span>
<span data-ttu-id="ff526-128">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[plannerPlan](../resources/plannerplan.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="ff526-128">If successful, this method returns a `200 OK` response code and a collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ff526-129">例</span><span class="sxs-lookup"><span data-stu-id="ff526-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ff526-130">要求</span><span class="sxs-lookup"><span data-stu-id="ff526-130">Request</span></span>
<span data-ttu-id="ff526-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ff526-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_recentplans"
}-->
```http
GET https://graph.microsoft.com/beta/me/planner/recentPlans
```
##### <a name="response"></a><span data-ttu-id="ff526-132">応答</span><span class="sxs-lookup"><span data-stu-id="ff526-132">Response</span></span>
<span data-ttu-id="ff526-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ff526-133">The following is an example of the response.</span></span> 

><span data-ttu-id="ff526-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="ff526-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "List recentPlans",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/planneruser-list-recentplans.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
