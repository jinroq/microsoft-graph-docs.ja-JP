---
title: windowsUniversalAppXContainedApp リソースの種類
description: WindowsUniversalAppX アプリケーションの格納されているアプリケーションを表すクラスです。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d7b9c814b73ce08bacdba97b40b5b7f07362606e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837717"
---
# <a name="windowsuniversalappxcontainedapp-resource-type"></a>windowsUniversalAppXContainedApp リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

WindowsUniversalAppX アプリケーションの格納されているアプリケーションを表すクラスです。

[MobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト windowsUniversalAppXContainedApps](../api/intune-apps-windowsuniversalappxcontainedapp-list.md)|[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)コレクション|[WindowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)オブジェクトのプロパティと関係を一覧表示します。|
|[WindowsUniversalAppXContainedApp を取得します。](../api/intune-apps-windowsuniversalappxcontainedapp-get.md)|[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)|[WindowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)オブジェクトのプロパティと関係を参照してください。|
|[WindowsUniversalAppXContainedApp を作成します。](../api/intune-apps-windowsuniversalappxcontainedapp-create.md)|[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)|新しい[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)オブジェクトを作成します。|
|[WindowsUniversalAppXContainedApp を削除します。](../api/intune-apps-windowsuniversalappxcontainedapp-delete.md)|なし|の[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)を削除します。|
|[WindowsUniversalAppXContainedApp を更新します。](../api/intune-apps-windowsuniversalappxcontainedapp-update.md)|[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)|[WindowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|エンティティのキー。 [MobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)から継承されました。|
|appUserModelId|String|WindowsUniversalAppX アプリケーションの格納されているアプリケーションのアプリケーション ユーザー モデル ID です。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUniversalAppXContainedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "id": "String (identifier)",
  "appUserModelId": "String"
}
```





