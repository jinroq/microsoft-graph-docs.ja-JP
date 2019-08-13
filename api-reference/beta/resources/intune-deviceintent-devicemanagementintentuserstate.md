---
title: deviceManagementIntentUserState リソースの種類
description: 目的のユーザー状態を表すエンティティ
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1ad8fe7e61f883bae43522a0aaafecacaf090be0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371363"
---
# <a name="devicemanagementintentuserstate-resource-type"></a>deviceManagementIntentUserState リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

目的のユーザー状態を表すエンティティ

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[DeviceManagementIntentUserStates のリスト](../api/intune-deviceintent-devicemanagementintentuserstate-list.md)|[Devicemanagementintentuserstate](../resources/intune-deviceintent-devicemanagementintentuserstate.md)コレクション|[Devicemanagementintentuserstate](../resources/intune-deviceintent-devicemanagementintentuserstate.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[DeviceManagementIntentUserState の取得](../api/intune-deviceintent-devicemanagementintentuserstate-get.md)|[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|[Devicemanagementintentuserstate](../resources/intune-deviceintent-devicemanagementintentuserstate.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[DeviceManagementIntentUserState の作成](../api/intune-deviceintent-devicemanagementintentuserstate-create.md)|[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|新しい[Devicemanagementintentuserstate](../resources/intune-deviceintent-devicemanagementintentuserstate.md)オブジェクトを作成します。|
|[DeviceManagementIntentUserState の削除](../api/intune-deviceintent-devicemanagementintentuserstate-delete.md)|None|[Devicemanagementintentuserstate](../resources/intune-deviceintent-devicemanagementintentuserstate.md)を削除します。|
|[DeviceManagementIntentUserState の更新](../api/intune-deviceintent-devicemanagementintentuserstate-update.md)|[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|[Devicemanagementintentuserstate](../resources/intune-deviceintent-devicemanagementintentuserstate.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|ID|
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



