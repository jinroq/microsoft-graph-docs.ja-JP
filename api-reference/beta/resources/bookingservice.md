---
title: bookingservice リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 35e439888b39c81451242f01d2aaae89b65ad8ee
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535498"
---
# <a name="bookingservice-resource-type"></a>bookingservice リソースの種類

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
通常はサービスを提供しているサービス名、価格、スタッフなど、 [bookingbusiness](bookingbusiness.md)によって提供される特定のサービスに関する情報を表します。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[サービスを一覧表示する](../api/bookingbusiness-list-services.md) | [bookingservice](bookingservice.md)コレクション | 指定した[bookingservice](../resources/bookingbusiness.md)の**bookingservice**オブジェクトのリストを取得します。|
|[bookingservice の作成](../api/bookingbusiness-post-services.md) | [bookingService](bookingservice.md) | 指定した[bookingservice](../resources/bookingbusiness.md)の**bookingservice**を作成します。 |
|[bookingservice を取得する](../api/bookingservice-get.md) | [bookingService](bookingservice.md) |指定した[bookingservice](../resources/bookingbusiness.md)の**bookingservice**オブジェクトのプロパティとリレーションシップを取得します。|
|[更新](../api/bookingservice-update.md) | [bookingService](bookingservice.md)    |指定した[bookingservice](../resources/bookingbusiness.md)の**bookingservice**オブジェクトを更新します。 |
|[削除](../api/bookingservice-delete.md) | なし |指定した[bookingservice](../resources/bookingbusiness.md)の**bookingservice**オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|defaultduration|期間|サービスの既定の長さ。日数、時間、分、および秒で表されます。 たとえば、p11d23h59m 59.999999999999 s のようになります。 |
|defaultLocation|[location](location.md)|サービスの既定の物理的な場所。|
|既定の価格|倍精度浮動小数点数|サービスの既定の通貨料金。|
|defaultPriceType|string|サービスの既定の課金方法。 可能な値は、`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet` です。|
|defaultreminders|[bookingreminder](bookingreminder.md)コレクション|このサービスの予定に対する既定のアラームのセット。 このプロパティの値は、この**bookingservice**を ID で読み取る場合にのみ使用できます。|
|description|String|サービスのテキストの説明。|
|displayName|String|サービス名。|
|emailAddress|String|電子メールアドレス|
|id|String|GUID 形式の、そのサービスの ID。 読み取り専用。|
|isHiddenFromCustomers|ブール値|True は、このサービスを予約にお客様が利用できないことを意味します。|
|notes|String|このサービスに関する追加情報。|
|postbuffer|期間|このサービスの予定が終了してから、次の顧客の予定が予約されるまでの時間。|
|prebuffer|期間|このサービスの予定を開始できるようになるまでの時間。|
|schedulingPolicy|[bookingSchedulingPolicy](bookingschedulingpolicy.md)|この種類のサービスの予定を作成および管理する方法を決定する一連のポリシー。|
|staffMemberIds|String collection|このサービスを提供する[スタッフメンバー](bookingstaffmember.md)を表します。 |

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
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingservice.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
