---
title: securityBaselineState リソースの種類
description: デバイスのセキュリティベースラインの状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3c81a3d351c7c1e854c26e05e32f8426ffdc0631
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2019
ms.locfileid: "31524562"
---
# <a name="securitybaselinestate-resource-type"></a>securityBaselineState リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイスのセキュリティベースラインの状態。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト securityBaselineStates](../api/intune-deviceintent-securitybaselinestate-list.md)|[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)コレクション|[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[securityBaselineState を取得する](../api/intune-deviceintent-securitybaselinestate-get.md)|[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)|[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[securityBaselineState を作成する](../api/intune-deviceintent-securitybaselinestate-create.md)|[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)|新しい[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)オブジェクトを作成します。|
|[securityBaselineState の削除](../api/intune-deviceintent-securitybaselinestate-delete.md)|なし|[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)を削除します。|
|[securityBaselineState の更新](../api/intune-deviceintent-securitybaselinestate-update.md)|[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)|[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|securityBaselineTemplateId|文字列|セキュリティ基準テンプレート id|
|displayName|String|セキュリティベースラインの表示名|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|settingStates|[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)コレクション|デバイスのさまざまな設定のセキュリティベースライン状態|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineState",
  "id": "String (identifier)",
  "securityBaselineTemplateId": "String",
  "displayName": "String"
}
```



