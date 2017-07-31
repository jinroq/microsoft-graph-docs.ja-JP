# <a name="add-custom-data-to-groups-using-schema-extensions"></a>スキーマ拡張機能を使用したグループへのカスタム データの追加 

*スキーマ拡張機能*の使用方法について、具体例を使って説明します。 

ここでは、企業向けトレーニングのコースや教材を製作する “Graph Learn” という名前の学習管理ソフトウェア会社で開発者として働いているとしましょう。充実した共同エクスペリエンスを備えた Office 365 グループは、オンライン コースの参加者および講師が指導するコースの参加者どちらに対しても、コース コンテンツを配信したりエクササイズの記録をとったりするのに最適なツールです。トレーニング コースのために使う Office 365 グループを、トレーニング コースとしてすぐに見分けがつくようにしておくと、他の開発者がグループを見つけやすくなり、学習コースに基づいて豊富なエクスペリエンスを構築するのに役立ちます。

このシナリオでは、以下の操作を行う方法を紹介します。

1. 利用可能なスキーマ拡張機能の定義を確認する
2. トレーニング コースの対象グループに適用されるスキーマ拡張機能の定義を登録する
3. 登録したスキーマ拡張機能の定義に基づいた拡張データで新しいグループを作成する
4. スキーマ拡張機能の定義に基づいて既存のグループのカスタム データを追加、更新または削除する
5. グループと拡張機能データを読み取る

>**注:**このトピックでは、**グループ** リソースでスキーマ拡張機能の値を作成し、読み取る方法について説明します (手順 3 から 5)。同じメソッドは、** administrativeUnit**、**デバイス**、**イベント**、**メッセージ**、**組織**、**投稿**、および **ユーザー** リソースの種類でもサポートされています。このため、これらのリソースのいずれかで、下にある要求例と同様の操作を実行できます。注: **administrativeUnit** はベータ版エンドポイントでのみ使用可能です。

## <a name="1-view-available-schema-extensions"></a>1.利用可能なスキーマ拡張機能を確認する
開発者は、まずアプリで再利用できるスキーマ拡張機能の定義が他にないか調べる必要があります。これは **schemaExtension** リソースをクエリすることによって可能です。  
次の例では、特定のスキーマ拡張機能を **id** でクエリします。

応答で返される拡張機能の**状態**値は **Available** であることに注意してください。これは、**targetTypes** プロパティのリソースへのアクセス許可を持つ任意のアプリが、拡張機能を使用でき、付加的な変更で拡張機能を更新できることを示しています。通常、この操作では、**状態**にかかわらず、指定されたフィルターに一致するすべてのスキーマ拡張機能が返されるため、使用する前に拡張機能の状態を必ず確認してください。


