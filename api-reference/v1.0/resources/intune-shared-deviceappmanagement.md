---
title: deviceAppManagement リソースの種類
description: すべてのデバイス アプリの管理機能のコンテナーとして機能する単一のエンティティです。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4a16d5656c90113c31595824925c79e801002de8
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253044"
---
# <a name="deviceappmanagement-resource-type"></a>deviceAppManagement リソースの種類

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

すべてのデバイス アプリの管理機能のコンテナーとして機能する単一のエンティティです。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[Get deviceAppManagement](../api/intune-shared-deviceappmanagement-get.md)|[deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Update deviceAppManagement](../api/intune-shared-deviceappmanagement-update.md)|[deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) オブジェクトのプロパティを更新します。|
|**オンボーディング**|
|[syncMicrosoftStoreForBusinessApps アクション](../api/intune-shared-deviceappmanagement-syncmicrosoftstoreforbusinessapps.md)|なし|ビジネス向け Microsoft Store と Intune アカウントを同期します|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。|
|**オンボーディング**|
|isEnabledForMicrosoftStoreForBusiness|Boolean|アカウントと、ビジネス向け Microsoft Store からのアプリケーションとの同期が有効にされているかどうか。|
|microsoftStoreForBusinessLanguage|String|ビジネス向け Microsoft Store からのアプリケーションの同期に使用されたロケール情報。 国/地域固有のカルチャ。 カルチャの名前は RFC 4646 に準拠します (Windows Vista 以降)。 形式の <languagecode2>-<country/regioncode2> は<languagecode2>  ISO 639-1 に基づく小文字 2 文字のコードで、<country/regioncode2> は ISO 3166 に基づく大文字 2 文字のコードです。 たとえば、英語 (米国) 固有のカルチャは en-US です。|
|microsoftStoreForBusinessLastCompletedApplicationSyncTime|DateTimeOffset|ビジネス向け Microsoft Store からのアプリケーション同期が最後に実行された日時。|
|microsoftStoreForBusinessLastSuccessfulSyncDateTime|DateTimeOffset|ビジネス向け Microsoft Store のアプリがアカウントに正常に同期された最終日時。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|**アプリ**|
|mobileAppCategories|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) コレクション|モバイル アプリ カテゴリ。|
|mobileAppConfigurations|[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) コレクション|管理対象デバイスのモバイル アプリケーション構成。|
|mobileApps|[mobileApp](../resources/intune-apps-mobileapp.md) コレクション|モバイル アプリ。|
|**書籍**|
|managedEBooks|[managedEBook](../resources/intune-books-managedebook.md) コレクション|管理対象の電子ブック。|
|**モバイル アプリの管理 (MAM)**|
|androidManagedAppProtections|[androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) コレクション|Android 管理対象アプリ ポリシーです。|
|defaultManagedAppProtections|[defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) コレクション|既定の管理対象アプリ ポリシーです。|
|iosManagedAppProtections|[iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) コレクション|iOS 管理対象アプリ ポリシーです。|
|managedAppPolicies|[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション|管理対象アプリ ポリシーです。|
|managedAppRegistrations|[managedAppRegistration](../resources/intune-mam-managedappregistration.md) コレクション|管理対象アプリの登録です。|
|managedAppStatuses|[managedAppStatus](../resources/intune-mam-managedappstatus.md) コレクション|管理対象アプリの状態です。|
|mdmWindowsInformationProtectionPolicies|[mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) コレクション|MDM に登録されたデバイス上で実行されているアプリの Windows 情報保護です。|
|targetedManagedAppConfigurations|[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) コレクション|ターゲットとなる管理対象アプリの構成です。|
|windowsInformationProtectionPolicies|[windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) コレクション|MDM に登録されていないデバイス上で実行されているアプリの Windows 情報保護です。|
|**オンボーディング**|
|vppTokens|[vppToken](../resources/intune-onboarding-vpptoken.md) コレクション|この組織への Vpp トークンのリストです。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。  これは単なる例であることに注意してください。実際のクエリに対するクエリ応答には、コンテキストに適したプロパティが含まれています。  
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)",
  "microsoftStoreForBusinessLastSuccessfulSyncDateTime": "String (timestamp)",
  "isEnabledForMicrosoftStoreForBusiness": true,
  "microsoftStoreForBusinessLanguage": "String",
  "microsoftStoreForBusinessLastCompletedApplicationSyncTime": "String (timestamp)"
}
```



