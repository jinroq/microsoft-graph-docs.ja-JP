---
title: リストのトレンド分析
description: ユーザーのトレンド分析項目の一覧を返す計算の把握。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 512dcdfb8a94a2a90c47c4005298537d1d83f137
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525109"
---
# <a name="list-trending"></a><span data-ttu-id="2e87a-103">リストのトレンド分析</span><span class="sxs-lookup"><span data-stu-id="2e87a-103">List trending</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e87a-104">ユーザーのトレンド分析項目の一覧を返す計算の把握。</span><span class="sxs-lookup"><span data-stu-id="2e87a-104">Calculated insight that returns the list of items trending around the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e87a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2e87a-105">Permissions</span></span>
<span data-ttu-id="2e87a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2e87a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2e87a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2e87a-108">Permission type</span></span>      | <span data-ttu-id="2e87a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2e87a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e87a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2e87a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2e87a-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e87a-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2e87a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2e87a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e87a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2e87a-113">Not supported.</span></span>    |
|<span data-ttu-id="2e87a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2e87a-114">Application</span></span> | <span data-ttu-id="2e87a-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e87a-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e87a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2e87a-116">HTTP request</span></span>
```http
GET /me/insights/trending
GET /users/{id | userPrincipalName}/insights/trending
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2e87a-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2e87a-117">Optional query parameters</span></span>
<span data-ttu-id="2e87a-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2e87a-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="2e87a-119">使用することができます、`$filter`トレンドのアイテムをフィルターするパラメーター クエリを実行します。</span><span class="sxs-lookup"><span data-stu-id="2e87a-119">You can use the `$filter` query parameter to filter trending items.</span></span> <span data-ttu-id="2e87a-120">などは、型に基づいています。</span><span class="sxs-lookup"><span data-stu-id="2e87a-120">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="2e87a-121">コンテナーの種類に基づくか。</span><span class="sxs-lookup"><span data-stu-id="2e87a-121">Or based on Container Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="2e87a-122">使用可能なコンテナーの種類と[resourceVisualization](../resources/insights-resourcevisualization.md)内でフィルターの種類を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2e87a-122">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="2e87a-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2e87a-123">Request headers</span></span>
| <span data-ttu-id="2e87a-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2e87a-124">Header</span></span>       |  <span data-ttu-id="2e87a-125">値</span><span class="sxs-lookup"><span data-stu-id="2e87a-125">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="2e87a-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e87a-126">Authorization</span></span>  | <span data-ttu-id="2e87a-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2e87a-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="2e87a-129">承諾</span><span class="sxs-lookup"><span data-stu-id="2e87a-129">Accept</span></span>  | <span data-ttu-id="2e87a-130">application/json</span><span class="sxs-lookup"><span data-stu-id="2e87a-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e87a-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="2e87a-131">Request body</span></span>
<span data-ttu-id="2e87a-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2e87a-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e87a-133">応答</span><span class="sxs-lookup"><span data-stu-id="2e87a-133">Response</span></span>

<span data-ttu-id="2e87a-134">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の[トレンド分析](../resources/insights-trending.md)の項目の一覧です。</span><span class="sxs-lookup"><span data-stu-id="2e87a-134">If successful, this method returns a `200 OK` response code and a list of [trending](../resources/insights-trending.md) items in the response body.</span></span> <span data-ttu-id="2e87a-135">各項目には、時にアイテムを表示するための視覚エフェクトのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="2e87a-135">Each item contains visualization properties for displaying the item in your experience.</span></span>

## <a name="example"></a><span data-ttu-id="2e87a-136">例</span><span class="sxs-lookup"><span data-stu-id="2e87a-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2e87a-137">要求</span><span class="sxs-lookup"><span data-stu-id="2e87a-137">Request</span></span>
<span data-ttu-id="2e87a-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2e87a-138">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/trending
```
#### <a name="response"></a><span data-ttu-id="2e87a-139">応答</span><span class="sxs-lookup"><span data-stu-id="2e87a-139">Response</span></span>
<span data-ttu-id="2e87a-140">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="2e87a-140">Here is an example of the response.</span></span> <span data-ttu-id="2e87a-141">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="2e87a-141">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="2e87a-142">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="2e87a-142">All of the properties will be returned from an actual call.</span></span> <span data-ttu-id="2e87a-143">ページの下部にある、例の切り捨てられていない応答を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2e87a-143">See an example un-truncated response at the bottom of the page.</span></span>
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 801

{
    "value": [
        {
            "id": "id-value",
            "weight": "weight-value",
            "resourceVisualization": {
                "title": "title-value",
                "type": "type-value",
                "mediaType": "mediaType-value",
                "previewImageUrl": "previewImageUrl-value",
                "previewText": "previewText-value",
                "containerWebUrl": "containerWebUrl-value",
                "containerDisplayName": "containerDisplayName-value",
                "containerType": "containerType-value"
            },
            "resourceReference": {
                "webUrl": "webUrl-value",
                "id": "id-value",
                "type": "type-value"
            }
        }
    ]
}
```

### <a name="expanding-resource"></a><span data-ttu-id="2e87a-144">リソースを展開します。</span><span class="sxs-lookup"><span data-stu-id="2e87a-144">Expanding resource</span></span>
<span data-ttu-id="2e87a-145">トレンドの把握によって参照されるリソースを展開します。</span><span class="sxs-lookup"><span data-stu-id="2e87a-145">The resource referenced by a trending insight can be expanded.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/trending/{id}/resource
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/insights-list-trending.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
