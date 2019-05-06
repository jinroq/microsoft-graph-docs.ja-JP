---
title: group リソース タイプ
description: Office 365 グループ、動的なグループ、セキュリティ グループのいずれかの Azure Active Directory (Azure AD) グループを表します。
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: aa18cf9ce8a0dbaf7f50c0b643335a5a992d9049
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324795"
---
# <a name="group-resource-type"></a>group リソースの種類

Office 365 グループ、動的なグループ、セキュリティ グループのいずれかの Azure Active Directory (Azure AD) グループを表します。[directoryObject](directoryobject.md) から継承します。

パフォーマンス上の理由から、[create](../api/group-post-groups.md) 操作、[get](../api/group-get.md) 操作、および [list](../api/group-list.md) 操作は、既定ではより一般的に使用されるプロパティのみを返します。 これらの_既定_のプロパティは、「[プロパティ](#properties)」セクションに記載されています。 既定では返されないプロパティを取得するには、そのプロパティを `$select` OData クエリ オプションで指定します。 [例](../api/group-get.md#request-2)を参照してください。

このリソースは以下をサポートしています。

- [拡張機能](/graph/extensibility-overview)として、カスタム プロパティに独自のデータを追加します。
- [変更通知](/graph/webhooks)を受信します。
- [デルタ](../api/user-delta.md)関数を提供することにより、[デルタ クエリ](/graph/delta-query-overview)を使用して、増分の追加、削除、更新を追跡します。


## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|**グループの管理**| | |
|[グループを作成する](../api/group-post-groups.md) | [group](group.md) |新しいグループを作成します。 Office 365 グループ、動的なグループ、またはセキュリティ グループのいずれかにできます。|
|[グループを取得する](../api/group-get.md) | [group](group.md) |グループ オブジェクトのプロパティを読み取ります。|
|[グループを一覧表示する](../api/group-list.md) |[group](group.md) コレクション |グループ オブジェクトとそのプロパティを一覧表示します。|
|[グループを更新する](../api/group-update.md) | なし |グループ オブジェクトのプロパティを更新します。 |
|[グループを削除する](../api/group-delete.md) | なし |グループ オブジェクトを削除します。 |
|[delta](../api/group-delta.md)|group コレクション| グループに対する増分の変更を取得します。 |
|[List groupLifecyclePolicies](../api/group-list-grouplifecyclepolicies.md) |[groupLifecyclePolicy](grouplifecyclepolicy.md) コレクション| グループのライフサイクル ポリシーを一覧表示します。 |
|[Renew](../api/group-renew.md)|ブール型|グループの有効期限を更新します。 グループが更新されると、グループの有効期限はポリシーで定義された日数、延長されます。|
|[Add owner](../api/group-post-owners.md) |なし| **owners** ナビゲーション プロパティ (セキュリティ グループおよびメールが有効なセキュリティ グループのみをサポート) に投稿することによってグループの新規所有者を追加します。|
|[所有者を一覧表示する](../api/group-list-owners.md) |[directoryObject](directoryobject.md) コレクション| **owners** ナビゲーション プロパティからグループの所有者を取得します。|
|[所有者を削除する](../api/group-delete-owners.md) | なし |**owners** ナビゲーション プロパティを使用して Office 365 のグループ、セキュリティ グループ、またはメールが有効なセキュリティ グループから所有者を削除します。|
|[メンバーを追加する](../api/group-post-members.md) |なし| **members** ナビゲーション プロパティ (セキュリティ グループおよびメールが有効なセキュリティ グループでのみサポートされます) に投稿することによってこのグループにユーザーまたはグループを追加します。|
|[メンバーを一覧表示する](../api/group-list-members.md) |[directoryObject](directoryobject.md) コレクション| **members** ナビゲーション プロパティからこのグループの直接のメンバーであるユーザーおよびグループを取得します。|
|[推移的なメンバーを一覧表示する](../api/group-list-transitivemembers.md) |[directoryObject](directoryobject.md) コレクション| このグループの入れ子のメンバーを含む、メンバーになっているユーザー、グループ、デバイスを取得します。|
|[推移的な memberOf を一覧表示する](../api/group-list-transitivememberof.md) |[directoryObject](directoryobject.md) コレクション| ユーザーがメンバーになっているグループを一覧表示します。 この操作は推移的で、このグループが入れ子のメンバーになっているグループが含まれます。 |
|[メンバーを削除する](../api/group-delete-members.md) | なし |**members** ナビゲーション プロパティを使用して Office 365 のグループ、セキュリティ グループ、またはメールが有効なセキュリティ グループからメンバーを削除できます。ユーザーや他のグループを削除できます。 |
|[checkMemberGroups](../api/group-checkmembergroups.md)|String collection|グループの一覧内のメンバーシップについてこのグループを確認します。この関数は、推移的です。|
|[getMemberGroups](../api/group-getmembergroups.md)|String collection|このグループがメンバーであるすべてのグループを返します。この関数は、推移的です。|
|[getMemberObjects](../api/group-getmemberobjects.md)|String collection|このグループがメンバーであるすべてのグループを返します。この関数は、推移的です。 |
|[Create setting](../api/groupsetting-post-groupsettings.md) | [groupSetting](groupsetting.md) |groupSettingTemplate に基づいて、設定オブジェクトを作成します。POST 要求は、テンプレートに定義されているすべての設定の settingValues を提供する必要があります。グループ固有のテンプレートにのみ、この操作を使用します。|
|[設定を取得する](../api/groupsetting-get.md) | [groupSetting](groupsetting.md) | 特定の設定オブジェクトのプロパティを参照します。 |
|[設定を一覧表示する](../api/groupsetting-list.md) | [groupSetting](groupsetting.md) コレクション | すべての設定オブジェクトのプロパティを一覧表示します。 |
|[設定を更新する](../api/groupsetting-update.md) | [groupSetting](groupsetting.md) | 設定オブジェクトを更新します。 |
|[設定を削除する](../api/groupsetting-delete.md) | なし | 設定オブジェクトを削除します。 |
|**予定表**| | |
|[イベントを作成する](../api/group-post-events.md) |[event](event.md)| event コレクションへの投稿によって、新しいイベントを作成します。|
|[イベントを取得する](../api/group-get-event.md) |[event](event.md)|event オブジェクトのプロパティを読み取ります。|
|[イベントを一覧表示する](../api/group-list-events.md) |[event](event.md) コレクション| event オブジェクトのコレクションを取得します。|
|[イベントを更新する](../api/group-update-event.md) |なし|event オブジェクトのプロパティを更新します。|
|[イベントを削除する](../api/group-delete-event.md) |なし|event オブジェクトを削除します。|
|[calendarView を一覧表示する](../api/group-list-calendarview.md) |[event](event.md) コレクション| 指定された時間枠のイベントのコレクションを取得します。|
|**会話**| | |
|[会話を作成する](../api/group-post-conversations.md) |[conversation](conversation.md)| conversation コレクションに投稿して、新しい会話を作成します。|
|[会話を取得する](../api/group-get-conversation.md) |[conversation](conversation.md)| conversation オブジェクトのプロパティを読み取ります。|
|[会話を一覧表示する](../api/group-list-conversations.md) |[conversation](conversation.md) コレクション| conversation オブジェクトのコレクションを取得します。|
|[会話を削除する](../api/group-delete-conversation.md) |なし|conversation オブジェクトを削除します。|
|[スレッドを取得する](../api/group-get-thread.md) |[conversationThread](conversationthread.md)| thread オブジェクトのプロパティを読み取ります。|
|[スレッドを一覧表示する](../api/group-list-threads.md) |[conversationThread](conversationthread.md) コレクション| グループのすべてのスレッドを取得します。|
|[スレッドを更新する](../api/group-update-thread.md) |なし| thread オブジェクトのプロパティを更新します。|
|[スレッドを削除する](../api/group-delete-thread.md) |なし| thread オブジェクトを削除します。|
|[acceptedSenders を一覧表示する](../api/group-list-acceptedsenders.md) |[directoryObject](directoryobject.md) collection| このグループの許可された送信者リストに含まれるユーザーまたはグループの一覧を取得します。|
|[acceptedSender を追加する](../api/group-post-acceptedsenders.md) |[directoryObject](directoryobject.md)| acceptSenders コレクションにユーザーまたはグループを追加します。|
|[acceptedSender を削除する](../api/group-delete-acceptedsenders.md) |[directoryObject](directoryobject.md)| acceptedSenders コレクションからユーザーまたはグループを削除します。|
|[rejectedSenders を一覧表示する](../api/group-list-rejectedsenders.md) |[directoryObject](directoryobject.md) collection| このグループの拒否された送信者リストに含まれるユーザーまたはグループの一覧を取得します。|
|[rejectedSender を追加する](../api/group-post-rejectedsenders.md) |[directoryObject](directoryobject.md)| rejectedSender コレクションに新しいユーザーまたはグループを追加します。|
|[rejectedSender を削除する](../api/group-delete-rejectedsenders.md) |[directoryObject](directoryobject.md)| rejectedSender コレクションから新しいユーザーまたはグループを削除します。|
|[設定を作成する](../api/groupsetting-post-groupsettings.md) | [groupSetting](groupsetting.md) |groupSettingTemplate に基づいて、設定オブジェクトを作成します。POST 要求は、テンプレートに定義されているすべての設定の settingValues を提供する必要があります。グループ固有のテンプレートにのみ、この操作を使用します。|
|[設定を取得する](../api/groupsetting-get.md) | [groupSetting](groupsetting.md) | 特定の設定オブジェクトのプロパティを参照します。 |
|[設定を一覧表示する](../api/groupsetting-list.md) | [groupSetting](groupsetting.md) コレクション | すべての設定オブジェクトのプロパティを一覧表示します。 |
|[設定を更新する](../api/groupsetting-update.md) | なし | 設定オブジェクトを更新します。 |
|[設定を削除する](../api/groupsetting-delete.md) | なし | 設定オブジェクトを削除します。 |
|**オープン拡張機能**| | |
|[オープン拡張機能を作成する](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| オープン拡張機能を作成し、新規または既存のリソースにカスタム プロパティを追加します。|
|[オープン拡張機能を取得する](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md) コレクション| 拡張機能の名前で識別されるオープン拡張機能を取得します。|
|**スキーマ拡張機能**| | |
|[スキーマ拡張機能の値を追加する](/graph/extensibility-schema-groups) || スキーマ拡張機能の定義を作成し、それを使用してカスタムの型指定されたデータをリソースに追加します。|
|**その他のグループ リソース**| | |
|[写真を一覧表示する](../api/group-list-photos.md) |[profilePhoto](photo.md) コレクション| グループのプロファイル写真のコレクションを取得します。|
|[plannerPlans を一覧表示する](../api/plannergroup-list-plans.md) |[plannerPlan](plannerplan.md) コレクション| グループが所有しているプランナーの計画を取得します。|
|**ユーザーの設定**| | |
|[addFavorite](../api/group-addfavorite.md)|なし|サインインしているユーザーのお気に入りのグループ一覧にグループを追加します。 Office 365 のグループのみをサポートします。|
|[removeFavorite](../api/group-removefavorite.md)|なし|サインインしているユーザーのお気に入りのグループ一覧からグループを削除します。 Office 365 のグループのみをサポートします。|
|[memberOf を一覧表示する](../api/group-list-memberof.md) |[directoryObject](directoryobject.md) コレクション| このユーザーが直接のメンバーであるグループおよび管理単位を、**memberOf** ナビゲーション プロパティから取得します。|
|[subscribeByMail](../api/group-subscribebymail.md)|なし|isSubscribedByMail プロパティを **true** に設定します。 サインインしているユーザーが電子メールの会話を受信できるようにします。 Office 365 のグループのみをサポートします。|
|[unsubscribeByMail](../api/group-unsubscribebymail.md)|なし|isSubscribedByMail プロパティを **false** に設定します。 サインインしているユーザーが電子メールの会話を受信できないようにします。 Office 365 のグループのみをサポートします。|
|[resetUnseenCount](../api/group-resetunseencount.md)|なし|サインインしているユーザーが最後の訪問以降見ていない、すべての投稿の unseenCount を 0 にリセットします。 Office 365 のグループのみをサポートします。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|allowExternalSenders|Boolean| 組織外部のユーザーがグループにメッセージを送信できるかどうかを示します。 既定値は **false** です。 <br><br>$select でのみ返されます。 |
|assignedLicenses|[assignedLicense](assignedlicense.md) コレクション|グループに割り当てられているライセンス。 <br><br>$select でのみ返されます。 読み取り専用です。|
|autoSubscribeNewMembers|Boolean|グループに追加された新しいメンバーが、電子メールの通知を受信するように自動的にサブスクライブされるかどうかを示します。 グループの PATCH 要求でこのプロパティを設定できます。グループを作成する最初の POST 要求では設定しないでください。 既定値は **false** です。 <br><br>$select でのみ返されます。|
|classification|String|グループの分類 (低、中、高程度の企業への影響など) を説明します。このプロパティの有効な値は、[テンプレート定義](groupsettingtemplate.md)に基づいて ClassificationList [設定](groupsetting.md)値を作成することによって定義されます。<br><br>既定で返されます。|
|createdDateTime|DateTimeOffset| グループ作成時のタイムスタンプです。 値は変更できず、グループが作成されると自動的に設定されます。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。 <br><br>既定で返されます。 読み取り専用です。 |
|説明|String|グループに関するオプションの説明。 <br><br>既定で返されます。|
|displayName|文字列|グループの表示名。 このプロパティは、グループの作成時の必須プロパティであり、更新時にクリアすることはできません。 <br><br>既定で返されます。 $filter および $orderby をサポートします。 |
|groupTypes|String コレクション| 作成するグループの種類を指定します。 使用可能な値は `Unified` (Office 365 のグループを作成する場合) または `DynamicMembership` (動的なグループを作成する場合) です。  その他のグループの種類 (セキュリティが有効なグループやメールが有効なセキュリティ グループなど) の場合、このプロパティは設定しないでください。 <br><br>既定で返されます。 $filter をサポートします。|
|hasMembersWithLicenseErrors|Boolean|このグループの中に、そのグループに基づくライセンス割り当てのライセンス エラーが発生しているメンバーがいるかどうかを示します。 <br><br>このプロパティは GET 操作では返されません。 これを $ filter 引数として使用して、ライセンス エラーが発生しているメンバーがいるグループを取得できます (つまり、このプロパティが true であるフィルターです)。 [例](../api/group-list.md)を参照してください。|
|id|String|グループの一意の識別子。 <br><br>既定で返されます。 [directoryObject](directoryobject.md) から継承されます。 キー。 null 許容ではありません。 読み取り専用です。|
|isSubscribedByMail|Boolean|サインインしているユーザーが電子メールの会話を受信するように登録されているかどうかを示します。 既定値は **true** です。 <br><br>$select でのみ返されます。 |
|licenseProcessingState|String|グループのメンバー全員にグループ ライセンスの割り当ての状態を示します。 既定値は **false** です。 読み取り専用です。 使用可能な値: `QueuedForProcessing`、`ProcessingInProgress`、`ProcessingComplete`。<br><br>$select でのみ返されます。 読み取り専用です。|
|mail|String|グループの SMTP アドレス (たとえば、"Serviceadmins@contoso.onmicrosoft.com")。 <br><br>既定で返されます。 読み取り専用です。 $filter をサポートします。|
|mailEnabled|Boolean|メールが有効なグループであるかどうかを指定します。**securityEnabled** プロパティも **true** の場合、グループはメールが有効なセキュリティ グループになります。それ以外の場合は、Microsoft Exchange 配布グループになります。 <br><br>既定で返されます。|
|mailNickname|String|グループのメール エイリアスです (組織内で一意)。 このプロパティは、グループの作成時に指定する必要があります。 <br><br>既定で返されます。 $filter をサポートします。|
|onPremisesLastSyncDateTime|DateTimeOffset|グループがオンプレミスのディレクトリと最後に同期した日時を示します。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。 <br><br>既定で返されます。 読み取り専用です。 $filter をサポートします。|
|onPremisesProvisioningErrors|[onPremisesProvisioningError](onpremisesprovisioningerror.md) コレクション| Microsoft 同期製品のプロビジョニング中に発生するエラーです。 <br><br>既定で返されます。|
|onPremisesSecurityIdentifier|String|オンプレミスからクラウドに同期されたグループのオンプレミスのセキュリティ識別子 (SID) が含まれます。 <br><br>既定で返されます。 読み取り専用です。 |
|onPremisesSyncEnabled|Boolean|このグループがオンプレミスのディレクトリから同期される場合は **true**、このグループが最初にオンプレミスのディレクトリから同期されていて、今後は同期しない場合は **false**、このオブジェクトがオンプレミスのディレクトリから一度も同期されたことがない場合は **null**。 <br><br>既定で返されます。 読み取り専用です。 $filter をサポートします。|
|preferredDataLocation|String|グループの優先されるデータの場所。 詳細については、「[OneDrive Online Multi-Geo](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction)」を参照してください。 <br><br>既定で返されます。|
|proxyAddresses|String コレクション| 同じグループ メールボックスに送信されるグループのメール アドレスです。 例: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]`。 複数値プロパティのフィルター式には **any** 演算子が必要です。 <br><br>既定で返されます。 読み取り専用です。 null 許容ではありません。 $filter をサポートします。 |
|renewedDateTime|DateTimeOffset| グループの最後の更新時のタイムスタンプです。 これは直接変更することはできず、[更新サービス アクション](../api/group-renew.md)経由でのみ更新されます。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。 <br><br>既定で返されます。 読み取り専用です。|
|securityEnabled|ブール値|グループがセキュリティ グループであるかどうかを指定します。 **mailEnabled** プロパティも true の場合、グループはメールが有効なセキュリティ グループになります。それ以外の場合は、セキュリティ グループになります。 Office 365 グループの場合、**false** にする必要があります。 <br><br>既定で返されます。 $filter をサポートします。|
|unseenCount|Int32|サインにしているユーザーのグループへの最後のアクセス以降に新しい投稿を受け取った会話の数です。 <br><br>$select でのみ返されます。 |
|visibility|String| Office 365 グループの表示を指定します。 使用可能な値: `private`、`public`、`hiddenmembership`。空の値はパブリックとして扱われます。  詳細については、「[グループの表示オプション](#group-visibility-options)」を参照してください。<br>表示はグループが作成されているときのみ設定することができます。編集はできません。<br>表示は、統合グループのみでサポートされています。セキュリティ グループではサポートされていません。 <br><br>既定で返されます。|


### <a name="group-visibility-options"></a>グループの表示オプション

各 **visibility** プロパティの値が表す意味は次のとおりです。
 
|値|説明|
|:----|-----------|
| `public` | 所有者のアクセス許可の必要がなく、だれでもグループに参加することができます。<br>グループのコンテンツをだれでも読むことができます。|
| `private` | グループに参加するには、所有者のアクセス許可が必要です。<br>メンバー以外はグループのコンテンツを読むことができません。|
| `hiddenmembership` | グループに参加するには、所有者のアクセス許可が必要です。<br>メンバー以外はグループのコンテンツを読むことができません。<br>メンバー以外はグループのメンバーを確認することができません。<br>管理者 (グローバル、会社、ユーザー、ヘルプデスク) が、グループのメンバーシップを参照できます。<br>グループは、グローバル アドレス帳 (GAL) に表示されます。|


## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|acceptedSenders|[directoryObject](directoryobject.md) コレクション|このグループで投稿または予定表のイベントを作成することが許可されているユーザーまたはグループの一覧。この一覧が空でない場合、ここに記載されているユーザーまたはグループだけが投稿を許可されます。|
|予定表|[calendar](calendar.md)|グループの予定表。読み取り専用です。|
|calendarView|[event](event.md) コレクション|予定表のカレンダー ビュー。読み取り専用です。|
|conversations|[conversation](conversation.md) コレクション|グループの会話。|
|createdOnBehalfOf|[directoryObject](directoryobject.md)| グループを作成したユーザー (またはアプリケーション)。注: ユーザーが管理者である場合、これは設定されません。読み取り専用です。|
|ドライブ|[drive](drive.md)|グループの既定のドライブ。 読み取り専用です。|
|drives|[drive](drive.md) コレクション|グループのドライブ。 読み取り専用です。|
|events|[event](event.md) コレクション|グループの予定表イベント。|
|extensions|[extension](extension.md) コレクション|グループに対して定義されているオープン拡張機能のコレクション。読み取り専用です。Null 許容型。|
|groupLifecyclePolicies|[groupLifecyclePolicy](grouplifecyclepolicy.md) コレクション|このグループのライフ サイクル ポリシーのコレクション。 読み取り専用です。 Null 許容型。|
|memberOf|[directoryObject](directoryobject.md) コレクション|このグループがメンバーとして含まれているグループ。HTTP メソッド:GET (すべてのグループでサポートされます)。読み取り専用です。Null 許容型。|
|members|[directoryObject](directoryobject.md) コレクション| このグループのメンバーであるユーザーとグループ。HTTP メソッド:GET (すべてのグループでサポートされます)、POST (Office 365 グループ、セキュリティ グループ、およびメールが有効なセキュリティ グループでサポートされます)、DELETE (Office 365 グループとセキュリティ グループでサポートされます)。Null 許容型。|
|membersWithLicenseErrors|[User](user.md) コレクション|このグループに基づくライセンスの割り当てからのライセンス エラーが発生しているグループ メンバーの一覧です。 読み取り専用です。|
|onenote|[OneNote](onenote.md)| 読み取り専用です。|
|owners|[directoryObject](directoryobject.md) コレクション|グループの所有者。所有者は、このオブジェクトの変更を許可されている管理者以外のユーザーです。10 人の所有者に制限されます。HTTP メソッド:GET (すべてのグループでサポートされます)、POST (Office 365 グループ、セキュリティ グループ、およびメールが有効なセキュリティ グループでサポートされます)、DELETE (Office 365 グループとセキュリティ グループでサポートされます)。Null 許容型。|
|写真|[profilePhoto](profilephoto.md)| グループのプロファイル写真 |
|photos|[profilePhoto](profilephoto.md) コレクション| グループが所有しているプロファイル写真。読み取り専用です。Null 許容型。|
|planner|[plannerGroup](plannergroup.md)| 統合グループに存在する可能性がある Planner リソースのエントリ ポイント。|
|rejectedSenders|[directoryObject](directoryobject.md) コレクション|このグループで投稿またはカレンダーのイベントを作成することが許可されていないグループの一覧。Null 許容型|
|設定|[groupSetting](groupsetting.md) コレクション| 読み取り専用。Null 許容型。|
|sites|[site](site.md) コレクション|このグループ内の SharePoint サイトの一覧。/sites/root を使用して既定のサイトにアクセスします。|
|threads|[conversationThread](conversationthread.md) コレクション| グループの会話スレッド。Null 許容型。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true,
  "optionalProperties": [
    "acceptedSenders",
    "appRoleAssignments",
    "calendar",
    "calendarView",
    "conversations",
    "createdOnBehalfOf",
    "drive",
    "drives",
    "events",
    "extensions",
    "groupLifecyclePolicies",
    "memberOf",
    "members",
    "onenote",
    "owners",
    "photo",
    "photos",
    "planner",
    "rejectedSenders",
    "settings",
    "sites",
    "threads",

    "allowExternalSenders",
    "assignedLicenses",
    "autoSubscribeNewMembers",
    "hasMembersWithLicenseErrors",
    "isSubscribedByMail",
    "licenseProcessingState",
    "unseenCount"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.group",
  "@odata.annotations": [
    {
      "capabilities": {
        "changeTracking": true
      }
    },
    {
      "property": "acceptedSenders",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "calendar",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "calendarView",
      "capabilities": {
        "changeTracking": true,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "conversations",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "updatable": false
      }
    },
    {
      "property": "events",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "photo",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false
      }
    },
    {
      "property": "photos",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "rejectedSenders",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "threads",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "allowExternalSenders": false,
  "assignedLicenses": [{"@odata.type": "microsoft.graph.assignedLicense"}],
  "autoSubscribeNewMembers": true,
  "classification": "string",
  "createdDateTime": "String (timestamp)",
  "description": "string",
  "displayName": "string",
  "groupTypes": ["string"],
  "hasMembersWithLicenseErrors": "Boolean",
  "id": "string (identifier)",
  "isSubscribedByMail": true,
  "licenseProcessingState": "string",
  "mail": "string",
  "mailEnabled": true,
  "mailNickname": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
  "preferredDataLocation": "string",
  "proxyAddresses": ["string"],
  "renewedDateTime": "String (timestamp)",
  "securityEnabled": true,
  "unseenCount": 1024,
  "visibility": "string",
  "acceptedSenders": [ { "@odata.type": "microsoft.graph.directoryObject"} ],
  "calendar": { "@odata.type": "microsoft.graph.calendar" },
  "calendarView": [{ "@odata.type": "microsoft.graph.event" }],
  "conversations": [ { "@odata.type": "microsoft.graph.conversation" }],
  "createdOnBehalfOf": { "@odata.type": "microsoft.graph.directoryObject" },
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "events": [ { "@odata.type": "microsoft.graph.event" }],
  "memberOf": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "members": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "membersWithLicenseErrors": [{"@odata.type": "microsoft.graph.user"}],
  "owners": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "photo": { "@odata.type": "microsoft.graph.profilePhoto" },
  "rejectedSenders": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "sites": [ { "@odata.type": "microsoft.graph.site" } ],
  "threads": [ { "@odata.type": "microsoft.graph.conversationThread" }]
}

```

## <a name="see-also"></a>関連項目

- [拡張機能を使用してカスタム データをリソースに追加する](/graph/extensibility-overview)
- [オープン拡張機能を使用してカスタム データをユーザーに追加する](/graph/extensibility-open-users)
- [スキーマ拡張機能を使用したグループへのカスタム データの追加](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
