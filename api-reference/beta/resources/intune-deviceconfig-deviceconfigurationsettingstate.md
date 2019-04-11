---
title: deviceConfigurationSettingState リソースの種類
description: 指定されたデバイスのデバイス構成設定の状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2f24c08a2f2345f44ee4350ec5cd7d9415b2d6b5
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31790600"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a>deviceConfigurationSettingState リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

指定されたデバイスのデバイス構成設定の状態。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|setting|文字列|レポートされる設定値。|
|settingName|文字列|レポートされている、ローカライズされた設定名またはユーザー フレンドリな設定名|
|instanceDisplayName|文字列|レポートされている設定インスタンスの名前です。|
|state|[complianceStatus](../resources/intune-shared-compliancestatus.md)|設定のコンプライアンス状態。 可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。|
|errorCode|Int64|設定のエラー コード|
|errorDescription|文字列|エラーの説明|
|userId|文字列|UserId|
|userName|文字列|UserName|
|userEmail|文字列|UserEmail|
|userPrincipalName|String|UserPrincipalName。|
|sources|[settingSource](../resources/intune-deviceconfig-settingsource.md) コレクション|投稿ポリシー|
|currentValue|String|デバイスに関する設定の現在の値|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceConfigurationSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationSettingState",
  "setting": "String",
  "settingName": "String",
  "instanceDisplayName": "String",
  "state": "String",
  "errorCode": 1024,
  "errorDescription": "String",
  "userId": "String",
  "userName": "String",
  "userEmail": "String",
  "userPrincipalName": "String",
  "sources": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "String",
      "displayName": "String"
    }
  ],
  "currentValue": "String"
}
```





