---
title: microsoftStoreForBusinessContainedApp リソースの種類
description: MicrosoftStoreForBusinessApp の格納されているアプリケーションを表すクラスです。
author: tfitzmac
ms.openlocfilehash: a4ba31870ab98c509a16814bd52179e1f2deab63
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328288"
---
# <a name="microsoftstoreforbusinesscontainedapp-resource-type"></a>microsoftStoreForBusinessContainedApp リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

MicrosoftStoreForBusinessApp の格納されているアプリケーションを表すクラスです。

[MobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト microsoftStoreForBusinessContainedApps](../api/intune-apps-microsoftstoreforbusinesscontainedapp-list.md)|[microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)コレクション|[MicrosoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)オブジェクトのプロパティと関係を一覧表示します。|
|[MicrosoftStoreForBusinessContainedApp を取得します。](../api/intune-apps-microsoftstoreforbusinesscontainedapp-get.md)|[microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)|[MicrosoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)オブジェクトのプロパティと関係を参照してください。|
|[MicrosoftStoreForBusinessContainedApp を作成します。](../api/intune-apps-microsoftstoreforbusinesscontainedapp-create.md)|[microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)|新しい[microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)オブジェクトを作成します。|
|[MicrosoftStoreForBusinessContainedApp を削除します。](../api/intune-apps-microsoftstoreforbusinesscontainedapp-delete.md)|なし|の[microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)を削除します。|
|[MicrosoftStoreForBusinessContainedApp を更新します。](../api/intune-apps-microsoftstoreforbusinesscontainedapp-update.md)|[microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)|[MicrosoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>Properties
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|エンティティのキー。 [MobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)から継承されました。|
|appUserModelId|String|MicrosoftStoreForBusinessApp の格納されているアプリケーションのアプリケーション ユーザー モデル ID です。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftStoreForBusinessContainedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "id": "String (identifier)",
  "appUserModelId": "String"
}
```





