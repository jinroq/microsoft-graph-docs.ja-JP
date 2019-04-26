---
title: bookingcurrency リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 6ab74cff24e1f575166f6672523ecc5d94bc1826
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328236"
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
|id|String| [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html)に基づく3文字の通貨コード。 たとえば、米国ドルの通貨コードは USD で、オーストラリアドルは AUD になります。 読み取り専用です。|
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
  "suppressions": []
}
-->
