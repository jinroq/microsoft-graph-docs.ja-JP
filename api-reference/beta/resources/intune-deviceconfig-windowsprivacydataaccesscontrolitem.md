---
title: windowsPrivacyDataAccessControlItem リソースの種類
description: プライバシー データのカテゴリごとのアクセス制御レベルを指定します。
ms.openlocfilehash: b72571602b96f7b228361db4bf2526fda8def70f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074279"
---
# <a name="windowsprivacydataaccesscontrolitem-resource-type"></a>windowsPrivacyDataAccessControlItem リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

プライバシー データのカテゴリごとのアクセス制御レベルを指定します。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト windowsPrivacyDataAccessControlItems](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-list.md)|[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)コレクション|[WindowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)オブジェクトのプロパティと関係を一覧表示します。|
|[WindowsPrivacyDataAccessControlItem を取得します。](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-get.md)|[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|[WindowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)オブジェクトのプロパティと関係を参照してください。|
|[WindowsPrivacyDataAccessControlItem を作成します。](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-create.md)|[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|新しい[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)オブジェクトを作成します。|
|[WindowsPrivacyDataAccessControlItem を削除します。](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-delete.md)|なし|の[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)を削除します。|
|[WindowsPrivacyDataAccessControlItem を更新します。](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-update.md)|[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|[WindowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|WindowsPrivacyDataAccessControlItem のキー。|
|accessLevel|[windowsPrivacyDataAccessLevel](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|プライバシー データ カテゴリに、指定したアプリケーションを指定するアクセス レベルを示します。 可能な値は、`notConfigured`、`forceAllow`、`forceDeny`、`userInControl` です。|
|dataCategory|[windowsPrivacyDataCategory](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|これは、特定のアクセス制御が適用されるプライバシー データのカテゴリを示します。 使用可能な値: `notConfigured`、 `accountInfo`、 `appsRunInBackground`、 `calendar`、 `callHistory`、 `camera`、 `contacts`、 `diagnosticsInfo`、 `email`、 `location`、 `messaging`、 `microphone`、 `motion`、 `notifications`、 `phone`、 `radios`、 `tasks`、 `syncWithDevices`、 `trustedDevices`.|
|appPackageFamilyName|String|Windows アプリケーションのパッケージ ファミリ名です。 アクセス レベルを設定すると、指定したアプリケーションを適用します。|
|appDisplayName|String|Windows アプリケーションのパッケージ ファミリ名です。 アクセス レベルを設定すると、指定したアプリケーションを適用します。|

## <a name="relationships"></a>リレーションシップ
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





