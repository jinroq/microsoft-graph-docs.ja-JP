---
title: windows10AppsForceUpdateSchedule リソースの種類
description: アプリの Windows 10 強制更新スケジュール
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7aa5573c3d644299b9c0aa424f348a67db8379d0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158227"
---
# <a name="windows10appsforceupdateschedule-resource-type"></a>windows10AppsForceUpdateSchedule リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

アプリの Windows 10 強制更新スケジュール

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|startDateTime|DateTimeOffset|強制再起動の開始時刻。|
|recurrence|[windows10AppsUpdateRecurrence](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|定期的なスケジュール。 使用可能な値は、`none`、`daily`、`weekly`、`monthly` です。|
|runImmediatelyIfAfterStartDateTime|ブール値|true の場合は、StartDateTime が過去の場合はすぐにタスクを実行します。それ以外の場合は、次の定期的なパターンが実行されます。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10AppsForceUpdateSchedule",
  "startDateTime": "String (timestamp)",
  "recurrence": "String",
  "runImmediatelyIfAfterStartDateTime": true
}
```




