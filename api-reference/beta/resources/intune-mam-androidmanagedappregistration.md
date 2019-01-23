---
title: androidManagedAppRegistration リソースの種類
description: 特定のユーザーに対する、Android アプリの管理機能との同期の詳細を表します。 ManagedAppRegistration リソースは、組織のメンバーに使用されるアプリの詳細を管理機能と共に示します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 627de31a0d51aea6f91a10adf9c2cfb3da95b588
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395539"
---
# <a name="androidmanagedappregistration-resource-type"></a>androidManagedAppRegistration リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

特定のユーザーに対する、Android アプリの管理機能との同期の詳細を表します。
ManagedAppRegistration リソースは、組織のメンバーに使用されるアプリの詳細を管理機能と共に示します。


[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[androidManagedAppRegistrations のリスト](../api/intune-mam-androidmanagedappregistration-list.md)|[androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) コレクション|[androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[androidManagedAppRegistration の取得](../api/intune-mam-androidmanagedappregistration-get.md)|[androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md)|[androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[androidManagedAppRegistration の作成](../api/intune-mam-androidmanagedappregistration-create.md)|[androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md)|新しい [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) オブジェクトを作成します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|作成日時 ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)。|
|lastSyncDateTime|DateTimeOffset|アプリが管理サービスと最後に同期した日時。 [managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します|
|applicationVersion|String|アプリのバージョン ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)|
|managementSdkVersion|String|アプリ管理 SDK のバージョン ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)|
|platformVersion|String|オペレーティング システムのバージョン ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)|
|deviceType|String|ホスト デバイスの種類 ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)|
|deviceTag|String|アプリ管理 SDK が生成したタグ。同じデバイスでホストされているアプリの関連付けに役立ちます。 あらゆる状況でのアプリの関連付けを保証するものではありません。 [managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します|
|deviceName|String|ホスト デバイスの名前 ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)|
|managedDeviceId|String|ホスト ・ デバイスの管理デバイスの識別子です。 ホスト ・ デバイスが管理されている場合にも、値を空にする可能性があります。 [managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します|
|azureADDeviceId|String|ホスト ・ デバイスの Azure Active Directory のデバイスの識別子です。 ホスト ・ デバイスは、Azure Active Directory が登録されている場合でも、値を空にする可能性があります。 [managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します|
|deviceModel|String|[ManagedAppRegistration](../resources/intune-mam-managedappregistration.md)から現在のアプリケーション登録継承用のデバイス モデル|
|deviceManufacturer|String|[ManagedAppRegistration](../resources/intune-mam-managedappregistration.md)から現在のアプリケーション登録継承のデバイスの製造元|
|flaggedReasons|[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)コレクション|アプリ登録にフラグが設定された、0 個以上の理由。 例: ルートのデバイス上で実行されているアプリ ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)|
|userId|String|このアプリの登録が属するユーザー ID。 [managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します|
|appIdentifier|[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)|アプリ パッケージの識別子 ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)|
|id|String|エンティティのキー。 [managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します|
|version|String|エンティティのバージョン。 [managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します|
|patchVersion|String|現在 android アプリの登録の修正プログラムのバージョン|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|appliedPolicies|[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション|登録済みのアプリが管理サービスと最後に同期したときに、すでに適用されていた 0 個以上のポリシーです。 [managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します|
|intendedPolicies|[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション|現時点で、管理者がアプリに対して意図した 0 個以上のポリシーです。 [managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します|
|operations|[managedAppOperation](../resources/intune-mam-managedappoperation.md) コレクション|アプリ登録でトリガーされた、0 個以上の長時間実行の操作です。 [managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidManagedAppRegistration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
  "createdDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "applicationVersion": "String",
  "managementSdkVersion": "String",
  "platformVersion": "String",
  "deviceType": "String",
  "deviceTag": "String",
  "deviceName": "String",
  "managedDeviceId": "String",
  "azureADDeviceId": "String",
  "deviceModel": "String",
  "deviceManufacturer": "String",
  "flaggedReasons": [
    "String"
  ],
  "userId": "String",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "String"
  },
  "id": "String (identifier)",
  "version": "String",
  "patchVersion": "String"
}
```




