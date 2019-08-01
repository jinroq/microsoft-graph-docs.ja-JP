---
title: androidManagedAppRegistration リソースの種類
description: 特定のユーザーに対する、Android アプリの管理機能との同期の詳細を表します。 ManagedAppRegistration リソースは、組織のメンバーに使用されるアプリの詳細を管理機能と共に示します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7505c6183c628e26528b7fe2820373a8be17d359
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027336"
---
# <a name="androidmanagedappregistration-resource-type"></a>androidManagedAppRegistration リソースの種類

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

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
|flaggedReasons|[Managedappflaggedreason](../resources/intune-mam-managedappflaggedreason.md)コレクション|アプリ登録にフラグが設定された、0 個以上の理由。 例: ルートのデバイス上で実行されているアプリ ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)|
|userId|String|このアプリの登録が属するユーザー ID。 [managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します|
|appIdentifier|[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)|アプリ パッケージの識別子 ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)|
|id|文字列|エンティティのキー。 [managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します|
|version|文字列型 (String)|エンティティのバージョン。 [managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します|

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
  "flaggedReasons": [
    "String"
  ],
  "userId": "String",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "String"
  },
  "id": "String (identifier)",
  "version": "String"
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: /api-reference/v1.0/resources/intune-mam-androidmanagedappregistration.md/microsoft.graph.androidManagedAppRegistration/appIdentifier:
      Type mismatch between example and table. Parameter name: appIdentifier; example type: (microsoft.graph.androidMobileAppIdentifier); table type: (microsoft.graph.mobileAppIdentifier)",
      "Warning: /api-reference/v1.0/resources/intune-mam-androidmanagedappregistration.md/microsoft.graph.androidManagedAppRegistration/flaggedReasons:

      Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->
 
