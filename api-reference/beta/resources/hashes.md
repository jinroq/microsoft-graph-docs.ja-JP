# <a name="hashes-resource-type"></a>ハッシュ リソースの種類

 **ハッシュ** リソースは、利用可能なハッシュをアイテムの 1 つの構造にグループ化します。

**注:**すべてのサービスで、表示されているすべてのハッシュ プロパティに対して値が指定されているわけではありません。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "sha1Hash", "crc32Hash", "quickXorHash" ],
  "@odata.type": "microsoft.graph.hashes"
}-->

```json
{
  "crc32Hash": "string",
  "sha1Hash": "string",
  "quickXorHash": "string"
}
```


## <a name="properties"></a>プロパティ

| プロパティ         | 型   | 説明                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| **sha1Hash**     | String | ファイルの内容の SHA1 ハッシュ (使用可能な場合)。読み取り専用。 |
| **crc32Hash**    | String | ファイルの CRC32 の値 (使用可能な場合)。読み取り専用。            |
| **quickXorHash** | String | ファイルの内容が変更されているかどうかの判別に使用できるファイルの専用ハッシュ (使用可能な場合)。読み取り専用。 | 

**注:**ハッシュ値が使用可能ではない場合があります。その場合、アイテムのハッシュ値は、アイテムがダウンロードされた後に更新されます。


## <a name="remarks"></a>注釈

OneDrive for Business では、**sha1Hash** と **crc32Hash** は利用できません。OneDrive Personal では、**quickXorHash** は利用できません。

DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "hashes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
