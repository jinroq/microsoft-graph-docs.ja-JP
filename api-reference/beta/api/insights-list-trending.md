---
title: 人気上昇中を一覧表示する
description: ユーザーの周囲のアイテムのリストを返す、計算された洞察。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 2d84e2c4470b17b3073856a73d0b8cb7251ea830
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35953060"
---
# <a name="list-trending"></a><span data-ttu-id="fe955-103">人気上昇中を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="fe955-103">List trending</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe955-104">ユーザーの周囲のアイテムのリストを返す、計算された洞察。</span><span class="sxs-lookup"><span data-stu-id="fe955-104">Calculated insight that returns the list of items trending around the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe955-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fe955-105">Permissions</span></span>
<span data-ttu-id="fe955-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fe955-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fe955-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fe955-108">Permission type</span></span>      | <span data-ttu-id="fe955-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fe955-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe955-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fe955-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fe955-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe955-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="fe955-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fe955-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe955-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe955-113">Not supported.</span></span>    |
|<span data-ttu-id="fe955-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fe955-114">Application</span></span> | <span data-ttu-id="fe955-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe955-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe955-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fe955-116">HTTP request</span></span>
```http
GET /me/insights/trending
GET /users/{id | userPrincipalName}/insights/trending
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fe955-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="fe955-117">Optional query parameters</span></span>
<span data-ttu-id="fe955-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="fe955-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="fe955-119">クエリパラメーターを使用`$filter`して、傾向分析項目をフィルター処理できます。</span><span class="sxs-lookup"><span data-stu-id="fe955-119">You can use the `$filter` query parameter to filter trending items.</span></span> <span data-ttu-id="fe955-120">たとえば、Type に基づいています。</span><span class="sxs-lookup"><span data-stu-id="fe955-120">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="fe955-121">またはコンテナーの種類に基づきます。</span><span class="sxs-lookup"><span data-stu-id="fe955-121">Or based on Container Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="fe955-122">利用可能なコンテナーの種類と種類を表示します。これは、 [Resourcevisualization](../resources/insights-resourcevisualization.md)でフィルター処理できます。</span><span class="sxs-lookup"><span data-stu-id="fe955-122">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="fe955-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fe955-123">Request headers</span></span>
| <span data-ttu-id="fe955-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fe955-124">Header</span></span>       |  <span data-ttu-id="fe955-125">値</span><span class="sxs-lookup"><span data-stu-id="fe955-125">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="fe955-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe955-126">Authorization</span></span>  | <span data-ttu-id="fe955-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fe955-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="fe955-129">承諾</span><span class="sxs-lookup"><span data-stu-id="fe955-129">Accept</span></span>  | <span data-ttu-id="fe955-130">application/json</span><span class="sxs-lookup"><span data-stu-id="fe955-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe955-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="fe955-131">Request body</span></span>
<span data-ttu-id="fe955-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fe955-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe955-133">応答</span><span class="sxs-lookup"><span data-stu-id="fe955-133">Response</span></span>

<span data-ttu-id="fe955-134">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[傾向](../resources/insights-trending.md)項目のリストを返します。</span><span class="sxs-lookup"><span data-stu-id="fe955-134">If successful, this method returns a `200 OK` response code and a list of [trending](../resources/insights-trending.md) items in the response body.</span></span> <span data-ttu-id="fe955-135">各アイテムには、アイテムを表示するための視覚エフェクトプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="fe955-135">Each item contains visualization properties for displaying the item in your experience.</span></span>

## <a name="example"></a><span data-ttu-id="fe955-136">例</span><span class="sxs-lookup"><span data-stu-id="fe955-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="fe955-137">要求</span><span class="sxs-lookup"><span data-stu-id="fe955-137">Request</span></span>
<span data-ttu-id="fe955-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fe955-138">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/trending
```
#### <a name="response"></a><span data-ttu-id="fe955-139">応答</span><span class="sxs-lookup"><span data-stu-id="fe955-139">Response</span></span>
<span data-ttu-id="fe955-140">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="fe955-140">Here is an example of the response.</span></span> <span data-ttu-id="fe955-141">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="fe955-141">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="fe955-142">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="fe955-142">All of the properties will be returned from an actual call.</span></span> <span data-ttu-id="fe955-143">ページの下部にある、切り捨てられていない応答の例を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fe955-143">See an example un-truncated response at the bottom of the page.</span></span>
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

### <a name="expanding-resource"></a><span data-ttu-id="fe955-144">リソースの展開</span><span class="sxs-lookup"><span data-stu-id="fe955-144">Expanding resource</span></span>
<span data-ttu-id="fe955-145">傾向分析によって参照されているリソースを展開できます。</span><span class="sxs-lookup"><span data-stu-id="fe955-145">The resource referenced by a trending insight can be expanded.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/trending/{id}/resource
```
