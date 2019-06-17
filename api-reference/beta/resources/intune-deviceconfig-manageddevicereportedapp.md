---
title: managedDeviceReportedApp リソースの種類
description: レポート用のアプリケーションデータ
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e028ec07142a7902ec02b2b8eeccdc9c378170d8
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34992025"
---
# <a name="manageddevicereportedapp-resource-type"></a>managedDeviceReportedApp リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

レポート用のアプリケーションデータ

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|appId|String|アプリケーションのアプリケーションまたはバンドルの識別子|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceReportedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceReportedApp",
  "appId": "String"
}
```





