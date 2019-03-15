---
title: androidManagedAppRegistration の作成
description: 新しい androidManagedAppRegistration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0c05ba7fa13577134b148c8af836e3ba453a1e40
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571460"
---
# <a name="create-androidmanagedappregistration"></a>androidManagedAppRegistration の作成

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

新しい [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) オブジェクトを作成します。

## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校のアカウント)|DeviceManagementApps.ReadWrite.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません。|
|アプリケーション|サポートされていません。|

## <a name="http-request"></a>HTTP 要求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必要です。|
|承諾|application/json|

## <a name="request-body"></a>要求本文
要求本文で、androidManagedAppRegistration オブジェクトの JSON 表記を指定します。

次の表に、androidManagedAppRegistration の作成時に必要なプロパティを示します。

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
|manageddeviceid|String|ホストデバイスの管理デバイス識別子。 ホストデバイスが管理されている場合でも、値を空にすることができます。 [managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します|
|azureADDeviceId|String|ホストデバイスの Azure Active Directory デバイス識別子。 ホストデバイスが Azure Active Directory に登録されている場合でも、値を空にすることができます。 [managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します|
|deviceModel|String|[managedAppRegistration](../resources/intune-mam-managedappregistration.md)から継承された現在のアプリの登録のデバイスモデル。|
|deviceManufacturer|String|[managedAppRegistration](../resources/intune-mam-managedappregistration.md)から継承された現在のアプリの登録のデバイスの製造元|
|flaggedReasons|[managedappflaggedreason](../resources/intune-mam-managedappflaggedreason.md)コレクション|アプリ登録にフラグが設定された、0 個以上の理由。 例: [managedAppRegistration](../resources/intune-mam-managedappregistration.md)から継承されたルートデバイスで実行されているアプリ。 可能な値は、`none`、`rootedDevice`、`androidBootloaderUnlocked`、`androidFactoryRomModified` です。|
|userId|String|このアプリの登録が属するユーザー ID。 [managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します|
|appIdentifier|[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)|アプリ パッケージの識別子 ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)|
|id|String|エンティティのキー。 [managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します|
|version|文字列型 (String)|エンティティのバージョン。 [managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します|
|パッチバージョン|String|現在の android アプリの登録のパッチバージョン|



## <a name="response"></a>応答
成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations
Content-type: application/json
Content-length: 879

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "managedDeviceId": "Managed Device Id value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "version": "Version value",
  "patchVersion": "Patch Version value"
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 987

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "managedDeviceId": "Managed Device Id value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "id": "0e064997-4997-0e06-9749-060e9749060e",
  "version": "Version value",
  "patchVersion": "Patch Version value"
}
```




