---
title: mobileAppContent リソースの種類
description: 特定のアプリのバージョンに関するコンテンツのプロパティが含まれています。 各 mobileAppContent には、複数の mobileAppContentFile を含めることができます。
ms.openlocfilehash: e57c4c0823636143962ac5fe1c50f4377e731f84
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070095"
---
# <a name="mobileappcontent-resource-type"></a>mobileAppContent リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

特定のアプリのバージョンに関するコンテンツのプロパティが含まれています。 各 mobileAppContent には、複数の mobileAppContentFile を含めることができます。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[mobileAppContents のリスト](../api/intune-apps-mobileappcontent-list.md)|[mobileAppContent](../resources/intune-apps-mobileappcontent.md) コレクション|[mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[MobileAppContent の取得](../api/intune-apps-mobileappcontent-get.md)|[mobileAppContent](../resources/intune-apps-mobileappcontent.md)|[mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[mobileAppContent の作成](../api/intune-apps-mobileappcontent-create.md)|[mobileAppContent](../resources/intune-apps-mobileappcontent.md)|新しい [mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトを作成します。|
|[mobileAppContent の削除](../api/intune-apps-mobileappcontent-delete.md)|なし|[mobileAppContent](../resources/intune-apps-mobileappcontent.md) を削除します。|
|[mobileAppContent の更新](../api/intune-apps-mobileappcontent-update.md)|[mobileAppContent](../resources/intune-apps-mobileappcontent.md)|[mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|アプリのコンテンツのバージョンです。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|files|[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) コレクション|このアプリのコンテンツのバージョンに関するファイルのリストです。|
|containedApps|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)コレクション|パッケージとして機能する、MobileLobApp に含まれているアプリケーションのコレクションです。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "String (identifier)"
}
```





