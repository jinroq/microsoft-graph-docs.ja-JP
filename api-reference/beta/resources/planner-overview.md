---
title: Planner REST APIを使用する
description: Microsoft GraphのPlanner APIを使用してタスクを作成し、それらをOffice 365のグループ内のユーザーに割り当てることができます。
author: TarkanSevilmis
localization_priority: Priority
ms.prod: planner
ms.openlocfilehash: 29fdbe5403292638e8b6067a5e8b81d8e1bef250
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344617"
---
# <a name="use-the-planner-rest-api"></a>Planner REST APIを使用する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft GraphのPlanner APIを使用してタスクを作成し、それらをOffice 365のグループ内のユーザーに割り当てることができます。

Planner APIを使い始める前に、メインオブジェクト同士や、Office 365グループとの関係について理解しておく必要があります。

## <a name="office-365-groups"></a>Office 365 グループ

Office 365 のグループは、Planner API のプランの所有者です。
[グループが所有するプランを取得する](../api/plannergroup-list-plans.md)には、次に示す HTTP 要求を行います。

``` http
GET /groups/{id}/planner/plans
```

[新しいプランを作成する](../api/planner-post-plans.md)場合は、プラン オブジェクトに `owner` プロパティを設定することで、グループを所有者にできます。 プランはグループによって所有される必要があります。

>**注意:** プランを作成するユーザーは、プランを所有するグループのメンバーである必要があります。 あなたが新しいグループを[グループの作成](../api/group-post-groups.md)を使用して作成しても、メンバーとしてそのグループに追加されることはありません。 グループを作成したら、[グループ投稿メンバー](../api/group-post-members.md)を使用して自分自身をメンバーとして追加します。

## <a name="plans"></a>プラン

[プラン](plannerplan.md)は[タスク](plannertask.md)のコンテナーです。 [プランのタスクを作成する](../api/planner-post-tasks.md)には、タスクの作成時にタスク オブジェクトの `planId` プロパティをプランの ID に設定します。
現在、プランなしでタスクを作成することはできません。
[プラン内のタスクを取得する](../api/plannerplan-list-tasks.md)には、次のHTTPリクエストを行います。

``` http
GET /planner/plans/{id}/tasks
```

## <a name="tasks"></a>タスク

各タスクは、タスク オブジェクトの [assignments](plannerassignments.md) プロパティに [assignment](plannerassignment.md) を追加することにより、ユーザーに割り当てることができます。
タスクを割り当てるユーザーの ID は `assignments` の open プロパティの名前であり、assignment の `orderHint` プロパティを指定する必要があります。

## <a name="task-and-plan-details"></a>タスクとプランの詳細 

Planner のリソースは、基本オブジェクトと詳細オブジェクトに配置されます。 基本オブジェクトは、リスト ビューに適したリソースの共通プロパティへのアクセスを提供し、詳細オブジェクトは、ドリル ダウン ビューに適したリソースの大規模なプロパティへのアクセスを提供します。

## <a name="visualization"></a>視覚化

Planner API は、タスクとプランのデータのほかに、データの共通した視覚化をクライアント全体に提供するためのリソースも提供します。 次の表にリストされているように、タスクにはいくつかの種類の視覚化データがあります。

| タスクの表示                                                                        | タスクを順序付ける情報の情報源                                         |
| :---------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------ |
| フラット リスト (プラン内のタスク)                                                               | タスクの `orderHint` プロパティ                                                   |
| フラット リスト (ユーザーに割り当てられたタスク)                                                      | タスクの `assigneePriority` プロパティ                                            |
| 割り当て先の列を含むボード ビュー (タスク ボードに割り当て)                            | [assignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md) オブジェクト |
| タスクの進行状況を示す列を含むボード ビュー (進行状況タスク ボード) | [progressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md)オブジェクト     |
| タスクのカスタム列を含むボード ビュー (バケット タスク ボード)                              | [bucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md) オブジェクト         |

バケット タスク ボードのカスタム列は [bucket](plannerbucket.md) オブジェクトで表され、その順序はオブジェクトの `orderHint` プロパティによって表されます。

すべての順序は、[Planner の順序のヒント](planner-order-hint-format.md)に書かれた原則によって制御されます。

## <a name="delta">デルタクエリを使用して変更を追跡する</a>

Plannerのデルタクエリは、ユーザがサブスクライブしているオブジェクトのクエリをサポートします。

ユーザーは以下のオブジェクトをサブスクライブしています。

