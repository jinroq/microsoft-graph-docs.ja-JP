---
title: リストのトレンド分析
description: ユーザーのトレンド分析項目の一覧を返す計算の把握。
author: simonhult
ms.openlocfilehash: de169f9960a1694e452b8dcfd16aafde89d3ac29
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343415"
---
# <a name="list-trending"></a><span data-ttu-id="9d50b-103">リストのトレンド分析</span><span class="sxs-lookup"><span data-stu-id="9d50b-103">List trending</span></span>

> <span data-ttu-id="9d50b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9d50b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9d50b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d50b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9d50b-106">ユーザーのトレンド分析項目の一覧を返す計算の把握。</span><span class="sxs-lookup"><span data-stu-id="9d50b-106">Calculated insight that returns the list of items trending around the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d50b-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9d50b-107">Permissions</span></span>
<span data-ttu-id="9d50b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9d50b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9d50b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9d50b-110">Permission type</span></span>      | <span data-ttu-id="9d50b-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9d50b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d50b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9d50b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9d50b-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d50b-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="9d50b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9d50b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d50b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d50b-115">Not supported.</span></span>    |
|<span data-ttu-id="9d50b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9d50b-116">Application</span></span> | <span data-ttu-id="9d50b-117">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d50b-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d50b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9d50b-118">HTTP request</span></span>
```http
GET /me/insights/trending
GET /users/{id | userPrincipalName}/insights/trending
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9d50b-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="9d50b-119">Optional query parameters</span></span>
<span data-ttu-id="9d50b-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="9d50b-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="9d50b-121">使用することができます、`$filter`トレンドのアイテムをフィルターするパラメーター クエリを実行します。</span><span class="sxs-lookup"><span data-stu-id="9d50b-121">You can use the `$filter` query parameter to filter trending items.</span></span> <span data-ttu-id="9d50b-122">などは、型に基づいています。</span><span class="sxs-lookup"><span data-stu-id="9d50b-122">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="9d50b-123">コンテナーの種類に基づくか。</span><span class="sxs-lookup"><span data-stu-id="9d50b-123">Or based on Container Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="9d50b-124">使用可能なコンテナーの種類と[resourceVisualization](../resources/insights-resourcevisualization.md)内でフィルターの種類を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9d50b-124">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="9d50b-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9d50b-125">Request headers</span></span>
| <span data-ttu-id="9d50b-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9d50b-126">Header</span></span>       |  <span data-ttu-id="9d50b-127">値</span><span class="sxs-lookup"><span data-stu-id="9d50b-127">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="9d50b-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d50b-128">Authorization</span></span>  | <span data-ttu-id="9d50b-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9d50b-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="9d50b-131">承諾</span><span class="sxs-lookup"><span data-stu-id="9d50b-131">Accept</span></span>  | <span data-ttu-id="9d50b-132">application/json</span><span class="sxs-lookup"><span data-stu-id="9d50b-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d50b-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="9d50b-133">Request body</span></span>
<span data-ttu-id="9d50b-134">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9d50b-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d50b-135">応答</span><span class="sxs-lookup"><span data-stu-id="9d50b-135">Response</span></span>

<span data-ttu-id="9d50b-136">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の[トレンド分析](../resources/insights-trending.md)の項目の一覧です。</span><span class="sxs-lookup"><span data-stu-id="9d50b-136">If successful, this method returns a `200 OK` response code and a list of [trending](../resources/insights-trending.md) items in the response body.</span></span> <span data-ttu-id="9d50b-137">各項目には、時にアイテムを表示するための視覚エフェクトのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="9d50b-137">Each item contains visualization properties for displaying the item in your experience.</span></span>

## <a name="example"></a><span data-ttu-id="9d50b-138">例</span><span class="sxs-lookup"><span data-stu-id="9d50b-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="9d50b-139">要求</span><span class="sxs-lookup"><span data-stu-id="9d50b-139">Request</span></span>
<span data-ttu-id="9d50b-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9d50b-140">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/trending
```
#### <a name="response"></a><span data-ttu-id="9d50b-141">応答</span><span class="sxs-lookup"><span data-stu-id="9d50b-141">Response</span></span>
<span data-ttu-id="9d50b-142">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="9d50b-142">Here is an example of the response.</span></span> <span data-ttu-id="9d50b-143">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="9d50b-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9d50b-144">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="9d50b-144">All of the properties will be returned from an actual call.</span></span> <span data-ttu-id="9d50b-145">ページの下部にある、例の切り捨てられていない応答を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9d50b-145">See an example un-truncated response at the bottom of the page.</span></span>
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

### <a name="expanding-resource"></a><span data-ttu-id="9d50b-146">リソースを展開します。</span><span class="sxs-lookup"><span data-stu-id="9d50b-146">Expanding resource</span></span>
<span data-ttu-id="9d50b-147">トレンドの把握によって参照されるリソースを展開します。</span><span class="sxs-lookup"><span data-stu-id="9d50b-147">The resource referenced by a trending insight can be expanded.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/trending/{id}/resource
```
