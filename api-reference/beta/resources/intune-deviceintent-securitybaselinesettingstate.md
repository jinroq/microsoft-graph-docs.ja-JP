---
title: securityBaselineSettingState リソースの種類
description: デバイスの設定のセキュリティベースラインコンプライアンスの状態
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ab5dd14c0929c58b9c076d1115d487e560d80333
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562280"
---
# <a name="securitybaselinesettingstate-resource-type"></a>securityBaselineSettingState リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイスの設定のセキュリティベースラインコンプライアンスの状態

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト securityBaselineSettingStates](../api/intune-deviceintent-securitybaselinesettingstate-list.md)|[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)コレクション|[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[securityBaselineSettingState を取得する](../api/intune-deviceintent-securitybaselinesettingstate-get.md)|[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)|[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[securityBaselineSettingState を作成する](../api/intune-deviceintent-securitybaselinesettingstate-create.md)|[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)|新しい[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)オブジェクトを作成します。|
|[securityBaselineSettingState の削除](../api/intune-deviceintent-securitybaselinesettingstate-delete.md)|なし|[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)を削除します。|
|[securityBaselineSettingState の更新](../api/intune-deviceintent-securitybaselinesettingstate-update.md)|[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)|[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティの一意識別子|
|settingName|String|レポートされている設定の名前|
|state|[securityBaselineComplianceState](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|セキュリティベースライン設定のコンプライアンス状態。 使用可能な値: `unknown`、`secure`、`notApplicable`、`notSecure`、`error`、`conflict`。|
|settingcategoryid|String|この設定が属する設定カテゴリ id|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineSettingState",
  "id": "String (identifier)",
  "settingName": "String",
  "state": "String",
  "settingCategoryId": "String"
}
```



