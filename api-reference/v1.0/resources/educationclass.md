# <a name="educationclass-resource-type"></a>educationClass リソース タイプ

学校内のクラスを表します。 **educationClass** リソースは Office 365 グループに相当し、同じ ID を共有します。 学生はクラスの通常のメンバーであり、教師は所有者であり適切な権限を持ちます。 Office の操作性が適切に機能するために、教師は、teachers コレクションと members コレクションの両方のメンバーになっている必要があります。  


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[educationClass を取得
](../api/educationclass_get.md) | [educationClass](educationclass.md) |**educationClass** オブジェクトのプロパティとリレーションシップを読み取ります。|
|[メンバーを追加する](../api/educationclass_post_members.md) |[educationUser](educationuser.md)| members ナビゲーション プロパティに投稿することで、クラスの新しい **educationUser** を追加します。|
|[メンバーをリストする](../api/educationclass_list_members.md) |[educationUser](educationuser.md) コレクション| **educationUser** オブジェクト コレクションを取得します。|
|[学生を削除する](../api/educationclass_delete_members.md) |[educationUser](educationuser.md)| members ナビゲーション プロパティによって、クラスから **educationUser** を削除します。|
|[学校をリスト](../api/educationclass_list_schools.md) |[educationSchool](educationschool.md) コレクション| **educationSchool** オブジェクト コレクションを取得します。|
|[教師の追加](../api/educationclass_post_teachers.md) |[educationUser](educationuser.md)| teachers ナビゲーション プロパティに投稿することで、クラスの新しい **educationUser** を追加します。|
|[教師をリスト](../api/educationclass_list_teachers.md) |[educationUser](educationuser.md) コレクション| クラスの教師一覧を取得します。|
|[教師を削除](../api/educationclass_delete_teachers.md) |[educationUser](educationuser.md)| teachers ナビゲーション プロパティによって、クラスから **educationUser** を削除します。|
|[グループを取得](../api/educationclass_get_group.md) |[group](group.md)| この **educationClass** に対応する Office 365 **group**を取得します。|
|[更新](../api/educationclass_update.md) | [educationClass](educationclass.md)    |**educationClass** オブジェクトを更新します。 |
|[削除](../api/educationclass_delete.md) | なし |**educationClass** オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | タイプ   |説明|
|:---------------|:--------|:----------|
|id| 文字列| クラスの一意の識別子。|
|説明|文字列| クラスの説明。|
|displayName|文字列| クラスの名前。|
|mailNickname|文字列| すべてのメンバーに電子メールを送信する際のメール名 (この機能が有効な場合)。 |
|createdBy|[identitySet](identityset.md)| クラスを作成したエンティティ。 |
|classCode|文字列| クラスを識別するために学校が使用するクラス コード。|
|externalId|文字列| 同期システムからのクラスの ID。 |
|externalName|文字列|同期システムからのクラスの名前。|
|externalSource|educationExternalSource| このクラスの作成方法。 可能な値は、 `sis`、`manual`、`unknownFutureValue` です。|
|term|[educationTerm](educationterm.md)|このクラスの学期。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|members|[educationUser](../resources/educationuser.md) コレクション| クラスのすべてのユーザー。 Null 許容型。|
|schools|[educationSchool](../resources/educationschool.md) コレクション| このクラスに関連付けられているすべての学校。 Null 許容型。|
|teachers|[educationUser](../resources/educationuser.md) コレクション|  このクラスのすべての教師。 Null 許容型。|
|group|[group](../resources/group.md)| このクラスに対応するディレクトリのグループです。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.educationClass"
}-->

```json
{
  "id": "String",
  "description": "String",
  "classCode": "String",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "displayName": "String",
  "externalId": "String",
  "externalName": "String",
  "externalSource": "string",
  "mailNickname": "String",
  "term": {"@odata.type": "microsoft.graph.educationTerm"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationClass resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
