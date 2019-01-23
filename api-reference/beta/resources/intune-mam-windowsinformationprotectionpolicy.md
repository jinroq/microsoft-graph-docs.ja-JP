---
title: windowsInformationProtectionPolicy リソース タイプ
description: MDM を使用しない、Windows 情報保護のポリシー
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a0da31cd2f487e3e9acaf97c543781a5ec316169
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419304"
---
# <a name="windowsinformationprotectionpolicy-resource-type"></a>windowsInformationProtectionPolicy リソース タイプ

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

MDM を使用しない、Windows 情報保護のポリシー


[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List windowsInformationProtectionPolicies](../api/intune-mam-windowsinformationprotectionpolicy-list.md)|[windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) コレクション|[windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get windowsInformationProtectionPolicy](../api/intune-mam-windowsinformationprotectionpolicy-get.md)|[windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md)|[windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create windowsInformationProtectionPolicy](../api/intune-mam-windowsinformationprotectionpolicy-create.md)|[windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md)|新しい [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) オブジェクトを作成します。|
|[Delete windowsInformationProtectionPolicy](../api/intune-mam-windowsinformationprotectionpolicy-delete.md)|なし|[windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) を削除します。|
|[Update windowsInformationProtectionPolicy](../api/intune-mam-windowsinformationprotectionpolicy-update.md)|[windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md)|[windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|displayName|String|ポリシーの表示名。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|説明|String|ポリシーの説明。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|createdDateTime|DateTimeOffset|ポリシーが作成された日時。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|ポリシーが変更された最終日時。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|roleScopeTagIds|String コレクション|このエンティティ インスタンスのスコープのタグのリストです。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|id|String|エンティティのキー。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|version|String|エンティティのバージョン。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|enforcementLevel|[windowsInformationProtectionEnforcementLevel](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|WIP の適用レベルです。[WindowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)からサポートされている値継承の列挙型定義を参照してください。 可能な値は、`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock` です。|
|enterpriseDomain|String|プライマリ エンタープライズ ドメイン ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)|
|enterpriseProtectedDomainNames|[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション|保護するエンタープライズ ドメインのリスト ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)|
|protectionUnderLockConfigRequired|Boolean|ロック機能による保護 (pin での暗号化) を構成するかどうかを指定します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)|
|dataRecoveryCertificate|[windowsInformationProtectionDataRecoveryCertificate](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|暗号化されたファイルのデータ回復に使用できる回復証明書を指定します。 これは、暗号化ファイル システム (EFS) のデータ回復エージェント (DRA) 証明書と同じです ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)|
|revokeOnUnenrollDisabled|Boolean|このポリシーは、デバイスが管理サービスから登録を解除するときに WIP キーを取り消すかどうかを制御します。 1 (キーの取り消しをしない) に設定すると、キーは取り消されず、ユーザーは登録解除後も引き続き保護されたファイルにアクセスできます。 キーが取り消されない場合は、その後、取り消されたファイルのクリーンアップは行われません。 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します|
|rightsManagementServicesTemplateId|Guid|RMS の暗号化に使用する TemplateID GUID。 RMS テンプレートを使用すると、IT 管理者は、RMS で保護されたファイルにアクセスできるユーザーの詳細とアクセスできる期間の詳細を構成することができます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)|
|azureRightsManagementServicesAllowed|Boolean|WIP 用の Azure RMS の暗号化を許可するかどうかを指定します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)|
|iconsVisible|Boolean|エクスプローラーでの WIP で保護されたファイルと、スタート メニューのエンタープライズ専用のアプリ タイルについて、アイコンにオーバーレイを追加するかどうかを決定します。 Windows 10 Version 1703 以降では、この設定は WIP で保護されたアプリのタイトル バーにおける WIP アイコンの可視性も構成します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)|
|protectedApps|[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) コレクション|保護されたアプリケーションはエンタープライズ データにアクセスすることができ、これらのアプリケーションによって処理されるデータは暗号化によって保護されます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)|
|exemptApps|[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) コレクション|適用除外アプリケーションはエンタープライズ データにアクセスできますが、これらのアプリケーションによって処理されるデータは保護されません。 これは、重要なエンタープライズ アプリケーションの中には、暗号化されたデータとの互換性の問題がある可能性があるためです。 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します|
|enterpriseNetworkDomainNames|[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション|これは、エンタープライズの境界を構成するドメインのリストです。 デバイスに送信されるこれらのドメインの 1 つからのデータは、エンタープライズ データと見なされ、保護されます。これらの場所は、エンタープライズ データを共有するための安全なコピー先と見なされます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)|
|enterpriseProxiedDomains|[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) コレクション|保護が必要な、クラウドでホストされているエンタープライズ リソース ドメインのリストが含まれています。 これらのリソースへの接続は、エンタープライズ データと見なされます。 プロキシがクラウド リソースとペアリング済みの場合、クラウド リソースへのトラフィックは、指定されたプロキシ サーバー (ポート 80) を介してエンタープライズ ネットワーク経由でルーティングされます。 この目的で使用されるプロキシ サーバーは、EnterpriseInternalProxyServers ポリシーを使用して構成する必要があります ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)|
|enterpriseIPRanges|[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) コレクション|エンタープライズ ネットワーク内のコンピューターを定義するエンタープライズ IP の範囲を設定します。 これらのコンピューターからのデータはエンタープライズの一部と見なされ、保護されます。 これらの場所は、エンタープライズ データを共有するための安全なコピー先と見なされます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)|
|enterpriseIPRangesAreAuthoritative|Boolean|構成済みのリストを承諾し、ヒューリスティックを使用した他のサブネットの検索を行わないよう、クライアントに指示するブール値。 既定値は false です ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)|
|enterpriseProxyServers|[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション|これは、プロキシ サーバーのリストです。 このリストにないサーバーは、非エンタープライズと見なされます ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)|
|enterpriseInternalProxyServers|[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション|これは、内部プロキシ サーバーのコンマ区切りのリストです。 例: "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59"。 これらのプロキシは、管理者により、インターネット上の特定のリソースに接続するように構成されています。 それらはエンタープライズ ネットワークの場所にあると見なされます。 これらのプロキシは、EnterpriseProxiedDomains ポリシーの構成のみで活用され、これらのプロキシを介して、一致するドメインにトラフィックを強制します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)|
|enterpriseProxyServersAreAuthoritative|Boolean|プロキシの構成済みリストを承諾し、他の作業プロキシの検出を試みないよう、クライアントに指示するブール値。 既定値は false です ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)|
|neutralDomainResources|[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション|職場または個人のリソースに使用できるドメイン名のリスト ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)|
|indexingEncryptedStoresOrItemsBlocked|Boolean|このスイッチは Windows Search Indexer 用で、アイテムのインデックス作成を許可または禁止します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)|
|smbAutoEncryptedFileExtensions|[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) コレクション|企業の境界内で SMB 共有からコピーするときに、当該拡張子を持つファイルが暗号化されるように、ファイル拡張子のリストを指定します ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)|
|isAssigned|Boolean|包含グループにポリシーを配置するかどうかを示します。 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します|
|revokeOnMdmHandoffDisabled|Boolean|RS2 の新しいプロパティ、保留中のドキュメント|
|mdmEnrollmentUrl|String|MDM の登録 URL|
|windowsHelloForBusinessBlocked|Boolean|Windows にサインインするためのメソッドとして Windows Hello for Business を設定するブール値です。|
|pinMinimumLength|Int32|PIN に必要な文字の最小数を設定する整数値です。 既定値は 4 です。 このポリシー設定で構成できる最小値は 4 です。 構成できる最大値は、[PIN の最大文字数] ポリシー設定で構成された値、または 127 のうち、どちらか小さい方です。|
|pinUppercaseLetters|[windowsInformationProtectionPinCharacterRequirements](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|Windows Hello for Business の PIN における大文字の使用を構成する整数値です。 既定値は NotAllow です。 可能な値は、`notAllow`、`requireAtLeastOne`、`allow` です。|
|pinLowercaseLetters|[windowsInformationProtectionPinCharacterRequirements](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|Windows Hello for Business の PIN における小文字の使用を構成する整数値です。 既定値は NotAllow です。 可能な値は、`notAllow`、`requireAtLeastOne`、`allow` です。|
|pinSpecialCharacters|[windowsInformationProtectionPinCharacterRequirements](../resources/intune-mam-windowsinformationprotectionpincharacterrequirements.md)|Windows Hello for Business の PIN における特殊文字の使用を構成する整数値です。 Windows Hello for Business の PIN ジェスチャの有効な特殊文字は以下のとおりです: ! " # $ % & ' ( ) * + , - . / : ; < = > ? @ \[ \ \] ^ _ ` { | } ~。 既定値は NotAllow です。 可能な値は、`notAllow`、`requireAtLeastOne`、`allow` です。|
|pinExpirationDays|Int32|この整数値は、システムがユーザーに PIN の変更を要求する前の、PIN の使用可能な期間 (日数) を指定します。 このポリシー設定で構成できる最大値は 730 です。 このポリシー設定で構成できる最小値は 0 です。 このポリシーが 0 に設定されている場合、ユーザーの PIN は期限切れになりません。 このノードは、Windows 10 バージョン 1511 で追加されました。 既定値は 0 です。|
|numberOfPastPinsRemembered|Int32|再使用できないユーザー アカウントに関連付けられる過去の PIN の数を指定する整数値です。 このポリシー設定で構成できる最大値は 50 です。 このポリシー設定で構成できる最小値は 0 です。 このポリシーが 0 に設定されている場合、以前の PIN の格納は不要です。 このノードは、Windows 10 バージョン 1511 で追加されました。 既定値は 0 です。|
|passwordMaximumAttemptCount|Int32|デバイスがワイプされるまでの、許可されている認証失敗の回数です。 値を 0 にすると、デバイス ワイプ機能が無効になります。 範囲は整数 X (デスクトップの場合: 4 <= X <= 16、モバイル デバイスの場合: 0 <= X <= 999) です。|
|minutesOfInactivityBeforeDeviceLock|Int32|デバイスがアイドルになった後に、デバイスの PIN またはパスワードがロックされるまでの最大時間 (分) を指定します。   範囲は整数 X (0 < = X < = 999) です。|
|daysWithoutContactBeforeUnenroll|Int32|アプリのデータがワイプされるまでのオフライン期間 (日数) |

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|protectedAppLockerFiles|[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) コレクション|xml ファイルを使用して、保護されたアプリを入力する別の方法 ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)|
|exemptAppLockerFiles|[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) コレクション|xml ファイルを使用して、保護されていないアプリを入力する別の方法 ([windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承)|
|assignments|[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) コレクション|ポリシーを対象とするセキュリティ グループのリストへのナビゲーション プロパティ。 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) から継承します|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
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
  "isAssigned": true,
  "revokeOnMdmHandoffDisabled": true,
  "mdmEnrollmentUrl": "String",
  "windowsHelloForBusinessBlocked": true,
  "pinMinimumLength": 1024,
  "pinUppercaseLetters": "String",
  "pinLowercaseLetters": "String",
  "pinSpecialCharacters": "String",
  "pinExpirationDays": 1024,
  "numberOfPastPinsRemembered": 1024,
  "passwordMaximumAttemptCount": 1024,
  "minutesOfInactivityBeforeDeviceLock": 1024,
  "daysWithoutContactBeforeUnenroll": 1024
}
```




