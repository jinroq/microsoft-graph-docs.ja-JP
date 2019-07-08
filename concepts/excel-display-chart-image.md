---
title: Microsoft Graph を使用して Excel のグラフ イメージを表示する
description: グラフ イメージを取得する GET 操作を実行すると、Excel API は Base-64 文字列としてイメージを返します。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 5cdf5522ccd0a72798ee62211e9221cf2ea9cd53
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526294"
---
# <a name="display-a-chart-image-in-excel-with-microsoft-graph"></a>Microsoft Graph を使用して Excel のグラフ イメージを表示する

[グラフ イメージを取得する GET 操作](/api-reference/v1.0/api/chart-image.md)を実行すると、Excel API は Base-64 文字列としてイメージを返します。

HTML イメージ タグ: `<img src="data:image/png;base64,{base-64 chart image string}/>` 内の Base-64 文字列を表示できます。

既定の動作には、`Image(width=0,height=0,fittingMode='fit')` を使用します。 既定のパラメーターで返されるグラフ イメージの例を次に示します。

![既定値の高さと幅の Excel グラフのイメージです。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

イメージの表示をカスタマイズする場合は、高さ、幅、自動調整モードを指定します。 これらのパラメーターを使用してグラフ イメージを取得する場合、どのように表示されるかを次に示します。`Image(width=500,height=500,fittingMode='Fill')`。

## <a name="see-also"></a>関連項目

* [Microsoft Graph で Excel のセッションを管理する](excel-manage-sessions.md)
* [Microsoft Graph を使用して Excel ブックに書き込む](excel-write-to-workbook.md)
* [Microsoft Graph で Excel のブック関数を使用する](excel-use-functions.md)
* [Microsoft Graph により Excel のある範囲の書式を更新する](excel-update-range-format.md)
* [Excel REST API を使用する](/graph/api/resources/excel?view=graph-rest-1.0)
