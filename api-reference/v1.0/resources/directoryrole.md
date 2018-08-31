# <a name="directoryrole-resource-type"></a>directoryRole リソース型

Azure AD ディレクトリ ロールを表します。Azure AD ディレクトリ ロールは、*管理者ロール*と呼ばれることもあります。ディレクトリ (管理者) ロールの詳細については、「[Azure Active Directory での管理者ロールの割り当て](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/)」を参照してください。Microsoft Graph では、ユーザーにディレクトリ ロールを割り当てることで、ターゲット ロールのアクセス許可をユーザーに付与できます。ディレクトリ ロールを読み取る場合や、そのメンバーを更新する場合は、まず、そのディレクトリ ロールをテナントでアクティブにする必要があります。既定では、会社の管理者 (Company Administrators) ディレクトリ ロールのみがアクティブ化されています。その他の使用可能なディレクトリ ロールをアクティブ化するには、[directoryRoleTemplate](directoryroletemplate.md) の ID を使用して POST 要求を送信します。この ID は、ディレクトリ ロールに基づきます。[directoryObject](directoryobject.md) から継承します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[directoryRole を取得](../api/directoryrole_get.md) | [directoryRole](directoryrole.md) | directoryRole オブジェクトのプロパティとリレーションシップを読み取ります。 |
|[directoryRoles を一覧表示する](../api/directoryrole_list.md) | [directoryRole](directoryrole.md) コレクション | テナントでアクティブになっているディレクトリ ロールを一覧表示します。 |
|[メンバーを追加する](../api/directoryrole_post_members.md) |[directoryObject](directoryobject.md)| members ナビゲーション プロパティを送信することで、ユーザーをディレクトリ ロールに追加します。|
|[メンバーをリストする](../api/directoryrole_list_members.md) |[directoryObject](directoryobject.md) コレクション| members ナビゲーション プロパティから、ディレクトリ ロールのメンバーであるユーザーを取得します。|
|[メンバーを削除する](../api/directoryrole_delete_member.md) |[directoryObject](directoryobject.md)| ディレクトリ ロールからユーザーを削除します。|
|[directoryRole をアクティブ化](../api/directoryrole_post_directoryroles.md) |[directoryRole](directoryrole.md) | ディレクトリ ロールをアクティブ化します。|

## <a name="properties"></a>プロパティ
| プロパティ   | タイプ | 説明 |
|:---------------|:--------|:----------|
|説明|文字列|ディレクトリ ロールの説明。読み取り専用。 |
|displayName|文字列|ディレクトリ ロールの表示名。読み取り専用。 |
|ID|文字列|ディレクトリ ロールの一意識別子。[directoryObject](directoryobject.md) から継承されます。キーであり、Null は許容されません。読み取り専用です。|
|roleTemplateId|文字列| このロールが基づいている [directoryRoleTemplate](directoryroletemplate.md) の **id**。このプロパティは、POST 操作でテナント内のディレクトリ ロールをアクティブ化するときに指定する必要があります。そのディレクトリ ロールがアクティブ化されると、このプロパティは読み取り専用になります。 |

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型 |説明|
|:---------------|:--------|:----------|
|メンバー|[directoryObject](directoryobject.md) コレクション|このディレクトリ ロールのメンバーであるユーザー。HTTP メソッド: GET、POST、DELETE。読み取り専用。Null 許容型。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "memberOf",
    "members",
    "ownedObjects",
    "owners"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.directoryRole",
  "@odata.annotations": [
    {
      "capabilities": {
        "toppable": false
      }
    }
  ]
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "roleTemplateId": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
