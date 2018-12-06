---
title: Microsoft Graph を使用して Excel のグラフ イメージを表示する
description: グラフ イメージを取得する GET 操作を実行すると、Excel API は Base-64 文字列としてイメージを返します。
ms.openlocfilehash: ae721547fca9a6fe835843544bf550c5fe222426
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092523"
---
# <a name="display-a-chart-image-in-excel-with-microsoft-graph"></a><span data-ttu-id="0aa48-103">Microsoft Graph を使用して Excel のグラフ イメージを表示する</span><span class="sxs-lookup"><span data-stu-id="0aa48-103">Display a chart image in Excel with Microsoft Graph</span></span>

<span data-ttu-id="0aa48-104">[グラフ イメージを取得する GET 操作](/api-reference/v1.0/api/chart-image.md)を実行すると、Excel API は Base-64 文字列としてイメージを返します。</span><span class="sxs-lookup"><span data-stu-id="0aa48-104">When you perform a [GET operation to retrieve a chart image](/api-reference/v1.0/api/chart-image.md), the Excel API returns the image as a base-64 string.</span></span>

<span data-ttu-id="0aa48-105">HTML イメージ タグ: `<img src="data:image/png;base64,{base-64 chart image string}/>` 内の Base-64 文字列を表示できます。</span><span class="sxs-lookup"><span data-stu-id="0aa48-105">You can display the base-64 string inside an HTML image tag: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span></span>

<span data-ttu-id="0aa48-106">既定の動作には、`Image(width=0,height=0,fittingMode='fit')` を使用します。</span><span class="sxs-lookup"><span data-stu-id="0aa48-106">For default behavior, use `Image(width=0,height=0,fittingMode='fit')`.</span></span> <span data-ttu-id="0aa48-107">既定のパラメーターで返されるグラフ イメージの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0aa48-107">Here is an example of a chart image returned with the default parameters.</span></span>

![既定値の高さと幅の Excel グラフのイメージです。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

<span data-ttu-id="0aa48-109">イメージの表示をカスタマイズする場合は、高さ、幅、自動調整モードを指定します。</span><span class="sxs-lookup"><span data-stu-id="0aa48-109">If you want to customize the display of the image, specify a height, width, and a fitting mode.</span></span> <span data-ttu-id="0aa48-110">これらのパラメーターを使用してグラフ イメージを取得する場合、どのように表示されるかを次に示します。`Image(width=500,height=500,fittingMode='Fill')`。</span><span class="sxs-lookup"><span data-stu-id="0aa48-110">Here is what the same chart image looks like if you retrieve it with these parameters: `Image(width=500,height=500,fittingMode='Fill')`.</span></span>

## <a name="see-also"></a><span data-ttu-id="0aa48-111">関連項目</span><span class="sxs-lookup"><span data-stu-id="0aa48-111">See also</span></span>

* [<span data-ttu-id="0aa48-112">Microsoft Graph で Excel のセッションを管理する</span><span class="sxs-lookup"><span data-stu-id="0aa48-112">Manage sessions in Excel with Microsoft Graph</span></span>](excel-manage-sessions.md)
* [<span data-ttu-id="0aa48-113">Microsoft Graph を使用して Excel ブックに書き込む</span><span class="sxs-lookup"><span data-stu-id="0aa48-113">Write to an Excel workbook using Microsoft Graph</span></span>](excel-write-to-workbook.md)
* [<span data-ttu-id="0aa48-114">Microsoft Graph で Excel のブック関数を使用する</span><span class="sxs-lookup"><span data-stu-id="0aa48-114">Use workbook functions in Excel with Microsoft Graph</span></span>](excel-use-functions.md)
* [<span data-ttu-id="0aa48-115">Microsoft Graph により Excel のある範囲の書式を更新する</span><span class="sxs-lookup"><span data-stu-id="0aa48-115">Update a range’s format in Excel with Microsoft Graph</span></span>](excel-update-range-format.md)
* [<span data-ttu-id="0aa48-116">Excel REST API を使用する</span><span class="sxs-lookup"><span data-stu-id="0aa48-116">Use the Excel REST API</span></span>](/graph/api/resources/excel?view=graph-rest-1.0)
