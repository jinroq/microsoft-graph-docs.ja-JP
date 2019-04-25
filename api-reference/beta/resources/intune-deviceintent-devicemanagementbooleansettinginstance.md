---
title: deviceManagementBooleanSettingInstance リソースの種類
description: ブール値を表す設定インスタンス
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ff746cc368ba3048075ce795f514709ad2866bee
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523547"
---
# <a name="devicemanagementbooleansettinginstance-resource-type"></a>deviceManagementBooleanSettingInstance リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ブール値を表す設定インスタンス


[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト deviceManagementBooleanSettingInstances](../api/intune-deviceintent-devicemanagementbooleansettinginstance-list.md)|[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)コレクション|[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[deviceManagementBooleanSettingInstance を取得する](../api/intune-deviceintent-devicemanagementbooleansettinginstance-get.md)|[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)|[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[deviceManagementBooleanSettingInstance を作成する](../api/intune-deviceintent-devicemanagementbooleansettinginstance-create.md)|[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)|新しい[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)オブジェクトを作成します。|
|[deviceManagementBooleanSettingInstance の削除](../api/intune-deviceintent-devicemanagementbooleansettinginstance-delete.md)|なし|[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)を削除します。|
|[deviceManagementBooleanSettingInstance の更新](../api/intune-deviceintent-devicemanagementbooleansettinginstance-update.md)|[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)|[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された設定インスタンス ID|
|definitionId|String|[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承されたこのインスタンスの設定定義の ID|
|valuejson|String|[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された値の JSON 表現|
|value|ブール型 (Boolean)|ブール値|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementBooleanSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementBooleanSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String",
  "value": true
}
```





