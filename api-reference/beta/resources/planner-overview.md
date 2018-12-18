---
title: プランナーの REST API を使用します。
description: Graph でプランナーの API を使用するにはタスクを作成し、Office 365 で、グループ内のユーザーに割り当てます。
author: TarkanSevilmis
ms.openlocfilehash: a57bdce9c61046d05bc969ff69d31971a85cf537
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346740"
---
# <a name="use-the-planner-rest-api"></a>プランナーの REST API を使用します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

Graph でプランナーの API を使用するにはタスクを作成し、Office 365 で、グループ内のユーザーに割り当てます。

プランナーの API を使用して開始する前に互いにも Office 365 のグループを主なオブジェクトの関係を理解するおくと便利になります。

## <a name="office-365-groups"></a>Office 365 グループ

Office 365 のグループは、プランナーの API で、計画の所有者です。
[グループによって所有されているプランを取得する](../api/plannergroup-list-plans.md)には、次の HTTP 要求を確認します。

``` http
GET /groups/{id}/planner/plans
```

[新しい計画を作成する](../api/planner-post-plans.md)をグループにする、その所有者を設定することにより、 `owner` 、プラン オブジェクトのプロパティです。 プランは、グループが所有する必要があります。

>**注:** 計画を作成しているユーザーは、計画を所有するグループのメンバーである必要があります。 [グループの作成](../api/group-post-groups.md)を使用して新しいグループを作成するときにいない追加されますグループにメンバーとして。 グループが作成されると、自分自身を追加メンバーとして[グループのメンバーの投稿](../api/group-post-members.md)を使用しています。

## <a name="plans"></a>プラン

[計画](plannerplan.md)は、[タスク](plannertask.md)のコンテナーです。 [計画にタスクを作成](../api/planner-post-tasks.md)するには、設定、 `planId` 、タスクの作成中に計画の ID をタスク オブジェクトのプロパティです。
現在のタスクを計画しなくても作成できません。
[計画内のタスクを取得](../api/plannerplan-list-tasks.md)するには、次の HTTP 要求を確認します。

``` http
GET /planner/plans/{id}/tasks
```

## <a name="tasks"></a>タスク

各タスクは、タスク オブジェクトの [assignments](plannerassignments.md) プロパティに [assignment](plannerassignment.md) を追加することにより、ユーザーに割り当てることができます。タスクを割り当てるユーザーの ID は `assignments` の open プロパティの名前であり、assignment の `orderHint` プロパティを指定する必要があります。

## <a name="task-and-plan-details"></a>タスクとプランの詳細 

Planner のリソースは、基本オブジェクトと詳細オブジェクトに配置されます。基本オブジェクトは、リスト ビューに適したリソースの共通プロパティへのアクセスを提供し、詳細オブジェクトは、ドリル ダウン ビューに適したリソースの大規模なプロパティへのアクセスを提供します。

## <a name="visualization"></a>視覚化

作業および計画のデータは別にプランナー API はクライアント間でデータの一般的な視覚エフェクトを作成するためのリソースも備えています。 ビジュアル化データのいくつかの種類があるタスクについては、次の表に記載されています。

| タスクの表示                                                                        | タスクを順序付ける情報の情報源                                         |
| :---------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------ |
| フラット リスト (プラン内のタスク)                                                               | タスクの `orderHint` プロパティ                                                   |
| フラット リスト (ユーザーに割り当てられたタスク)                                                      | タスクの `assigneePriority` プロパティ                                            |
| 割り当て先の列を含むボード ビュー (タスク ボードに割り当て)                            | [assignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md) オブジェクト |
| タスクの進行状況を示す列を含むボード ビュー (進行状況タスク ボード) | [progressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md)オブジェクト     |
| タスクのカスタム列を含むボード ビュー (バケット タスク ボード)                              | [bucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md) オブジェクト         |

バケット タスク ボードのカスタム列は [bucket](plannerbucket.md) オブジェクトで表され、その順序はオブジェクトの `orderHint` プロパティによって表されます。

[プランナーの順序のヒント](planner-order-hint-format.md)で説明した原則には、すべての順序が制御されます。

## <a name="delta">デルタのクエリを使用して変更履歴の記録します。</a>

プランナーのデルタのクエリは、ユーザーが購読しているオブジェクトのクエリをサポートしています。

ユーザーは、次のオブジェクトを購読します。

