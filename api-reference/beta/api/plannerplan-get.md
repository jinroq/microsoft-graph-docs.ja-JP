---
title: Get plannerPlan
description: '**plannerplan** オブジェクトのプロパティと関係を取得します。'
ms.openlocfilehash: 5b8ad9f212a3e5010ac7479ddfafca250bbb2f01
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074437"
---
# <a name="get-plannerplan"></a><span data-ttu-id="c18b3-103">Get plannerPlan</span><span class="sxs-lookup"><span data-stu-id="c18b3-103">Get plannerPlan</span></span>

> <span data-ttu-id="c18b3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c18b3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c18b3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c18b3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c18b3-106">**plannerplan** オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="c18b3-106">Retrieve the properties and relationships of **plannerplan** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c18b3-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c18b3-107">Permissions</span></span>
<span data-ttu-id="c18b3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c18b3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c18b3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c18b3-110">Permission type</span></span>      | <span data-ttu-id="c18b3-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c18b3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c18b3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c18b3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c18b3-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c18b3-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c18b3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c18b3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c18b3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c18b3-115">Not supported.</span></span>    |
|<span data-ttu-id="c18b3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c18b3-116">Application</span></span> | <span data-ttu-id="c18b3-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c18b3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c18b3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c18b3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/<id>
```
## <a name="request-headers"></a><span data-ttu-id="c18b3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c18b3-119">Request headers</span></span>
| <span data-ttu-id="c18b3-120">名前</span><span class="sxs-lookup"><span data-stu-id="c18b3-120">Name</span></span>      |<span data-ttu-id="c18b3-121">説明</span><span class="sxs-lookup"><span data-stu-id="c18b3-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c18b3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c18b3-122">Authorization</span></span>  | <span data-ttu-id="c18b3-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c18b3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c18b3-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="c18b3-125">Request body</span></span>
<span data-ttu-id="c18b3-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c18b3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c18b3-127">応答</span><span class="sxs-lookup"><span data-stu-id="c18b3-127">Response</span></span>

<span data-ttu-id="c18b3-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [plannerPlan](../resources/plannerplan.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c18b3-128">If successful, this method returns a `200 OK` response code and [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="c18b3-p104">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、403 および 404 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c18b3-p104">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="c18b3-132">例</span><span class="sxs-lookup"><span data-stu-id="c18b3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c18b3-133">要求</span><span class="sxs-lookup"><span data-stu-id="c18b3-133">Request</span></span>
<span data-ttu-id="c18b3-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c18b3-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannerplan"
}-->
```http
GET https://graph.microsoft.com/beta/planner/plans/<id>
```
##### <a name="response"></a><span data-ttu-id="c18b3-135">応答</span><span class="sxs-lookup"><span data-stu-id="c18b3-135">Response</span></span>
<span data-ttu-id="c18b3-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c18b3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 357

{
  "createdBy": {
    "application": {
      "id": "95e27074-6c4a-447a-aa24-9d718a0b86fa"
    },
    "user": {
      "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
    }
  },
  "createdDateTime": "2015-03-30T18:36:49.2407981Z",
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value",
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerPlan",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->