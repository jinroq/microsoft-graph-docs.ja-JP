# <a name="userinstallstatesummary-resource-type"></a>userInstallStateSummary リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

ユーザーのインストール状態の要約のプロパティが含まれています。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[userInstallStateSummaries のリスト](../api/intune_books_userinstallstatesummary_list.md)|[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) コレクション|[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[userInstallStateSummary の取得](../api/intune_books_userinstallstatesummary_get.md)|[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md)|[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[userInstallStateSummary の作成](../api/intune_books_userinstallstatesummary_create.md)|[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md)|新しい [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) オブジェクトを作成します。|
|[userInstallStateSummary の削除](../api/intune_books_userinstallstatesummary_delete.md)|なし|[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) を削除します。|
|[userInstallStateSummary の更新](../api/intune_books_userinstallstatesummary_update.md)|[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md)|[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|userName|String|ユーザー名です。|
|installedDeviceCount|Int32|インストールされたデバイスの数です。|
|failedDeviceCount|Int32|障害のあるデバイスの数です。|
|notInstalledDeviceCount|Int32|インストールされていないデバイスの数です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|deviceStates|[deviceInstallState](../resources/intune_books_deviceinstallstate.md) コレクション|電子ブックのインストールの状態です。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userInstallStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "id": "String (identifier)",
  "userName": "String",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024
}
```



