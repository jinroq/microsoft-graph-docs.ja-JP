---
title: officeConfigurationGroupAssignmentTarget リソースの種類
description: Office クライアント構成 AAD グループの割り当て先。
localization_priority: Normal
author: rolyon
ms.prod: Intune
ms.openlocfilehash: 7458b1071b6133f3b46c8412270e30fdd0bf7638
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949312"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a>officeConfigurationGroupAssignmentTarget リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Office クライアント構成 AAD グループの割り当て先。

[OfficeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|groupId|文字列型 (String)|デバイス構成を対象としている AAD グループの Id。|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeConfigurationGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeConfigurationGroupAssignmentTarget",
  "groupId": "String"
}
```



