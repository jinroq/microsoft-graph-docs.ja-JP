---
title: mobileAppDependency リソースの種類
description: 2つのモバイルアプリ間の依存関係の種類を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fbad9cc613ff97d0f627109316d58f9f0c8f1364
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551758"
---
# <a name="mobileappdependency-resource-type"></a>mobileAppDependency リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

2つのモバイルアプリ間の依存関係の種類を表します。


[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト mobileAppDependencies](../api/intune-apps-mobileappdependency-list.md)|[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)コレクション|[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[mobileAppDependency を取得する](../api/intune-apps-mobileappdependency-get.md)|[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)|[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[mobileAppDependency を作成する](../api/intune-apps-mobileappdependency-create.md)|[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)|新しい[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)オブジェクトを作成します。|
|[mobileAppDependency の削除](../api/intune-apps-mobileappdependency-delete.md)|なし|[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)を削除します。|
|[mobileAppDependency の更新](../api/intune-apps-mobileappdependency-update.md)|[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)|[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|リレーションシップエンティティ id。[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)から継承します。|
|targetId|String|ターゲットの子モバイルアプリのアプリ id。[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)から継承します。|
|targetdisplayname|String|ターゲットの子モバイルアプリの表示名。 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)から継承します。|
|dependencytype|[mobileAppDependecyType](../resources/intune-apps-mobileappdependecytype.md)|親アプリと子アプリ間の依存関係の種類。 可能な値は、`detect`、`autoInstall` です。|
|dependentappcount|Int32|子アプリが持つ依存関係の合計数。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppDependency"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "id": "String (identifier)",
  "targetId": "String",
  "targetDisplayName": "String",
  "dependencyType": "String",
  "dependentAppCount": 1024
}
```





