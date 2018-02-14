# <a name="windowsinformationprotectionapplockerfile-resource-type"></a>windowsInformationProtectionAppLockerFile リソースの種類

> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Windows 情報保護 AppLocker ファイル
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List windowsInformationProtectionAppLockerFiles](../api/intune_mam_windowsinformationprotectionapplockerfile_list.md)|[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) コレクション|[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get windowsInformationProtectionAppLockerFile](../api/intune_mam_windowsinformationprotectionapplockerfile_get.md)|[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md)|[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create windowsInformationProtectionAppLockerFile](../api/intune_mam_windowsinformationprotectionapplockerfile_create.md)|[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md)|新しい [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) オブジェクトを作成します。|
|[Delete windowsInformationProtectionAppLockerFile](../api/intune_mam_windowsinformationprotectionapplockerfile_delete.md)|なし|[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) を削除します。|
|[Update windowsInformationProtectionAppLockerFile](../api/intune_mam_windowsinformationprotectionapplockerfile_update.md)|[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md)|[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|displayName|文字列型 (String)|フレンドリ名|
|fileHash|文字列型 (String)|ファイルの SHA256 ハッシュ|
|file|バイナリ型 (Binary)|バイト配列のファイル|
|id|文字列型 (String)|エンティティのキー。|
|version|文字列型 (String)|エンティティのバージョン。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionAppLockerFile"
}
-->
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



