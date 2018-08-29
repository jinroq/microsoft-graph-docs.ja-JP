# <a name="plannerplandetails-resource-type"></a>plannerPlanDetails リソースの種類


**plannerPlanDetails** リソースは、計画に関する追加情報を表します。各 [plan](plannerplan.md) オブジェクトには詳細オブジェクトがあります。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[plannerPlanDetails を取得](../api/plannerplandetails_get.md) | [plannerPlanDetails](plannerplandetails.md) |**plannerPlanDetails** オブジェクトのプロパティとリレーションシップを読み取ります。|
|[更新する](../api/plannerplandetails_update.md) | [plannerPlanDetails](plannerplandetails.md)    |**plannerPlanDetails** オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | タイプ   |説明|
|:---------------|:--------|:----------|
|categoryDescriptions|[plannerCategoryDescriptions](plannercategorydescriptions.md)|計画内のタスクに関連付けられる 6 つのカテゴリの説明を指定するオブジェクト|
|ID|文字列| 読み取り専用。 計画の ID です。 28 文字で大文字小文字を区別します。 サービスの[フォーマットの検証](planner_identifiers_disclaimer.md) が行われます。|
|sharedWith|[plannerUserIds](planneruserids.md)|この計画を共有するユーザー ID を設定します。Office 365 グループを活用している場合は、グループの API を使用してグループのメンバーシップを管理し、[グループの](group.md)計画を共有します。グループの既存のメンバーもこのコレクションに追加できますが、このグループが所有する計画へのアクセスは必要とされません。 |

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerPlanDetails"
}-->

```json
{
  "categoryDescriptions": {"@odata.type": "microsoft.graph.plannerCategoryDescriptions"},
  "id": "String (identifier)",
  "sharedWith": {"@odata.type": "microsoft.graph.plannerUserIds"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->