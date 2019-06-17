---
title: managedAppDiagnosticStatus リソースの種類
description: 診断状態を表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 907f9940b7cbb4a35f69e0792092e14c99aebdae
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34996296"
---
# <a name="managedappdiagnosticstatus-resource-type"></a>managedAppDiagnosticStatus リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

診断状態を表します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|validationName|String|検証のフレンドリ名|
|state|String|操作の状態|
|mitigationInstruction|文字列型 (String)|検証の失敗を減らすための方法に関する説明|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedAppDiagnosticStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppDiagnosticStatus",
  "validationName": "String",
  "state": "String",
  "mitigationInstruction": "String"
}
```





