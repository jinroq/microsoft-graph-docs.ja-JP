---
title: mobileContainedApp リソースの種類
description: パッケージとして機能する mobileApp に含まれているアプリを表す抽象クラス。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 500d8329f998f340468b676d054211392ae6a6a4
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949907"
---
# <a name="mobilecontainedapp-resource-type"></a>mobileContainedApp リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

パッケージとして機能する mobileApp に含まれているアプリを表す抽象クラス。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト mobileContainedApps](../api/intune-apps-mobilecontainedapp-list.md)|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)コレクション|[MobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[MobileContainedApp を取得する](../api/intune-apps-mobilecontainedapp-get.md)|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)|[MobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)オブジェクトのプロパティとリレーションシップを読み取ります。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|

## <a name="relationships"></a>関係
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




