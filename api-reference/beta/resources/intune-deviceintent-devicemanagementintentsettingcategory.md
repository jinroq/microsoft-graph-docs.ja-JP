---
title: deviceManagementIntentSettingCategory リソースの種類
description: 意図の設定カテゴリを表すエンティティ
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 90768fbc999860d2f5dcfcd8f0a71a3149ff58e2
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34963997"
---
# <a name="devicemanagementintentsettingcategory-resource-type"></a>deviceManagementIntentSettingCategory リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

意図の設定カテゴリを表すエンティティ


[Devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[DeviceManagementIntentSettingCategories のリスト](../api/intune-deviceintent-devicemanagementintentsettingcategory-list.md)|[Devicemanagementintentsettingcategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)コレクション|[Devicemanagementintentsettingcategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[DeviceManagementIntentSettingCategory の取得](../api/intune-deviceintent-devicemanagementintentsettingcategory-get.md)|[deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|[Devicemanagementintentsettingcategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[DeviceManagementIntentSettingCategory の作成](../api/intune-deviceintent-devicemanagementintentsettingcategory-create.md)|[deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|新しい[Devicemanagementintentsettingcategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)オブジェクトを作成します。|
|[DeviceManagementIntentSettingCategory の削除](../api/intune-deviceintent-devicemanagementintentsettingcategory-delete.md)|None|[Devicemanagementintentsettingcategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)を削除します。|
|[DeviceManagementIntentSettingCategory の更新](../api/intune-deviceintent-devicemanagementintentsettingcategory-update.md)|[deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|[Devicemanagementintentsettingcategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|[Devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)から継承されるカテゴリ ID|
|displayName|String|[Devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)から継承されるカテゴリ名|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|settingDefinitions|[Devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)コレクション|このカテゴリには、 [Devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)から継承する設定定義が含まれます。|
|settings|[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)コレクション|このカテゴリに含まれる設定|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentSettingCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentSettingCategory",
  "id": "String (identifier)",
  "displayName": "String"
}
```





