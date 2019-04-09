---
title: devicemanagementtemplate リソースの種類
description: デバイス設定の定義済みコレクションを表すエンティティ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3cf144ed30a017dc1f3ae84fc481568adc0d0d09
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522518"
---
# <a name="devicemanagementtemplate-resource-type"></a>devicemanagementtemplate リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイス設定の定義済みコレクションを表すエンティティ

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[devicemanagementtemplates を一覧表示する](../api/intune-deviceintent-devicemanagementtemplate-list.md)|[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)コレクション|[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[devicemanagementtemplate の取得](../api/intune-deviceintent-devicemanagementtemplate-get.md)|[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[devicemanagementtemplate の作成](../api/intune-deviceintent-devicemanagementtemplate-create.md)|[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|新しい[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトを作成します。|
|[devicemanagementtemplate の削除](../api/intune-deviceintent-devicemanagementtemplate-delete.md)|なし|[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)を削除します。|
|[devicemanagementtemplate の更新](../api/intune-deviceintent-devicemanagementtemplate-update.md)|[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトのプロパティを更新します。|
|[createInstance アクション](../api/intune-deviceintent-devicemanagementtemplate-createinstance.md)|[devicemanagementintent](../resources/intune-deviceintent-devicemanagementintent.md)|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|テンプレート ID|
|displayName|String|テンプレートの表示名|
|説明|String|テンプレートの説明|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|settings|[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)コレクション|このテンプレートに含まれるすべての設定のコレクション|
|categories|[devicemanagementtemplatesettingcategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)コレクション|テンプレート内のカテゴリ設定のコレクション|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```







