---
title: bookingservice を更新する
description: 指定した bookingservice の bookingservice オブジェクトのプロパティを更新します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 6049fe68eaa45597246bef1c1b11952e3c4a5d42
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461634"
---
# <a name="update-bookingservice"></a>bookingservice を更新する

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定した[bookingservice](../resources/bookingbusiness.md)の[bookingservice](../resources/bookingservice.md)オブジェクトのプロパティを更新します。

以下に、サービスに対してカスタマイズできる例をいくつか示します。
- Price
- 予定の通常の長さ
- Reminders
- サービスの実行前または完了後にセットアップする任意の時間バッファー
- 予約またはキャンセルするための最小限の通知や、ユーザーが予定に対して特定のスタッフメンバーを選択できるかどうかの[スケジュールポリシー](../resources/bookingschedulingpolicy.md)パラメーター。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) |  予約します。すべての予約   |
|委任 (個人用 Microsoft アカウント) | サポートされていません。   |
|アプリケーション | サポートされていません。  |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-request-headers"></a>オプションの要求ヘッダー
| 名前       | 説明|
|:-----------|:-----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>要求本文
要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|defaultduration|期間|サービスの既定の長さ。日数、時間、分、および秒で表されます。 たとえば、p11d23h59m 59.999999999999 s のようになります。 |
|defaultLocation|[location](../resources/location.md)|サービスの既定の物理的な場所。|
|既定の価格|倍精度浮動小数点数|サービスの既定の通貨料金。|
|defaultPriceType|string|サービスの既定の課金方法。 可能な値は、`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet` です。|
|defaultreminders|[bookingreminder](../resources/bookingreminder.md)コレクション|このサービスの予定に対する既定のアラームのセット。 このプロパティの値は、この**bookingservice**を ID で読み取る場合にのみ使用できます。|
|説明|String|サービスのテキストの説明。|
|displayName|String|サービス名。|
|emailAddress|String|電子メールアドレス|
|id|String| 読み取り専用です。|
|isHiddenFromCustomers|Boolean|True は、このサービスを予約にお客様が利用できないことを意味します。|
|notes|String|このサービスに関する追加情報。|
|postbuffer|期間|このサービスの予定が終了してから、次の顧客の予定が予約されるまでの時間。|
|prebuffer|期間|このサービスの予定を開始できるようになるまでの時間。|
|schedulingPolicy|[bookingSchedulingPolicy](../resources/bookingschedulingpolicy.md)|この種類のサービスの予定を作成および管理する方法を決定する一連のポリシー。|
|staffMemberIds|String collection|このサービスを提供する[スタッフメンバー](../resources/bookingstaffmember.md)を表します。 |

## <a name="response"></a>応答
成功した場合、このメソッドは `204 No content` 応答コードを返します。応答本文には何も返されません。
## <a name="example"></a>例
##### <a name="request"></a>要求
次の使用例は、指定されたサービスの期間を更新します。
<!-- {
  "blockType": "request",
  "name": "update_bookingservice"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingService",
    "defaultDuration":"PT30M"
}
```
##### <a name="response"></a>応答
応答の例を次に示します。
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update bookingservice",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingservice-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
