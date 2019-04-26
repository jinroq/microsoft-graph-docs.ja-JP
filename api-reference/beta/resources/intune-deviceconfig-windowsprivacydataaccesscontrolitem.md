---
title: windowsPrivacyDataAccessControlItem リソースの種類
description: プライバシーデータカテゴリごとにアクセス制御レベルを指定する
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 18cae7e3afe2d9deb0efd55092b1fc1f5e3693b8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563785"
---
# <a name="windowsprivacydataaccesscontrolitem-resource-type"></a>windowsPrivacyDataAccessControlItem リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

プライバシーデータカテゴリごとにアクセス制御レベルを指定する

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト windowsPrivacyDataAccessControlItems](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-list.md)|[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)コレクション|[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[windowsPrivacyDataAccessControlItem を取得する](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-get.md)|[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[windowsPrivacyDataAccessControlItem を作成する](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-create.md)|[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|新しい[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)オブジェクトを作成します。|
|[windowsPrivacyDataAccessControlItem の削除](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-delete.md)|なし|[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)を削除します。|
|[windowsPrivacyDataAccessControlItem の更新](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-update.md)|[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|WindowsPrivacyDataAccessControlItem のキー。|
|accessLevel|[windowsPrivacyDataAccessLevel](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|これは、指定されたアプリケーションに割り当てられるプライバシーデータカテゴリのアクセスレベルを示します。 使用可能な値は、`notConfigured`、`forceAllow`、`forceDeny`、`userInControl` です。|
|引数 datacategory|[windowsPrivacyDataCategory](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|これは、特定のアクセス制御が適用されるプライバシーデータカテゴリを示します。 可能な値: `notConfigured`、 `accountInfo` `appsRunInBackground` `calendar` `callHistory` `camera` `contacts` `diagnosticsInfo` `email` `location` `messaging` `microphone`、、、、、、、、、、、、 `motion` `notifications` `phone` `radios` `tasks` `syncWithDevices` `trustedDevices`.|
|app・パッケージ efamilyname|String|Windows アプリのパッケージファミリ名。 設定すると、指定したアプリケーションにアクセスレベルが適用されます。|
|appDisplayName|String|Windows アプリのパッケージファミリ名。 設定すると、指定したアプリケーションにアクセスレベルが適用されます。|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsPrivacyDataAccessControlItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
  "id": "String (identifier)",
  "accessLevel": "String",
  "dataCategory": "String",
  "appPackageFamilyName": "String",
  "appDisplayName": "String"
}
```





