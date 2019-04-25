---
title: グラフ:画像
description: 指定したサイズに合わせてグラフを拡大、縮小することで、グラフを Base64 でエンコードされた画像としてレンダリングします。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 0f61866885f0798b9e96f80e22a636fb5f619e34
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581686"
---
# <a name="chart-image"></a><span data-ttu-id="0b7b8-103">グラフ:画像</span><span class="sxs-lookup"><span data-stu-id="0b7b8-103">Chart: Image</span></span>

<span data-ttu-id="0b7b8-104">指定したサイズに合わせてグラフを拡大、縮小することで、グラフを Base64 でエンコードされた画像としてレンダリングします。</span><span class="sxs-lookup"><span data-stu-id="0b7b8-104">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>
## <a name="permissions"></a><span data-ttu-id="0b7b8-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0b7b8-105">Permissions</span></span>
<span data-ttu-id="0b7b8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0b7b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b7b8-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0b7b8-108">Permission type</span></span>      | <span data-ttu-id="0b7b8-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0b7b8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b7b8-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0b7b8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0b7b8-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b7b8-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0b7b8-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0b7b8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b7b8-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0b7b8-113">Not supported.</span></span>    |
|<span data-ttu-id="0b7b8-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0b7b8-114">Application</span></span> | <span data-ttu-id="0b7b8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0b7b8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b7b8-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0b7b8-116">HTTP request</span></span>
<!-- { "blockType": "samples" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/image
GET /workbook/worksheets/{id|name}/charts/{name}/image(width=640)
GET /workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480)
GET /workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480,fittingMode='fit')
```
## <a name="request-headers"></a><span data-ttu-id="0b7b8-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0b7b8-117">Request headers</span></span>
| <span data-ttu-id="0b7b8-118">名前</span><span class="sxs-lookup"><span data-stu-id="0b7b8-118">Name</span></span>       | <span data-ttu-id="0b7b8-119">説明</span><span class="sxs-lookup"><span data-stu-id="0b7b8-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0b7b8-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b7b8-120">Authorization</span></span>  | <span data-ttu-id="0b7b8-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0b7b8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0b7b8-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0b7b8-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="0b7b8-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="0b7b8-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="0b7b8-126">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="0b7b8-126">Path parameters</span></span>
<span data-ttu-id="0b7b8-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="0b7b8-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0b7b8-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="0b7b8-128">Parameter</span></span>    | <span data-ttu-id="0b7b8-129">型</span><span class="sxs-lookup"><span data-stu-id="0b7b8-129">Type</span></span>   |<span data-ttu-id="0b7b8-130">説明</span><span class="sxs-lookup"><span data-stu-id="0b7b8-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b7b8-131">height</span><span class="sxs-lookup"><span data-stu-id="0b7b8-131">height</span></span>|<span data-ttu-id="0b7b8-132">Int32</span><span class="sxs-lookup"><span data-stu-id="0b7b8-132">Int32</span></span>|<span data-ttu-id="0b7b8-133">結果の画像の希望する高さ。</span><span class="sxs-lookup"><span data-stu-id="0b7b8-133">The desired height of the resulting image.</span></span> <span data-ttu-id="0b7b8-134">省略可能。</span><span class="sxs-lookup"><span data-stu-id="0b7b8-134">Optional.</span></span>|
|<span data-ttu-id="0b7b8-135">width</span><span class="sxs-lookup"><span data-stu-id="0b7b8-135">width</span></span>|<span data-ttu-id="0b7b8-136">Int32</span><span class="sxs-lookup"><span data-stu-id="0b7b8-136">Int32</span></span>|<span data-ttu-id="0b7b8-137">結果の画像の希望する幅。</span><span class="sxs-lookup"><span data-stu-id="0b7b8-137">The desired width of the resulting image.</span></span> <span data-ttu-id="0b7b8-138">省略可能。</span><span class="sxs-lookup"><span data-stu-id="0b7b8-138">Optional.</span></span>|
|<span data-ttu-id="0b7b8-139">fittingMode</span><span class="sxs-lookup"><span data-stu-id="0b7b8-139">fittingMode</span></span>|<span data-ttu-id="0b7b8-140">string</span><span class="sxs-lookup"><span data-stu-id="0b7b8-140">string</span></span>|<span data-ttu-id="0b7b8-141">指定した寸法 (高さと幅の両方が設定されている場合) にグラフを拡大または縮小するために使用されるメソッドです。</span><span class="sxs-lookup"><span data-stu-id="0b7b8-141">The method used to scale the chart to the specified dimensions (if both height and width are set)."</span></span>  <span data-ttu-id="0b7b8-142">使用可能な値: `Fit`、`FitAndCenter`、`Fill`。</span><span class="sxs-lookup"><span data-stu-id="0b7b8-142">The possible values are: `Fit`, `FitAndCenter`, `Fill`.</span></span>|

## <a name="response"></a><span data-ttu-id="0b7b8-143">応答</span><span class="sxs-lookup"><span data-stu-id="0b7b8-143">Response</span></span>

<span data-ttu-id="0b7b8-144">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で base-64 画像 string を返します。</span><span class="sxs-lookup"><span data-stu-id="0b7b8-144">If successful, this method returns `200 OK` response code and base-64 image string in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b7b8-145">例</span><span class="sxs-lookup"><span data-stu-id="0b7b8-145">Example</span></span>
<span data-ttu-id="0b7b8-146">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="0b7b8-146">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="0b7b8-147">要求</span><span class="sxs-lookup"><span data-stu-id="0b7b8-147">Request</span></span>
<span data-ttu-id="0b7b8-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0b7b8-148">Here is an example of the request.</span></span>

<!-- { "blockType": "request" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480,fittingMode='fit')
```

