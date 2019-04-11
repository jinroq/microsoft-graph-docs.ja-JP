---
title: deviceManagementExchangeOnPremisesPolicy リソースの種類
description: テナントに対して構成された Exchange onpremises ポリシーを表すシングルトンエンティティ。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d8605a3062d8808ea6a4d0b5397283f0ca82d920
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31791195"
---
# <a name="devicemanagementexchangeonpremisespolicy-resource-type"></a>deviceManagementExchangeOnPremisesPolicy リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

テナントに対して構成された Exchange onpremises ポリシーを表すシングルトンエンティティ。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[deviceManagementExchangeOnPremisesPolicy を取得する](../api/intune-onboarding-devicemanagementexchangeonpremisespolicy-get.md)|[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[deviceManagementExchangeOnPremisesPolicy の更新](../api/intune-onboarding-devicemanagementexchangeonpremisespolicy-update.md)|[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|まだ文書化されていません|
|notificationContent|Binary|このポリシーによって検疫されたユーザーに送信される通知テキスト。 これは、UTF8 でエンコードされたバイト配列 HTML です。|
|defaultaccesslevel|[devicemanagementexchangeaccesslevel](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|Exchange の既定のアクセス状態。 このルールは、Exchange 組織全体にグローバルに適用されます。 可能な値は、`none`、`allow`、`block`、`quarantine` です。|
|accessrules|[devicemanagementexchangeaccessrule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md)コレクション|Exchange のデバイスアクセスルールの一覧。 アクセスルールは、Exchange 組織全体にグローバルに適用されます。|
|knowndeviceclasses 場合|[devicemanagementexchangedeviceclass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)コレクション|Exchange に認識されているデバイスクラスの一覧|

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





