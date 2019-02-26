---
title: managementcondition リソースの種類
description: 管理条件は、地域フェンス、タイムフェンス、ネットワークフェンスなど、動的にトリガーされる可能性があるイベントです。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 594716867cec1dcef9e0fee87af21fb63af99df0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163106"
---
# <a name="managementcondition-resource-type"></a>managementcondition リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

管理条件は、地域フェンス、タイムフェンス、ネットワークフェンスなど、動的にトリガーされる可能性があるイベントです。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[managementconditions を一覧表示する](../api/intune-fencing-managementcondition-list.md)|[managementcondition](../resources/intune-fencing-managementcondition.md)コレクション|[managementcondition](../resources/intune-fencing-managementcondition.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[managementcondition の取得](../api/intune-fencing-managementcondition-get.md)|[managementcondition](../resources/intune-fencing-managementcondition.md)|[managementcondition](../resources/intune-fencing-managementcondition.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[getmanagementconditionsforplatform 関数](../api/intune-fencing-managementcondition-getmanagementconditionsforplatform.md)|[managementcondition](../resources/intune-fencing-managementcondition.md)コレクション|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|管理条件の一意識別子。 作成時に割り当てられたシステム生成値。|
|uniqueName|String|管理条件の一意の名前。 管理条件式で使用されます。|
|displayName|String|管理条件の管理者定義の名前。|
|説明|String|管理条件の管理者定義の説明。|
|createdDateTime|DateTimeOffset|管理条件が作成された時刻。 サービス側を生成しました。|
|変更された日時|DateTimeOffset|管理条件が最後に変更された時刻。 サービス側を更新しました。|
|eTag|String|管理条件の ETag。 サービス側を更新しました。|
|アプリケーションのプラットフォーム|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション|この管理条件の適用可能なプラットフォーム。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|managementconditionstatements|[managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)コレクション|管理条件に関連付けられている管理条件ステートメント。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementCondition",
  "id": "String (identifier)",
  "uniqueName": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ]
}
```




