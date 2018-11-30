---
title: bookingCustomer リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
ms.openlocfilehash: 1eef44dfe994238d654a21c5f26ec102dcf1881d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067530"
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
|[削除](../api/bookingcustomer-delete.md) | なし |**BookingCustomer**オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|displayName|String|顧客の名前。|
|emailAddress|String|お客様の SMTP アドレスです。|
|id|String| 顧客の ID です。 読み取り専用。|

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