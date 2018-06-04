# <a name="microsoft-graph-rest-api-v10-reference"></a>Microsoft Graph REST API v1.0 リファレンス

v1.0 エンドポイント用の Microsoft Graph REST API リファレンスへようこそ。

v1.0 エンドポイントの API セット (`https://graph.microsoft.com/v1.0`) は、一般提供 (GA) ステータスで、顧客との厳密なレビューとフィードバック プロセスを経て、運用環境の実用的なニーズを満たすものとなっています。 このエンドポイントの API の更新は、追加的なものであり、既存のアプリのシナリオを損なうものではありません。

## <a name="common-use-cases"></a>一般的なユース ケース

Microsoft Graph では、単一の Microsoft Graph REST エンドポイントで公開されている異なるサービスのエンティティやリレーションシップのナビゲーションが簡単に行うことができます。

これらのサービスの多くは、[ユーザー](../api-reference/v1.0/resources/user.md)および[グループ](../api-reference/v1.0/resources/group.md)にとって、さまざまなシナリオを実現できるよう設計されています。

### <a name="user-centric-use-cases-in-v10"></a>V1.0 でのユーザー中心のユース ケース

1. ユーザー (Lisa) の[プロファイルを取得](../api-reference/v1.0/api/user_get.md)し、[写真](../api-reference/v1.0/resources/profilephoto.md)を取得します。
2. Azure Active Directory に保存されている [Lisa のマネージャーのプロファイル情報を取得](../api-reference/v1.0/api/user_list_manager.md)し、[直属の部下の ID](../api-reference/v1.0/api/user_list_directreports.md) を取得します。
3. [OneDrive for Business 上で、Lisa のファイルにアクセス](../api-reference/v1.0/api/driveitem_list_children.md)し、最後にその[ファイル](../api-reference/v1.0/resources/driveitem.md)を更新した[ユーザー](../api-reference/v1.0/resources/identityset.md)を特定し、その人のプロファイルに移動します。
4. Exchange Online 上の [Lisa の予定表にアクセス](../api-reference/v1.0/api/calendar_get.md)し、向こう 2 週間で [Lisa が彼女のチームとの会議に最適な時間を決定](../api-reference/v1.0/api/user_findmeetingtimes.md)します。
5. Lisa の予定表を[購読](../api-reference/v1.0/api/subscription_post_subscriptions.md)し、[変更履歴を記録](../api-reference/v1.0/api/event_delta.md)し、Lisa が会議に自分の時間の 80% 以上を費やしている場合に報告します。
6. Lisa が外出中のときに[自動応答を設定](../api-reference/v1.0/api/user_update_mailboxsettings.md#example)します。
7. コミュニケーション、コラボレーション、ビジネスのリレーションシップに基づいて、[Lisa にもっとも関連のある人物を取得](../api-reference/v1.0/api/user_list_people.md)します。
8. Lisa の OneDrive for Business 上の Excel ファイルの、[グラフ](../api-reference/v1.0/resources/chart.md)から、最新の販売計画を取得します。
9. [Planner で Lisa に割り当てられているタスクを検索](../api-reference/v1.0/api/planneruser_list_tasks.md)します。

### <a name="office-365-group-use-cases-in-v10"></a>V1.0 での Office 365 グループのユース ケース

1. 組織内の Office 365 グループに関するレポートを実行し、[グループのメンバー間の通信](../api-reference/v1.0/api/reportroot_getoffice365groupsactivitycounts.md)がもっとも多いグループを特定します。
2. [この Office 365 グループの計画を検索](../api-reference/v1.0/api/plannergroup_list_plans.md)し、その計画の[タスクの割り当て](../api-reference/v1.0/resources/plannerassignments.md)を検索します。
3. Office 365 グループ内で[新しい会話を開始](../api-reference/v1.0/api/group_post_conversations.md)し、メンバーがワークロードを共有するために[別のグループを作成する](../api-reference/v1.0/api/group_post_groups.md)かどうかを決定します。
4. グループの[既定のノートブックを取得](../api-reference/v1.0/api/notebook_get.md)し、調査の結果を記録する[新しいページを作成](../api-reference/v1.0/api/section_post_pages.md)します。

## <a name="other-api-versions"></a>その他の API バージョン

現在、Microsoft Graph REST API には、- v1.0 とベータ版の 2 つのバージョンがあります。
プレビューの状態にある新しいまたは拡張の API を検討する場合は 「[Microsoft Graph ベータ エンドポイント リファレンス](../api-reference/beta/beta-overview.md)」を参照してください。 プレビュー状態の API は今後変更される可能性があり、予告なしに既存のシナリオが動作しなくなる場合があることにご注意ください。 ベータ版のエンドポイントの API に運用環境で依存関係を持たないようにしてください。

詳細については、「[バージョン管理とサポート](versioning_and_support.md)」を参照してください。

## <a name="connect-with-us"></a>連絡方法

Microsoft Graph に追加したい API や機能がある場合 新しい機能のリクエストを [UserVoice](https://officespdev.uservoice.com/forums/224641-general/filters/new?category_id=101632) に投稿してください。

既存の Microsoft Graph API に対するフィードバックがある場合 [Github](https://github.com/microsoftgraph/microsoft-graph-docs/issues) から連絡してください。

Microsoft Graph を使用したコードに関する質問や、ヘルプを受けるには、[Stack Overflow](https://stackoverflow.com/questions/tagged/microsoftgraph) に参加してください。
