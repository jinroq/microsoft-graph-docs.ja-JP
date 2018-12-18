---
title: appConfigurationSettingItem リソースの種類
description: アプリの構成設定アイテムのプロパティが含まれています。
author: tfitzmac
ms.openlocfilehash: b75579e56602ad5359bc32d52312931342b42a6b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353579"
---
# <a name="appconfigurationsettingitem-resource-type"></a>appConfigurationSettingItem リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

アプリの構成設定アイテムのプロパティが含まれています。
## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|appConfigKey|String|アプリの構成キー。|
|appConfigKeyType|[mdmAppConfigKeyType](../resources/intune-apps-mdmappconfigkeytype.md)|アプリの構成キーの種類。 可能な値は、`stringType`、`integerType`、`realType`、`booleanType`、`tokenType` です。|
|appConfigKeyValue|String|アプリの構成キーの値。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appConfigurationSettingItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appConfigurationSettingItem",
  "appConfigKey": "String",
  "appConfigKeyType": "String",
  "appConfigKeyValue": "String"
}
```



