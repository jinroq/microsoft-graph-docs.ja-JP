---
title: プランのユーザーを取得する
description: 'プランユーザーオブジェクトのプロパティとリレーションシップを取得します。 返されるプロパティには、ユーザーのお気に入りのプランと最近表示されたプランが含まれます。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: bf4c0bdc613795294e9657a30e27aa42732e1085
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36413021"
---
# <a name="get-planneruser"></a><span data-ttu-id="364fb-104">プランのユーザーを取得する</span><span class="sxs-lookup"><span data-stu-id="364fb-104">Get plannerUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="364fb-105">[プランユーザー](../resources/planneruser.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="364fb-105">Retrieve the properties and relationships of a [plannerUser](../resources/planneruser.md) object.</span></span> <span data-ttu-id="364fb-106">返されるプロパティには、ユーザーのお気に入りのプランと最近表示されたプランが含まれます。</span><span class="sxs-lookup"><span data-stu-id="364fb-106">The returned properties include the user's favorite plans and recently viewed plans.</span></span> 
## <a name="permissions"></a><span data-ttu-id="364fb-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="364fb-107">Permissions</span></span>
<span data-ttu-id="364fb-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="364fb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="364fb-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="364fb-110">Permission type</span></span>      | <span data-ttu-id="364fb-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="364fb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="364fb-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="364fb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="364fb-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="364fb-113">Group.Read.All</span></span>    |
|<span data-ttu-id="364fb-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="364fb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="364fb-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="364fb-115">Not supported.</span></span>    |
|<span data-ttu-id="364fb-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="364fb-116">Application</span></span> | <span data-ttu-id="364fb-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="364fb-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="364fb-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="364fb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner
GET /users/{id}/planner
```

## <a name="request-headers"></a><span data-ttu-id="364fb-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="364fb-119">Request headers</span></span>
| <span data-ttu-id="364fb-120">名前</span><span class="sxs-lookup"><span data-stu-id="364fb-120">Name</span></span>      |<span data-ttu-id="364fb-121">説明</span><span class="sxs-lookup"><span data-stu-id="364fb-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="364fb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="364fb-122">Authorization</span></span>  | <span data-ttu-id="364fb-123">ベアラー {code}。</span><span class="sxs-lookup"><span data-stu-id="364fb-123">Bearer {code}.</span></span> <span data-ttu-id="364fb-124">必須です。</span><span class="sxs-lookup"><span data-stu-id="364fb-124">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="364fb-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="364fb-125">Request body</span></span>
<span data-ttu-id="364fb-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="364fb-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="364fb-127">応答</span><span class="sxs-lookup"><span data-stu-id="364fb-127">Response</span></span>
<span data-ttu-id="364fb-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[プランのユーザー](../resources/planneruser.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="364fb-128">If successful, this method returns a `200 OK` response code and a [plannerUser](../resources/planneruser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="364fb-129">例</span><span class="sxs-lookup"><span data-stu-id="364fb-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="364fb-130">要求</span><span class="sxs-lookup"><span data-stu-id="364fb-130">Request</span></span>
<span data-ttu-id="364fb-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="364fb-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_planneruser"
}-->
```http
GET https://graph.microsoft.com/beta/me/planner
```
##### <a name="response"></a><span data-ttu-id="364fb-132">応答</span><span class="sxs-lookup"><span data-stu-id="364fb-132">Response</span></span>
<span data-ttu-id="364fb-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="364fb-133">The following is an example of the response.</span></span> 

><span data-ttu-id="364fb-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="364fb-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Get plannerUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
