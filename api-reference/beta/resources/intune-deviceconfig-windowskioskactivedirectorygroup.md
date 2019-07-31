---
title: windowsKioskActiveDirectoryGroup リソースの種類
description: キオスク構成の Azure ディレクトリグループを識別するために使用されるクラス
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2c64fe517fd610bad07b7a029e120c7657b834f7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969024"
---
# <a name="windowskioskactivedirectorygroup-resource-type"></a>windowsKioskActiveDirectoryGroup リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

キオスク構成の Azure ディレクトリグループを識別するために使用されるクラス


[Windowskioskuser](../resources/intune-deviceconfig-windowskioskuser.md)からの継承

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|groupName|String|このキオスク構成にロックされる AD グループの名前|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskActiveDirectoryGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskActiveDirectoryGroup",
  "groupName": "String"
}
```





