---
title: windowsInformationProtectionAppLearningSummary リソースの種類
description: Windows 情報保護アプリの学習概要エンティティ。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4149d585c187e8ec9c1f8f1f58aa1d646ba4a298
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585126"
---
# <a name="windowsinformationprotectionapplearningsummary-resource-type"></a>windowsInformationProtectionAppLearningSummary リソースの種類

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Windows 情報保護アプリの学習概要エンティティ。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List windowsInformationProtectionAppLearningSummaries](../api/intune-wip-windowsinformationprotectionapplearningsummary-list.md)|[windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) コレクション|[windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get windowsInformationProtectionAppLearningSummary](../api/intune-wip-windowsinformationprotectionapplearningsummary-get.md)|[windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)|[windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create windowsInformationProtectionAppLearningSummary](../api/intune-wip-windowsinformationprotectionapplearningsummary-create.md)|[windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)|新しい [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) オブジェクトを作成します。|
|[Delete windowsInformationProtectionAppLearningSummary](../api/intune-wip-windowsinformationprotectionapplearningsummary-delete.md)|なし|[windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) を削除します。|
|[Update windowsInformationProtectionAppLearningSummary](../api/intune-wip-windowsinformationprotectionapplearningsummary-update.md)|[windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)|[windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|WindowsInformationProtectionAppLearningSummary の一意識別子。|
|applicationName|String|アプリケーション名|
|applicationType|[applicationType](../resources/intune-wip-applicationtype.md)|アプリケーションの種類。 可能な値は、`universal`、`desktop` です。|
|deviceCount|Int32|デバイス数|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionAppLearningSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "id": "String (identifier)",
  "applicationName": "String",
  "applicationType": "String",
  "deviceCount": 1024
}
```



