---
title: windows10EndpointProtectionConfiguration リソース タイプ
description: このトピックでは、Windows10EndpointProtectionConfiguration リソースによって公開された、宣言されたメソッド、プロパティ、リレーションシップについて説明します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e64a218dc9ee507567df1271edb2d27051190cbe
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027735"
---
# <a name="windows10endpointprotectionconfiguration-resource-type"></a>windows10EndpointProtectionConfiguration リソース タイプ

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

このトピックでは、Windows10EndpointProtectionConfiguration リソースによって公開された、宣言されたメソッド、プロパティ、リレーションシップについて説明します。


[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List windows10EndpointProtectionConfigurations](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-list.md)|[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) コレクション|[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get windows10EndpointProtectionConfiguration](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-get.md)|[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)|[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create windows10EndpointProtectionConfiguration](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-create.md)|[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)|新しい [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) オブジェクトを作成します。|
|[Delete windows10EndpointProtectionConfiguration](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-delete.md)|なし|[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) を削除します。|
|[Update windows10EndpointProtectionConfiguration](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-update.md)|[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)|[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトの最終更新の DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|description|String|管理者が指定した、デバイス構成についての説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|管理者が指定した、デバイス構成の名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|firewallBlockStatefulFTP|Boolean|デバイスへのステートフル FTP 接続をブロックします|
|firewallIdleTimeoutForSecurityAssociationInSeconds|Int32|セキュリティ アソシエーションのアイドル タイムアウトを 300 から 3600 まで (両端を含む) の秒単位で構成します。 これは、セキュリティ アソシエーションが期限切れになり、削除されるまでの期間です。 有効な値は 300 から 3600 までです|
|firewallPreSharedKeyEncodingMethod|[firewallPreSharedKeyEncodingMethodType](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|使用する事前共有キーのエンコードを選択します。 可能な値は、`deviceDefault`、`none`、`utF8` です。|
|firewallIPSecExemptionsAllowNeighborDiscovery|Boolean|IPSec 除外を構成し、近隣探索の IPv6 ICMP の種類コードを許可します|
|firewallIPSecExemptionsAllowICMP|Boolean|IPSec 除外を構成し、ICMP を許可します|
|firewallIPSecExemptionsAllowRouterDiscovery|Boolean|IPSec 除外を構成し、ルーター発見の IPv6 ICMP の種類コードを許可します|
|firewallIPSecExemptionsAllowDHCP|Boolean|IPSec 除外を構成し、IPv4 と IPv6 の両方の DHCP トラフィックを許可します|
|firewallCertificateRevocationListCheckMethod|[firewallCertificateRevocationListCheckMethodType](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|証明書失効リストの適用方法を指定します。 使用可能な値は、`deviceDefault`、`none`、`attempt`、`require` です。|
|firewallMergeKeyingModuleSettings|Boolean|認証セットがキー モジュールによって完全にサポートされていない場合は、セット全体ではなくサポートされていない認証スイートのみを無視するようにモジュールに指示します|
|firewallPacketQueueingMethod|[firewallPacketQueueingMethodType](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|トンネルゲートウェイのシナリオでパケットキューを適用する方法を構成します。 可能な値は、`deviceDefault`、`disabled`、`queueInbound`、`queueOutbound`、`queueBoth` です。|
|firewallProfileDomain|[windowsFirewallNetworkProfile](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|ドメイン ネットワーク用のファイアウォールのプロファイル設定を構成します|
|firewallProfilePublic|[windowsFirewallNetworkProfile](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|パブリック ネットワーク用のファイアウォールのプロファイル設定を構成します|
|firewallProfilePrivate|[windowsFirewallNetworkProfile](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|プライベート ネットワーク用のファイアウォールのプロファイル設定を構成します|
|defenderAttackSurfaceReductionExcludedPaths|文字列コレクション|攻撃回避規則から除外する exe ファイルとフォルダーのリスト|
|defenderGuardedFoldersAllowedAppPaths|文字列コレクション|保護されたフォルダーへのアクセスが許可されている exe へのパスのリスト|
|defenderAdditionalGuardedFolders|String コレクション|保護されたフォルダーのリストに追加されるフォルダー パスのリスト|
|defenderExploitProtectionXml|Binary|Exploit Protection の詳細に関する情報を含む XML コンテンツ。|
|defenderExploitProtectionXmlFileName|String|DefenderExploitProtectionXml の取得元となるファイルの名前。|
|defenderSecurityCenterBlockExploitProtectionOverride|Boolean|ユーザーによる Exploit Protection の設定の上書きを禁止するかどうかを示します。|
|appLockerApplicationControl|[appLockerApplicationControlType](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|管理者がデバイスで許可するアプリの種類を選択できるようにします。 可能な値は、`notConfigured`、`enforceComponentsAndStoreApps`、`auditComponentsAndStoreApps`、`enforceComponentsStoreAppsAndSmartlocker`、`auditComponentsStoreAppsAndSmartlocker` です。|
|smartScreenEnableInShell|Boolean|IT 管理者が Windows 用の SmartScreen を構成することを許可します。|
|smartScreenBlockOverrideForFiles|Boolean|ユーザーが SmartScreen 警告を無視したり、悪意のあるファイルを実行したりできるかどうかを IT 管理者が制御できるようにします。|
|applicationGuardEnabled|Boolean|Windows Defender Application Guard を有効にします|
|applicationGuardBlockFileTransfer|[Applicationgu/Blockfiletransfertype](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|画像ファイル、テキストファイル、またはそのどちらも転送しないように、クリップボードをブロックします。 可能な値は、`notConfigured`、`blockImageAndTextFile`、`blockImageFile`、`blockNone`、`blockTextFile` です。|
|applicationGuardBlockNonEnterpriseContent|Boolean|サード パーティのプラグインなどエンタープライズ以外のコンテンツを読み込むエンタープライズ サイトをブロックします|
|applicationGuardAllowPersistence|Boolean|App Guard のコンテナー内のユーザー生成データ (お気に入り、Cookie、Web パスワードなど) の保存を許可します|
|applicationGuardForceAuditing|Boolean|監査の実施では、セキュリティ/コンプライアンスの基準 (サンプル イベントでは、ユーザーのログインとログオフ、特権の使用、ソフトウェアのインストール、システムの変更など) を満たすために Windows のログとイベントが保持されます|
|applicationGuardBlockClipboardSharing|[Applicationgu/Blockクリップボード Sharingtype](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|ホストからコンテナーへ、コンテナーからホストへ、または両方向にデータを共有するクリップボードをブロックします。あるいは、どちらの方向の共有もブロックしません。 可能な値は、`notConfigured`、`blockBoth`、`blockHostToContainer`、`blockContainerToHost`、`blockNone` です。|
|applicationGuardAllowPrintToPDF|Boolean|コンテナーから PDF への出力を許可します|
|applicationGuardAllowPrintToXPS|Boolean|コンテナーから XPS への出力を許可します|
|applicationGuardAllowPrintToLocalPrinters|Boolean|コンテナーからローカル プリンターへの出力を許可します|
|applicationGuardAllowPrintToNetworkPrinters|Boolean|コンテナーからネットワーク プリンターへの出力を許可します|
|bitLockerDisableWarningForOtherDiskEncryption|Boolean|管理者がユーザーのマシンで他のディスクの暗号化に関する警告プロンプトを無効にすることを許可します。|
|bitLockerEnableStorageCardEncryptionOnMobile|Boolean|管理者が BitLocker を使用して暗号化をオンにすることを許可します。 このポリシーは、携帯電話の SKU に対してのみ有効です。|
|bitLockerEncryptDevice|Boolean|管理者が BitLocker を使用して暗号化をオンにすることを許可します。|
|bitLockerRemovableDrivePolicy|[bitLockerRemovableDrivePolicy](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|BitLocker リムーバブル ドライブ ポリシー。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション|デバイスの構成プロファイルの割り当てのリスト。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション|デバイスごとのデバイス構成のインストール状況。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション|ユーザーごとのデバイス構成のインストール状態。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション|デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10EndpointProtectionConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 1024,
  "firewallPreSharedKeyEncodingMethod": "String",
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "String",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "String",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "String",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "firewallProfilePublic": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "String",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "firewallProfilePrivate": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "String",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "defenderAttackSurfaceReductionExcludedPaths": [
    "String"
  ],
  "defenderGuardedFoldersAllowedAppPaths": [
    "String"
  ],
  "defenderAdditionalGuardedFolders": [
    "String"
  ],
  "defenderExploitProtectionXml": "binary",
  "defenderExploitProtectionXmlFileName": "String",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "appLockerApplicationControl": "String",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardBlockFileTransfer": "String",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "String",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "String",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  }
}
```