##### <a name="request"></a>要求
```http
GET https://graph.microsoft.com/v1.0/schemaExtensions?$filter=id eq 'graphlearn_test'
```
##### <a name="response"></a>応答
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 420
{
    "value": [
        {
            "id":"graphlearn_test",
            "description": "Yet another test schema",
            "targetTypes": [
                "User", "Group"
            ],
            "status": "Available",
            "owner": "24d3b144-21ae-4080-943f-7067b395b913",
            "properties": [
                {
                    "name": "testName",
                    "type": "String"
                }
            ]
        }
    ]
}
```
## <a name="2-register-a-schema-extension-definition-that-describes-a-training-course"></a>2.トレーニング コースについて説明するスキーマ拡張機能の定義を登録する
ニーズに*適した*スキーマ拡張機能が見つからない場合は、**グループ** リソースでトレーニング コースの新しい拡張機能の定義を作成し登録します。  

スキーマ拡張機能定義を作成する場合、**id** プロパティに文字列を指定する必要があります。これを実行するには、次の 2 つの方法があります。次の例は優先される方法を示しています。この方法では、ご使用のテナントで検証済みのバニティ ドメイン名 (`graphlearn.com`) を使用します。検証済みドメイン名 (`graphlearn`) とスキーマ拡張機能名 (`courses`) を連結し、連結後の文字列 `graphlearn_courses` を使用して **ID** を割り当てます。  

説明 (見つけやすくするため)、(この拡張機能が適用されるリソースを定義する) 対象の種類、およびスキーマを構成するカスタム プロパティも指定します。この例の場合、`courseId`、`courseName`、`courseType` のカスタム プロパティとその種類を指定します。

[要求で **ID** を割り当てる他の方法の例](../api-reference/v1.0/api/schemaextension_post_schemaextensions.md#request-2)を参照してください。この例で必要となるのは、スキーマ名の指定のみです。

スキーマ拡張機能を最初に作成するとき、その状態は **InDevelopment** であることに注意してください。拡張機能の開発中は、この状態を保持できます。その間、拡張機能を付加的な変更で更新したり、削除したりできるのは拡張機能を作成したアプリだけです。他のアプリで使用するために拡張機能を共有する準備ができたら、**status** を **Available** に設定します。

##### <a name="request"></a>要求
```http
POST https://graph.microsoft.com/v1.0/schemaExtensions
Content-type: application/json
{
    "id":"graphlearn_courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "properties": [
        {
            "name": "courseId",
            "type": "Integer"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```
##### <a name="response"></a>応答
```http
HTTP/1.1 201 Created
Content-Type: application/json
Content-length: 420
{
    "id": "graphlearn_course",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "status": "InDevelopment",
    "owner": "24d3b144-21ae-4080-943f-7067b395b913",
    "properties": [
        {
            "name": "courseId",
            "type": "Integer"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```

## <a name="3-create-a-new-group-with-extended-data"></a>3.拡張データを含む新しいグループを作成する 
_新しい_グループを作成し、登録したばかりの `graphlearn_courses` スキーマ拡張機能定義を使って、追加のデータでグループを拡張します。これは、**グループ** リソースへの標準的な ```POST``` と、要求本文で定義された追加の `graphlearn_courses` の複合型の拡張機能です。応答では、データ拡張機能を返しません。```GET``` 操作を使用して、名前により拡張機能を明示的に ```$select``` する必要があります。

##### <a name="request"></a>要求
```http
POST https://graph.microsoft.com/v1.0/groups
Content-type: application/json
{
    "displayName": "New Managers March 2017",
    "description": "New Managers training course for March 2017",
    "groupTypes": ["Unified"],
    "mailEnabled": true,
    "mailNickname": "newMan201703",
    "securityEnabled": false,
    "graphlearn_courses": {
        "courseId":"123",
        "courseName":"New Managers",
        "courseType":"Online"
    }
}
```
##### <a name="response"></a>応答
```http
HTTP/1.1 201 Created
Content-Type: application/json
Content-length: 420
{
    "id": "dfc8016f-db97-4c47-a582-49cb8f849355",
    "createdDateTime": "2017-02-09T00:17:05Z",
    "description": "New Managers training course for March 2017",
    "displayName": "New Managers March 2017",
    "groupTypes": [
        "Unified"
    ],
    "mail": "newMan201703@graphlearn.com",
    "mailEnabled": true,
    "mailNickname": "newMan201703",
    "securityEnabled": false,
    "theme": null,
    "visibility": "Public"
}
```

## <a name="4-add-update-or-remove-custom-data-in-an-existing-group"></a>4.既存のグループのカスタム データを追加、更新、または削除します。
```PATCH``` 要求の本文で定義した追加の `graphlearn_courses` の複合型の拡張機能を使って、カスタム データを拡張し、_既存_のグループ インスタンスに追加することができます。  

##### <a name="request"></a>要求
```http
PATCH https://graph.microsoft.com/v1.0/groups/dfc8016f-db97-4c47-a582-49cb8f849355
Content-type: application/json
Content-length: 230
{
    "graphlearn_courses":{
        "courseId":"123",
        "courseName":"New Managers",
        "courseType":"Online"
    }   
}
```
##### <a name="response"></a>応答
```http
HTTP/1.1 204 No Content
```

拡張機能データの値を更新する場合は、複合型拡張機能の全体を ```PATCH``` 要求の本文に置きます (既存のリソースにカスタム データを追加するのと同様)。

対応する拡張機能のプロパティを Null に設定することで、リソース インスタンスに追加されたカスタム データを削除できます。 

リソース インスタンスからスキーマ拡張機能を削除する場合、当該インスタンスの複合型拡張機能を Null に設定します。


## <a name="5-get-a-group-and-its-extension-data"></a>5.グループとその拡張機能データを取得する
拡張機能の名前や ID など特定の拡張機能のプロパティ値に一致する `$filter` を使用すると簡単にグループ (または複数のグループ) を検索できます。 

次に、`$select` を使って、拡張機能の名前を指定し (この場合は `graphlearn_courses`)、グループのカスタムデータを取得します。

次の例では、`graphlearn_courses` の拡張機能と `123` に一致する `courseId` のプロパティ値を有するグループを検索し、`graphlearn_courses` 拡張機能のグループのプロパティ、**displayName**、**ID**、**説明**、カスタム データを取得します。(実際のクエリでは、必要に応じて URL エンコードを行ってください。)

#### <a name="request"></a>要求

```http
GET https://graph.microsoft.com/v1.0/groups?$filter=graphlearn_courses/courseId eq ‘123’&$select=displayName,id,description,graphlearn_courses
```


##### <a name="response"></a>応答
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 326
{
  "value": [
    {
      "displayName": "New Managers March 2017",
      "id": "14429ae5-3e74-41a2-9fa8-028fbb984637",
      "description": "New Managers training course for March 2017",
      "graphlearn_courses": {
        "@odata.type": "#microsoft.graph.ComplexExtensionValue",
        "courseId":"123",
        "courseName":"New Managers",
        "courseType":"Online"
      }
    }
  ]
}
```

## <a name="see-also"></a>関連項目

- [拡張機能を使用してカスタム データをリソースに追加する](extensibility_overview.md)
- [オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)](extensibility_open_users.md)
- [Office 365 のドメイン](https://technet.microsoft.com/en-us/library/office-365-domains.aspx)
- [新しい Office 365 のドメインの追加および検証](http://office365support.ca/adding-and-verifying-a-domain-for-the-new-office-365/)
- [schemaExtension リソース タイプ](../api-reference/v1.0/resources/schemaextension.md)
- [schemaExtensions を一覧表示する](../api-reference/v1.0/api/schemaextension_list.md)
- [schemaExtension を作成する](../api-reference/v1.0/api/schemaextension_post_schemaextensions.md)
- [schemaExtension を取得する](../api-reference/v1.0/api/schemaextension_get.md)
- [schemaExtension を更新する](../api-reference/v1.0/api/schemaextension_update.md)
- [schemaExtension を削除する](../api-reference/v1.0/api/schemaextension_delete.md)
