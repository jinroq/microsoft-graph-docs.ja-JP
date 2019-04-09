---
title: securityBaselineDeviceState リソースの種類
description: デバイスのセキュリティベースラインのセキュリティベースラインコンプライアンスの状態の要約。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d32e5523f540d5b9fa2e517efe88bc123825ae6b
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522532"
---
# <a name="securitybaselinedevicestate-resource-type"></a>securityBaselineDeviceState リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイスのセキュリティベースラインのセキュリティベースラインコンプライアンスの状態の要約。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト securityBaselineDeviceStates](../api/intune-deviceintent-securitybaselinedevicestate-list.md)|[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)コレクション|[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[securityBaselineDeviceState を取得する](../api/intune-deviceintent-securitybaselinedevicestate-get.md)|[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)|[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[securityBaselineDeviceState を作成する](../api/intune-deviceintent-securitybaselinedevicestate-create.md)|[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)|新しい[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)オブジェクトを作成します。|
|[securityBaselineDeviceState の削除](../api/intune-deviceintent-securitybaselinedevicestate-delete.md)|なし|[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)を削除します。|
|[securityBaselineDeviceState の更新](../api/intune-deviceintent-securitybaselinedevicestate-update.md)|[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)|[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティの一意識別子|
|manageddeviceid|文字列|Intune デバイス id|
|deviceDisplayName|String|デバイスの表示名|
|userPrincipalName|String|ユーザー プリンシパル名|
|state|[securityBaselineComplianceState](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|セキュリティベースラインコンプライアンスの状態。 可能な値は `unknown`、`secure`、`notApplicable`、`notSecure`、`error`、`conflict` です。|
|lastReportedDateTime|DateTimeOffset|ポリシーレポートの最終変更日時|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineDeviceState",
  "id": "String (identifier)",
  "managedDeviceId": "String",
  "deviceDisplayName": "String",
  "userPrincipalName": "String",
  "state": "String",
  "lastReportedDateTime": "String (timestamp)"
}
```







