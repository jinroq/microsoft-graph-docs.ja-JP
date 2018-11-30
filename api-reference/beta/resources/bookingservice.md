---
title: bookingService リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
ms.openlocfilehash: bb42768cb913abca7c17e6d617670a3a035ec16a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067822"
---
# <a name="bookingservice-resource-type"></a>bookingService リソースの種類

 > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。
 
[BookingBusiness](bookingbusiness.md)サービス名、価格、通常このようなサービスを提供するスタッフなどによって提供される特定のサービスに関する情報を表します。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[サービスの一覧](../api/bookingbusiness-list-services.md) | [bookingService](bookingservice.md)コレクション | 指定された[bookingbusiness](../resources/bookingbusiness.md)では、 **bookingService**オブジェクトのリストを取得します。|
|[BookingService を作成します。](../api/bookingbusiness-post-services.md) | [bookingService](bookingservice.md) | 指定した[bookingbusiness](../resources/bookingbusiness.md)用の**bookingService**を作成します。 |
|[BookingService を取得します。](../api/bookingservice-get.md) | [bookingService](bookingservice.md) |指定された[bookingbusiness](../resources/bookingbusiness.md)のプロパティと、 **bookingService**オブジェクトの関係を取得します。|
|[Update](../api/bookingservice-update.md) | [bookingService](bookingservice.md)    |指定された[bookingbusiness](../resources/bookingbusiness.md)で、 **bookingService**オブジェクトを更新します。 |
|[削除](../api/bookingservice-delete.md) | なし |指定された[bookingbusiness](../resources/bookingbusiness.md)で、 **bookingService**オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|defaultDuration|Duration|日、時間、分、秒単位の数値で表される、サービスの既定の長さです。 たとえば、P11D23H59M59.999999999999S です。 |
|defaultLocation|[location](location.md)|サービスの既定の物理的な場所です。|
|defaultPrice|倍精度浮動小数点数|サービスの既定通貨の価格です。|
|defaultPriceType|文字列|サービスの既定の方法に請求されます。 可能な値は、`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet` です。|
|defaultReminders|[bookingReminder](bookingreminder.md)コレクション|このサービスの予定に対するアラームの既定値を設定します。 その ID ではこの**bookingService**を読み取るときにのみ、このプロパティの値があります。|
|説明|String|サービスの説明です。|
|displayName|String|サービスの名前です。|
|emailAddress|String|電子メール アドレス|
|id|String|GUID 形式で、そのサービスの ID です。 読み取り専用。|
|isHiddenFromCustomers|ブール値|True は、このサービスは予約のお客様に利用できないことを意味します。|
|notes|String|このサービスに関する追加情報。|
|事後バッファリング|Duration|このサービスの予定の後のバッファーに時間が終了して、次の前に顧客の予定が予約できます。|
|事前バッファリング|Duration|このサービスに対する予定を開始する前に、バッファーに格納する時間です。|
|schedulingPolicy|[bookingSchedulingPolicy](bookingschedulingpolicy.md)|この種類のサービスの予定を作成および管理する方法を決定するポリシーのセットです。|
|staffMemberIds|String コレクション|このサービスを提供している[スタッフのメンバー](bookingstaffmember.md)を表します。 |

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingService"
}-->

```json
{
  "defaultDuration": "String (timestamp)",
  "defaultLocation": {"@odata.type": "microsoft.graph.location"},
  "defaultPrice": 1024,
  "defaultPriceType": "string",
  "defaultReminders": [{"@odata.type": "microsoft.graph.bookingReminder"}],
  "description": "String",
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)",
  "isHiddenFromCustomers": true,
  "notes": "String",
  "postBuffer": "String (timestamp)",
  "preBuffer": "String (timestamp)",
  "schedulingPolicy": {"@odata.type": "microsoft.graph.bookingSchedulingPolicy"},
  "staffMemberIds": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingService resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->