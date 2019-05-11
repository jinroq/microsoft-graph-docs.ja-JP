---
title: loggedOnUser リソースの種類
description: ログオンユーザー
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eeacee7d4d3a22e0d069851c1f9271ceb0e32c0d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941969"
---
# <a name="loggedonuser-resource-type"></a>loggedOnUser リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ログオンユーザー

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|userId|String|ユーザー ID|
|lastLogOnDateTime|DateTimeOffset|ユーザーがログオンした日時|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.loggedOnUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.loggedOnUser",
  "userId": "String",
  "lastLogOnDateTime": "String (timestamp)"
}
```




