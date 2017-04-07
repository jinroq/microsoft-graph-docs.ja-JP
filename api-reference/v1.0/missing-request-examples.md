# <a name="helpers-examples-that-arent-included-in-the-docs"></a>ヘルパー (ドキュメントに含まれていない例)

これらはマークダウン スキャナーがグラフ ドキュメントを適切に処理できるようにするため、ドキュメントに追加する必要があったものです。


## <a name="define-the-me-as-singleton"></a>(me) をシングルトンとして定義します。

<!-- {"blockType": "request", "name": "get_current_user" } -->
```http
GET https://graph.microsoft.com/v1.0/me
```

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.user", truncated: true } -->
```http
HTTP/1.1 200 OK

{
}
```


## <a name="define-drives-as-an-queryable-entityset"></a>ドライブをクエリ可能な entityset として定義します。
<!-- {"blockType": "request", "name": "get_drive_from_id" } -->
```http
GET https://graph.microsoft.com/v1.0/drives/{drive-id}
```

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.drive", truncated: true } -->
```http
HTTP/1.1 200 OK

{
}
```


## <a name="define-users-as-an-queryable-entityset"></a>ユーザーをクエリ可能な entityset として定義します。

<!-- {"blockType": "request", "name": "get_users" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{user-id}
```

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.user", truncated: true } -->
```http
HTTP/1.1 200 OK

{
}
```
