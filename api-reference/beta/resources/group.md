---
title: group リソースの種類
description: Office 365 のグループ、マイクロソフトのチームで、チーム、動的グループ、またはセキュリティ グループは、Azure Active Directory (AD の Azure) のグループを表します。
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 84f4f1121c6ca407fcf6064d63970aa4fc5f663e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960148"
---
# <a name="group-resource-type"></a>group リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

Office 365 のグループ、マイクロソフトのチームで、チーム、動的グループ、またはセキュリティ グループは、Azure Active Directory (AD の Azure) のグループを表します。
[directoryObject](directoryobject.md) から継承します。

このリソースは以下をサポートしています。

- [拡張機能](/graph/extensibility-overview)として、カスタム プロパティに独自のデータを追加します。
- [変更通知](/graph/webhooks)にサブスクライブします。
- [デルタ](../api/user-delta.md)関数を提供することにより、[デルタ クエリ](/graph/delta-query-overview)を使用して、増分の追加、削除、更新を追跡します。

> **マイクロソフトのチームと Office 365 のグループはグループの共同作業をサポート**します。 マイクロソフトのチームでは、ほとんどの Office 365 グループ API を使用できます。 作成する[チーム](team.md)、最初の[グループを作成して](../api/group-post-groups.md)、[それをチームに追加](../api/team-put-teams.md)します。 詳細については、[マイクロソフトのチームの概要](teams-api-overview.md)を参照してください。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|**グループの管理**| | |
|[グループを作成する](../api/group-post-groups.md) | [group](group.md) |指定された新しいグループを作成します。 Office 365 のグループ、動的グループ、セキュリティ グループ、またはチームであることができます。|
|[グループを取得する](../api/group-get.md) | [group](group.md) |グループ オブジェクトのプロパティと関係を参照してください。|
|[グループを更新する](../api/group-update.md) | なし |グループ オブジェクトのプロパティを更新します。 |
|[グループを削除する](../api/group-delete.md) | なし |グループ オブジェクトを削除します。 |
|[delta](../api/group-delta.md)|group コレクション| グループに対する増分の変更を取得します。 |
|[List groupLifecyclePolicies](../api/group-list-grouplifecyclepolicies.md) |[groupLifecyclePolicy](grouplifecyclepolicy.md) コレクション| グループのライフサイクル ポリシーを一覧表示します。 |
|[所有者を一覧表示する](../api/group-list-owners.md) |[directoryObject](directoryobject.md) コレクション| **owners** ナビゲーション プロパティからグループの所有者を取得します。|
|[Add owner](../api/group-post-owners.md) |[directoryObject](directoryobject.md)| **owners** ナビゲーション プロパティ (セキュリティ グループおよびメールが有効なセキュリティ グループのみをサポート) に投稿することによってグループの新規所有者を追加します。|
|[所有者を削除する](../api/group-delete-owners.md) | なし |**owners** ナビゲーション プロパティを使用して Office 365 のグループ、セキュリティ グループ、またはメールが有効なセキュリティ グループから所有者を削除します。|
|[メンバーを一覧表示する](../api/group-list-members.md) |[directoryObject](directoryobject.md) コレクション| **members** ナビゲーション プロパティからこのグループの直接のメンバーであるユーザーおよびグループを取得します。|
|[推移的なメンバーの一覧](../api/group-list-transitivemembers.md) |[directoryObject](directoryobject.md) コレクション| ユーザー、グループ、デバイス、およびサービス プリンシパルは、このグループの入れ子にされたメンバーを含むメンバーを取得します。|
|[メンバーを追加する](../api/group-post-members.md) |[directoryObject](directoryobject.md)| **members** ナビゲーション プロパティ (セキュリティ グループおよびメールが有効なセキュリティ グループでのみサポートされます) に投稿することによってこのグループにユーザーまたはグループを追加します。|
|[メンバーを削除する](../api/group-delete-members.md) | なし |**members** ナビゲーション プロパティを使用して Office 365 のグループ、セキュリティ グループ、またはメールが有効なセキュリティ グループからメンバーを削除できます。ユーザーや他のグループを削除できます。 |
|[memberOf を一覧表示する](../api/group-list-memberof.md) |[directoryObject](directoryobject.md) コレクション| グループとは、このグループへの後方リンクのナビゲーション プロパティから直接メンバーの管理の単位を取得します。|
|[推移的な所属するグループ] ボックスの一覧](../api/group-list-transitivememberof.md) |[directoryObject](directoryobject.md) コレクション| グループとメンバーであるユーザーの管理の単位を一覧表示します。 この操作では、推移的では、このグループの入れ子にされたメンバーであるグループが含まれています。 |
|[checkMemberGroups](../api/group-checkmembergroups.md)|String コレクション|グループの一覧のメンバーシップを確認します。 関数は、推移的です。|
|[getMemberGroups](../api/group-getmembergroups.md)|String コレクション|このグループがメンバーであるすべてのグループを返します。この関数は、推移的です。|
|[getMemberObjects](../api/group-getmemberobjects.md)|String コレクション|すべてのグループとグループのメンバーである管理の単位を返します。 関数は、推移的です。 |
|[設定を作成する](../api/directorysetting-post-settings.md) | [directorySetting](directorysetting.md) |DirectorySettingTemplate に基づいて、設定オブジェクトを作成します。 POST 要求は、テンプレートで定義されているすべての設定 settingValues を提供する必要があります。 この操作には、グループ固有のテンプレートのみを使用できます。|
|[設定を取得する](../api/directorysetting-get.md) | [directorySetting](directorysetting.md) |特定の設定オブジェクトのプロパティを参照します。|
|[設定を一覧表示する](../api/directorysetting-list.md) | [directorySetting](directorysetting.md)コレクション |すべての設定オブジェクトのプロパティを一覧表示します。|
|[設定を更新する](../api/directorysetting-update.md) | [directorySetting](directorysetting.md)  |設定オブジェクトを更新します。 |
|[設定を削除する](../api/directorysetting-delete.md) | なし |設定オブジェクトを削除します。 |
|[エンドポイントのリスト](../api/group-list-endpoints.md) |[エンドポイント](endpoint.md)のコレクション| エンドポイント オブジェクトのコレクションを取得します。 |
|[エンドポイントを取得します。](../api/endpoint-get.md) | [エンドポイント](endpoint.md) | エンドポイント オブジェクトのプロパティと関係を参照してください。 |
|[delta](../api/group-delta.md)|group コレクション| グループに対する増分の変更を取得します。 |
|[validateProperties](../api/group-validateproperties.md)|JSON| メールのニックネームは、命名ポリシーに準拠しているまたは、Office 365 のグループの表示名を検証します。 | 
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
|[スレッドを削除する](../api/group-delete-thread.md) |なし| スレッド オブジェクトを削除します。
|[acceptedSenders を一覧表示する](../api/group-list-acceptedsenders.md) |[directoryObject](directoryobject.md) コレクション| このグループの acceptedSenders リストに含まれるユーザーまたはグループの一覧を取得します。|
|[acceptedSender を追加する](../api/group-post-acceptedsenders.md) |[directoryObject](directoryobject.md)| acceptSenders コレクションにユーザーまたはグループを追加します。|
|[acceptedSender を削除する](../api/group-delete-acceptedsenders.md) |[directoryObject](directoryobject.md)| acceptedSenders コレクションからユーザーまたはグループを削除します。|
|[rejectedSenders を一覧表示する](../api/group-list-rejectedsenders.md) |[directoryObject](directoryobject.md) コレクション| このグループの rejectedSenders リストに含まれるユーザーまたはグループの一覧を取得します。|
|[rejectedSender を追加する](../api/group-post-rejectedsenders.md) |[directoryObject](directoryobject.md)| rejectedSender コレクションに新しいユーザーまたはグループを追加します。|
|[rejectedSender を削除する](../api/group-delete-rejectedsenders.md) |[directoryObject](directoryobject.md)| rejectedSender コレクションから新しいユーザーまたはグループを削除します。|
|**オープン拡張機能**| | |
|[オープン拡張機能を作成する](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| オープン拡張機能を作成し、新規または既存のリソースにカスタム プロパティを追加します。|
|[オープン拡張機能を取得する](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md) コレクション| 拡張機能の名前で識別されるオープン拡張機能を取得します。|
|**スキーマ拡張機能**| | |
|[スキーマ拡張機能の値を追加する](/graph/extensibility-schema-groups) || スキーマ拡張機能の定義を作成し、それを使用してカスタムの型指定されたデータをリソースに追加します。|
|**その他のグループ リソース**| | |
|[写真を一覧表示する](../api/group-list-photos.md) |[profilePhoto](photo.md) コレクション| グループのプロファイル写真のコレクションを取得します。|
|[plannerPlans を一覧表示する](../api/plannergroup-list-plans.md) |[plannerPlan](plannerplan.md) コレクション| グループが所有しているプランナーの計画を取得します。|
|**ユーザーの設定**| | |
|[addFavorite](../api/group-addfavorite.md)|なし|現在のユーザーのお気に入りのグループ一覧にグループを追加します。Office 365 のグループのみをサポートします。|
|[removeFavorite](../api/group-removefavorite.md)|なし|現在のユーザーのお気に入りのグループ一覧からグループを削除します。Office 365 のグループのみをサポートします。|
|[memberOf を一覧表示する](../api/group-list-memberof.md) |[directoryObject](directoryobject.md) コレクション| このユーザーが直接のメンバーであるグループおよび管理単位を、**memberOf** ナビゲーション プロパティから取得します。|
|[参加チームのリストを作成する](../api/user-list-joinedteams.md) |[group](group.md) コレクション| ユーザーの直接のメンバーでは、マイクロソフトのチームを取得します。|
|[subscribeByMail](../api/group-subscribebymail.md)|なし|IsSubscribedByMail プロパティを**true**に設定します。 電子メールを受信する現在のユーザーを有効にします。 Office 365 のグループのみをサポートします。|
|[unsubscribeByMail](../api/group-unsubscribebymail.md)|なし|IsSubscribedByMail プロパティを**false**に設定します。 受信電子メールのやり取りなどから現在のユーザーを無効にします。 Office 365 のグループのみをサポートします。|
|[resetUnseenCount](../api/group-resetunseencount.md)|なし|UnseenCount が、前回のアクセス以降に現在のユーザーが認識されていないすべての投稿の 0 にリセットします。 Office 365 のグループのみをサポートします。|

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|allowExternalSenders|ブール値|既定値は **false** です。組織外部のユーザーがグループにメッセージを送信できるかどうかを示します。|
|assignedLicenses|[assignedLicense](assignedlicense.md) collection|グループに割り当てられているライセンスです。 読み取り専用です。|
|autoSubscribeNewMembers|Boolean|既定値は **false** です。グループに追加された新しいメンバーが、電子メールの通知を受信するように自動的にサブスクライブされるかどうかを示します。グループの PATCH 要求でこのプロパティを設定できます。グループを作成する最初の POST 要求では設定しないでください。|
|分類|String|グループの分類 (低、中、高程度の企業への影響など) を説明します。このプロパティの有効な値は、[テンプレート定義](directorysettingtemplate.md)に基づいて ClassificationList [設定](directorysetting.md)値を作成することによって定義されます。|
|createdDateTime|DateTimeOffset| グループ作成時のタイムスタンプです。 値は変更できず、グループが作成されると自動的に設定されます。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'` 読み取り専用です。 |
|説明|String|グループに関するオプションの説明。|
|displayName|String|グループの表示名。このプロパティは、グループの作成時の必須プロパティであり、更新時にクリアすることはできません。$filter および $orderby をサポートします。|
|groupTypes|String コレクション| 作成するグループの種類を指定します。 使用可能な値は、 `Unified` 、Office 365 のグループを作成するまたは`DynamicMembership`動的グループにします。  他のすべてのグループのセキュリティが有効なグループなど、メールが有効なセキュリティ グループの種類には、このプロパティが設定されません。|
|id|String|グループの一意の識別子。[directoryObject](directoryobject.md) から継承されます。キー。null 許容ではありません。読み取り専用です。|
|isSubscribedByMail|Boolean|既定値は **true** です。現在のユーザーが電子メールの会話を受信するように登録されているかどうかを示します。|
|licenseProcessingState|String|グループのすべてのメンバー グループのライセンスの割り当ての状態を示します。 読み取り専用です。 使用可能な値: `QueuedForProcessing`、`ProcessingInProgress`と`ProcessingComplete`。|
|mail|String|グループの SMTP アドレス (たとえば、"Serviceadmins@contoso.onmicrosoft.com")。読み取り専用です。$filter をサポートします。|
|mailEnabled|Boolean|メールが有効なグループであるかどうかを指定します。**securityEnabled** プロパティも **true** の場合、グループはメールが有効なセキュリティ グループになります。それ以外の場合は、Microsoft Exchange 配布グループになります。|
|mailNickname|String|組織内で一意のグループのメール エイリアス。このプロパティは、グループの作成時に指定する必要があります。$filter をサポートします。|
|membershipRule|String|グループが動的グループの場合、このグループのメンバーを決定するルール (groupTypes が含まれています`DynamicMembership`)。 メンバーシップの規則の構文の詳細については、[メンバーシップの規則の構文](https://azure.microsoft.com/en-us/documentation/articles/active-directory-accessmanagement-groups-with-advanced-rules/)を参照してください。|
|membershipRuleProcessingState|String|動的メンバーシップ処理が上または一時停止するかどうかを示します。 値には"On"または「一時停止」|
|onPremisesLastSyncDateTime|DateTimeOffset|最後にオブジェクトが設置ディレクトリと同期された時刻を示します。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、UTC 時間に常に。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'` 読み取り専用です。 $filter をサポートします。|
|onPremisesProvisioningErrors|[onPremisesProvisioningError](onpremisesprovisioningerror.md)コレクション| 提供処理中に同期の Microsoft 製品を使用するときのエラーです。 |
|onPremisesSecurityIdentifier|String|オンプレミスからクラウドに同期されたグループのオンプレミスのセキュリティ識別子 (SID) が含まれます。読み取り専用です。 |
|onPremisesSyncEnabled|Boolean|このオブジェクトがオンプレミスのディレクトリから同期される場合は **true**。このオブジェクトが最初にオンプレミスのディレクトリから同期されていて、今後は同期されない場合は **false**。このオブジェクトがオンプレミスのディレクトリから一度も同期されたことがない場合は **null** (既定値)。 読み取り専用です。 $filter をサポートします。|
|preferredDataLocation|String|グループの希望するデータの場所です。 詳細については、[オンラインの複数の地域 OneDrive](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction)を参照してください。|
|preferredLanguage|String|Office 365 のグループの言語です。 ISO 639-1 コードに従う必要があります。たとえば"EN-US"です。|
|proxyAddresses|String コレクション| 例: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` **any**演算子は、複数値を持つプロパティのフィルター式に必要です。 読み取り専用です。 null 許容ではありません。 $filter をサポートします。 |
|renewedDateTime|DateTimeOffset| グループの最後の更新時のタイムスタンプです。 これは直接変更することはできず、[更新サービス アクション](../api/grouplifecyclepolicy-renewgroup.md)経由でのみ更新されます。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'` 読み取り専用です。|
|securityEnabled|Boolean|グループがセキュリティ グループであるかどうかを指定します。**mailEnabled** プロパティも true の場合、グループはメールが有効なセキュリティ グループになります。それ以外の場合は、セキュリティ グループになります。Office 365 グループの場合、**false** にする必要があります。$filter をサポートします。|
|theme|String|Office 365 のグループの色のテーマを指定します。 使用可能な値は、 `Teal`、 `Purple`、 `Green`、 `Blue`、 `Pink`、`Orange`または`Red`。|
|unseenConversationsCount|Int32|1 つまたは複数の新規投稿、グループにサインインしているユーザーの前回のアクセス以降配信された会話の数。 このプロパティは、 **unseenCount**と同じです。|
|unseenCount|Int32|1 つまたは複数の新規投稿、グループにサインインしているユーザーの前回のアクセス以降配信された会話の数。 このプロパティは、 **unseenConversationsCount**と同じです。|
|unseenMessagesCount|Int32|グループにサインインしているユーザーの前回のアクセス以降、グループの会話に配信された新規の投稿の数です。|
|visibility|String| Office 365 のグループの表示/非表示を指定します。 使用可能な値: `private`、 `public`、または`hiddenmembership`。空白の値は、public として扱われます。  詳細については、[グループの表示/非表示のオプション](#group-visibility-options)を参照してください。<br>グループが作成されたときにのみ、表示/非表示を設定できます。編集はできません。<br>可視性が統一されたグループでのみサポートされています。セキュリティ グループのことはサポートされていません。|

### <a name="group-visibility-options"></a>グループの表示/非表示のオプション

各**表示**プロパティの値の意味を以下に示します。
 
|値|説明|
|:----|-----------|
| `public` | グループは、所有者のアクセス許可がなくても誰でも参加できます。<br>すべてのユーザーは、グループの内容を表示できます。|
| `private` | グループに参加するには、所有者の権限が必要です。<br>メンバー以外には、グループの内容を表示できません。|
| `hiddenmembership` | グループに参加するには、所有者の権限が必要です。<br>メンバー以外には、グループの内容を表示できません。<br>メンバー以外には、グループのメンバーを表示できません。<br>(グローバル、会社、ユーザー、およびヘルプデスク) の管理者は、グループのメンバーシップを表示できます。<br>グループは、グローバル アドレス一覧 (GAL) に表示されます。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|acceptedSenders|[directoryObject](directoryobject.md) コレクション|このグループで投稿または予定表のイベントを作成することが許可されているユーザーまたはグループの一覧。この一覧が空でない場合、ここに記載されているユーザーまたはグループだけが投稿を許可されます。|
|予定表|[calendar](calendar.md)|グループの予定表。読み取り専用です。|
|calendarView|[event](event.md) コレクション|予定表のカレンダー ビュー。読み取り専用です。|
|conversations|[conversation](conversation.md) コレクション|グループの会話。|
|createdOnBehalfOf|[directoryObject](directoryobject.md)| グループを作成したユーザー (またはアプリケーション)。注: ユーザーが管理者である場合、これは設定されません。読み取り専用です。|
|ドライブ|[drive](drive.md)|グループの既定のドライブです。 読み取り専用です。|
|drives|[drive](drive.md) コレクション|グループのドライブです。 読み取り専用です。|
|エンドポイント|[エンドポイント](endpoint.md)のコレクション| グループに対応するエンドポイントです。 読み取り専用です。 Null 許容型。|
|events|[event](event.md) コレクション|グループのイベントです。|
|extensions|[extension](extension.md) コレクション|グループに対して定義されているオープン拡張機能のコレクション。読み取り専用です。Null 許容型。|
|groupLifecyclePolicies|[groupLifecyclePolicy](grouplifecyclepolicy.md) コレクション|このグループのライフ サイクル ポリシーのコレクションです。 読み取り専用です。 Null 許容型。|
|memberOf|[directoryObject](directoryobject.md) コレクション|出荷単位一覧および管理者はこのグループのメンバーであります。 : の HTTP メソッドを取得 (サポートされているすべてのグループ)。 読み取り専用です。 Null 許容型。|
|members|[directoryObject](directoryobject.md) コレクション| ユーザー、連絡先およびグループがこのグループのメンバーであります。 HTTP メソッド: 取得 (サポートされているすべてのグループ)、(セキュリティ グループ、およびメールが有効なセキュリティ グループのサポート) の投稿、削除の (セキュリティ グループに対してのみサポートされています) 読み取り専用です。 Null 許容型。|
|membersWithLicenseErrors|[ユーザー](user.md)のコレクション|このグループ ・ ベースのライセンスの割り当てからのライセンス エラーのあるグループのメンバーの一覧です。 読み取り専用です。|
|onenote|[OneNote](onenote.md)| 読み取り専用です。|
|owners|[directoryObject](directoryobject.md) コレクション|グループの所有者です。 所有者は、このオブジェクトを変更するのには許可されている管理者以外のユーザーのセットです。 HTTP メソッド: 取得 (サポートされているすべてのグループ)、(セキュリティ グループ、およびメールが有効なセキュリティ グループのサポート) の投稿、削除の (セキュリティ グループに対してのみサポートされています) 読み取り専用です。 Null 許容型。|
|photo|[profilePhoto](profilephoto.md)| グループのプロフィールの写真です。 |
|photos|[profilePhoto](profilephoto.md) コレクション| グループが所有しているプロファイル写真。読み取り専用です。Null 許容型。|
|プランナー|[plannerGroup](plannergroup.md)| 選択的プランナー サービス グループで使用します。 読み取り専用です。 Null 許容型。 |
|rejectedSenders|[directoryObject](directoryobject.md) コレクション|このグループで投稿またはカレンダーのイベントを作成することが許可されていないグループの一覧。Null 許容型|
|設定|[directorySetting](directorysetting.md)コレクション| メンバーがグループに guest ユーザーを招待するかどうかのように、このグループの動作を制御する設定です。 Null 許容型。|
|sites|[site](site.md) コレクション|このグループ内の SharePoint サイトの一覧。/sites/root を使用して既定のサイトにアクセスします。|
|threads|[conversationThread](conversationthread.md) コレクション| グループの会話スレッド。Null 許容型。|

## <a name="json-representation"></a>JSON 表記
次は、JSON 形式のリソース

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "acceptedSenders",
    "appRoleAssignments",
    "calendar",
    "calendarView",
    "conversations",
    "createdOnBehalfOf",
    "drive",
    "events",
    "extensions",
    "memberOf",
    "members",
    "onenote",
    "owners",
    "photo",
    "photos",    
    "rejectedSenders",
    "threads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.group"
}-->

```json
{
  "accessType": "string",
  "assignedLicenses": [{"@odata.type": "microsoft.graph.assignedLicense"}],
  "allowExternalSenders": false,
  "autoSubscribeNewMembers": true,
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "description": "string",
  "displayName": "string",
  "groupTypes": ["string"],
  "id": "string (identifier)",
  "isFavorite": true,  
  "isSubscribedByMail": true,
  "licenseProcessingState": "string",
  "mail": "string",
  "mailEnabled": true,
  "mailNickname": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
  "preferredDataLocation": ["string"],
  "proxyAddresses": ["string"],
  "renewedDateTime": "String (timestamp)",
  "securityEnabled": true,
  "unseenConversationsCount": 1024,
  "unseenCount": 1024,
  "unseenMessagesCount": 1024,
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
