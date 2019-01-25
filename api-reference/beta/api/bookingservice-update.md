---
title: Bookingservice を更新します。
description: 指定された bookingbusiness で、bookingService オブジェクトのプロパティを更新します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 6049fe68eaa45597246bef1c1b11952e3c4a5d42
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519718"
---
# <a name="update-bookingservice"></a>Bookingservice を更新します。

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定された[bookingbusiness](../resources/bookingbusiness.md)で、 [bookingService](../resources/bookingservice.md)オブジェクトのプロパティを更新します。

サービスをカスタマイズすることができます例を次に示します。
- Price
- 予定の標準的な長さ
- Reminders
- バッファーを設定する前にまたはサービス終了するたび
- 予約を取り消すには、最低限の通知などのパラメーターの[ポリシーのスケジュールを設定](../resources/bookingschedulingpolicy.md)し、お客様が予定の特定のスタッフのメンバーを選択するかどうか。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) |  Bookings.ReadWrite.All、Bookings.Manage.All   |
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
|defaultDuration|Duration|日、時間、分、秒単位の数値で表される、サービスの既定の長さです。 たとえば、P11D23H59M59.999999999999S です。 |
|defaultLocation|[location](../resources/location.md)|サービスの既定の物理的な場所です。|
|defaultPrice|倍精度浮動小数点数|サービスの既定通貨の価格です。|
|defaultPriceType|string|サービスの既定の方法に請求されます。 可能な値は、`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet` です。|
|defaultReminders|[bookingReminder](../resources/bookingreminder.md)コレクション|このサービスの予定に対するアラームの既定値を設定します。 その ID ではこの**bookingService**を読み取るときにのみ、このプロパティの値があります。|
|説明|文字列|サービスの説明です。|
|displayName|String|サービスの名前です。|
|emailAddress|String|電子メール アドレス:  |
|id|文字列| 読み取り専用です。|
|isHiddenFromCustomers|ブール値|True は、このサービスは予約のお客様に利用できないことを意味します。|
|notes|String|このサービスに関する追加情報。|
|事後バッファリング|Duration|このサービスの予定の後のバッファーに時間が終了して、次の前に顧客の予定が予約できます。|
|事前バッファリング|Duration|このサービスに対する予定を開始する前に、バッファーに格納する時間です。|
|schedulingPolicy|[bookingSchedulingPolicy](../resources/bookingschedulingpolicy.md)|この種類のサービスの予定を作成および管理する方法を決定するポリシーのセットです。|
|staffMemberIds|String コレクション|このサービスを提供している[スタッフのメンバー](../resources/bookingstaffmember.md)を表します。 |

## <a name="response"></a>応答
成功した場合、このメソッドは `204 No content` 応答コードを返します。応答本文には何も返されません。
## <a name="example"></a>例
##### <a name="request"></a>要求
次の例では、指定されたサービスの期間を更新します。
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
