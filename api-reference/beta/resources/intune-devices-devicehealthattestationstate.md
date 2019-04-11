---
title: deviceHealthAttestationState リソース タイプ
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 66a22d0d3cc5caa53c41607da1d1de8185f22a62
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31793757"
---
# <a name="devicehealthattestationstate-resource-type"></a>deviceHealthAttestationState リソース タイプ

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

まだ文書化されていません

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|lastUpdateDateTime|文字列|最終更新のタイムスタンプ。|
|contentNamespaceUrl|文字列|DHA レポートのバージョン。 (名前空間のバージョン)|
|deviceHealthAttestationStatus|文字列|DHA レポートのバージョン。 (名前空間のバージョン)|
|contentVersion|文字列|HealthAttestation 状態のスキーマのバージョン|
|issuedDateTime|DateTimeOffset|デバイスの評価または MDM への発行が行われた DateTime|
|attestationIdentityKey|文字列|構成証明識別キー (AIK) がデバイス上に存在するときに、デバイスに保証キー (EK) 証明書があることを示します。|
|resetCount|Int64|PC デバイスが休止または再開した回数|
|restartCount|Int64|PC デバイスが再起動した回数|
|dataExcutionPolicy|文字列|DEP ポリシーは、メモリに関する追加のチェックを実行する、一連のハードウェアおよびソフトウェアのテクノロジを定義します |
|bitLockerStatus|文字列|BitLocker ドライブ暗号化のオンまたはオフ|
|bootManagerVersion|文字列|ブート マネージャーのバージョン|
|codeIntegrityCheckVersion|文字列|ブート マネージャーのバージョン|
|secureBoot|文字列|セキュア ブートが有効になっている場合、コア コンポーネントには正しい暗号化署名が必要です|
|bootDebugging|文字列|bootDebugging を有効にすると、デバイスを開発およびテストに使用できます|
|operatingSystemKernelDebugging|文字列|operatingSystemKernelDebugging を有効にすると、デバイスを開発およびテストに使用できます|
|codeIntegrity|文字列| コードの整合性が有効な場合は、整合性が検証済みコードのみが実行されます|
|testSigning|文字列|テスト署名が許可されている場合、デバイスは起動時に署名確認を行いません|
|safeMode|文字列|セーフ モードは、制限された状態でコンピューターを起動する、Windows のトラブルシューティング オプションです|
|windowsPE|文字列|Windows 用のコンピューターの準備に使用される、限られたサービスで動作するオペレーティング システム|
|earlyLaunchAntiMalwareDriverProtection|文字列|ELAM は、起動時にネットワーク内のコンピューターを保護します|
|virtualSecureMode|文字列|VSM は、危害を受けたカーネルから、高い価値のアセットを保護するコンテナーです|
|pcrHashAlgorithm|文字列|TPM で使用されていた HASH アルゴリズムを識別する情報の属性|
|bootAppSecurityVersion|文字列|ブート アプリケーションのセキュリティ バージョン番号|
|bootManagerSecurityVersion|文字列|ブート アプリケーションのセキュリティ バージョン番号|
|tpmVersion|文字列|ブート アプリケーションのセキュリティ バージョン番号|
|pcr0|文字列|PCR\[0\] でキャプチャされた測定値|
|secureBootConfigurationPolicyFingerPrint|文字列|カスタム セキュア ブート構成ポリシーの指紋|
|codeIntegrityPolicy|文字列|ブート環境のセキュリティを制御するコードの整合性ポリシー|
|bootRevisionListInfo|文字列|構成証明されたデバイスの初期ブート時に読み込まれた、ブートの変更履歴のリスト|
|operatingSystemRevListInfo|文字列|構成証明されたデバイスの初期ブート時に読み込まれた、オペレーティング システムの変更履歴のリスト|
|healthStatusMismatchInfo|String|この属性は、DHA サービスが整合性の問題を検出した場合に表示されます|
|healthAttestationSupportedStatus|String|この属性は、DHA がデバイス向けにサポートされているかどうかを示します|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthAttestationState"
}
-->
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





