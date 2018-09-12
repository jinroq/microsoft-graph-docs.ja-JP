# <a name="windowsinformationprotectionapplockerfile-resource-type"></a>windowsInformationProtectionAppLockerFile リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Windows 情報保護 AppLocker ファイル
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[windowsInformationProtectionAppLockerFiles の一覧表示](../api/intune_mam_windowsinformationprotectionapplockerfile_list.md)|[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) コレクション|[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[windowsInformationProtectionAppLockerFile の取得](../api/intune_mam_windowsinformationprotectionapplockerfile_get.md)|[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md)|[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[windowsInformationProtectionAppLockerFile の作成](../api/intune_mam_windowsinformationprotectionapplockerfile_create.md)|[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md)|新しい [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) オブジェクトを作成します。|
|[windowsInformationProtectionAppLockerFile の削除](../api/intune_mam_windowsinformationprotectionapplockerfile_delete.md)|なし|[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) を削除します。|
|[windowsInformationProtectionAppLockerFile の更新](../api/intune_mam_windowsinformationprotectionapplockerfile_update.md)|[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md)|[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|displayName|文字列|フレンドリ名|
|fileHash|文字列|ファイルの SHA256 ハッシュ|
|ファイル|バイナリ型 (Binary)|バイト配列のファイル|
|ID|文字列|エンティティのキー。|
|バージョン|文字列|エンティティのバージョン。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionAppLockerFile"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
  "displayName": "String",
  "fileHash": "String",
  "file": "binary",
  "id": "String (identifier)",
  "version": "String"
}
```








