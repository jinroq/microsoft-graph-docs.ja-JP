---
title: onPremisesConditionalAccessSettings リソースの種類
description: テナントの Exchange OnPremises 条件付きアクセス設定を表す単一エンティティ。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cbcdbd43811f26ef62d26d04cb30e9f0c0476600
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986811"
---
# <a name="onpremisesconditionalaccesssettings-resource-type"></a>onPremisesConditionalAccessSettings リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

テナントの Exchange OnPremises 条件付きアクセス設定を表す単一エンティティ。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[Get onPremisesConditionalAccessSettings](../api/intune-onboarding-onpremisesconditionalaccesssettings-get.md)|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Update onPremisesConditionalAccessSettings](../api/intune-onboarding-onpremisesconditionalaccesssettings-update.md)|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|まだ文書化されていません|
|enabled|Boolean|対象組織で、オンプレミスの条件付きアクセスが有効かどうかを示します。|
|includedGroups|Guid コレクション|オンプレミスの条件付きアクセスで対象となるユーザー グループ。 これらのグループ内のユーザーすべては、管理対象のモバイル デバイスを持っており、メール アクセスに準拠している必要があります。|
|excludedGroups|Guid コレクション|オンプレミスの条件付きアクセスで除外されるユーザー グループ。 これらのグループ内のすべてのユーザーは、条件付きアクセス ポリシーから除外されます。|
|overrideDefaultRule|Boolean|デバイスでアクセスが付与されていることを確認できるようにするとき、既定のアクセス ルールを上書きします。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onPremisesConditionalAccessSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "String (identifier)",
  "enabled": true,
  "includedGroups": [
    "Guid"
  ],
  "excludedGroups": [
    "Guid"
  ],
  "overrideDefaultRule": true
}
```





