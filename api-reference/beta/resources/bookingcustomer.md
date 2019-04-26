---
title: bookingcustomer リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: f97f3d36599fe088f28176d001fecc701bb5e3ab
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339072"
---
# <a name="bookingcustomer-resource-type"></a>bookingcustomer リソースの種類

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
[bookingBsiness](bookingbusiness.md)のお客様を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[顧客を一覧表示する](../api/bookingbusiness-list-customers.md) | [bookingcustomer](bookingcustomer.md)コレクション | **bookingcustomer**オブジェクトのリストを取得します。 |
|[bookingcustomer の作成](../api/bookingbusiness-post-customers.md) | [bookingcustomer](bookingcustomer.md) | 新しい**bookcustomer**オブジェクトを作成します。 |
|[bookingcustomer を取得する](../api/bookingcustomer-get.md) | [bookingcustomer](bookingcustomer.md) |**bookingcustomer**オブジェクトのプロパティとリレーションシップを読み取ります。|
|[更新する](../api/bookingcustomer-update.md) | [bookingcustomer](bookingcustomer.md) |**bookingcustomer**オブジェクトを更新します。 |
|[削除](../api/bookingcustomer-delete.md) | なし |**bookingcustomer**オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|displayName|String|顧客の名前。|
|emailAddress|String|顧客の SMTP アドレス。|
|id|String| 顧客の ID。 読み取り専用です。|

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
