---
title: devicemanagementsettinginstance リソースの種類
description: 設定インスタンスの基本型
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d9aef844dd4957b75b51f8d16014c2253b0253cc
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2019
ms.locfileid: "31523610"
---
# <a name="devicemanagementsettinginstance-resource-type"></a>devicemanagementsettinginstance リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

設定インスタンスの基本型

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[devicemanagementsettinginstances を一覧表示する](../api/intune-deviceintent-devicemanagementsettinginstance-list.md)|[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)コレクション|[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[devicemanagementsettinginstance を取得する](../api/intune-deviceintent-devicemanagementsettinginstance-get.md)|[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)オブジェクトのプロパティとリレーションシップを読み取ります。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|設定インスタンス ID|
|definitionId|文字列|このインスタンスの設定定義の ID|
|valuejson|文字列|値の JSON 表現|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String"
}
```