| Planner リソースの種類 | サブスクライブしているインスタンス                                                                                                                                                                                    |
| :-------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| タスク                 | <ul><li>ユーザーによって作成</li><li>ユーザーに割り当て済</li><li>ユーザーが所有しているプランに属しています。</li><li>planの**SharedWith**コレクションを通じてユーザーと共有されているplanに含まれています</li> |
| プラン                 | <ul><li>planの**SharedWith**コレクションを通じてユーザーと共有されています</li></ul>                                                                                                                     |
| バケット               | <ul><li>planの**SharedWith**コレクションを通じてユーザーと共有されているplanに含まれています</li></ul>                                                                                                 |  |

### <a name="objectcache">デルタクエリ用にオブジェクトキャッシュを生成する</a>

PlannerデルタクエリAPIを使用したい場合は、デルタ応答フィードからの変更を適用するために、ユーザーが観察したいオブジェクトのローカル・キャッシュを維持してください。

Plannerデルタクエリが現在返すことができるデルタペイロードオブジェクトは、次のタイプになります。

* [plannerTask](plannertask.md)
* [plannerTaskDetails](plannertaskdetails.md)
* [plannerPlan](plannerplan.md)
* [plannerPlanDetails](plannerplandetails.md)
* [plannerBucket](plannerbucket.md)
* [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)
* [plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)
* [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)

リソース上の対応する`GET`メソッドを使用して、ローカルキャッシュに移入するオブジェクトの初期状態を取得します。

### <a name="differentiating-between-object-creation-and-object-modification"></a>オブジェクトの作成とオブジェクトの変更の違い

特定のシナリオでは、呼び出し側は、Plannerのデルタクエリフィード内でオブジェクトの作成とオブジェクトの変更を区別したい場合があります。

これらのガイドラインは、オブジェクト作成を推測するために使用できます。

* `createdBy`プロパティは、新しく作成されたオブジェクトにのみ表示されます。
* 新しく作成された `plannerTask`オブジェクトには、それに対応する `plannerTaskDetails`オブジェクトが続きます。
* 新しく作成された `plannerPlan`オブジェクトには、それに対応する `plannerPlanDetails`オブジェクトが続きます。

### <a name="usage"></a>使用方法

