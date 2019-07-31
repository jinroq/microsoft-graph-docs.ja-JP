---
title: グラフ:画像
description: 指定したサイズに合わせてグラフを拡大、縮小することで、グラフを Base64 でエンコードされた画像としてレンダリングします。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: b75b7700d3b4a862e04a086000831f6fd4b50489
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35944150"
---
# <a name="chart-image"></a><span data-ttu-id="4b102-103">グラフ:画像</span><span class="sxs-lookup"><span data-stu-id="4b102-103">Chart: Image</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b102-104">指定したサイズに合わせてグラフを拡大、縮小することで、グラフを Base64 でエンコードされた画像としてレンダリングします。</span><span class="sxs-lookup"><span data-stu-id="4b102-104">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>
## <a name="permissions"></a><span data-ttu-id="4b102-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4b102-105">Permissions</span></span>
<span data-ttu-id="4b102-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4b102-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b102-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4b102-108">Permission type</span></span>      | <span data-ttu-id="4b102-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4b102-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b102-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4b102-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4b102-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b102-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4b102-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4b102-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b102-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b102-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4b102-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4b102-114">Application</span></span> | <span data-ttu-id="4b102-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4b102-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b102-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4b102-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/Image(width=0,height=0,fittingMode='fit')

```
## <a name="request-headers"></a><span data-ttu-id="4b102-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4b102-117">Request headers</span></span>
| <span data-ttu-id="4b102-118">名前</span><span class="sxs-lookup"><span data-stu-id="4b102-118">Name</span></span>       | <span data-ttu-id="4b102-119">説明</span><span class="sxs-lookup"><span data-stu-id="4b102-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4b102-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b102-120">Authorization</span></span>  | <span data-ttu-id="4b102-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4b102-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4b102-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4b102-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="4b102-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="4b102-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b102-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4b102-126">Request body</span></span>
<span data-ttu-id="4b102-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="4b102-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4b102-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="4b102-128">Parameter</span></span>    | <span data-ttu-id="4b102-129">型</span><span class="sxs-lookup"><span data-stu-id="4b102-129">Type</span></span>   |<span data-ttu-id="4b102-130">説明</span><span class="sxs-lookup"><span data-stu-id="4b102-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b102-131">height</span><span class="sxs-lookup"><span data-stu-id="4b102-131">height</span></span>|<span data-ttu-id="4b102-132">番号</span><span class="sxs-lookup"><span data-stu-id="4b102-132">number</span></span>|<span data-ttu-id="4b102-p104">省略可能。結果の画像の希望する高さ。</span><span class="sxs-lookup"><span data-stu-id="4b102-p104">Optional. The desired height of the resulting image.</span></span>|
|<span data-ttu-id="4b102-135">width</span><span class="sxs-lookup"><span data-stu-id="4b102-135">width</span></span>|<span data-ttu-id="4b102-136">number</span><span class="sxs-lookup"><span data-stu-id="4b102-136">number</span></span>|<span data-ttu-id="4b102-p105">省略可能。結果の画像の希望する幅。</span><span class="sxs-lookup"><span data-stu-id="4b102-p105">Optional. The desired width of the resulting image.</span></span>|
|<span data-ttu-id="4b102-139">fittingMode</span><span class="sxs-lookup"><span data-stu-id="4b102-139">fittingMode</span></span>|<span data-ttu-id="4b102-140">string</span><span class="sxs-lookup"><span data-stu-id="4b102-140">string</span></span>|<span data-ttu-id="4b102-p106">省略可能。指定したディメンションに合わせてグラフを拡大または縮小するために使用するメソッド (高さと幅の両方が設定されている場合)。可能な値は、`Fit`、`FitAndCenter`、`Fill` です。</span><span class="sxs-lookup"><span data-stu-id="4b102-p106">Optional. The method used to scale the chart to the specified to the specified dimensions (if both height and width are set)."  Possible values are: `Fit`, `FitAndCenter`, `Fill`.</span></span>|

## <a name="response"></a><span data-ttu-id="4b102-144">応答</span><span class="sxs-lookup"><span data-stu-id="4b102-144">Response</span></span>

<span data-ttu-id="4b102-145">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で base-64 画像 string を返します。</span><span class="sxs-lookup"><span data-stu-id="4b102-145">If successful, this method returns `200 OK` response code and base-64 image string in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b102-146">例</span><span class="sxs-lookup"><span data-stu-id="4b102-146">Example</span></span>
<span data-ttu-id="4b102-147">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="4b102-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4b102-148">要求</span><span class="sxs-lookup"><span data-stu-id="4b102-148">Request</span></span>
<span data-ttu-id="4b102-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4b102-149">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/Image(width=0,height=0,fittingMode='fit')
```

##### <a name="response"></a><span data-ttu-id="4b102-150">応答</span><span class="sxs-lookup"><span data-stu-id="4b102-150">Response</span></span>
<span data-ttu-id="4b102-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4b102-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call. </span></span><!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 3

{
"value" : "base-64 chart image string"
}
```

##### <a name="usage"></a><span data-ttu-id="4b102-154">使用方法</span><span class="sxs-lookup"><span data-stu-id="4b102-154">Usage</span></span>

<span data-ttu-id="4b102-155">HTML イメージ タグ: `<img src="data:image/png;base64,{base-64 chart image string}/>` 内の Base-64 文字列を表示できます。</span><span class="sxs-lookup"><span data-stu-id="4b102-155">You can display the base-64 string inside an HTML image tag: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span></span>

<span data-ttu-id="4b102-156">既定の動作には、`Image(width=0,height=0,fittingMode='fit')` を使用します。</span><span class="sxs-lookup"><span data-stu-id="4b102-156">For default behavior, use `Image(width=0,height=0,fittingMode='fit')`.</span></span> <span data-ttu-id="4b102-157">既定のパラメーターで返されるグラフ イメージの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4b102-157">Here is an example of a chart image returned with the default parameters.</span></span>

![既定値の高さと幅の Excel グラフのイメージです。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

<span data-ttu-id="4b102-159">イメージの表示をカスタマイズする場合は、高さ、幅、自動調整モードを指定します。</span><span class="sxs-lookup"><span data-stu-id="4b102-159">If you want to customize the display of the image, specify a height, width, and a fitting mode.</span></span> <span data-ttu-id="4b102-160">これらのパラメーターを使用してグラフ イメージを取得する場合、どのように表示されるかを次に示します。`Image(width=500,height=500,fittingMode='Fill')`。</span><span class="sxs-lookup"><span data-stu-id="4b102-160">Here is what the same chart image looks like if you retrieve it with these parameters: `Image(width=500,height=500,fittingMode='Fill')`.</span></span>

![既定値の高さと幅の Excel グラフのイメージです。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-fill.png)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Chart: Image",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
