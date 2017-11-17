# <a name="sharinginvitation-resource-type"></a>SharingInvitation リソースの種類

**SharingInvitation** リソースは、招待に関連するデータ項目を 1 つの構造にグループ化します。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sharingInvitation"
}-->

```json
{
  "email": "string",
  "invitedBy": {"@odata.type": "microsoft.graph.identitySet" },
  "signInRequired": true
}

```

## <a name="properties"></a>プロパティ

| プロパティ名  | 型                          | 説明                                                                                                                   |
|:---------------|:------------------------------|:------------------------------------------------------------------------------------------------------------------------------|
| email          | String                        | 共有への招待の受信者について指定された電子メール アドレス。読み取り専用です。                                          |
| invitedBy      | [identitySet](identityset.md) | このアクセス許可を作成した招待状を送信したユーザーに関する情報を提供します (その情報が利用可能な場合)。読み取り専用です。 |
| signInRequired | ブール型                       | `true` の場合、招待状の受信者は共有アイテムにアクセスするためにサインインする必要があります。読み取り専用です。                     |

## <a name="remarks"></a>注釈 

DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sharingInvitation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
