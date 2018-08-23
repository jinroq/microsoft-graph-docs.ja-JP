# <a name="use-the-planner-rest-api"></a>Planner REST API を使用する

Microsoft Graph の Planner API を使用して、タスクを作成して Office 365 のグループ内のユーザーに割り当てることができます。

Planner API の使用を開始する前に、主要なオブジェクトの Office 365 のグループとの関係と同様に、それらの相互関係を理解しておくとよいでしょう。

## <a name="groups"></a>グループ

Office 365 のグループは、Planner API のプランの所有者です。
 [グループが所有しているプランを取得する](../api/plannergroup_list_plans.md) には、次の HTTP 要求を行います。

``` http
GET /groups/{id}/planner/plans
```

[新しいプランを作成する](../api/planner_post_plans.md) 場合は、プランのオブジェクトの `owner` プロパティを設定してグループを所有者にしてください。 プランは、グループが所有する必要があります。

>**注意:** プランを作成しているユーザーは、プランを所有するグループのメンバーである必要があります。 [グループの作成](../api/group_post_groups.md) を使用して新しいグループを作成する場合は、メンバーとしてグループに追加されません。 グループが作成されたら、[グループ ポスト メンバー](../api/group_post_members.md) を使用してご自分をメンバーとして追加します。

## <a name="plans"></a>プラン

[プラン](plannerplan.md) は、[タスク](plannertask.md) のコンテナーです。  [プランにタスクを作成](../api/planner_post_tasks.md) するには、タスクの作成中にタスク オブジェクトの `planId` プロパティをプランの ID に設定します。
現在、タスクはプランなしでは作成できません。
 [プラン内のタスクを取得](../api/plannerplan_list_tasks.md)するには、次の HTTP 要求を確認します。

``` http
GET /planner/plans/{id}/tasks
```

## <a name="tasks"></a>タスク

各タスクは、タスク オブジェクトの [assignments](plannerassignments.md) プロパティに [assignment](plannerassignment.md) を追加することにより、ユーザーに割り当てることができます。タスクを割り当てるユーザーの ID は `assignments` の open プロパティの名前であり、assignment の `orderHint` プロパティを指定する必要があります。

## <a name="task-and-plan-details"></a>タスクとプランの詳細 

Planner のリソースは、基本オブジェクトと詳細オブジェクトに配置されます。基本オブジェクトは、リスト ビューに適したリソースの共通プロパティへのアクセスを提供し、詳細オブジェクトは、ドリル ダウン ビューに適したリソースの大規模なプロパティへのアクセスを提供します。

## <a name="visualization"></a>視覚化

Planner API は、タスクとプランのデータのほかに、データの共通した視覚化をクライアント全体に提供するためのリソースも提供します。タスクには、いくつかの種類のデータの視覚化が利用できます。

| タスクの表示                                                                        | タスクを順序付ける情報の情報源                                         |
| :---------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------ |
| フラット リスト (プラン内のタスク)                                                               | `orderHint` タスクのプロパティ                                                   |
| フラット リスト (ユーザーに割り当てられたタスク)                                                      | `assigneePriority` タスクのプロパティ                                            |
| 割り当て先の列を含むボード ビュー (タスク ボードに割り当て)                            | [assignedToTaskBoardTaskFormat](plannerassignedToTaskBoardTaskFormat.md) オブジェクト |
| タスク完了までの進行状況を示す列を含むボード ビュー (進行状況タスク ボード) | [progressTaskBoardTaskFormat](plannerprogressTaskBoardTaskFormat.md) オブジェクト     |
| タスクのカスタム列を含むボード ビュー (バケット タスク ボード)                              | [bucketTaskBoardTaskFormat](plannerbucketTaskBoardTaskFormat.md) オブジェクト         |

|||UNTRANSLATED_CONTENT_START|||The custom columns in the bucket task board are represented by [bucket](plannerbucket.md) objects, and their order by `orderHint` property on the object.|||UNTRANSLATED_CONTENT_END|||

すべての順序は、[Planner の順序のヒント](planner_order_hint_format.md) に定められた原則によって制御されます。

## <a name="planner-resource-versioning"></a>Planner のリソース バージョン管理

