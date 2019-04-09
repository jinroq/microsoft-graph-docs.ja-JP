---
title: devicemanagementsettingcategory リソースの種類
description: 設定カテゴリを表すエンティティ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7c373ef2bfa72bf08e6259ece1166b4e10101789
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522504"
---
# <a name="devicemanagementsettingcategory-resource-type"></a>devicemanagementsettingcategory リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

設定カテゴリを表すエンティティ

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[devicemanagementsettingcategories を一覧表示する](../api/intune-deviceintent-devicemanagementsettingcategory-list.md)|[devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)コレクション|[devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[devicemanagementsettingcategory の取得](../api/intune-deviceintent-devicemanagementsettingcategory-get.md)|[devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|[devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[devicemanagementsettingcategory の作成](../api/intune-deviceintent-devicemanagementsettingcategory-create.md)|[devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|新しい[devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)オブジェクトを作成します。|
|[devicemanagementsettingcategory の削除](../api/intune-deviceintent-devicemanagementsettingcategory-delete.md)|なし|[devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)を削除します。|
|[devicemanagementsettingcategory の更新](../api/intune-deviceintent-devicemanagementsettingcategory-update.md)|[devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|[devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|カテゴリ ID|
|displayName|String|カテゴリ名|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|settingdefinitions|[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)コレクション|このカテゴリに含まれる設定の定義は次のとおりです。|

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