| プランナーのリソースの種類 | 購読済みのインスタンス                                                                                                                                                                                    |
| :-------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| タスク                 | <ul><li>ユーザーによって作成されました。</li><li>ユーザーに割り当てられています。</li><li>ユーザーが所有する計画に属しています。</li><li>計画の**SharedWith**コレクションをユーザーと共有の計画に含まれています。</li> |
| プラン                 | <ul><li>計画の**SharedWith**コレクションをユーザーと共有</li></ul>                                                                                                                     |
| バケット               | <ul><li>計画の**SharedWith**コレクションをユーザーと共有の計画に含まれています。</li></ul>                                                                                                 |  |

### <a name="objectcache">デルタ ・ クエリのオブジェクト キャッシュを設定します。</a>

プランナーのデルタ ・ クエリ API を使用する場合は、デルタの応答フィードから変更を適用するために観察することで、ユーザーが興味を示しているオブジェクトのローカル キャッシュを保持します。

次の種類のプランナーのデルタ ・ クエリが返すことができる現在のデルタ ・ ペイロード オブジェクトになります。

* [plannerTask](plannertask.md)
* [plannerTaskDetails](plannertaskdetails.md)
* [plannerPlan](plannerplan.md)
* [plannerPlanDetails](plannerplandetails.md)
* [plannerBucket](plannerbucket.md)
* [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)
* [plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)
* [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)

使用して、対応する`GET`のリソースをローカルのキャッシュを格納するオブジェクトの初期状態を取得するメソッドです。

### <a name="differentiating-between-object-creation-and-object-modification"></a>オブジェクトの作成とオブジェクトの変更の違いを知る

特定のシナリオでは、呼び出し元がオブジェクトを作成し、フィードのプランナーのデルタのクエリ内のオブジェクトの変更を区別する必要があります。

これらのガイドラインを使用して、オブジェクトの作成を推論することができます。

* `createdBy`プロパティは、新しく作成されたオブジェクトにのみ表示されます。
* 新しく作成された A`plannerTask`オブジェクトに対応する、続いて`plannerTaskDetails`オブジェクトです。
* 新しく作成された A`plannerPlan`オブジェクトに対応する、続いて`plannerPlanDetails`オブジェクトです。

### <a name="usage"></a>使用方法

