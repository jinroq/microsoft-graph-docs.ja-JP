---
title: deviceManagementExchangeOnPremisesPolicy リソースの種類
description: テナントに対して構成された Exchange OnPremises ポリシーを表すシングルトンエンティティ。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: aea09b84b2c028e70bde3f509b74f1e785bc7d61
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367478"
---
# <a name="devicemanagementexchangeonpremisespolicy-resource-type"></a>deviceManagementExchangeOnPremisesPolicy リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

テナントに対して構成された Exchange OnPremises ポリシーを表すシングルトンエンティティ。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[DeviceManagementExchangeOnPremisesPolicy を取得する](../api/intune-onboarding-devicemanagementexchangeonpremisespolicy-get.md)|[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|[DeviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[DeviceManagementExchangeOnPremisesPolicy の更新](../api/intune-onboarding-devicemanagementexchangeonpremisespolicy-update.md)|[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|[DeviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|まだ文書化されていません|
|notificationContent|Binary|このポリシーによって検疫されたユーザーに送信される通知テキスト。 これは、UTF8 でエンコードされたバイト配列 HTML です。|
|defaultAccessLevel|[deviceManagementExchangeAccessLevel](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|Exchange の既定のアクセス状態。 このルールは、Exchange 組織全体にグローバルに適用されます。 使用可能な値は、`none`、`allow`、`block`、`quarantine` です。|
|accessRules|[Devicemanagementexchangeaccessrule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md)コレクション|Exchange のデバイスアクセスルールの一覧。 アクセスルールは、Exchange 組織全体にグローバルに適用されます。|
|knownDeviceClasses 場合|[Devicemanagementexchangedeviceclass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)コレクション|Exchange に認識されているデバイスクラスの一覧|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|Exchange のオンプレミスでの条件付きアクセス設定。 オンプレミスの条件付きアクセスでは、デバイスを登録し、メール アクセスに準拠させる必要があります|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementExchangeOnPremisesPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeOnPremisesPolicy",
  "id": "String (identifier)",
  "notificationContent": "binary",
  "defaultAccessLevel": "String",
  "accessRules": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule",
      "deviceClass": {
        "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
        "name": "String",
        "type": "String"
      },
      "accessLevel": "String"
    }
  ],
  "knownDeviceClasses": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
      "name": "String",
      "type": "String"
    }
  ]
}
```



