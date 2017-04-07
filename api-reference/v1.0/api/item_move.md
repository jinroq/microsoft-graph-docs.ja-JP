# <a name="move-a-driveitem"></a>DriveItem を移動する

DriveItem を新しい親アイテムに移動する場合は、移動する DriveItem の **parentReference** をアプリで更新します。これは、[更新](item_update.md)メソッドの特殊なケースです。アプリでは、新しいコンテナーへのアイテムの移動と、アイテムの別のプロパティの更新を単一の要求に組み合わせることができます。

この要求を使用して、アイテムを[ドライブ](../resources/drive.md)間で移動することはできません。

## <a name="prerequisites"></a>前提条件
この API を実行するには、以下のいずれかの**スコープ**が必要です。

  * Files.ReadWrite

## <a name="http-request"></a>HTTP 要求

```http
PATCH /me/drive/items/{item-id}
PATCH /me/drive/root:/{item-path}
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/{item-id}
```

## <a name="request-headers"></a>要求ヘッダー

| 名前          | 型   | 説明                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| if-match      | String | この要求ヘッダーが含まれていて、指定された eTag (または cTag) がフォルダーの現在の eTag に一致しない場合には、`412 Precondition Failed` 応答が返されます。 |


## <a name="request-body"></a>要求本文
要求の本文内に、**parentReference** プロパティの新しい値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。

**注:**OneDrive のルートにアイテムを移動するときには、`"id:" "root"` 構文は使用できません。ルート フォルダーの実際の ID を使用するか、親参照の `{"path": "/drive/root"}` を使用する必要があります。

## <a name="response"></a>応答
成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [DriveItem](../resources/driveitem.md) リソースを返します。

## <a name="example"></a>例
この例では、{item-id} で指定したアイテムを、ユーザーの OneDrive の **Documents** フォルダーに移動します

<!-- {
  "blockType": "request",
  "name": "update_item"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{item-id}
Content-type: application/json

{
    "name": "new-item-name",
    "parentReference" : {"path": "/drive/root:/Documents"}
}
```

## <a name="response"></a>応答
以下は、応答の例です。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "0123456789abc",
    "name": "new-item-name",
    "folder": { "childCount": 3 },
  "parentReference": {
    "id": "507DE6D5-0201-496A-AA87-5E2563247982",
    "path": "/drive/root:/Documents"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Move item",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
