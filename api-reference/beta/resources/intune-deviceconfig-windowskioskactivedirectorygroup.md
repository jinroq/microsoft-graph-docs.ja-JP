---
title: windowsKioskActiveDirectoryGroup リソースの種類
description: キオスク構成の Azure ディレクトリグループを識別するために使用されるクラス
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 20f4c0eaf8470f01619a9ff4067bec0d95851b3c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464625"
---
# <a name="windowskioskactivedirectorygroup-resource-type"></a>windowsKioskActiveDirectoryGroup リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

キオスク構成の Azure ディレクトリグループを識別するために使用されるクラス


[windowskioskuser](../resources/intune-deviceconfig-windowskioskuser.md)からの継承

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





