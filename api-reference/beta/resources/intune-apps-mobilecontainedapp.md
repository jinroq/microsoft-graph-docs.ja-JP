---
title: mobileContainedApp リソースの種類
description: パッケージとして機能する、mobileApp に含まれているアプリケーションを表す抽象クラスです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c5d4ed392d681d97478cb1baf5ff6f854cb74011
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425667"
---
# <a name="mobilecontainedapp-resource-type"></a>mobileContainedApp リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

パッケージとして機能する、mobileApp に含まれているアプリケーションを表す抽象クラスです。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト mobileContainedApps](../api/intune-apps-mobilecontainedapp-list.md)|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)コレクション|[MobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)オブジェクトのプロパティと関係を一覧表示します。|
|[MobileContainedApp を取得します。](../api/intune-apps-mobilecontainedapp-get.md)|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)|[MobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)オブジェクトのプロパティと関係を参照してください。|

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




