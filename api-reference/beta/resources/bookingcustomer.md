---
title: bookingCustomer リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 864635014b3e215dabd11896922ca9e73a5e8cb9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974172"
---
# <a name="bookingcustomer-resource-type"></a>bookingCustomer リソースの種類

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
[Bookingbusiness](bookingbusiness.md)のお客様を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[顧客を一覧表示する](../api/bookingbusiness-list-customers.md) | [Bookingcustomer](bookingcustomer.md)コレクション | **Bookingcustomer**オブジェクトのリストを取得します。 |
|[BookingCustomer の作成](../api/bookingbusiness-post-customers.md) | [bookingCustomer](bookingcustomer.md) | 新しい**Bookcustomer**オブジェクトを作成します。 |
|[BookingCustomer を取得する](../api/bookingcustomer-get.md) | [bookingCustomer](bookingcustomer.md) |**Bookingcustomer**オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Update](../api/bookingcustomer-update.md) | [bookingCustomer](bookingcustomer.md) |**Bookingcustomer**オブジェクトを更新します。 |
|[Delete](../api/bookingcustomer-delete.md) | None |**Bookingcustomer**オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|displayName|String|顧客の名前。|
|emailAddress|String|顧客の SMTP アドレス。|
|id|文字列| 顧客の ID。 読み取り専用です。|

## <a name="relationships"></a>関係
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
  "suppressions": []
}
-->
