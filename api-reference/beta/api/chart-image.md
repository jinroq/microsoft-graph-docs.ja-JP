---
title: グラフ:画像
description: 指定したサイズに合わせてグラフを拡大、縮小することで、グラフを Base64 でエンコードされた画像としてレンダリングします。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5892864d8adb94c4c6193dc4776f8febd938ff36
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456536"
---
# <a name="chart-image"></a>グラフ:画像

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定したサイズに合わせてグラフを拡大、縮小することで、グラフを Base64 でエンコードされた画像としてレンダリングします。
## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Files.ReadWrite    |
|委任 (個人用 Microsoft アカウント) | Files.ReadWrite    |
|アプリケーション | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts(<name>)/Image(width=0,height=0,fittingMode='fit')

```
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 説明|
|:---------------|:----------|
| Authorization  | ベアラー {トークン}。必須。 |
| Workbook-Session-Id  | 変更を保持するかどうかを決定するブック セッション ID。省略可能。|

## <a name="request-body"></a>要求本文
要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。

| パラメーター    | 型   |説明|
|:---------------|:--------|:----------|
|height|number|省略可能。結果の画像の希望する高さ。|
|width|number|省略可能。結果の画像の希望する幅。|
|fittingMode|string|省略可能。指定したディメンションに合わせてグラフを拡大または縮小するために使用するメソッド (高さと幅の両方が設定されている場合)。可能な値は、`Fit`、`FitAndCenter`、`Fill` です。|

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で base-64 画像 string を返します。

## <a name="example"></a>例
以下は、この API を呼び出す方法の例です。
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/Image(width=0,height=0,fittingMode='fit')
```

##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 3

{
"value" : "base-64 chart image string"
}
```

##### <a name="usage"></a>使用方法

HTML イメージ タグ: `<img src="data:image/png;base64,{base-64 chart image string}/>` 内の Base-64 文字列を表示できます。

既定の動作には、`Image(width=0,height=0,fittingMode='fit')` を使用します。 既定のパラメーターで返されるグラフ イメージの例を次に示します。

![既定値の高さと幅の Excel グラフのイメージです。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

イメージの表示をカスタマイズする場合は、高さ、幅、自動調整モードを指定します。 これらのパラメーターを使用してグラフ イメージを取得する場合、どのように表示されるかを次に示します。`Image(width=500,height=500,fittingMode='Fill')`。

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
  "suppressions": [
    "Error: /api-reference/beta/api/chart-image.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
