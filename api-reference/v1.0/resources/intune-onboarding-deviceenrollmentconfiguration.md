---
title: deviceEnrollmentConfiguration リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fc515f291e2ab32b744756063869ca3ca0c86cb5
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259578"
---
# <a name="deviceenrollmentconfiguration-resource-type"></a>deviceEnrollmentConfiguration リソースの種類

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

まだ文書化されていません

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List deviceEnrollmentConfigurations](../api/intune-onboarding-deviceenrollmentconfiguration-list.md)|[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) コレクション|[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get deviceEnrollmentConfiguration](../api/intune-onboarding-deviceenrollmentconfiguration-get.md)|[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[setPriority アクション](../api/intune-onboarding-deviceenrollmentconfiguration-setpriority.md)|なし|まだ文書化されていません|
|[assign アクション](../api/intune-onboarding-deviceenrollmentconfiguration-assign.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|まだ文書化されていません|
|displayName|String|まだ文書化されていません|
|説明|String|まだ文書化されていません|
|priority|Int32|まだ文書化されていません|
|createdDateTime|DateTimeOffset|まだ文書化されていません|
|lastModifiedDateTime|DateTimeOffset|まだ文書化されていません|
|version|Int32|まだ文書化されていません|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|assignments|[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) コレクション|デバイスの構成プロファイルのグループ割り当てのリストです。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024
}
```