呼び出し元は、購読しているオブジェクトが含まれているキャッシュを持つと思われます。 購読しているオブジェクトのローカル キャッシュを設定する方法についての詳細は、[デルタのクエリでオブジェクト キャッシュの作成](#populate-the-object-cache-for-delta-queries)を参照してください。

プランナーのデルタのクエリの呼び出しのフローは次のとおりです。

1. デルタ同期クエリを開始する呼び出し元を取得する、`nextLink`と変更の空のコレクションです。
2. 呼び出し元する必要があります[デルタ クエリでオブジェクト キャッシュの設定](#populate-the-object-cache-for-delta-queries)とオブジェクトをユーザーが購読して、そのキャッシュを更新します。
3. 呼び出し元に依存して、 `nextLink` 、新しいを取得する最初のデルタ ・同期クエリで提供されている`deltaLink`前の手順の変更を反映します。
4. 呼び出し元に返されたデルタのキャッシュ内のオブジェクトに対して変更が適用されます。
5. 呼び出し元は、次の deltaLink を取得する新しい deltaLink に依存して、現在以降の変更`deltaLink`が生成されました。
6. 呼び出し元が (もしあれば) 変更が適用され、短時間を待機する前に実行する前にステップし、この手順です。

## <a name="planner-resource-versioning"></a>Planner のリソースのバージョン管理

プランナーのバージョンすべてのリソースの**etag**を使用します。 返されるこれらの**etag**が`@odata.etag`の各リソースのプロパティです。 `PATCH``DELETE`を使用して指定するのには既知のクライアントによって最後の**etag**を要求、`If-Match`ヘッダー。
プランナーは、目的の変更が新しい変更を受け入れ、プランナーのサービスで同じリソースと競合していない場合、古いバージョンのリソースへの変更を使用できます。 **Etag**値が大きい序数の文字列比較で計算することで同じリソースの**etag**のどちらの方が新しいクライアントを識別できます。 各リソースには、独自の**etag**があります。 包含関係では、ある方を含め、さまざまなリソースの Etag 値を比較することはできません。
クライアント アプリケーションは、バージョン管理を処理するために期待される関連[のエラー コード](/graph/errors) **409** 、 **412**項目の最新バージョンの読み取りと変更の競合を解決します。

## <a name="common-planner-error-conditions"></a>一般的な Planner のエラー条件

Microsoft Graph に適用される[一般的なエラー](/graph/errors)のほかに、Planner API に固有のエラー条件もあります。

### <a name="400-bad-request"></a>400 要求が正しくありません

いくつかの一般的なシナリオでは、`POST`と`PATCH`の要求は、400 のステータス コードを返すことができます。 以下は、いくつかの一般的な原因です。

* Open Type プロパティが正しい型でないか、型が指定されていないか、またはプロパティが含まれていません。たとえば、複雑な値が指定された [plannerAssignments](plannerassignments.md) プロパティは、値 `microsoft.graph.plannerAssignment` を指定した `@odata.type` プロパティで宣言する必要があります。
* ORDER ヒントの値が[正しい書式](planner-order-hint-format.md)になっていません。たとえば、ORDER ヒントの値は、クライアントに返される値に直接設定されています。
* データが論理的に矛盾しています。たとえば、タスクの開始日がタスクの期日よりも後になる場合などです。

### <a name="403-forbidden"></a>403 アクセスは許可されていません

一般的なエラーだけでなくプランナー API も 403 ステータス コードを返しますサービスで定義された制限を超えているとき。 この場合は、`code`エラーのリソースの種類のプロパティには、要求によって制限の種類が表示されます。
制限の種類の有効な値を次に示します。

| 値                         | 説明                                                                                                                                                                                              |
| :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| MaximumProjectsOwnedByUser    | グループが所有するプランの最大数の制限を超過しています。この制限は、[plannerPlan](plannerplan.md) リソースの `owner` プロパティに基づいています。                                         |
| MaximumProjectsSharedWithUser | ユーザーが共有するプランの最大数の制限を超過しています。この制限は、[plannerPlanDetails](plannerplandetails.md) リソースの `sharedWith` プロパティに基づいています。                   |
| MaximumTasksCreatedByUser     | ユーザーが作成するタスクの最大数の制限を超過しています。この制限は、[plannerTask](plannertask.md) リソースの `createdBy` プロパティに基づいています。                                    |
| MaximumTasksAssignedToUser    | ユーザーに割り当てられるタスクの最大数の制限を超過しています。この制限は、[plannerTask](plannertask.md) リソースの `assignments` プロパティに基づいています。                                 |
| MaximumTasksInProject         | プランにおけるタスクの最大数の制限を超過しています。この制限は、[plannerTask](plannertask.md) リソースの `planId` プロパティに基づいています。                                               |
| MaximumActiveTasksInProject   | プランで完了されないタスクの最大数の制限を超過しています。この制限は、[plannerTask](plannertask.md) リソースの `planId` および `percentComplete` プロパティに基づいています。 |
| MaximumBucketsInProject       | プランにおけるバケットの最大数の制限を超過しています。この制限は、[plannerBucket](plannerbucket.md) リソースの `planId` プロパティに基づいています。                                         |
| MaximumUsersSharedWithProject | [plannerPlanDetails](plannerplandetails.md) リソースの `sharedWith` プロパティに含まれる値が多すぎます。                                                                                          |
| MaximumReferencesOnTask       | [plannerTaskDetails](plannertaskdetails.md) リソースの `references` プロパティに含まれる値が多すぎます。                                                                                          |
| MaximumChecklistItemsOnTask   | [plannerTaskDetails](plannertaskdetails.md) リソースの `checklist` プロパティに含まれる値が多すぎます。                                                                                           |
| MaximumAssigneesInTasks       | [plannerTask](plannertask.md) リソースの `assignments` プロパティに含まれる値が多すぎます。                                                                                                       |
| MaximumFavoritePlansForUser   | `favoritePlanReferences` [PlannerUser](planneruser.md)リソースのプロパティに値が多すぎますが含まれています。                                                                                            |
| MaximumRecentPlansForUser     | `recentPlanReferences` [PlannerUser](planneruser.md)リソースのプロパティに値が多すぎますが含まれています。                                                                                              |
| MaximumContextsOnPlan         | `contexts` [PlannerPlan](plannerplan.md)リソースのプロパティに値が多すぎますが含まれています。                                                                                                          |
| MaximumPlannerPlans       | グループには、計画が既に含まれています。 現在、グループは 1 つの計画のみ含めることができます。 **注:** いくつかの Microsoft アプリケーションでは、この制限を超えることができます。 今後、すべてのアプリケーションにこの機能は拡張します。                                                                                                      |

### <a name="412-precondition-failed"></a>412 必須条件に失敗しました 

平面のすべての API `POST`、 `PATCH`、および`DELETE`要求を`If-Match`ヘッダーは、要求の対象となるリソースの最後の既知の etag 値を指定します。
412 のステータス コードは、要求で指定された etag 値には不要になったサービス内のリソースのバージョンが一致する場合にも返されます。 この例では、クライアントは、リソースの読み取りを再試行する必要があり、新しい etag を取得します。