##### <a name="response"></a><span data-ttu-id="0b7b8-149">応答</span><span class="sxs-lookup"><span data-stu-id="0b7b8-149">Response</span></span>
<span data-ttu-id="0b7b8-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0b7b8-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call. </span></span><!-- { "blockType": "response", "@odata.type": "Edm.String" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json;odata.metadata=minimal;odata.streaming=true

{
"value" : "base-64 chart image string"
}
```

## <a name="usage"></a><span data-ttu-id="0b7b8-153">使用方法</span><span class="sxs-lookup"><span data-stu-id="0b7b8-153">Usage</span></span>

<span data-ttu-id="0b7b8-154">HTML イメージ タグ: `<img src="data:image/png;base64,{base-64 chart image string}/>` 内の Base-64 文字列を表示できます。</span><span class="sxs-lookup"><span data-stu-id="0b7b8-154">You can display the base-64 string inside an HTML image tag: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span></span>

<span data-ttu-id="0b7b8-155">既定の動作には、`Image(width=0,height=0,fittingMode='fit')` を使用します。</span><span class="sxs-lookup"><span data-stu-id="0b7b8-155">For default behavior, use `Image(width=0,height=0,fittingMode='fit')`.</span></span> <span data-ttu-id="0b7b8-156">既定のパラメーターで返されるグラフ イメージの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0b7b8-156">Here is an example of a chart image returned with the default parameters.</span></span>

![既定値の高さと幅の Excel グラフのイメージです。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

<span data-ttu-id="0b7b8-158">イメージの表示をカスタマイズする場合は、高さ、幅、自動調整モードを指定します。</span><span class="sxs-lookup"><span data-stu-id="0b7b8-158">If you want to customize the display of the image, specify a height, width, and a fitting mode.</span></span> <span data-ttu-id="0b7b8-159">これらのパラメーターを使用してグラフ イメージを取得する場合、どのように表示されるかを次に示します。`Image(width=500,height=500,fittingMode='Fill')`。</span><span class="sxs-lookup"><span data-stu-id="0b7b8-159">Here is what the same chart image looks like if you retrieve it with these parameters: `Image(width=500,height=500,fittingMode='Fill')`.</span></span>

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
