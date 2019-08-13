---
title: managedDeviceReportedApp リソースの種類
description: レポート用のアプリケーションデータ
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6561a6cee5a02f46c3347a1919c93c3807250fa8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36368829"
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



