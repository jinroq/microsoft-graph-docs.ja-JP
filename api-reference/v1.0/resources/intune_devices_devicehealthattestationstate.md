# <a name="devicehealthattestationstate-resource-type"></a>deviceHealthAttestationState リソース タイプ

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

まだ文書化されていません
## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|lastUpdateDateTime|String|最終更新のタイムスタンプ。|
|contentNamespaceUrl|String|DHA レポートのバージョン。 (名前空間のバージョン)|
|deviceHealthAttestationStatus|String|DHA レポートのバージョン。 (名前空間のバージョン)|
|contentVersion|String|HealthAttestation 状態のスキーマのバージョン|
|issuedDateTime|DateTimeOffset|デバイスの評価または MDM への発行が行われた DateTime|
|attestationIdentityKey|String|構成証明識別キー (AIK) がデバイス上に存在するときに、デバイスに保証キー (EK) 証明書があることを示します。|
|resetCount|Int64|PC デバイスが休止または再開した回数|
|restartCount|Int64|PC デバイスが再起動した回数|
|dataExcutionPolicy|String|DEP ポリシーは、メモリに関する追加のチェックを実行する、一連のハードウェアおよびソフトウェアのテクノロジを定義します |
|bitLockerStatus|String|BitLocker ドライブ暗号化のオンまたはオフ|
|bootManagerVersion|String|ブート マネージャーのバージョン|
|codeIntegrityCheckVersion|String|ブート マネージャーのバージョン|
|secureBoot|String|セキュア ブートが有効になっている場合、コア コンポーネントには正しい暗号化署名が必要です|
|bootDebugging|String|bootDebugging を有効にすると、デバイスを開発およびテストに使用できます|
|operatingSystemKernelDebugging|String|operatingSystemKernelDebugging を有効にすると、デバイスを開発およびテストに使用できます|
|codeIntegrity|String| コードの整合性が有効な場合は、整合性が検証済みコードのみが実行されます|
|testSigning|String|テスト署名が許可されている場合、デバイスは起動時に署名確認を行いません|
|safeMode|String|セーフ モードは、制限された状態でコンピューターを起動する、Windows のトラブルシューティング オプションです|
|windowsPE|String|Windows 用のコンピューターの準備に使用される、限られたサービスで動作するオペレーティング システム|
|earlyLaunchAntiMalwareDriverProtection|String|ELAM は、起動時にネットワーク内のコンピューターを保護します|
|virtualSecureMode|String|VSM は、危害を受けたカーネルから、高い価値のアセットを保護するコンテナーです|
|pcrHashAlgorithm|String|TPM で使用されていた HASH アルゴリズムを識別する情報の属性|
|bootAppSecurityVersion|String|ブート アプリケーションのセキュリティ バージョン番号|
|bootManagerSecurityVersion|String|ブート アプリケーションのセキュリティ バージョン番号|
|tpmVersion|String|ブート アプリケーションのセキュリティ バージョン番号|
|pcr0|String|PCR\[0\] でキャプチャされた測定値|
|secureBootConfigurationPolicyFingerPrint|String|カスタム セキュア ブート構成ポリシーの指紋|
|codeIntegrityPolicy|String|ブート環境のセキュリティを制御するコードの整合性ポリシー|
|bootRevisionListInfo|String|構成証明されたデバイスの初期ブート時に読み込まれた、ブートの変更履歴のリスト|
|operatingSystemRevListInfo|String|構成証明されたデバイスの初期ブート時に読み込まれた、オペレーティング システムの変更履歴のリスト|
|healthStatusMismatchInfo|String|この属性は、DHA サービスが整合性の問題を検出した場合に表示されます|
|healthAttestationSupportedStatus|String|この属性は、DHA がデバイス向けにサポートされているかどうかを示します|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthAttestationState"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthAttestationState",
  "lastUpdateDateTime": "String",
  "contentNamespaceUrl": "String",
  "deviceHealthAttestationStatus": "String",
  "contentVersion": "String",
  "issuedDateTime": "String (timestamp)",
  "attestationIdentityKey": "String",
  "resetCount": 1024,
  "restartCount": 1024,
  "dataExcutionPolicy": "String",
  "bitLockerStatus": "String",
  "bootManagerVersion": "String",
  "codeIntegrityCheckVersion": "String",
  "secureBoot": "String",
  "bootDebugging": "String",
  "operatingSystemKernelDebugging": "String",
  "codeIntegrity": "String",
  "testSigning": "String",
  "safeMode": "String",
  "windowsPE": "String",
  "earlyLaunchAntiMalwareDriverProtection": "String",
  "virtualSecureMode": "String",
  "pcrHashAlgorithm": "String",
  "bootAppSecurityVersion": "String",
  "bootManagerSecurityVersion": "String",
  "tpmVersion": "String",
  "pcr0": "String",
  "secureBootConfigurationPolicyFingerPrint": "String",
  "codeIntegrityPolicy": "String",
  "bootRevisionListInfo": "String",
  "operatingSystemRevListInfo": "String",
  "healthStatusMismatchInfo": "String",
  "healthAttestationSupportedStatus": "String"
}
```








