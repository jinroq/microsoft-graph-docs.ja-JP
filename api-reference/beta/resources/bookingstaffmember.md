---
title: bookingStaffMember リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 72130f46dc67d4491f9855706528ee5894b8352f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520278"
---
# <a name="bookingstaffmember-resource-type"></a>bookingStaffMember リソースの種類

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
の[bookingBusiness](bookingbusiness.md)でサービスを提供できるスタッフ メンバーを表します。

スタッフ メンバーは、予約業務を構成すると、またはその他の電子メール プロバイダーからのメール サービスを使用することができます Office 355 テナントの一部にできます。

予定を予約するには、予約の API は、スタッフ メンバーの空き時間を決定するのには次の設定を考慮します。 

1. ( [BookingBusiness](bookingbusiness.md)エンティティの**businessHours**プロパティ) のビジネスの操作の時間は、既定では、スタッフ メンバーの全般的な可用性を表します。
2. **UseBusinessHours**が false の場合は、スタッフ メンバーの特定の作業時間 ( **bookingStaffmember**エンティティのプロパティを**workingHours** ) はそのメンバーの全般的な可用性を表します。
3. **AvailabilityIsAffectedByPersonalCalendar**が true の場合は、予約 API は最初にによって決定される 1 または 2 のいずれか)、スタッフ メンバーの一般に利用可能な時間を見てし、スタッフ メンバーの個人に、その時間帯に可用性を検証します。予定表、予約をする前にします。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[スタッフ メンバーの一覧](../api/bookingbusiness-list-staffmembers.md) | [bookingStaffMember](bookingstaffmember.md)コレクション | 指定された[bookingbusiness](../resources/bookingbusiness.md)では、 **bookingStaffMember**オブジェクトのリストを取得します。 |
|[BookingStaff を作成します。](../api/bookingbusiness-post-staffmembers.md) | [bookingStaffMember](bookingstaffmember.md)コレクション | 指定された[bookingbusiness](../resources/bookingbusiness.md)では、新しい**bookingStaffMember**を作成します。 |
|[BookingStaffMember を取得します。](../api/bookingstaffmember-get.md) | [bookingStaffMember](bookingstaffmember.md) |指定された[bookingbusiness](../resources/bookingbusiness.md)のプロパティと、 **bookingStaffMember**の関係を取得します。|
|[Update](../api/bookingstaffmember-update.md) | [bookingStaffMember](bookingstaffmember.md)    |指定された[bookingbusiness](../resources/bookingbusiness.md)では、 **bookingStaffMember**のプロパティを更新します。|
|[Delete](../api/bookingstaffmember-delete.md) | なし |指定された[bookingbusiness](../resources/bookingbusiness.md)のスタッフ メンバーを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|availabilityIsAffectedByPersonalCalendar|ブール値|True では、あるスタッフ メンバーが、Office 365 ユーザーの場合は、予約 API はスタッフ メンバーの可用性を確認、Office 365 で、個人用の予定表で予約を行う前にことを意味します。 |
|ColorIndex|Int32|スタッフ メンバーを表す色を識別します。 予約アプリケーションでは、**スタッフの詳細**ページでカラー パレットに色が対応しています。|
|displayName|文字列型 (String)|顧客に表示されるよう、スタッフ メンバーの名前です。 必須です。|
|emailAddress|String|スタッフ メンバーの電子メール アドレスです。 ビジネスとして同じ Office 365 テナントにまたは別の電子メール ドメインを指定できます。 **SendConfirmationsToOwner**プロパティが設定されている場合、この e メール アドレスを使用することがビジネスのスケジュー リング ポリシーの場合は true です。 必須です。|
|id|文字列| GUID 形式で、スタッフ メンバーの ID。 読み取り専用です。|
|role|string| ビジネスのスタッフの役割です。 可能な値は、`guest`、`administrator`、`viewer`、`externalGuest` です。 必須です。|
|useBusinessHours|ブール値|真のスタッフ メンバーの可用性とは、ビジネスの**businessHours**プロパティで指定されています。 False は、利用可能時間は、スタッフ メンバーの**workingHours**プロパティの設定によって決定されますを意味します。|
|workingHours|[bookingWorkHours](bookingworkhours.md)コレクション|スタッフ メンバーは、予約に使用される 1 週間の各日の時間の範囲です。 既定では、ビジネスの**businessHours**プロパティと同じにするのに初期化されます。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingStaffMember"
}-->

```json
{
  "availabilityIsAffectedByPersonalCalendar": true,
  "colorIndex": 1024,
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)",
  "role": "string",
  "useBusinessHours": true,
  "workingHours": [{"@odata.type": "microsoft.graph.bookingWorkHours"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingStaffMember resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingstaffmember.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
