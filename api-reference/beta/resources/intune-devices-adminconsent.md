---
title: adminConsent リソースの種類
description: 管理者の同意情報。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aaac2bb11d90f1e6fec52fae0c17f374c33868ce
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943369"
---
# <a name="adminconsent-resource-type"></a>adminConsent リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

管理者の同意情報。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|/Sharepoint データの編集|[Adminconの状態](../resources/intune-devices-adminconsentstate.md)|ユーザーとデバイスのデータを Apple に共有するための管理者の同意状態。 可能な値は、`notConfigured`、`granted`、`notGranted` です。|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.adminConsent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.adminConsent",
  "shareAPNSData": "String"
}
```




