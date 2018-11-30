---
title: PlannerUser を取得します。
description: 'プロパティと、plannerUser オブジェクトの関係を取得します。 返されるプロパティは、ユーザーのお気に入りのプランが含まれ、計画が最近閲覧しました。 '
ms.openlocfilehash: fca4b37560ad0c6cd7e05aee56ebdeb1e6509101
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067006"
---
# <a name="get-planneruser"></a><span data-ttu-id="ff8d1-104">PlannerUser を取得します。</span><span class="sxs-lookup"><span data-stu-id="ff8d1-104">Get plannerUser</span></span>

> <span data-ttu-id="ff8d1-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ff8d1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff8d1-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff8d1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ff8d1-107">プロパティと、 [plannerUser](../resources/planneruser.md)オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="ff8d1-107">Retrieve the properties and relationships of a [plannerUser](../resources/planneruser.md) object.</span></span> <span data-ttu-id="ff8d1-108">返されるプロパティは、ユーザーのお気に入りのプランが含まれ、計画が最近閲覧しました。</span><span class="sxs-lookup"><span data-stu-id="ff8d1-108">The returned properties include the user's favorite plans and recently viewed plans.</span></span> 
## <a name="permissions"></a><span data-ttu-id="ff8d1-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ff8d1-109">Permissions</span></span>
<span data-ttu-id="ff8d1-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ff8d1-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff8d1-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ff8d1-112">Permission type</span></span>      | <span data-ttu-id="ff8d1-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ff8d1-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff8d1-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ff8d1-114">Delegated (work or school account)</span></span> | <span data-ttu-id="ff8d1-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="ff8d1-115">Group.Read.All</span></span>    |
|<span data-ttu-id="ff8d1-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ff8d1-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff8d1-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff8d1-117">Not supported.</span></span>    |
|<span data-ttu-id="ff8d1-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ff8d1-118">Application</span></span> | <span data-ttu-id="ff8d1-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff8d1-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff8d1-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ff8d1-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner
GET /users/<id>/planner
```

## <a name="request-headers"></a><span data-ttu-id="ff8d1-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ff8d1-121">Request headers</span></span>
| <span data-ttu-id="ff8d1-122">名前</span><span class="sxs-lookup"><span data-stu-id="ff8d1-122">Name</span></span>      |<span data-ttu-id="ff8d1-123">説明</span><span class="sxs-lookup"><span data-stu-id="ff8d1-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ff8d1-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff8d1-124">Authorization</span></span>  | <span data-ttu-id="ff8d1-p105">Bearer {code}。必須。</span><span class="sxs-lookup"><span data-stu-id="ff8d1-p105">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff8d1-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ff8d1-127">Request body</span></span>
<span data-ttu-id="ff8d1-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ff8d1-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ff8d1-129">応答</span><span class="sxs-lookup"><span data-stu-id="ff8d1-129">Response</span></span>
<span data-ttu-id="ff8d1-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[plannerUser](../resources/planneruser.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="ff8d1-130">If successful, this method returns a `200 OK` response code and a [plannerUser](../resources/planneruser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ff8d1-131">例</span><span class="sxs-lookup"><span data-stu-id="ff8d1-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ff8d1-132">要求</span><span class="sxs-lookup"><span data-stu-id="ff8d1-132">Request</span></span>
<span data-ttu-id="ff8d1-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ff8d1-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_planneruser"
}-->
```http
GET https://graph.microsoft.com/beta/me/planner
```
##### <a name="response"></a><span data-ttu-id="ff8d1-134">応答</span><span class="sxs-lookup"><span data-stu-id="ff8d1-134">Response</span></span>
<span data-ttu-id="ff8d1-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ff8d1-135">The following is an example of the response.</span></span> 

><span data-ttu-id="ff8d1-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="ff8d1-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 979

{
  "favoritePlanReferences": {
    "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
      "@odata.type": "#microsoft.graph.plannerFavoritePlanReference",
      "orderHint": "8586866870001551087",
      "planTitle": "Next Release Discussion"
    },
    "uZWtCtli30CGoWLIWSat1mQAC0ai": {
      "@odata.type": "#microsoft.graph.plannerFavoritePlanReference",
      "orderHint": "8586888705198093378",
      "planTitle": "Product Support"
    }
  },
  "recentPlanReferences": {
    "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
      "@odata.type": "#microsoft.graph.plannerRecentPlanReference",
      "lastAccessedDateTime": "2018-01-02T22:49:46.155Z",
      "planTitle": "Next Release Discussion"
    },
    "XYE5pqNJu0uuRC2PM4ZQrmQAF2Pn": {
      "@odata.type": "#microsoft.graph.plannerRecentPlanReference",
      "lastAccessedDateTime": "2018-01-01T19:39:17.57Z",
      "planTitle": "Success Metrics"
    }
  },
  "id": "-YPnMJRiIUSKFyaVjYEkBWQAAc47"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
