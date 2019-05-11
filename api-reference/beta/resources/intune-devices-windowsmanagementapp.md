---
title: windowsManagementApp リソースの種類
description: Windows management app エンティティ。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4525767a81b0e69ed1c99ae4b1a20051304cf1f2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941913"
---
# <a name="windowsmanagementapp-resource-type"></a>windowsManagementApp リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Windows management app エンティティ。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[WindowsManagementApp の取得](../api/intune-devices-windowsmanagementapp-get.md)|[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)|[Windowsmanagementapp](../resources/intune-devices-windowsmanagementapp.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[WindowsManagementApp の更新](../api/intune-devices-windowsmanagementapp-update.md)|[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)|[Windowsmanagementapp](../resources/intune-devices-windowsmanagementapp.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|id|String|Windows management アプリの一意識別子|
|プロパティ availableversion|String|Windows management アプリの利用可能なバージョン。|

## <a name="relationships"></a>関係
|リレーションシップ|型|説明|
|:---|:---|:---|
|healthSummary|[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)|Windows management アプリの正常性の概要。|
|healthStates|[Windowsmanagementapphealthstate](../resources/intune-devices-windowsmanagementapphealthstate.md)コレクション|インストールされている Windows management アプリの正常性状態の一覧。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "id": "String (identifier)",
  "availableVersion": "String"
}
```




