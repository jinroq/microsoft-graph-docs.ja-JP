---
title: mobileContainedApp リソースの種類
description: パッケージとして機能する、mobileApp に含まれているアプリケーションを表す抽象クラスです。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5a9b36193aeda51679018bc534974c3678326a19
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963816"
---
# <a name="mobilecontainedapp-resource-type"></a>mobileContainedApp リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

パッケージとして機能する、mobileApp に含まれているアプリケーションを表す抽象クラスです。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト mobileContainedApps](../api/intune-apps-mobilecontainedapp-list.md)|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)コレクション|[MobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)オブジェクトのプロパティと関係を一覧表示します。|
|[MobileContainedApp を取得します。](../api/intune-apps-mobilecontainedapp-get.md)|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)|[MobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)オブジェクトのプロパティと関係を参照してください。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|エンティティのキー。|

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





