---
title: windowsInformationProtectionNetworkLearningSummary リソースの種類
description: Windows 情報保護のネットワークの学習概要エンティティ。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d3564ca3afc92ae1ac4dab84f04df6660364f9a0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36356572"
---
# <a name="windowsinformationprotectionnetworklearningsummary-resource-type"></a>windowsInformationProtectionNetworkLearningSummary リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Windows 情報保護のネットワークの学習概要エンティティ。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List windowsInformationProtectionNetworkLearningSummaries](../api/intune-wip-windowsinformationprotectionnetworklearningsummary-list.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) コレクション|[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get windowsInformationProtectionNetworkLearningSummary](../api/intune-wip-windowsinformationprotectionnetworklearningsummary-get.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create windowsInformationProtectionNetworkLearningSummary](../api/intune-wip-windowsinformationprotectionnetworklearningsummary-create.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)|新しい [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) オブジェクトを作成します。|
|[Delete windowsInformationProtectionNetworkLearningSummary](../api/intune-wip-windowsinformationprotectionnetworklearningsummary-delete.md)|なし|[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) を削除します。|
|[Update windowsInformationProtectionNetworkLearningSummary](../api/intune-wip-windowsinformationprotectionnetworklearningsummary-update.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|WindowsInformationProtectionNetworkLearningSummary の一意識別子。|
|url|String|Web サイト URL|
|deviceCount|Int32|デバイス数|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionNetworkLearningSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "id": "String (identifier)",
  "url": "String",
  "deviceCount": 1024
}
```



