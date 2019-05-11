---
title: deviceManagementSettingCategory リソースの種類
description: 設定カテゴリを表すエンティティ
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 39c87774cf0aa8a5e3a4cb65b10566323b2c7749
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943390"
---
# <a name="devicemanagementsettingcategory-resource-type"></a>deviceManagementSettingCategory リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

設定カテゴリを表すエンティティ

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[DeviceManagementSettingCategories を一覧表示する](../api/intune-deviceintent-devicemanagementsettingcategory-list.md)|[Devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)コレクション|[Devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[DeviceManagementSettingCategory の取得](../api/intune-deviceintent-devicemanagementsettingcategory-get.md)|[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|[Devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[DeviceManagementSettingCategory の作成](../api/intune-deviceintent-devicemanagementsettingcategory-create.md)|[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|新しい[Devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)オブジェクトを作成します。|
|[DeviceManagementSettingCategory の削除](../api/intune-deviceintent-devicemanagementsettingcategory-delete.md)|None|[Devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)を削除します。|
|[DeviceManagementSettingCategory の更新](../api/intune-deviceintent-devicemanagementsettingcategory-update.md)|[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|[Devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|id|文字列|カテゴリ ID|
|displayName|String|カテゴリ名|

## <a name="relationships"></a>関係
|リレーションシップ|型|説明|
|:---|:---|:---|
|settingDefinitions|[Devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)コレクション|このカテゴリに含まれる設定の定義は次のとおりです。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementSettingCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "id": "String (identifier)",
  "displayName": "String"
}
```




