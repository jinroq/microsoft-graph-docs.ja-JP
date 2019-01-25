---
title: Get plannerPlan
description: '**plannerplan** オブジェクトのプロパティと関係を取得します。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 8859452848f8459cba596b95503a8355c331c05d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512340"
---
# <a name="get-plannerplan"></a><span data-ttu-id="be2b4-103">Get plannerPlan</span><span class="sxs-lookup"><span data-stu-id="be2b4-103">Get plannerPlan</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be2b4-104">**plannerplan** オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="be2b4-104">Retrieve the properties and relationships of **plannerplan** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="be2b4-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="be2b4-105">Permissions</span></span>
<span data-ttu-id="be2b4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="be2b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be2b4-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="be2b4-108">Permission type</span></span>      | <span data-ttu-id="be2b4-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="be2b4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be2b4-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="be2b4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="be2b4-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be2b4-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="be2b4-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="be2b4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be2b4-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be2b4-113">Not supported.</span></span>    |
|<span data-ttu-id="be2b4-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="be2b4-114">Application</span></span> | <span data-ttu-id="be2b4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be2b4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="be2b4-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="be2b4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/<id>
```
## <a name="request-headers"></a><span data-ttu-id="be2b4-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="be2b4-117">Request headers</span></span>
| <span data-ttu-id="be2b4-118">名前</span><span class="sxs-lookup"><span data-stu-id="be2b4-118">Name</span></span>      |<span data-ttu-id="be2b4-119">説明</span><span class="sxs-lookup"><span data-stu-id="be2b4-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="be2b4-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="be2b4-120">Authorization</span></span>  | <span data-ttu-id="be2b4-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="be2b4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="be2b4-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="be2b4-123">Request body</span></span>
<span data-ttu-id="be2b4-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="be2b4-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be2b4-125">応答</span><span class="sxs-lookup"><span data-stu-id="be2b4-125">Response</span></span>

<span data-ttu-id="be2b4-126">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [plannerPlan](../resources/plannerplan.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="be2b4-126">If successful, this method returns a `200 OK` response code and [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="be2b4-p103">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、403 および 404 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="be2b4-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="be2b4-130">例</span><span class="sxs-lookup"><span data-stu-id="be2b4-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="be2b4-131">要求</span><span class="sxs-lookup"><span data-stu-id="be2b4-131">Request</span></span>
<span data-ttu-id="be2b4-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="be2b4-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannerplan"
}-->
```http
GET https://graph.microsoft.com/beta/planner/plans/<id>
```
##### <a name="response"></a><span data-ttu-id="be2b4-133">応答</span><span class="sxs-lookup"><span data-stu-id="be2b4-133">Response</span></span>
<span data-ttu-id="be2b4-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="be2b4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get plannerPlan",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/plannerplan-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
