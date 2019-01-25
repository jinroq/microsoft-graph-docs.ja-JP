---
title: bookingCustomer リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: cd4991b28f1dee0ba647a7f95b70817beffbef95
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522218"
---
# <a name="bookingcustomer-resource-type"></a>bookingCustomer リソースの種類

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
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
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|displayName|文字列型 (String)|顧客の名前。|
|emailAddress|String|お客様の SMTP アドレスです。|
|id|文字列| 顧客の ID です。 読み取り専用です。|

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
<!--
{
  "type": "#page.annotation",
  "description": "bookingCustomer resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingcustomer.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
