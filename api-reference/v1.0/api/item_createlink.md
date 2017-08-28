# <a name="create-a-sharing-link-for-a-driveitem"></a>DriveItem の共有リンクを作成する

**createLink** アクションを使用して、共有リンクを使って [DriveItem](../resources/driveitem.md) を共有できます。

**createLink** アクションは、呼び出し元のアプリケーションに指定されたリンクの種類が存在しない場合に、新しい共有リンクを作成します。指定された種類の共有リンクがアプリで既に存在している場合、既存の共有リンクが返されます。

DriveItem リソースは、そのリソースの先祖からアクセス許可を継承します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | Files.ReadWrite、Files.ReadWrite.All    |
|アプリケーション | Files.ReadWrite.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{item-id}/createLink
POST /me/drive/root:/{item-path}:/createLink
POST /groups/{group-id}/drive/items/{item-id}/createLink
POST /drives/{drive-id}/items/{item-id}/createLink
```

## <a name="request-body"></a>要求本文
要求本文はアプリが検索する共有リンクの種類を定義します。要求は、次のプロパティを持つ JSON オブジェクトである必要があります。

| 名前      | 型   | 説明                                                                  |
|:----------|:-------|:-----------------------------------------------------------------------------|
| **type**  | string | 作成する共有リンクの種類。`view`、`edit`、または `embed` です。       |
| **scope** | string | 作成するリンクのスコープ。`anonymous` または `organization` です。省略可能。 |

## <a name="link-types"></a>リンクの種類
**type** パラメーターには次の値を使用できます。

| 種類の値 | 説明                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| `view`     | そのアイテムへの読み取り専用リンクを作成します。                                                        |
| `edit`     | そのアイテムへの読み取り/書き込みリンクを作成します。                                                       |
| `embed`    | そのアイテムへの埋め込み可能なリンクを作成します。このオプションは OneDrive 個人用でのみ選択可能です。 |

## <a name="scope-types"></a>スコープの種類
**scope** パラメーターには次の値を使用できます。このパラメーターは省略可能です。**scope** パラメーターを指定しない場合、最も制限の少ないリンクが作成されます。

| 種類の値     | 説明                                                                                                                   |
|:---------------|:------------------------------------------------------------------------------------------------------------------------------|
| `anonymous`    | そのアイテムへの、すべてのユーザーがアクセス可能なリンクを作成します。匿名リンクはテナント管理者により無効にされることがあります。                 |
| `organization` | そのアイテムへの、組織内でアクセス可能なリンクを作成します。組織のリンク スコープは、OneDrive 個人用では使用できません。 |

## <a name="response"></a>応答

正常に実行されると、このメソッドは要求された共有リンクのアクセス許可を表す応答本文で、単一の[アクセス許可](../resources/permission.md)リソースを返します。

サービスはまず、現在のアクセス許可を調べ、呼び出し元アプリケーションで同じ **型**を持つアクセス許可があるかどうかを確認します。

応答は、アイテムに新しい共有リンクが作成される場合は `201 Created`、既存のリンクが返される場合は `200 OK` となります。

## <a name="example"></a>例
以下は、この API を呼び出す方法の例です。

##### <a name="request"></a>要求
以下は、要求の例です。

<!-- {
  "blockType": "request",
  "name": "item_createlink"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root:/{item-path}:/createLink
Content-type: application/json

{
  "type": "view",
  "scope": "anonymous"
}
```

##### <a name="response"></a>応答

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "view",
    "scope": "anonymous",
    "webUrl": "https://1drv.ms/A6913278E564460AA616C71B28AD6EB6",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="creating-company-sharable-links"></a>会社の共有可能リンクを作成する

OneDrive for Business および SharePoint は、会社の共有可能リンクをサポートしています。これらは匿名リンクに似ていますが、所有テナントのメンバーだけが使用できる点が異なります。会社の共有可能リンクを作成するには、**scope** パラメーターで値 `organization` を指定して使用します。

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "request", "name": "create-link-scoped", "scopes": "files.readwrite service.sharepoint" } -->
```
POST https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```

## <a name="http-response"></a>HTTP 応答

応答は、アイテムに新しい共有リンクが作成される場合は `201 Created`、既存のリンクが返される場合は `200 OK` となります。

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "view",
    "scope": "organization",
    "webUrl": "https://contoso-my.sharepoint.com/personal/ellen_contoso_com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="embeddable-links"></a>埋め込み可能なリンク

リンクの種類で `embed` を使用する場合、返される webUrl は `<iframe>` HTML 要素に埋め込むことができます。埋め込みリンクが作成されると、`webHtml` プロパティに `<iframe>` がコンテンツをホストするための HTML コードが含まれます。

**注:**埋め込みリンクは **driveType** が `personal` である[ドライブ](../resources/drive.md)でのみ、サポートされます。

## <a name="remarks"></a>注釈

* 組織に既定の有効期限ポリシーが適用されている場合を除き、このアクションを使用して作成されたリンクに期限はありません。
* リンクはそのアイテムの共有アクセス許可に表示され、アイテムの所有者はそれを削除できます。
* リンクは、そのアイテムがチェックアウトされない限り、常にアイテムの現在のバージョンをポイントします (SharePoint の場合のみ)。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "item: createLink",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Create sharing link"
} -->
