# <a name="overview-of-office-365-groups-in-microsoft-graph"></a>Microsoft Graph での Office 365 グループの概要

Office 365 グループは、ユーザーが会話、ファイル、ノート、予定表、プラン、その他の多くのアセットを共有するための基本メンバーシップ サービスを提供します。 

## <a name="why-integrate-with-office-365-groups"></a>Office 365 グループを統合する理由   

グループは、さまざまなサービスを通じたユーザーのコラボレーションおよび統合を可能にし、タスクの計画、共同作業、教育、その他における豊富なシナリオをサポートするための基盤を形成します。 Office 365 グループを統合することにより、何百万というユーザーが Office 365 スイートでのさまざまなエクスペリエンスやその他の間で移行するのをアプリケーションでサポートすることができます。  
 
### <a name="create-groups-to-facilitate-teamwork-across-services"></a>さまざまなサービスの間の共同作業を容易にするためにグループを作成する 
 
Microsoft Graph API を使用することにより、コラボレーションのライフサイクルを通じてグループを作成、管理、または削除することができます。 たとえば次のことを実行できます。  
 
- [グループ作成](../api-reference/v1.0/api/group_post_groups.md) API を使用することにより、新しいグループを提供する。 そのグループは、Outlook、SharePoint、Microsoft Teams、Planner、さらには Microsoft Stream など、一定の範囲のアプリケーションで利用できます。 Microsoft Graph は、それら互いに接続されているサービスを通じて同期を保つことにより、グループの全メンバーに対してアクセスをシームレスに提供します。  
 
    **あらゆる Office 365 グループは、Office 365 のサービスの既定セットに統合されています**

    ![Office 365 グループのファイル、メモ、タスク、サイト、会話、および予定表との統合を示す図](images/office365-groups-concept-overview-related-services-infographic.png)  

- グループを自分の[お気に入り](../api-reference/v1.0/api/group_addfavorite.md)の 1 つとして指定したり、必要に応じて[自分のお気に入りから削除](../api-reference/v1.0/api/group_removefavorite.md)したりする。 
- カスタム アプリケーションでグループ会話を[作成](../api-reference/v1.0/api/group_post_conversations.md)、[取得](../api-reference/v1.0/api/group_get_conversation.md)、または[削除](../api-reference/v1.0/api/group_delete_conversation.md)する。 
- グループ予定表で予定表[イベント](../api-reference/v1.0/resources/event.md)をスケジューリングする。 
- ドキュメント ライブラリの[リスト](../api-reference/v1.0/api/list_list.md)や[サブサイト](../api-reference/v1.0/api/site_list_subsites.md)など、グループに関連する [SharePoint サイト](../api-reference/v1.0/resources/site.md)についての情報を取得する。 
- Planner で、グループによって所有される[プランを作成](../api-reference/v1.0/api/planner_post_buckets.md)する。 プランは、[複数バケットを通じて整理](../api-reference/v1.0/api/planner_post_buckets.md)できる[タスクを作成](../api-reference/v1.0/api/planner_post_tasks.md)できるようにすることにより、共同作業を追跡するためのビジュアルな手段を提供します。 
- グループに関連する [OneNote](../api-reference/v1.0/resources/onenote.md) ノートブックにアクセスします。それは、会議のメモを収集し、アイデアを整理するために使用できます。 
  
    **Web における Outlook での Office 365 のグループおよび会話**

    ![Outlook on the web で Groups フォルダーにグループのリストが示されているスクリーンショット](images/office365-groups-concept-overview-groups-in-outlook.png) 

- [Microsoft Teams でグループを有効にする](../api-reference/beta/api/team_put_teams.md) (プレビュー) ことにより、グループ メンバーが永続的チャットに参加できるようにする。  
- [グループを削除する](../api-reference/v1.0/api/group_delete.md) グループが削除されると、関連するすべてのコンテンツも削除されるため、サイト、会話、プランが孤立することはありません。 
 
### <a name="manage-group-membership-seamlessly"></a>グループ メンバーシップをシームレスに管理する 
 
Office 365 グループとは、Microsoft サービス内またはアプリ内のリソースへのアクセスを共有しているユーザーの集合です。 グループ メンバーシップは一元的に集中管理されるため、メンバーシップに変更が加えられると、そのグループに関連するすべてのサービスに影響があります。 Microsoft Graph を使用することにより、グループ メンバーシップに関する次のタスクを実行できます:
 
- 既存のグループのメンバーを[追加](../api-reference/v1.0/api/group_post_members.md)したり[削除](../api-reference/v1.0/api/group_delete_members.md)したりする。 
- グループの[所有者の一覧](../api-reference/v1.0/api/group_list_owners.md)または[メンバーの一覧](../api-reference/v1.0/api/group_list_members.md)を取得する。 これは、グループ コンテンツにアクセスできるユーザー、またはグループの更新や参加依頼の承認などの管理作業を実行することが必要になる可能性のあるユーザーと通信するのに役立ちます。 
- [グループ更新](../api-reference/v1.0/api/group_update.md)操作により、グループ コンテンツが同じ組織内のどのユーザーにも表示されるようにグループを**パブリック**として指定したり、グループ コンテンツがメンバーにのみ表示されるようにグループを**プライベート**として指定したりする。 
- グループ所有者の一覧から、特定のグループの所有者責任に参加しなくなった[所有者を削除する](../api-reference/v1.0/api/group_delete_owners.md)。 
 
### <a name="establish-and-maintain-group-policy-settings"></a>グループ ポリシーの設定値を確立して維持する 
 
1 つの組織内で作成されるグループの数が増えてきた場合、Microsoft Graph では、グループの使用状況やライフサイクルを管理するための機能がサポートされています。 組織内のすべてのグループを通じて、グループ ポリシーを適用することができます。 Microsoft Graph API を使用することにより、次のことを実行できます:

- 幅広い範囲の[グループ ポリシー設定値](../api-reference/v1.0/resources/groupsetting.md)を構成する。これは、所有者によって更新されるのでない限りグループを自動削除したり、Office 365 グループに対して名前付けポリシーを適用したりするなどの動作を定義するのに役立ちます。 
- 期限切れの近いグループを[更新](../api-reference/v1.0/api/group_renew.md)することにより、チームのメンバーが、共同作業でコンテンツにアクセスし続けられるようにする。 確立されている期限切れポリシーに従ってグループが更新されない場合、そのグループは自動的に削除されます。 
- 削除されたグループを[復元する](../api-reference/v1.0/api/directory_deleteditems_restore.md)。
 
## <a name="next-steps"></a>次の手順

- [Graph Explorer](https://developer.microsoft.com/ja-JP/graph/graph-explorer) で、サンプル API リクエストを試す。 
- Microsoft Graph で[グループ API を使用する](../api-reference/v1.0/resources/groups-overview.md)方法に関する詳細を確認する。
