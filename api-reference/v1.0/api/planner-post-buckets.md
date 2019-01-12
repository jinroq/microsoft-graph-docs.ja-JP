---
title: Create plannerBucket
description: この API を使用して、新しい **plannerBucket** を作成します。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 5d642779f7ca179a6de485fae2caaafd065c050d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948353"
---
# <a name="create-plannerbucket"></a><span data-ttu-id="1783e-103">Create plannerBucket</span><span class="sxs-lookup"><span data-stu-id="1783e-103">Create plannerBucket</span></span>

<span data-ttu-id="1783e-104">この API を使用して、新しい **plannerBucket** を作成します。</span><span class="sxs-lookup"><span data-stu-id="1783e-104">Use this API to create a new **plannerBucket**.</span></span>

## <a name="permissions"></a><span data-ttu-id="1783e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1783e-105">Permissions</span></span>
<span data-ttu-id="1783e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1783e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1783e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1783e-108">Permission type</span></span>      | <span data-ttu-id="1783e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1783e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1783e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1783e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1783e-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1783e-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1783e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1783e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1783e-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1783e-113">Not supported.</span></span>    |
|<span data-ttu-id="1783e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1783e-114">Application</span></span> | <span data-ttu-id="1783e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1783e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1783e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1783e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /planner/buckets

```
## <a name="request-headers"></a><span data-ttu-id="1783e-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1783e-117">Request headers</span></span>
| <span data-ttu-id="1783e-118">名前</span><span class="sxs-lookup"><span data-stu-id="1783e-118">Name</span></span>       | <span data-ttu-id="1783e-119">説明</span><span class="sxs-lookup"><span data-stu-id="1783e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1783e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1783e-120">Authorization</span></span>  | <span data-ttu-id="1783e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1783e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1783e-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="1783e-123">Request body</span></span>
<span data-ttu-id="1783e-124">要求本文で、[plannerBucket](../resources/plannerbucket.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1783e-124">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1783e-125">応答</span><span class="sxs-lookup"><span data-stu-id="1783e-125">Response</span></span>

<span data-ttu-id="1783e-126">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [plannerBucket](../resources/plannerbucket.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1783e-126">If successful, this method returns `201 Created` response code and [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="1783e-p103">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、400、403 および 404 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1783e-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="1783e-130">例</span><span class="sxs-lookup"><span data-stu-id="1783e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1783e-131">要求</span><span class="sxs-lookup"><span data-stu-id="1783e-131">Request</span></span>
<span data-ttu-id="1783e-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1783e-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_plannerbucket_from_planner"
}-->
```http
POST https://graph.microsoft.com/v1.0/planner/buckets
Content-type: application/json
Content-length: 92

{
  "name": "Advertising",
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "orderHint": " !"
}
```
<span data-ttu-id="1783e-133">要求本文で、[plannerBucket](../resources/plannerbucket.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1783e-133">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="1783e-134">応答</span><span class="sxs-lookup"><span data-stu-id="1783e-134">Response</span></span>
<span data-ttu-id="1783e-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1783e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 145

{
  "name": "Advertising",
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "orderHint": "85752723360752+",
  "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create plannerBucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
