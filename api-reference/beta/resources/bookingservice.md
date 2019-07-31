---
title: bookingService リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 5f51ec999f0a2048b8dbcbdd533c609eb5a86757
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974130"
---
# <a name="bookingservice-resource-type"></a>bookingService リソースの種類

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
通常はサービスを提供しているサービス名、価格、スタッフなど、 [Bookingbusiness](bookingbusiness.md)によって提供される特定のサービスに関する情報を表します。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[サービスを一覧表示する](../api/bookingbusiness-list-services.md) | [Bookingservice](bookingservice.md)コレクション | 指定した[bookingservice](../resources/bookingbusiness.md)の**bookingservice**オブジェクトのリストを取得します。|
|[BookingService の作成](../api/bookingbusiness-post-services.md) | [bookingService](bookingservice.md) | 指定した[bookingservice](../resources/bookingbusiness.md)の**bookingservice**を作成します。 |
|[BookingService を取得する](../api/bookingservice-get.md) | [bookingService](bookingservice.md) |指定した[bookingservice](../resources/bookingbusiness.md)の**bookingservice**オブジェクトのプロパティとリレーションシップを取得します。|
|[Update](../api/bookingservice-update.md) | [bookingService](bookingservice.md)    |指定した[bookingservice](../resources/bookingbusiness.md)の**bookingservice**オブジェクトを更新します。 |
|[Delete](../api/bookingservice-delete.md) | None |指定した[bookingservice](../resources/bookingbusiness.md)の**bookingservice**オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|defaultDuration|期間|サービスの既定の長さ。日数、時間、分、および秒で表されます。 たとえば、P11D23H59M 59.999999999999 S のようになります。 |
|defaultLocation|[location](location.md)|サービスの既定の物理的な場所。|
|既定の価格|2 行分|サービスの既定の通貨料金。|
|defaultPriceType|string|サービスの既定の課金方法。 可能な値は、`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet` です。|
|defaultReminders|[Bookingreminder](bookingreminder.md)コレクション|このサービスの予定に対する既定のアラームのセット。 このプロパティの値は、この**Bookingservice**を ID で読み取る場合にのみ使用できます。|
|description|String|サービスのテキストの説明。|
|displayName|String|サービス名。|
|emailAddress|String|電子メールアドレス|
|id|文字列|GUID 形式の、そのサービスの ID。 読み取り専用です。|
|isHiddenFromCustomers|Boolean|True は、このサービスを予約にお客様が利用できないことを意味します。|
|notes|String|このサービスに関する追加情報。|
|postBuffer|期間|このサービスの予定が終了してから、次の顧客の予定が予約されるまでの時間。|
|preBuffer|期間|このサービスの予定を開始できるようになるまでの時間。|
|schedulingPolicy|[bookingSchedulingPolicy](bookingschedulingpolicy.md)|この種類のサービスの予定を作成および管理する方法を決定する一連のポリシー。|
|staffMemberIds|文字列コレクション|このサービスを提供する[スタッフメンバー](bookingstaffmember.md)を表します。 |

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
<!--
{
  "type": "#page.annotation",
  "description": "bookingService resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
