---
title: Microsoft Graph API を使用して、アプリにソーシャル インテリジェンスとワークプレイス インテリジェンスを統合する
description: Microsoft Graph は、人々にとって有用なソーシャルおよび職場データへのアクセスを可能にし、ユーザーのソーシャル コンテキストでのソーシャル ジェスチャーをサポートします。
localization_priority: Priority
author: simonhult
ms.prod: insights
doc_type: conceptualPageType
ms.openlocfilehash: 74beb2a66f103342f6dbc5e5977200751a309c08
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450670"
---
# <a name="use-the-microsoft-graph-api-to-integrate-social-and-workplace-intelligence-in-an-app"></a>Microsoft Graph API を使用して、アプリにソーシャル インテリジェンスとワークプレイス インテリジェンスを統合する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph は、人々にとってのソーシャルおよび職場データへのアクセスを可能にし、ユーザーのソーシャル コンテキストでのジェスチャーをサポートします。

## <a name="aggregate-and-extract-specific-information-about-people"></a>ユーザーに関する特有の情報を集約して抽出する

[person](../resources/person.md) リソースと People API を使用して、メール、連絡先、およびソーシャル ネットワークから、個人に関する情報を集約することができます。 結果は、複数のコミュニケーション、コラボレーション、およびビジネスのリレーションシップを基に、関連性によって並べられます。 API を使用すると、条件に基づいて、個人の閲覧、並べ替え、選択、フィルター、または検索を行うことができます。

- [ユーザーを一覧表示する](../api/user-list-people.md)

## <a name="help-users-get-the-most-relevant-documents-for-their-work"></a>ユーザーの仕事に最適なドキュメントの取得に役立つ

Insights API を使用して、ユーザーに最適なドキュメントを特定する:

- ユーザーの[周りで人気急上昇中](../api/insights-list-trending.md)のドキュメントを一覧表示する
- ユーザーによって[使用される](../api/insights-list-used.md)ドキュメントを一覧表示する 
- ユーザーが[共有先または共有元](../api/insights-list-shared.md)のドキュメントを一覧表示する 

## <a name="help-users-gain-insights-into-their-work-patterns"></a>ユーザーが自分の仕事のパターンに関する洞察を得るのを助けます

Analytics API を使用して、ユーザーのアクティビティ統計および関連する設定を取得します。

- [設定](../resources/settings.md): analytics API がユーザーの結果を返すには、現在のユーザー分析設定に有効な MyAnalytics ライセンスが表示され、MyAnalytics の使用が選択され、グラフ対応のクラウドホスト型メールボックスが必要です。
- [activityStatistics](../resources/activitystatistics.md): [通話](callactivitystatistics.md)、[チャット (インスタント メッセージ)](chatactivitystatistics.md)、[電子メール](emailactivitystatistics.md)、勤務時間中および勤務時間外の[会議](meetingactivitystatistics.md)に費やされた時間数や[集中作業](focusactivitystatistics.md)に利用できる時間数を含む、ユーザーが時間を費やした Office 365 アクティビティの最後の週全体 (または指定された時間範囲) のデータを取得します。

## <a name="manage--mentions"></a>@- メンションを管理する

ソーシャルの世界では、メッセージ内で受信者に通知して注意を引くために受信者に呼びかけることが一般的に行われています。
[mention](../resources/mention.md) リソースと Mentions API には、[メッセージ](../resources/message.md)内で受信者に呼びかけたり、ユーザーが @-メンションを使用して通知しているすべてのメッセージを取得したり、メッセージの内の各メンションを取得したりする軽量のメカニズムが備わっています。

<!--
Include the next sentence when supporting events.

**Mention** is also supported by [Event](../resources/event.md).

-->

- 新しいメッセージ内にメンションを作成する

  - [新しいメッセージの一部としてメンションを作成および送信する](../api/user-sendmail.md#request-2)
  - [下書きの一部としてメンションを作成する](../api/user-post-messages.md#request-2)

- メッセージのメンションに関する情報を取得する

  - [対象ユーザーについてメンションしている、サインイン ユーザーのメールボックス内のすべてのメッセージを取得する](../api/user-list-messages.md#request-2)
  - [特定のメッセージ内の各メンションの詳細を取得する](../api/message-get.md#request-2)

- 特定のメッセージ内の[メンションを削除する](../api/message-delete.md#request-2)
