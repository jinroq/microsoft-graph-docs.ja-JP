---
title: devicemanagementintentsettingcategory リソースの種類
description: 意図の設定カテゴリを表すエンティティ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1551d4d4217b03380feef46d07d9f0cc5dac4064
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550701"
---
# <a name="devicemanagementintentsettingcategory-resource-type"></a>devicemanagementintentsettingcategory リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

意図の設定カテゴリを表すエンティティ


[devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[devicemanagementintentsettingcategories のリスト](../api/intune-deviceintent-devicemanagementintentsettingcategory-list.md)|[devicemanagementintentsettingcategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)コレクション|[devicemanagementintentsettingcategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[devicemanagementintentsettingcategory の取得](../api/intune-deviceintent-devicemanagementintentsettingcategory-get.md)|[deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|[devicemanagementintentsettingcategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[devicemanagementintentsettingcategory の作成](../api/intune-deviceintent-devicemanagementintentsettingcategory-create.md)|[deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|新しい[devicemanagementintentsettingcategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)オブジェクトを作成します。|
|[devicemanagementintentsettingcategory の削除](../api/intune-deviceintent-devicemanagementintentsettingcategory-delete.md)|なし|[devicemanagementintentsettingcategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)を削除します。|
|[devicemanagementintentsettingcategory の更新](../api/intune-deviceintent-devicemanagementintentsettingcategory-update.md)|[deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|[devicemanagementintentsettingcategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|[devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)から継承されるカテゴリ ID|
|displayName|String|[devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)から継承されるカテゴリ名|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|settingdefinitions|[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)コレクション|このカテゴリには、 [devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)から継承する設定定義が含まれます。|
|settings|[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)コレクション|このカテゴリに含まれる設定|

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