呼び出し元は、サブスクライブしているオブジェクトが含まれるキャッシュを持っている必要があります。 サブスクライブされたオブジェクトのローカルキャッシュを埋める方法の詳細については、[デルタクエリ用にオブジェクトキャッシュを生成する](#populate-the-object-cache-for-delta-queries)を参照してください。

Plannerのデルタクエリコールフローは次のとおりです。

1. 呼び出し側がデルタ同期照会を開始し、`nextLink`と空の変更コレクションを取得します。
2. 呼び出し側はユーザーがサブスクライブしているオブジェクトを使用して、[差分キャッシュのオブジェクトキャッシュにデータを入力し](#populate-the-object-cache-for-delta-queries) そのキャッシュを更新する必要があります。
3. 呼び出し側は、最初のデルタ同期照会で提供された`nextLink`の内容に従って前のステップ以降に行われた`deltaLink`新しい変更を取得します 。
4. 呼び出し側は、返されたデルタレスポンスの変更をキャッシュ内のオブジェクトに適用します。
5. 呼び出し側は新しいdeltaLinkをたどって現在の `deltaLink`生成後の次のdeltaLinkと変更を取得します。
6. 呼び出し側は変更があればそれを適用して、前のステップとこのステップを再実行する前に少し待ちます。

## <a name="planner-resource-versioning"></a>Planner のリソースのバージョン管理

Plannerはすべてのリソースを **etags**を使ってバージョン管理します。 これらの**etags**は各リソースの`@odata.etag`プロパティとともに返されます 。 `PATCH`と`DELETE` リクエストは、クライアントが知っている最後の**etag**を`If-Match`ヘッダで指定することを要求します。
目的の変更が同じリソース上の Planner サービスによって受け入れられた新しい変更と競合しない場合、Planner は古いバージョンのリソースに変更を加えることができます。 クライアントは、**etag**順序文字列の比較でどの値が大きいかを計算することによって、同じリソースのどの**etag**がより新しいかを識別できます 。 各リソースには固有の **etag**があります。 異なるリソースの Etag 値は比較できません (包含関係のあるものを含む)。
クライアントアプリは、アイテムの最新バージョンを読み取り、競合する変更を解決することで、バージョニング関連の[エラーコード](/graph/errors) **409** および**412**を処理することが期待されています。

## <a name="common-planner-error-conditions"></a>一般的な Planner のエラー条件

Microsoft Graph に適用される[一般的なエラー](/graph/errors)のほかに、Planner API に固有のエラー条件もあります。

### <a name="400-bad-request"></a>400 要求が正しくありません

いくつかの一般的なシナリオでは、`POST` and `PATCH` リクエストは400ステータスコードを返す可能性があります。 以下は、よくある原因の一部です。

* Open Type プロパティが正しい型でないか、型が指定されていないか、またはプロパティが含まれていません。 たとえば、複雑な値が指定された [plannerAssignments](plannerassignments.md) プロパティは、値 `microsoft.graph.plannerAssignment` を指定した `@odata.type` プロパティで宣言する必要があります。
* ORDER ヒントの値が[正しい書式](planner-order-hint-format.md)になっていません。 たとえば、ORDER ヒントの値は、クライアントに返される値に直接設定されています。
* データが論理的に矛盾しています。 たとえば、タスクの開始日がタスクの期日よりも後になる場合などです。

### <a name="403-forbidden"></a>403 Forbidden

Planner API では、一般的なエラーのほかに、サービスで定義された制限を超えた場合にも403 ステータスコードを返します。 この場合、エラー リソースの種類の `code` プロパティは、要求が超過した制限の種類を示します。
以下は、制限タイプに有効な値です。

| 値                         | 説明                                                                                                                                                                                              |
| :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| MaximumProjectsOwnedByUser    | グループが所有するプランの最大数の制限を超過しています。 この制限は、[plannerPlan](plannerplan.md) リソースの `owner` プロパティに基づいています。                                         |
| MaximumProjectsSharedWithUser | ユーザーが共有するプランの最大数の制限を超過しています。  この制限は、[plannerPlanDetails](plannerplandetails.md) リソースの `sharedWith` プロパティに基づいています。                   |
| MaximumTasksCreatedByUser     | ユーザーが作成するタスクの最大数の制限を超過しています。 この制限は、[plannerTask](plannertask.md) リソースの `createdBy` プロパティに基づいています。                                    |
| MaximumTasksAssignedToUser    | ユーザーに割り当てられるタスクの最大数の制限を超過しています。 この制限は、[plannerTask](plannertask.md) リソースの `assignments` プロパティに基づいています。                                 |
| MaximumTasksInProject         | プランにおけるタスクの最大数の制限を超過しています。 この制限は、[plannerTask](plannertask.md) リソースの `planId` プロパティに基づいています。                                               |
| MaximumActiveTasksInProject   | プランで完了されないタスクの最大数の制限を超過しています。 この制限は、[plannerTask](plannertask.md) リソースの `planId` および `percentComplete` プロパティに基づいています。 |
| MaximumBucketsInProject       | プランにおけるバケットの最大数の制限を超過しています。 この制限は、[plannerBucket](plannerbucket.md) リソースの `planId` プロパティに基づいています。                                         |
| MaximumUsersSharedWithProject | [plannerPlanDetails](plannerplandetails.md) リソースの `sharedWith` プロパティに含まれる値が多すぎます。                                                                                          |
| MaximumReferencesOnTask       | [plannerTaskDetails](plannertaskdetails.md) リソースの `references` プロパティに含まれる値が多すぎます。                                                                                          |
| MaximumChecklistItemsOnTask   | [plannerTaskDetails](plannertaskdetails.md) リソースの `checklist` プロパティに含まれる値が多すぎます。                                                                                           |
| MaximumAssigneesInTasks       | [plannerTask](plannertask.md) リソースの `assignments` プロパティに含まれる値が多すぎます。                                                                                                       |
| MaximumFavoritePlansForUser   | [plannerUser](planneruser.md)リソースの`favoritePlanReferences` プロパティに含まれる値が多すぎます。                                                                                            |
| MaximumRecentPlansForUser     | [plannerUser](planneruser.md)リソースの`recentPlanReferences` プロパティに含まれる値が多すぎます。                                                                                              |
| MaximumContextsOnPlan         | [plannerPlan](plannerplan.md)リソースの`contexts` プロパティに含まれる値が多すぎます。                                                                                                          |
| MaximumPlannerPlans       | このグループには、プランが既に含まれています。 現時点では、グループは 1 つのプランのみ含めることができます。 **注意:** いくつかの Microsoft アプリは、この制限を超えることができます。 将来、すべてのアプリケーションにこの機能を拡張します。                                                                                                      |

### <a name="412-precondition-failed"></a>412 前提条件が失敗しました 

Planner API のすべての `POST`、`PATCH` および `DELETE` 要求には、要求の対象となるリソースと思われる最新の etag 値で `If-Match` ヘッダーを指定する必要があります。
さらに、要求に指定された etag 値がサービス内のリソースのバージョンと一致しなくなった場合は、412 ステータス コードが返されます。 この場合、クライアントはリソースを再度読み込んで、新しい etag を取得する必要があります。

