# <a name="recurrencepattern-resource-type"></a>recurrencePattern リソースの種類

定期的な[イベント](event.md)を繰り返す頻度について説明します。 

シナリオに応じて、定期的なイベントの 6 通りの繰り返しパターンのいずれかを指定できます。 パターンの種類ごとに、次のイベント発生までの期間を指定します。 イベントに対して指定した期間内に発生する定期的なイベントは、必ずこのパターンに従って発生します。 定期的なイベントは常に、**recurrencePattern** (イベントを繰り返す頻度)、および [recurrenceRange](recurrencerange.md) (イベントを繰り返す期間) によって定義されます。

**type** プロパティを使用して **recurrencePattern** のさまざまな種類からパターンを指定し、**interval** プロパティを使用してイベント発生までの期間を指定します。**type** によって、その期間は数日、数週間、数か月、数年になる可能性があります。 種類ごとに必要なプロパティについては、次の表の説明を参照してください。

> **注** 定期的なパターンに必要なプロパティのみを含めます。 含めたプロパティにサポートされている値がない場合、エラーになる可能性があります。

| 定期的なパターンの種類 | type プロパティの値 | 説明 | 例 | 必須のプロパティ |
|:---------------|:--------|:--------|:--------|:----------|
| Daily (日単位) | `daily` | **interval** で指定された、次のイベント発生までの日数に基づいて、イベントが繰り返されます。 | イベントを 3 日ごとに繰り返します。 | **type**、**interval** |
| Weekly (週単位) | `weekly` | 次の一連のイベント発生までの週数に基づいて、同じ曜日 (複数の曜日も可) にイベントが繰り返されます。 | イベントを隔週の月曜日と火曜日に繰り返します。 | **type**、**interval**、**daysOfWeek**、**firstDayOfWeek** |
| 絶対月 | `absoluteMonthly` | 次のイベント発生までの月数に基づいて、該当月の指定日 (例: 15 日) にイベントが繰り返されます。 | 四半期 (3 か月ごと) の 15 日にイベントを繰り返します。 | **type**、**interval**、**dayOfMonth** |
| 相対月 | `relativeMonthly` | 次のイベント発生までの月数に基づいて、該当月の同じ相対位置にある指定した曜日 (複数の曜日も可) にイベントが繰り返されます。 | 3 か月ごとに、第 2 木曜日または金曜日にイベントを繰り返します。 | **type**、**interval**、**daysOfWeek** |
| 絶対年 | `absoluteYearly` | 次のイベント発生までの年数に基づいて、指定した日付にイベントが繰り返されます。 | 3 年ごとに、3 月 15 日にイベントを繰り返します。 | **type**、**interval**、**dayOfMonth**、**month** |
| 相対年 | `relativeYearly` | 次のイベント発生までの年数に基づいて、該当年の特定の月の同じ相対位置にある指定した曜日 (複数の曜日も可) にイベントが繰り返されます。 | 3 年ごとに、11 月の第 2 木曜日または金曜日にイベントを繰り返します。 | **type**、**interval**、**daysOfWeek**、**month** |


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|dayOfMonth|Int32|イベントが発生する月の日付。 **type** が、`absoluteMonthly` または `absoluteYearly` の場合、必要です。 |
|daysOfWeek|String collection|イベントが発生する曜日のコレクションです。 使用可能な値は、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday` です。 <br>**type** が `relativeMonthly` または `relativeYearly` であり、**daysOfWeek** で 1 日以上を指定する場合、パターンを満たす最初の日にイベントが発生します。 <br> **type** が `weekly`、`relativeMonthly`、`relativeYearly` の場合、必要です。|
|firstDayOfWeek|String|週の最初の曜日。 使用可能な値は、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday` です。 既定値は `sunday` です。 **type** が `weekly` の場合、必要です。 |
|index|String|月の最初のインスタンスから数えて、**daysOfsWeek** で指定された許可日数のどのインスタンスでイベントが発生するか指定します。 使用可能な値は、`first`、`second`、`third`、`fourth`、`last` です。 既定値は `first` です。 オプションです。**type** が `relativeMonthly` か `relativeYearly` の場合、使用します。 |
|interval|Int32|次のイベント発生までの単位数。**type** によって、単位は、日、週、月、年などになります。 必須。 |
|month|Int32|イベントが発生する月。  これは、1 から 12 までの数字です。|
|type|String|定期的なパターンの種類は、`daily`、`weekly`、`absoluteMonthly`、`relativeMonthly`、`absoluteYearly`、`relativeYearly` です。 必須。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recurrencePattern"
}-->

```json
{
  "dayOfMonth": 1024,
  "daysOfWeek": ["String"],
  "firstDayOfWeek": "String",
  "index": "String",
  "interval": 1024,
  "month": 1024,
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recurrencePattern resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->