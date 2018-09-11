# <a name="bitlockerremovabledrivepolicy-resource-type"></a>bitLockerRemovableDrivePolicy リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

BitLocker リムーバブル ドライブ ポリシー。
## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|encryptionMethod|[bitLockerEncryptionMethod](../resources/intune_deviceconfig_bitlockerencryptionmethod.md)|リムーバブル ドライブの暗号化方法を選択します。指定できる値は、`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256` です。|
|requireEncryptionForWriteAccess|ブール値|別の組織で構成されたデバイスへの書き込みアクセスをブロックするかどうかを示します。  RequireEncryptionForWriteAccess が false の場合、この値は影響を与えません。|
|blockCrossOrganizationWriteAccess|ブール値|このポリシー設定は、コンピューター上でリムーバブル データ ドライブを書き込み可能にする際に、BitLocker 保護が必要かどうかを決定します。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRemovableDrivePolicy",
  "encryptionMethod": "String",
  "requireEncryptionForWriteAccess": true,
  "blockCrossOrganizationWriteAccess": true
}
```








