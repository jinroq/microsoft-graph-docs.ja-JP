---
title: devicemanagementcomplexsettinginstance リソースの種類
description: 複雑な値を表す設定インスタンス
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 52be2b37eff10c7d03ac20a731044fd9cdd97d68
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2019
ms.locfileid: "31523673"
---
# <a name="devicemanagementcomplexsettinginstance-resource-type"></a>devicemanagementcomplexsettinginstance リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

複雑な値を表す設定インスタンス


[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[devicemanagementcomplexsettinginstances を一覧表示する](../api/intune-deviceintent-devicemanagementcomplexsettinginstance-list.md)|[devicemanagementcomplexsettinginstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)コレクション|[devicemanagementcomplexsettinginstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[devicemanagementcomplexsettinginstance を取得する](../api/intune-deviceintent-devicemanagementcomplexsettinginstance-get.md)|[devicemanagementcomplexsettinginstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)|[devicemanagementcomplexsettinginstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[devicemanagementcomplexsettinginstance の作成](../api/intune-deviceintent-devicemanagementcomplexsettinginstance-create.md)|[devicemanagementcomplexsettinginstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)|新しい[devicemanagementcomplexsettinginstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)オブジェクトを作成します。|
|[devicemanagementcomplexsettinginstance の削除](../api/intune-deviceintent-devicemanagementcomplexsettinginstance-delete.md)|なし|[devicemanagementcomplexsettinginstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)を削除します。|
|[devicemanagementcomplexsettinginstance の更新](../api/intune-deviceintent-devicemanagementcomplexsettinginstance-update.md)|[devicemanagementcomplexsettinginstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)|[devicemanagementcomplexsettinginstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された設定インスタンス ID|
|definitionId|文字列|[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承されたこのインスタンスの設定定義の ID|
|valuejson|文字列|[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された値の JSON 表現|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|value|[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)コレクション|複合設定を構成する値|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementComplexSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String"
}
```







