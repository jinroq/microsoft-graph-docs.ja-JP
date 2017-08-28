# <a name="get-a-site-resource"></a>サイト リソースを取得する

[サイト][] リソースのプロパティとリレーションシップを取得します。**サイト** リソースは、SharePoint のチーム サイトを表します。

[サイト]: ../resources/site.md

**サイト**は、以下の値の複合 ID である、一意識別子にアドレス指定されます。

* サイト コレクションのホスト名 (contoso.sharepoint.com)
* サイト コレクションの一意 ID (guid)
* サイトの一意 ID (guid)

予約済みのサイト識別子 `root` もあります。これは次に示すように、常にターゲットのルート サイトを参照します。

* `/sites/root`:テナントのルート サイト。
* `/groups/{group-id}/sites/root`:グループのチーム サイト。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              | 
|:--------------------|:---------------------------------------------------------| 
|委任 (職場または学校のアカウント) | Sites.Read.All、Sites.ReadWrite.All    | 
|委任 (個人用 Microsoft アカウント) | サポートされていません。    | 
|アプリケーション | Sites.Read.All、Sites.ReadWrite.All | 

## <a name="get-the-tenants-root-site"></a>テナントのルート サイトを取得する

テナント内のルートの SharePoint サイトにアクセスするには次のようにします。

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a>サーバーの相対 URL でサイトにアクセスする

**サイト** リソースのサーバーの相対 URL がある場合、次のように要求を構築することができます。

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a>グループのチーム サイトにアクセスする

[グループ](../resources/group.md) のチーム サイトにアクセスするには次のようにします。

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a>例

##### <a name="request"></a>要求

<!-- { "blockType": "request", "name": "get-site", "scopes": "sites.read.all service.sharepoint" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}
```

##### <a name="response"></a>応答

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "d297964f-d325-424b-a002-f54048a4622e",
    "name": "OneDrive / SharePoint Team",
    "description": "Collaboration site for the OneDrive and SharePoint team",
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/Get site by ID"
} -->
