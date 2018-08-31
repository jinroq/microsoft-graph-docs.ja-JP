# <a name="educationstudent-resource-type"></a>educationStudent リソースの種類

ユーザーの primaryRole が `student` の場合に存在する [educationUser](educationuser.md) に追加される、その他の情報。

## <a name="properties"></a>プロパティ
| プロパティ     | タイプ   |説明|
|:---------------|:--------|:----------|
|birthDate|日付| 学生の生年月日。|
|externalId|文字列| ソース システムの学生の ID。|
|性別|educationGender| 指定できる値は、`female`、`male`、`other`、`unknownFutureValue` です。|
|成績|文字列|学生の現在の学年。|
|graduationYear|文字列| 学生が学校から卒業する年。|
|studentNumber|文字列| 学生番号。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationStudent"
}-->

```json
{
  "birthDate": "String (timestamp)",
  "externalId": "String",
  "gender": "educationGender",
  "grade": "String",
  "graduationYear": "String",
  "studentNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationStudent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
