---
title: Microsoft Graph REST API v1.0 リファレンス
description: v1.0 エンドポイント用の Microsoft Graph REST API リファレンスへようこそ。
ms.openlocfilehash: 628b631a877a29dc416671c4a0c5f9a5c0b849ec
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023724"
---
# <a name="microsoft-graph-rest-api-v10-reference"></a>Microsoft Graph REST API v1.0 リファレンス

v1.0 エンドポイント用の Microsoft Graph REST API リファレンスへようこそ。

v1.0 エンドポイントの API セット (`https://graph.microsoft.com/v1.0`) は、一般提供 (GA) ステータスで、顧客との厳密なレビューとフィードバック プロセスを経て、運用環境の実用的なニーズを満たすものとなっています。 このエンドポイントの API の更新は、追加的なものであり、既存のアプリのシナリオを損なうものではありません。

## <a name="common-use-cases"></a>一般的なユース ケース

Microsoft Graph では、単一の Microsoft Graph REST エンドポイントで公開されている異なるサービスのエンティティやリレーションシップのナビゲーションが簡単に行うことができます。

これらのサービスの多くは、[ユーザー](./resources/user.md)および[グループ](./resources/group.md)にとって、さまざまなシナリオを実現できるよう設計されています。

### <a name="user-centric-use-cases-in-v10"></a>V1.0 でのユーザー中心のユース ケース

1. ユーザー (Lisa) の[プロファイルを取得](./api/user-get.md)し、[写真](./resources/profilephoto.md)を取得します。
2. Azure Active Directory に保存されている [Lisa のマネージャーのプロファイル情報を取得](./api/user-list-manager.md)し、[直属の部下の ID](./api/user-list-directreports.md) を取得します。
3. [OneDrive for Business 上で、Lisa のファイルにアクセス](./api/driveitem-list-children.md)し、最後にその[ファイル](./resources/driveitem.md)を更新した[ユーザー](./resources/identityset.md)を特定し、その人のプロファイルに移動します。
4. Exchange Online 上の [Lisa の予定表にアクセス](./api/calendar-get.md)し、向こう 2 週間で [Lisa が彼女のチームとの会議に最適な時間を決定](./api/user-findmeetingtimes.md)します。
5. Lisa の予定表を[購読](./api/subscription-post-subscriptions.md)し、[変更履歴を記録](./api/event-delta.md)し、Lisa が会議に自分の時間の 80% 以上を費やしている場合に報告します。
6. Lisa が外出中のときに[自動応答を設定](./api/user-update-mailboxsettings.md#example)します。
7. コミュニケーション、コラボレーション、ビジネスのリレーションシップに基づいて、[Lisa にもっとも関連のある人物を取得](./api/user-list-people.md)します。
8. Lisa の OneDrive for Business 上の Excel ファイルの、[グラフ](./resources/chart.md)から、最新の販売計画を取得します。
9. [Planner で Lisa に割り当てられているタスクを検索](./api/planneruser-list-tasks.md)します。

### <a name="office-365-group-use-cases-in-v10"></a>V1.0 での Office 365 グループのユース ケース

1. 組織内の Office 365 グループに関するレポートを実行し、[グループのメンバー間の通信](./api/reportroot-getoffice365groupsactivitycounts.md)がもっとも多いグループを特定します。
2. [この Office 365 グループの計画を検索](./api/plannergroup-list-plans.md)し、その計画の[タスクの割り当て](./resources/plannerassignments.md)を検索します。
3. Office 365 グループ内で[新しい会話を開始](./api/group-post-conversations.md)し、メンバーがワークロードを共有するために[別のグループを作成する](./api/group-post-groups.md)かどうかを決定します。
4. グループの[既定のノートブックを取得](./api/notebook-get.md)し、調査の結果を記録する[新しいページを作成](./api/section-post-pages.md)します。

## <a name="other-api-versions"></a>その他の API バージョン

現在、Microsoft Graph REST API には、- v1.0 とベータ版の 2 つのバージョンがあります。
プレビューの状態にある新しいまたは拡張の API を検討する場合は 「[Microsoft Graph ベータ エンドポイント リファレンス](/graph/api/overview?toc=./ref/toc.json&view=graph-rest-beta)」を参照してください。 プレビュー状態の API は今後変更される可能性があり、予告なしに既存のシナリオが動作しなくなる場合があることにご注意ください。 ベータ版のエンドポイントの API に運用環境で依存関係を持たないようにしてください。

詳細については、「[バージョン管理とサポート](/graph/versioning-and-support)」を参照してください。

## <a name="connect-with-us"></a>連絡方法

Microsoft Graph に追加したい API や機能がある場合 新しい機能のリクエストを [UserVoice](https://officespdev.uservoice.com/forums/224641-general/filters/new?category_id=101632) に投稿してください。

既存の Microsoft Graph API に対するフィードバックがある場合 [Github](https://github.com/microsoftgraph/microsoft-graph-docs/issues) から連絡してください。

ご質問または Microsof を使用してコードのヘルプについて