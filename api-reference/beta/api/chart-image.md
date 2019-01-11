---
title: グラフ:画像
description: 指定したサイズに合わせてグラフを拡大、縮小することで、グラフを Base64 でエンコードされた画像としてレンダリングします。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: d7d3b0bc33be46301a4abffa90d37c53c553e37d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854237"
---
# <a name="chart-image"></a><span data-ttu-id="9a913-103">グラフ:画像</span><span class="sxs-lookup"><span data-stu-id="9a913-103">Chart: Image</span></span>

> <span data-ttu-id="9a913-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9a913-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9a913-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a913-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9a913-106">指定したサイズに合わせてグラフを拡大、縮小することで、グラフを Base64 でエンコードされた画像としてレンダリングします。</span><span class="sxs-lookup"><span data-stu-id="9a913-106">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>
## <a name="permissions"></a><span data-ttu-id="9a913-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9a913-107">Permissions</span></span>
<span data-ttu-id="9a913-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9a913-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a913-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9a913-110">Permission type</span></span>      | <span data-ttu-id="9a913-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9a913-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a913-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9a913-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9a913-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9a913-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9a913-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9a913-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a913-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9a913-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9a913-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9a913-116">Application</span></span> | <span data-ttu-id="9a913-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a913-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a913-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9a913-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts(<name>)/Image(width=0,height=0,fittingMode='fit')

```
## <a name="request-headers"></a><span data-ttu-id="9a913-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9a913-119">Request headers</span></span>
| <span data-ttu-id="9a913-120">名前</span><span class="sxs-lookup"><span data-stu-id="9a913-120">Name</span></span>       | <span data-ttu-id="9a913-121">説明</span><span class="sxs-lookup"><span data-stu-id="9a913-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9a913-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a913-122">Authorization</span></span>  | <span data-ttu-id="9a913-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9a913-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9a913-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9a913-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="9a913-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="9a913-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a913-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="9a913-128">Request body</span></span>
<span data-ttu-id="9a913-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="9a913-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9a913-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="9a913-130">Parameter</span></span>    | <span data-ttu-id="9a913-131">Type</span><span class="sxs-lookup"><span data-stu-id="9a913-131">Type</span></span>   |<span data-ttu-id="9a913-132">説明</span><span class="sxs-lookup"><span data-stu-id="9a913-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a913-133">height</span><span class="sxs-lookup"><span data-stu-id="9a913-133">height</span></span>|<span data-ttu-id="9a913-134">number</span><span class="sxs-lookup"><span data-stu-id="9a913-134">number</span></span>|<span data-ttu-id="9a913-p105">省略可能。結果の画像の希望する高さ。</span><span class="sxs-lookup"><span data-stu-id="9a913-p105">Optional. The desired height of the resulting image.</span></span>|
|<span data-ttu-id="9a913-137">width</span><span class="sxs-lookup"><span data-stu-id="9a913-137">width</span></span>|<span data-ttu-id="9a913-138">number</span><span class="sxs-lookup"><span data-stu-id="9a913-138">number</span></span>|<span data-ttu-id="9a913-p106">省略可能。結果の画像の希望する幅。</span><span class="sxs-lookup"><span data-stu-id="9a913-p106">Optional. The desired width of the resulting image.</span></span>|
|<span data-ttu-id="9a913-141">fittingMode</span><span class="sxs-lookup"><span data-stu-id="9a913-141">fittingMode</span></span>|<span data-ttu-id="9a913-142">文字列</span><span class="sxs-lookup"><span data-stu-id="9a913-142">string</span></span>|<span data-ttu-id="9a913-p107">省略可能。指定したディメンションに合わせてグラフを拡大または縮小するために使用するメソッド (高さと幅の両方が設定されている場合)。可能な値は、`Fit`、`FitAndCenter`、`Fill` です。</span><span class="sxs-lookup"><span data-stu-id="9a913-p107">Optional. The method used to scale the chart to the specified to the specified dimensions (if both height and width are set)."  Possible values are: `Fit`, `FitAndCenter`, `Fill`.</span></span>|

## <a name="response"></a><span data-ttu-id="9a913-146">応答</span><span class="sxs-lookup"><span data-stu-id="9a913-146">Response</span></span>

<span data-ttu-id="9a913-147">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で base-64 画像 string を返します。</span><span class="sxs-lookup"><span data-stu-id="9a913-147">If successful, this method returns `200 OK` response code and base-64 image string in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a913-148">例</span><span class="sxs-lookup"><span data-stu-id="9a913-148">Example</span></span>
<span data-ttu-id="9a913-149">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="9a913-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9a913-150">要求</span><span class="sxs-lookup"><span data-stu-id="9a913-150">Request</span></span>
<span data-ttu-id="9a913-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9a913-151">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/Image(width=0,height=0,fittingMode='fit')
```

##### <a name="response"></a><span data-ttu-id="9a913-152">応答</span><span class="sxs-lookup"><span data-stu-id="9a913-152">Response</span></span>
<span data-ttu-id="9a913-153">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="9a913-153">Here is an example of the response.</span></span> <span data-ttu-id="9a913-154">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="9a913-154">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9a913-155">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="9a913-155">All of the properties will be returned from an actual call.</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 3

{
"value" : "base-64 chart image string"
}
```

##### <a name="usage"></a><span data-ttu-id="9a913-156">使用方法</span><span class="sxs-lookup"><span data-stu-id="9a913-156">Usage</span></span>

<span data-ttu-id="9a913-157">HTML イメージ タグ: `<img src="data:image/png;base64,{base-64 chart image string}/>` 内の Base-64 文字列を表示できます。</span><span class="sxs-lookup"><span data-stu-id="9a913-157">You can display the base-64 string inside an HTML image tag: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span></span>

<span data-ttu-id="9a913-158">既定の動作には、`Image(width=0,height=0,fittingMode='fit')` を使用します。</span><span class="sxs-lookup"><span data-stu-id="9a913-158">For default behavior, use `Image(width=0,height=0,fittingMode='fit')`.</span></span> <span data-ttu-id="9a913-159">既定のパラメーターで返されるグラフ イメージの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9a913-159">Here is an example of a chart image returned with the default parameters.</span></span>

![既定値の高さと幅の Excel グラフのイメージです。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

<span data-ttu-id="9a913-161">イメージの表示をカスタマイズする場合は、高さ、幅、自動調整モードを指定します。</span><span class="sxs-lookup"><span data-stu-id="9a913-161">If you want to customize the display of the image, specify a height, width, and a fitting mode.</span></span> <span data-ttu-id="9a913-162">これらのパラメーターを使用してグラフ イメージを取得する場合、どのように表示されるかを次に示します。`Image(width=500,height=500,fittingMode='Fill')`。</span><span class="sxs-lookup"><span data-stu-id="9a913-162">Here is what the same chart image looks like if you retrieve it with these parameters: `Image(width=500,height=500,fittingMode='Fill')`.</span></span>

![既定値の高さと幅の Excel グラフのイメージです。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-fill.png)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart: Image",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
