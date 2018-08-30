# <a name="user-resource-type"></a>user リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Azure Active Directory ユーザー オブジェクトを表します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[ユーザー](../api/intune_shared_user_list.md) オブジェクト をリストする|
|オブジェクトの[ユーザーを取得](../api/intune_shared_user_get.md) する|
|[ユーザー](../api/intune_shared_user_create.md) オブジェクトを作成する|
|[ユーザーを削除する](../api/intune_shared_user_delete.md)|
|[ユーザー](../api/intune_shared_user_update.md) オブジェクトを更新する|
|**デバイス管理**|
|[removeAllDevicesFromManagement 操作](../api/intune_shared_user_removealldevicesfrommanagement.md)|なし|対象ユーザーの管理からすべてのデバイスを破棄します|
|**モバイル アプリケーション管理 (MAM)**|
|[getManagedAppDiagnosticStatuses 関数](../api/intune_shared_user_getmanagedappdiagnosticstatuses.md)|[managedAppDiagnosticStatus](../resources/intune_mam_managedappdiagnosticstatus.md) コレクション|特定のユーザーの診断検証状態を取得します。|
|[getManagedAppPolicies 関数](../api/intune_shared_user_getmanagedapppolicies.md)|[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) コレクション|特定のユーザーのアプリ制限を取得します。|
|[wipeManagedAppRegistrationsByDeviceTag アクション](../api/intune_shared_user_wipemanagedappregistrationsbydevicetag.md)|なし|指定されたデバイス タグが含まれるアプリ登録でワイプ操作を実行します。|

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|id|文字列|ユーザーの一意識別子。|
|**採用**|
|deviceEnrollmentLimit|Int32|ユーザーが登録を許可されているデバイスの最大数。 使用できる値は 5 または 1000 です。|


## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|**デバイス管理**|
|managedDevices|[managedDevice](../resources/intune_devices_manageddevice.md) コレクション|対象ユーザーに関連付けられている管理対象デバイス。|
|**モバイル アプリケーション管理 (MAM)**|
|managedAppRegistrations|[managedAppRegistration](../resources/intune_mam_managedappregistration.md) コレクション|対象ユーザーに属する 0 個以上の管理対象アプリ登録。|
|**トラブルシューティング**|
|deviceManagementTroubleshootingEvents|[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) コレクション|対象ユーザーのトラブルシューティング イベントの一覧です。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true,
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)",
  "deviceEnrollmentLimit": 5
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: Resource microsoft.graph.user is defined in multiple files: /api-reference/v1.0/resources/intune_shared_user.md, /api-reference/v1.0/resources/user.md",
  ]
}-->