Planner は Etag を使ってすべてのリソースをバージョン管理します。これらの Etag は各リソースで `@odata.etag` プロパティを指定して返されます。`PATCH` および `DELETE` 要求では、クライアントが知っている最新の Etag を `If-Match` ヘッダーで指定する必要があります。目的の変更が同じリソース上の Planner サービスによって受け入れられた新しい変更と競合しない場合、Planner は古いバージョンのリソースに変更を加えることができます。クライアントは、どの Etag 値が大きいかを序数の文字列比較で計算することによって、同じリソースで新しい Etag を識別できます。各リソースには個別の Etag があります。異なるリソースの Etag 値は比較できません (包含関係のあるものを含む)。クライアント アプリケーションは、アイテムの最新バージョンを読み取り、競合する変更を解決することにより、2 つのバージョン管理に関連するエラー ステータス コード 409 と 412 を処理することが予想されます。

## <a name="common-planner-error-conditions"></a>一般的な Planner のエラー条件

Microsoft Graph に適用される [一般的なエラー](../../../concepts/errors.md) のほかに、Planner API に固有のエラー条件もあります。

### <a name="400-bad-request"></a>400 要求が不適切です

`POST` および `PATCH` 要求で 400 ステータス コードを取得できる一般的なケースがいくつかあります。一般的な問題がは次のとおりです。

* Open Type プロパティが正しい型でないか、型が指定されていないか、またはプロパティが含まれていません。たとえば、複雑な値が指定された [plannerAssignments](plannerAssignments.md) プロパティは、値 `microsoft.graph.plannerAssignment` を指定した `@odata.type` プロパティで宣言する必要があります。
* ORDER ヒントの値が[正しい書式](planner_order_hint_format.md)になっていません。たとえば、ORDER ヒントの値は、クライアントに返される値に直接設定されています。
* データが論理的に矛盾しています。たとえば、タスクの開始日がタスクの期日よりも後になる場合などです。

### <a name="403-forbidden"></a>403 アクセスは許可されていません

Planner API では、一般的なエラーのほかに、サービスで定義された制限を超えた場合にもこのステータスコードを返します。この場合、エラー リソースの種類の `code` プロパティは、要求が超過した制限の種類を示します。制限の種類の有効な値は次のとおりです。

| 値                         | 説明                                                                                                                                                                                              |
| :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| MaximumProjectsOwnedByUser    | グループが所有するプランの最大数の制限を超過しています。この制限は、[plannerPlan](plannerPlan.md) リソースの `owner` プロパティに基づいています。                                         |
| MaximumProjectsSharedWithUser | ユーザーが共有するプランの最大数の制限を超過しています。この制限は、[plannerPlanDetails](plannerPlanDetails.md) リソースの `sharedWith` プロパティに基づいています。                   |
| MaximumTasksCreatedByUser     | ユーザーが作成するタスクの最大数の制限を超過しています。この制限は、[plannerTask](plannerTask.md) リソースの `createdBy` プロパティに基づいています。                                    |
| MaximumTasksAssignedToUser    | ユーザーに割り当てられるタスクの最大数の制限を超過しています。この制限は、[plannerTask](plannerTask.md) リソースの `assignments` プロパティに基づいています。                                 |
| MaximumTasksInProject         | プランにおけるタスクの最大数の制限を超過しています。この制限は、[plannerTask](plannerTask.md) リソースの `planId` プロパティに基づいています。                                               |
| MaximumActiveTasksInProject   | プランで完了されないタスクの最大数の制限を超過しています。この制限は、[plannerTask](plannerTask.md) リソースの `planId` および `percentComplete` プロパティに基づいています。 |
| MaximumBucketsInProject       | プランにおけるバケットの最大数の制限を超過しています。この制限は、[plannerBucket](plannerBucket.md) リソースの `planId` プロパティに基づいています。                                         |
| MaximumUsersSharedWithProject | [plannerPlanDetails](plannerPlanDetails.md) リソースの `sharedWith` プロパティに含まれる値が多すぎます。                                                                                          |
| MaximumReferencesOnTask       | [plannerTaskDetails](plannerTaskDetails.md) リソースの `references` プロパティに含まれる値が多すぎます。                                                                                          |
| MaximumChecklistItemsOnTask   | [plannerTaskDetails](plannerTaskDetails.md) リソースの `checklist` プロパティに含まれる値が多すぎます。                                                                                           |
| MaximumAssigneesInTasks       | [plannerTask](plannerTask.md) リソースの `assignments` プロパティに含まれる値が多すぎます。                                                                                                       |

### <a name="412-precondition-failed"></a>412 前提条件が失敗しました 

Planner API のすべての `POST`、`PATCH` および `DELETE` 要求には、要求の対象となるリソースと思われる最新の Etag 値で `If-Match` ヘッダーを指定する必要があります。さらに、要求に指定された Etag 値がサービス内のリソースのバージョンと一致しなくなった場合は、412 ステータス コードが返されます。この場合、クライアントはリソースを再度読み込んで、新しい Etag を取得する必要があります。

