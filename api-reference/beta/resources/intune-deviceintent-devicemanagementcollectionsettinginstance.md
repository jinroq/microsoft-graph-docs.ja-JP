---
title: devicemanagementcollectionsettinginstance リソースの種類
description: 値のコレクションを表す設定インスタンス
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 673268ce6679ea0dea393de4949cc005fa03c832
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523344"
---
# <a name="devicemanagementcollectionsettinginstance-resource-type"></a>devicemanagementcollectionsettinginstance リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

値のコレクションを表す設定インスタンス


[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[devicemanagementcollectionsettinginstances を一覧表示する](../api/intune-deviceintent-devicemanagementcollectionsettinginstance-list.md)|[devicemanagementcollectionsettinginstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)コレクション|[devicemanagementcollectionsettinginstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[devicemanagementcollectionsettinginstance を取得する](../api/intune-deviceintent-devicemanagementcollectionsettinginstance-get.md)|[deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)|[devicemanagementcollectionsettinginstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[devicemanagementcollectionsettinginstance の作成](../api/intune-deviceintent-devicemanagementcollectionsettinginstance-create.md)|[deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)|新しい[devicemanagementcollectionsettinginstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)オブジェクトを作成します。|
|[devicemanagementcollectionsettinginstance の削除](../api/intune-deviceintent-devicemanagementcollectionsettinginstance-delete.md)|なし|[devicemanagementcollectionsettinginstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)を削除します。|
|[devicemanagementcollectionsettinginstance の更新](../api/intune-deviceintent-devicemanagementcollectionsettinginstance-update.md)|[deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)|[devicemanagementcollectionsettinginstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|id|String|[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された設定インスタンス ID|
|definitionId|String|[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承されたこのインスタンスの設定定義の ID|
|valuejson|String|[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された値の JSON 表現|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|value|[devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)コレクション|値のコレクション|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementCollectionSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String"
}
```





