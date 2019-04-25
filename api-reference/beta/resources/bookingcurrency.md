---
title: bookingcurrency リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 9d4feac66e72c756173113101a88bf8bbe35563a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535460"
---
# <a name="bookingcurrency-resource-type"></a>bookingcurrency リソースの種類

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
[bookingbusiness](bookingbusiness.md)でサポートされている通貨通貨を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[bookingcurrencies のリスト](../api/bookingcurrency-list.md) | [bookingcurrency](bookingcurrency.md)コレクション |Microsoft の予約ビジネスで使用できる**bookingcurrency**オブジェクトの一覧を取得します。|
|[bookingcurrency の取得](../api/bookingcurrency-get.md) | [bookingCurrency](bookingcurrency.md) |**bookingcurrency**オブジェクトのプロパティを取得します。|


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|String| [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html)に基づく3文字の通貨コード。 たとえば、米国ドルの通貨コードは USD で、オーストラリアドルは AUD になります。 読み取り専用。|
|疑問符|String| 通貨記号。 たとえば、米ドルおよびオーストラリアドルの通貨記号は $ です。  |

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingCurrency"
}-->

```json
{
  "id": "String (identifier)",
  "symbol": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingCurrency resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingcurrency.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
