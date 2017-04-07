# <a name="device-resource-type"></a>デバイス リソース型

組織に登録されているデバイスを表します。デバイスは、Device Registration Service を使用するか、Intune によってクラウドで作成することもできます。これは、多要素認証の条件付きアクセス ポリシーで使用されます。該当するデバイスの範囲は、デスクトップやノート PC から携帯電話やタブレットに及びます。[directoryObject](directoryobject.md) から継承します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[デバイスを作成する](../api/device_post_devices.md) | [device](device.md) |ディレクトリに新しく登録されるデバイスを作成します。|
|[デバイスを取得する](../api/device_get.md) | [device](device.md) |デバイス オブジェクトのプロパティとリレーションシップを読み取ります。|
|[デバイスを一覧表示する](../api/device_list.md) | [device](device.md) コレクション| ディレクトリに登録されたデバイスの一覧を取得します。 |
|[デバイスを更新する](../api/device_update.md) | [device](device.md) |デバイス オブジェクトのプロパティを更新します。 |
|[デバイスを削除する](../api/device_delete.md) | なし |デバイス オブジェクトを削除します。 |
|[registeredOwner を作成する](../api/device_post_registeredowners.md) |[directoryObject](directoryobject.md)| registeredOwners ナビゲーション プロパティに投稿することで、デバイスの新しい所有者としてユーザーを追加します。|
|[registeredOwners を一覧表示する](../api/device_list_registeredowners.md) |[directoryObject](directoryobject.md) コレクション| registeredOwners ナビゲーション プロパティから、デバイスの登録済み所有者であるユーザーを取得します。|
|[registeredUser を作成する](../api/device_post_registeredusers.md) |[directoryObject](directoryobject.md)| registeredUsers ナビゲーション プロパティに投稿することで、デバイスの登録済みユーザーを追加します。|
|[registeredUsers を一覧表示します](../api/device_list_registeredusers.md) |[directoryObject](directoryobject.md) コレクション| registeredUsers ナビゲーション プロパティから、デバイスの登録済みユーザーを取得します。|

## <a name="properties"></a>プロパティ
| プロパティ       | 型    |説明|
|:---------------|:--------|:----------|
|accountEnabled|Boolean| アカウントが有効な場合は **true**。それ以外の場合は **false**。必須。|
|alternativeSecurityIds|[alternativeSecurityId](alternativesecurityid.md) コレクション| 複数値を持つプロパティのフィルター式には **any** 演算子が必要です。null 許容ではありません。必須。 |
|approximateLastSignInDateTime|DateTimeOffset| Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|deviceId|Guid| デバイスを表す一意のクライアント固有の GUID。必須。 |
|deviceMetadata|String|    |
|deviceVersion|Int32|            |
|displayName|String|デバイスの表示名。必須。 |
|id|String|デバイスの一意識別子。[directoryObject](directoryobject.md) から継承されます。キーであり、Null は許容されません。読み取り専用。|
|isCompliant|Boolean|デバイスがモバイル デバイス管理 (MDM) ポリシーに準拠している場合は **true**。それ以外の場合は **false**。|
|isManaged|Boolean|デバイスが Intune などのモバイル デバイス管理 (MDM) アプリで管理されている場合は **true**。それ以外の場合は **false**。|
|onPremisesLastSyncDateTime|DateTimeOffset|オブジェクトがオンプレミスのディレクトリと最後に同期された日時を示します。Timestamp 型は、ISO 8601 形式を使用して、常に UTC 時間での日付と時刻の情報を表します。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|onPremisesSyncEnabled|Boolean|このオブジェクトがオンプレミスのディレクトリから同期される場合は **true**。このオブジェクトが最初にオンプレミスのディレクトリから同期されていて、今後は同期されない場合は **false**。このオブジェクトがオンプレミスのディレクトリから一度も同期されたことがない場合は **null** (既定値)。|
|operatingSystem|String|デバイス上のオペレーティング システムの種類。必須。 |
|operatingSystemVersion|String|デバイス上のオペレーティング システムのバージョン。必須。 |
|physicalIds|String collection| null 許容ではありません。            |
|trustType|String|    ||

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型    |説明|
|:---------------|:--------|:----------|
|registeredOwners|[directoryObject](directoryobject.md) コレクション|デバイスの登録済み所有者であるユーザー。読み取り専用。Null 許容型。|
|registeredUsers|[directoryObject](directoryobject.md) コレクション|デバイスの登録済みユーザーであるユーザー。読み取り専用。Null 許容型。|



## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "registeredOwners",
    "registeredUsers"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.device"
}-->

```json
{
  "accountEnabled": true,
  "alternativeSecurityIds": [{"@odata.type": "microsoft.graph.alternativeSecurityId"}],
  "approximateLastSignInDateTime": "String (timestamp)",
  "deviceId": "string",
  "deviceMetadata": "string",
  "deviceVersion": 1024,
  "displayName": "string",
  "id": "string (identifier)",
  "isCompliant": true,
  "isManaged": true,
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": true,
  "operatingSystem": "string",
  "operatingSystemVersion": "string",
  "physicalIds": ["string"],
  "trustType": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "device resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
