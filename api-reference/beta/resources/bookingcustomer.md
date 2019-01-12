---
title: bookingCustomer リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: b213e4026ee33886c0e56db9790efff09fd8c522
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925106"
---
# <a name="bookingcustomer-resource-type"></a>bookingCustomer リソースの種類

 > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。
 
の[bookingBsiness](bookingbusiness.md)の顧客を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[顧客のリスト](../api/bookingbusiness-list-customers.md) | [bookingCustomer](bookingcustomer.md)コレクション | **BookingCustomer**オブジェクトのリストを取得します。 |
|[BookingCustomer を作成します。](../api/bookingbusiness-post-customers.md) | [bookingCustomer](bookingcustomer.md) | 新しい**bookingCustomer**オブジェクトを作成します。 |
|[BookingCustomer を取得します。](../api/bookingcustomer-get.md) | [bookingCustomer](bookingcustomer.md) |プロパティと、 **bookingCustomer**オブジェクトの関係を参照してください。|
|[Update](../api/bookingcustomer-update.md) | [bookingCustomer](bookingcustomer.md) |**BookingCustomer**オブジェクトを更新します。 |
|[Delete](../api/bookingcustomer-delete.md) | なし |**BookingCustomer**オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|displayName|String|顧客の名前。|
|emailAddress|String|お客様の SMTP アドレスです。|
|id|String| 顧客の ID です。 読み取り専用です。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingCustomer"
}-->

```json
{
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingCustomer resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
