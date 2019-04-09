---
title: devicemanagementintentuserstate リソースの種類
description: 目的のユーザー状態を表すエンティティ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 67d8a11816132d0867987c80325f100d5e9a1ecd
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2019
ms.locfileid: "31524331"
---
# <a name="devicemanagementintentuserstate-resource-type"></a>devicemanagementintentuserstate リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

目的のユーザー状態を表すエンティティ

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[devicemanagementintentuserstates のリスト](../api/intune-deviceintent-devicemanagementintentuserstate-list.md)|[devicemanagementintentuserstate](../resources/intune-deviceintent-devicemanagementintentuserstate.md)コレクション|[devicemanagementintentuserstate](../resources/intune-deviceintent-devicemanagementintentuserstate.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[devicemanagementintentuserstate の取得](../api/intune-deviceintent-devicemanagementintentuserstate-get.md)|[devicemanagementintentuserstate](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|[devicemanagementintentuserstate](../resources/intune-deviceintent-devicemanagementintentuserstate.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[devicemanagementintentuserstate の作成](../api/intune-deviceintent-devicemanagementintentuserstate-create.md)|[devicemanagementintentuserstate](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|新しい[devicemanagementintentuserstate](../resources/intune-deviceintent-devicemanagementintentuserstate.md)オブジェクトを作成します。|
|[devicemanagementintentuserstate の削除](../api/intune-deviceintent-devicemanagementintentuserstate-delete.md)|なし|[devicemanagementintentuserstate](../resources/intune-deviceintent-devicemanagementintentuserstate.md)を削除します。|
|[devicemanagementintentuserstate の更新](../api/intune-deviceintent-devicemanagementintentuserstate-update.md)|[devicemanagementintentuserstate](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|[devicemanagementintentuserstate](../resources/intune-deviceintent-devicemanagementintentuserstate.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|ID|
|userPrincipalName|String|デバイスで報告されているユーザープリンシパル名|
|userName|String|デバイスで報告されているユーザー名|
|deviceCount|Int32|目的のためにユーザーに属しているデバイスの数|
|lastReportedDateTime|DateTimeOffset|インテントレポートの最終更新日時|
|state|[complianceStatus](../resources/intune-shared-compliancestatus.md)|目的のユーザー状態。 可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentUserState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserState",
  "id": "String (identifier)",
  "userPrincipalName": "String",
  "userName": "String",
  "deviceCount": 1024,
  "lastReportedDateTime": "String (timestamp)",
  "state": "String"
}
```







