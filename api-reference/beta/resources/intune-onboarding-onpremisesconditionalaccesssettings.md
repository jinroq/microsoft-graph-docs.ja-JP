---
title: onPremisesConditionalAccessSettings リソースの種類
description: テナントの Exchange OnPremises 条件付きアクセス設定を表す単一エンティティ。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c2a696696a25382778ef043d6dcae1320ed75a58
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358014"
---
# <a name="onpremisesconditionalaccesssettings-resource-type"></a>onPremisesConditionalAccessSettings リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

テナントの Exchange OnPremises 条件付きアクセス設定を表す単一エンティティ。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[Get onPremisesConditionalAccessSettings](../api/intune-onboarding-onpremisesconditionalaccesssettings-get.md)|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Update onPremisesConditionalAccessSettings](../api/intune-onboarding-onpremisesconditionalaccesssettings-update.md)|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|まだ文書化されていません|
|enabled|Boolean|対象組織で、オンプレミスの条件付きアクセスが有効かどうかを示します。|
|includedGroups|Guid コレクション|オンプレミスの条件付きアクセスで対象となるユーザー グループ。 これらのグループ内のユーザーすべては、管理対象のモバイル デバイスを持っており、メール アクセスに準拠している必要があります。|
|excludedGroups|Guid コレクション|オンプレミスの条件付きアクセスで除外されるユーザー グループ。 これらのグループ内のすべてのユーザーは、条件付きアクセス ポリシーから除外されます。|
|overrideDefaultRule|ブール型 (Boolean)|デバイスでアクセスが付与されていることを確認できるようにするとき、既定のアクセス ルールを上書きします。|

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



