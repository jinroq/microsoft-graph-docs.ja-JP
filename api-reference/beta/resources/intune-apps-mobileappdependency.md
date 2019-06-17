---
title: mobileAppDependency リソースの種類
description: 2つのモバイルアプリ間の依存関係の種類を表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4a29f658a67c3930b1b693589dc9115c0c1ff185
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990261"
---
# <a name="mobileappdependency-resource-type"></a>mobileAppDependency リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

2つのモバイルアプリ間の依存関係の種類を表します。


[MobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト mobileAppDependencies](../api/intune-apps-mobileappdependency-list.md)|[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)コレクション|[MobileAppDependency](../resources/intune-apps-mobileappdependency.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[MobileAppDependency を取得する](../api/intune-apps-mobileappdependency-get.md)|[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)|[MobileAppDependency](../resources/intune-apps-mobileappdependency.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[MobileAppDependency を作成する](../api/intune-apps-mobileappdependency-create.md)|[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)|新しい[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)オブジェクトを作成します。|
|[MobileAppDependency の削除](../api/intune-apps-mobileappdependency-delete.md)|None|[MobileAppDependency](../resources/intune-apps-mobileappdependency.md)を削除します。|
|[MobileAppDependency の更新](../api/intune-apps-mobileappdependency-update.md)|[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)|[MobileAppDependency](../resources/intune-apps-mobileappdependency.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|リレーションシップエンティティ id。[MobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)から継承します。|
|targetId|String|ターゲットの子モバイルアプリのアプリ id。[MobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)から継承します。|
|targetDisplayName|String|ターゲットの子モバイルアプリの表示名。 [MobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)から継承します。|
|dependencyType|[mobileAppDependencyType](../resources/intune-apps-mobileappdependencytype.md)|親アプリと子アプリ間の依存関係の種類。 可能な値は、`detect`、`autoInstall` です。|
|dependentAppCount|Int32|子アプリが持つ依存関係の合計数。|

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





