---
title: devicemanagementintent リソースの種類
description: デバイスに設定を適用する目的を表すエンティティ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 909b071279b35c2ffec4c27b3431d25f7da8ac46
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2019
ms.locfileid: "31524247"
---
# <a name="devicemanagementintent-resource-type"></a>devicemanagementintent リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイスに設定を適用する目的を表すエンティティ

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[devicemanagementintents を一覧表示する](../api/intune-deviceintent-devicemanagementintent-list.md)|[devicemanagementintent](../resources/intune-deviceintent-devicemanagementintent.md)コレクション|[devicemanagementintent](../resources/intune-deviceintent-devicemanagementintent.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[devicemanagementintent の取得](../api/intune-deviceintent-devicemanagementintent-get.md)|[devicemanagementintent](../resources/intune-deviceintent-devicemanagementintent.md)|[devicemanagementintent](../resources/intune-deviceintent-devicemanagementintent.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[devicemanagementintent の作成](../api/intune-deviceintent-devicemanagementintent-create.md)|[devicemanagementintent](../resources/intune-deviceintent-devicemanagementintent.md)|新しい[devicemanagementintent](../resources/intune-deviceintent-devicemanagementintent.md)オブジェクトを作成します。|
|[devicemanagementintent の削除](../api/intune-deviceintent-devicemanagementintent-delete.md)|なし|[devicemanagementintent](../resources/intune-deviceintent-devicemanagementintent.md)を削除します。|
|[devicemanagementintent の更新](../api/intune-deviceintent-devicemanagementintent-update.md)|[devicemanagementintent](../resources/intune-deviceintent-devicemanagementintent.md)|[devicemanagementintent](../resources/intune-deviceintent-devicemanagementintent.md)オブジェクトのプロパティを更新します。|
|[updatesettings アクション](../api/intune-deviceintent-devicemanagementintent-updatesettings.md)|なし|まだ文書化されていません|
|[アクションの割り当て](../api/intune-deviceintent-devicemanagementintent-assign.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|インテント ID|
|displayName|String|ユーザーが指定した表示名|
|説明|String|ユーザーが指定した説明|
|isAssigned|Boolean|目的がユーザーに割り当てられているかどうかを表します。|
|lastModifiedDateTime|DateTimeOffset|目的が最後に変更された日時|
|templateId|文字列|この目的が作成されたテンプレートの ID (存在する場合)|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|settings|[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)コレクション|適用されるすべての設定のコレクション|
|categories|[devicemanagementintentsettingcategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)コレクション|目的内のカテゴリ設定のコレクション|
|assignments|[devicemanagementintentassignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)コレクション|割り当てのコレクション|
|deviceSettingStateSummaries|[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)コレクション|目的内のすべての設定について、対応する状態に属するデバイスの設定とその状態、およびそれらの状態のコレクション。|
|deviceStates|[devicemanagementintentdevicestate](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)コレクション|目的が適用されているすべてのデバイスの状態のコレクション|
|userstates|[devicemanagementintentuserstate](../resources/intune-deviceintent-devicemanagementintentuserstate.md)コレクション|目的が適用されているすべてのユーザーの状態のコレクション|
|deviceStateSummary|[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|目的が適用されているすべてのデバイスについて、対応する状態に属するデバイスの状態と数の概要|
|userStateSummary|[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|目的が適用されているすべてのユーザーについて、対応する状態に属するユーザーの状態と数の概要|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntent",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "isAssigned": true,
  "lastModifiedDateTime": "String (timestamp)",
  "templateId": "String"
}
```







