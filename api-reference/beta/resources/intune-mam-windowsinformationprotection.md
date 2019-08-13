---
title: windowsInformationProtection リソース タイプ
description: 詳細な管理設定を構成するための Windows 情報保護のポリシー
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: aee82b099ece03e280bd137220dfe10d697fce66
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372959"
---
# <a name="windowsinformationprotection-resource-type"></a>windowsInformationProtection リソース タイプ

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

詳細な管理設定を構成するための Windows 情報保護のポリシー


[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List windowsInformationProtections](../api/intune-mam-windowsinformationprotection-list.md)|[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) コレクション|[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get windowsInformationProtection](../api/intune-mam-windowsinformationprotection-get.md)|[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)|[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[assign action](../api/intune-mam-windowsinformationprotection-assign.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|displayName|String|ポリシーの表示名。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|description|String|ポリシーの説明。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|createdDateTime|DateTimeOffset|ポリシーが作成された日時。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|ポリシーが変更された最終日時。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|roleScopeTagIds|文字列コレクション|このエンティティインスタンスの範囲タグのリスト。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|id|文字列|エンティティのキー。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|version|文字列型 (String)|エンティティのバージョン。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|enforcementLevel|[windowsInformationProtectionEnforcementLevel](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|仕掛品の実施レベル。サポートされている値については、Enum 定義を参照してください。 使用可能な値は、`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock` です。|
|enterpriseDomain|String|プライマリ エンタープライズ ドメイン|
|enterpriseProtectedDomainNames|[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション|保護するエンタープライズ ドメインのリスト|
|protectionUnderLockConfigRequired|Boolean|ロック機能による保護 (pin での暗号化) を構成するかどうかを指定します|
|dataRecoveryCertificate|[windowsInformationProtectionDataRecoveryCertificate](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|暗号化されたファイルのデータ回復に使用できる回復証明書を指定します。 これは、暗号化ファイル システム (EFS) のデータ回復エージェント (DRA) 証明書と同じです。|
|revokeOnUnenrollDisabled|Boolean|このポリシーは、デバイスが管理サービスから登録を解除するときに WIP キーを取り消すかどうかを制御します。 1 (キーの取り消しをしない) に設定すると、キーは取り消されず、ユーザーは登録解除後も引き続き保護されたファイルにアクセスできます。 キーが取り消されない場合は、その後、取り消されたファイルのクリーンアップは行われません。|
|rightsManagementServicesTemplateId|GUID|RMS の暗号化に使用する TemplateID GUID。 RMS テンプレートを使用すると、IT 管理者は、RMS で保護されたファイルにアクセスできるユーザーとアクセスできる期間について、詳細を構成することができます|
|azureRightsManagementServicesAllowed|Boolean|WIP 用の Azure RMS の暗号化を許可するかどうかを指定します|
|iconsVisible|Boolean|エクスプローラーでの WIP で保護されたファイルと、スタート メニューのエンタープライズ専用のアプリ タイルについて、アイコンにオーバーレイを追加するかどうかを決定します。 Windows 10 Version 1703 以降では、この設定は WIP で保護されたアプリのタイトル バーにおける WIP アイコンの可視性も構成します|
|protectedApps|[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) コレクション|保護されたアプリケーションはエンタープライズ データにアクセスすることができ、これらのアプリケーションによって処理されるデータは暗号化によって保護されます|
|exemptApps|[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) コレクション|適用除外アプリケーションはエンタープライズ データにアクセスできますが、これらのアプリケーションによって処理されるデータは保護されません。 これは、重要なエンタープライズ アプリケーションの中には、暗号化されたデータとの互換性の問題がある可能性があるためです。|
|enterpriseNetworkDomainNames|[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション|これは、エンタープライズの境界を構成するドメインのリストです。 デバイスに送信されるこれらのドメインの 1 つからのデータは、エンタープライズ データとみなされ、保護されます。これらの場所は、エンタープライズ データを共有するための安全なコピー先とみなされます|
|enterpriseProxiedDomains|[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) コレクション|保護が必要な、クラウドでホストされているエンタープライズ リソース ドメインのリストが含まれています。 これらのリソースへの接続は、エンタープライズ データと見なされます。 プロキシがクラウド リソースとペアリング済みの場合、クラウド リソースへのトラフィックは、指定されたプロキシ サーバー (ポート 80) を介してエンタープライズ ネットワーク経由でルーティングされます。 この目的で使用されるプロキシ サーバーは、EnterpriseInternalProxyServers ポリシーを使用して構成する必要があります|
|enterpriseIPRanges|[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) コレクション|エンタープライズ ネットワーク内のコンピューターを定義するエンタープライズ IP の範囲を設定します。 これらのコンピューターからのデータはエンタープライズの一部とみなされ、保護されます。 これらの場所は、エンタープライズ データを共有するための安全なコピー先とみなされます|
|enterpriseIPRangesAreAuthoritative|Boolean|構成済みのリストを承諾し、ヒューリスティックを使用した他のサブネットの検索を行わないよう、クライアントに指示するブール値。 既定値は false です|
|enterpriseProxyServers|[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション|これは、プロキシ サーバーのリストです。 このリストにないサーバーは、非エンタープライズとみなされます|
|enterpriseInternalProxyServers|[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション|これは、内部プロキシ サーバーのコンマ区切りのリストです。 例: "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59"。 これらのプロキシは、管理者により、インターネット上の特定のリソースに接続するように構成されています。 それらはエンタープライズ ネットワークの場所にあるとみなされます。 これらのプロキシは、EnterpriseProxiedDomains ポリシーの構成のみで活用され、これらのプロキシを介して、一致するドメインにトラフィックを強制します|
|enterpriseProxyServersAreAuthoritative|Boolean|プロキシの構成済みリストを承諾し、他の作業プロキシの検出を試みないよう、クライアントに指示するブール値。 既定値は false です|
|neutralDomainResources|[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション|職場または個人のリソースに使用できるドメイン名のリスト|
|indexingEncryptedStoresOrItemsBlocked|Boolean|このスイッチは Windows Search Indexer 用で、アイテムのインデックス作成を許可または禁止します|
|smbAutoEncryptedFileExtensions|[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション|企業の境界内で SMB 共有からコピーするときに、当該拡張子を持つファイルが暗号化されるように、ファイル拡張子のリストを指定します|
|isAssigned|Boolean|包含グループにポリシーを配置するかどうかを示します。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|protectedAppLockerFiles|[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) コレクション|xml ファイルを使用して、保護されたアプリを入力する別の方法|
|exemptAppLockerFiles|[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) コレクション|xml ファイルを使用して、適用除外アプリを入力する別の方法|
|assignments|[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) コレクション|ポリシーを対象とするセキュリティ グループのリストへのナビゲーション プロパティ。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtection",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "version": "String",
  "enforcementLevel": "String",
  "enterpriseDomain": "String",
  "enterpriseProtectedDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "protectionUnderLockConfigRequired": true,
  "dataRecoveryCertificate": {
    "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
    "subjectName": "String",
    "description": "String",
    "expirationDateTime": "String (timestamp)",
    "certificate": "binary"
  },
  "revokeOnUnenrollDisabled": true,
  "rightsManagementServicesTemplateId": "Guid",
  "azureRightsManagementServicesAllowed": true,
  "iconsVisible": true,
  "protectedApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "displayName": "String",
      "description": "String",
      "publisherName": "String",
      "productName": "String",
      "denied": true
    }
  ],
  "exemptApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "displayName": "String",
      "description": "String",
      "publisherName": "String",
      "productName": "String",
      "denied": true
    }
  ],
  "enterpriseNetworkDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseProxiedDomains": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
      "displayName": "String",
      "proxiedDomains": [
        {
          "@odata.type": "microsoft.graph.proxiedDomain",
          "ipAddressOrFQDN": "String",
          "proxy": "String"
        }
      ]
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection",
      "displayName": "String",
      "ranges": [
        {
          "@odata.type": "microsoft.graph.iPv6Range",
          "lowerAddress": "String",
          "upperAddress": "String"
        }
      ]
    }
  ],
  "enterpriseIPRangesAreAuthoritative": true,
  "enterpriseProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseInternalProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseProxyServersAreAuthoritative": true,
  "neutralDomainResources": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "indexingEncryptedStoresOrItemsBlocked": true,
  "smbAutoEncryptedFileExtensions": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "isAssigned": true
}
```



