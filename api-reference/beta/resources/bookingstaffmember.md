---
title: bookingStaffMember リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 0d7461137c1a67d163d750b05fa056a17071561f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328296"
---
# <a name="bookingstaffmember-resource-type"></a>bookingStaffMember リソースの種類

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
[bookingbusiness](bookingbusiness.md)でサービスを提供するスタッフメンバーを表します。

スタッフメンバーは、予約ビジネスが構成されている Office 355 テナントの一部として、または他の電子メールプロバイダーの電子メールサービスを使用することができます。

予約時に予約 API は、次の設定を考慮してスタッフメンバーの可用性を判断します。 

1. 既定では、ビジネスの運用時間 ( [bookingbusiness](bookingbusiness.md)エンティティの**microsoft.rtc.rgs.management.writablesettings.businesshours**プロパティ) は、スタッフメンバーの一般利用可能性を表します。
2. **useBusinessHours**が false の場合、スタッフメンバーの特定の勤務時間 ( **bookingStaffmember**エンティティの**workingHours**プロパティ) は、そのメンバーの一般的な利用可能時間を表します。
3. **availabilityIsAffectedByPersonalCalendar**が true の場合、予約 API は最初にスタッフメンバーの使用可能な時間 (#1 または #2 のどちらかによって決まります) を調べて、スタッフメンバーの個人の時間帯に空き時間情報を確認します。予約する前に、予定表を作成します。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[スタッフメンバーを一覧表示する](../api/bookingbusiness-list-staffmembers.md) | [bookingStaffMember](bookingstaffmember.md)コレクション | 指定した[bookingbusiness](../resources/bookingbusiness.md)の**bookingStaffMember**オブジェクトのリストを取得します。 |
|[bookingstaff を作成する](../api/bookingbusiness-post-staffmembers.md) | [bookingStaffMember](bookingstaffmember.md)コレクション | 指定した[bookingbusiness](../resources/bookingbusiness.md)で新しい**bookingStaffMember**を作成します。 |
|[bookingStaffMember を取得する](../api/bookingstaffmember-get.md) | [bookingStaffMember](bookingstaffmember.md) |指定した[bookingbusiness](../resources/bookingbusiness.md)の**bookingStaffMember**のプロパティとリレーションシップを取得します。|
|[Update](../api/bookingstaffmember-update.md) | [bookingStaffMember](bookingstaffmember.md)    |指定した[bookingbusiness](../resources/bookingbusiness.md)の**bookingStaffMember**のプロパティを更新します。|
|[Delete](../api/bookingstaffmember-delete.md) | なし |指定した[bookingbusiness](../resources/bookingbusiness.md)のスタッフメンバーを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|availabilityIsAffectedByPersonalCalendar|Boolean|True は、スタッフメンバーが office 365 ユーザーの場合、予約 API は、予約を行う前に office 365 の個人用予定表でスタッフメンバーの利用可能性を確認します。 |
|colorIndex|Int32|スタッフメンバーを表す色を識別します。 この色は、予約アプリの [**スタッフの詳細**] ページのカラーパレットに対応しています。|
|displayName|String|スタッフメンバーの名前。顧客に表示されます。 必須です。|
|emailAddress|String|スタッフメンバーの電子メールアドレス。 これは、ビジネスと同じ Office 365 テナント内、または別の電子メールドメインに配置できます。 この電子メールアドレスは、ビジネスのスケジューリングポリシーで**sendConfirmationsToOwner**プロパティが true に設定されている場合に使用できます。 必須。|
|id|String| GUID 形式のスタッフメンバーの ID。 読み取り専用。|
|role|string| 業務のスタッフメンバーの役割。 使用可能な値は、`guest`、`administrator`、`viewer`、`externalGuest` です。 必須です。|
|useBusinessHours|Boolean|True は、スタッフメンバーの可用性が、ビジネスの**microsoft.rtc.rgs.management.writablesettings.businesshours**プロパティで指定されていることを意味します。 False は、可用性がスタッフメンバーの**workingHours**プロパティの設定によって決定されることを意味します。|
|workingHours|[bookingwork hours](bookingworkhours.md)コレクション|スタッフメンバーが予約に使用できる各曜日の時間の範囲。 既定では、ビジネスの**microsoft.rtc.rgs.management.writablesettings.businesshours**プロパティと同じになるように初期化されます。|

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
  "suppressions": []
}
-->
