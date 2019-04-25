---
title: bookingcustomer リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: cd4991b28f1dee0ba647a7f95b70817beffbef95
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543910"
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
|[更新](../api/bookingcustomer-update.md) | [bookingcustomer](bookingcustomer.md) |**bookingcustomer**オブジェクトを更新します。 |
|[削除](../api/bookingcustomer-delete.md) | なし |**bookingcustomer**オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|displayName|String|顧客の名前。|
|emailAddress|String|顧客の SMTP アドレス。|
|id|String| 顧客の ID。 読み取り専用。|

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
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingcustomer.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
