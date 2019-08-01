---
title: iosDeviceType リソースの種類
description: モバイル アプリを実行できる iOS デバイスの種類のプロパティが含まれます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 23d38faeafd9aac0d0e547596de51507b6932c20
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029164"
---
# <a name="iosdevicetype-resource-type"></a>iosDeviceType リソースの種類

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

モバイル アプリを実行できる iOS デバイスの種類のプロパティが含まれます。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|iPad|Boolean|アプリを iPad で実行できるかどうか。|
|iPhoneAndIPod|ブール型 (Boolean)|アプリを iPhone および iPod で実行できるかどうか。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosDeviceType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosDeviceType",
  "iPad": true,
  "iPhoneAndIPod": true
}
```



