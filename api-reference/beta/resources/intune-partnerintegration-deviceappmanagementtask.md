---
title: deviceAppManagementTask リソースの種類
description: デバイスアプリの管理タスク。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2767ec1fee73f7bc9cdc774d53f5d985cdfd2439
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "35001889"
---
# <a name="deviceappmanagementtask-resource-type"></a>deviceAppManagementTask リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイスアプリの管理タスク。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[DeviceAppManagementTasks のリスト](../api/intune-partnerintegration-deviceappmanagementtask-list.md)|[Deviceappmanagementtask](../resources/intune-partnerintegration-deviceappmanagementtask.md)コレクション|[Deviceappmanagementtask](../resources/intune-partnerintegration-deviceappmanagementtask.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[DeviceAppManagementTask の取得](../api/intune-partnerintegration-deviceappmanagementtask-get.md)|[deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|[Deviceappmanagementtask](../resources/intune-partnerintegration-deviceappmanagementtask.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[DeviceAppManagementTask の作成](../api/intune-partnerintegration-deviceappmanagementtask-create.md)|[deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|新しい[Deviceappmanagementtask](../resources/intune-partnerintegration-deviceappmanagementtask.md)オブジェクトを作成します。|
|[DeviceAppManagementTask の削除](../api/intune-partnerintegration-deviceappmanagementtask-delete.md)|None|[Deviceappmanagementtask](../resources/intune-partnerintegration-deviceappmanagementtask.md)を削除します。|
|[DeviceAppManagementTask の更新](../api/intune-partnerintegration-deviceappmanagementtask-update.md)|[deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|[Deviceappmanagementtask](../resources/intune-partnerintegration-deviceappmanagementtask.md)オブジェクトのプロパティを更新します。|
|[updateStatus アクション](../api/intune-partnerintegration-deviceappmanagementtask-updatestatus.md)|None|タスクの状態を設定し、メモを添付します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|エンティティキー。|
|displayName|文字列|名前を指定します。|
|description|String|説明。|
|createdDateTime|DateTimeOffset|作成日を指定します。|
|dueDateTime|DateTimeOffset|期限を指定します。|
|category|[deviceAppManagementTaskCategory](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|カテゴリ。 可能な値は、`unknown`、`advancedThreatProtection` です。|
|priority|[deviceAppManagementTaskPriority](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|優先度。 可能な値は、`none`、`high`、`low` です。|
|作成者|String|作成者の電子メールアドレス。|
|creatorNotes|String|作成者からのメモ。|
|assignedTo|String|このタスクが割り当てられている管理者の名前または電子メール。|
|status|[deviceAppManagementTaskStatus](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|ステータス。 可能な値は、`unknown`、`pending`、`active`、`completed`、`rejected` です。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagementTask"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagementTask",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "dueDateTime": "String (timestamp)",
  "category": "String",
  "priority": "String",
  "creator": "String",
  "creatorNotes": "String",
  "assignedTo": "String",
  "status": "String"
}
```





