---
title: mobileContainedApp リソースの種類
description: パッケージとして機能する mobileApp に含まれているアプリを表す抽象クラス。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c3400349244e738644d4885b2265c5f7f4ceb84e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145200"
---
# <a name="mobilecontainedapp-resource-type"></a>mobileContainedApp リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

パッケージとして機能する mobileApp に含まれているアプリを表す抽象クラス。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト mobileContainedApps](../api/intune-apps-mobilecontainedapp-list.md)|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)コレクション|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[mobileContainedApp を取得する](../api/intune-apps-mobilecontainedapp-get.md)|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)オブジェクトのプロパティとリレーションシップを読み取ります。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileContainedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileContainedApp",
  "id": "String (identifier)"
}
```




