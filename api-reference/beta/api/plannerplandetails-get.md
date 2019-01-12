---
title: Get plannerPlanDetails
description: '**plannerplandetails** オブジェクトのプロパティと関係を取得します。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 0e2931a36382c679e901a72caf42012f6cab303a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940275"
---
# <a name="get-plannerplandetails"></a><span data-ttu-id="60b06-103">Get plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="60b06-103">Get plannerPlanDetails</span></span>

> <span data-ttu-id="60b06-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="60b06-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="60b06-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60b06-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="60b06-106">**plannerplandetails** オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="60b06-106">Retrieve the properties and relationships of **plannerplandetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="60b06-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="60b06-107">Permissions</span></span>
<span data-ttu-id="60b06-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="60b06-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60b06-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="60b06-110">Permission type</span></span>      | <span data-ttu-id="60b06-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="60b06-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60b06-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="60b06-112">Delegated (work or school account)</span></span> | <span data-ttu-id="60b06-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60b06-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="60b06-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="60b06-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60b06-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60b06-115">Not supported.</span></span>    |
|<span data-ttu-id="60b06-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="60b06-116">Application</span></span> | <span data-ttu-id="60b06-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60b06-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="60b06-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="60b06-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/<id>/details
```

## <a name="request-headers"></a><span data-ttu-id="60b06-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="60b06-119">Request headers</span></span>
| <span data-ttu-id="60b06-120">名前</span><span class="sxs-lookup"><span data-stu-id="60b06-120">Name</span></span>      |<span data-ttu-id="60b06-121">説明</span><span class="sxs-lookup"><span data-stu-id="60b06-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="60b06-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="60b06-122">Authorization</span></span>  | <span data-ttu-id="60b06-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="60b06-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="60b06-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="60b06-125">Request body</span></span>
<span data-ttu-id="60b06-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="60b06-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60b06-127">応答</span><span class="sxs-lookup"><span data-stu-id="60b06-127">Response</span></span>

<span data-ttu-id="60b06-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [plannerPlanDetails](../resources/plannerplandetails.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="60b06-128">If successful, this method returns a `200 OK` response code and [plannerPlanDetails](../resources/plannerplandetails.md) object in the response body.</span></span>

<span data-ttu-id="60b06-p104">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、403 および 404 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="60b06-p104">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="60b06-132">例</span><span class="sxs-lookup"><span data-stu-id="60b06-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="60b06-133">要求</span><span class="sxs-lookup"><span data-stu-id="60b06-133">Request</span></span>
<span data-ttu-id="60b06-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="60b06-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannerplandetails"
}-->
```http
GET https://graph.microsoft.com/beta/planner/plans/xqQg5FS2LkCp935s-FIFm2QAFkHM/details
```
##### <a name="response"></a><span data-ttu-id="60b06-135">応答</span><span class="sxs-lookup"><span data-stu-id="60b06-135">Response</span></span>
<span data-ttu-id="60b06-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="60b06-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlanDetails"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 373

{
  "sharedWith": {
    "aaa27244-1db4-476a-a5cb-004607466324" : true,
    "6463a5ce-2119-4198-9f2a-628761df4a62" : true
  },
  "categoryDescriptions": {
    "category1": "Indoors",
    "category2": "Outdoors",
    "category3": null,
    "category4": null,
    "category5": "Needs materials",
    "category6": "Needs equipment"
  },
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerPlanDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
