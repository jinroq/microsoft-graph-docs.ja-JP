---
title: configurationManagerClientEnabledFeatures リソースの種類
description: 構成マネージャーのクライアントに対応した機能
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fcee21d1d6d9047b273b539ec10d3cfa63c2e3ce
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983226"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a>configurationManagerClientEnabledFeatures リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

構成マネージャーのクライアントに対応した機能

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|inventory|Boolean|在庫が Intune によって管理されているかどうか|
|modernApps|Boolean|モダン アプリケーションが Intune によって管理されているかどうか|
|resourceAccess|Boolean|リソース アクセスが Intune によって管理されているかどうか|
|deviceConfiguration|Boolean|デバイス構成が Intune によって管理されているかどうか|
|compliancePolicy|Boolean|コンプライアンス ポリシーが Intune によって管理されているかどうか|
|windowsUpdateForBusiness|Boolean|Windows Update for Business が Intune によって管理されているかどうか|
|endpointProtection|Boolean|エンドポイント保護が Intune によって管理されているかどうか|
|Officeoffice|Boolean|Office アプリケーションが Intune によって管理されているかどうか|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientEnabledFeatures",
  "inventory": true,
  "modernApps": true,
  "resourceAccess": true,
  "deviceConfiguration": true,
  "compliancePolicy": true,
  "windowsUpdateForBusiness": true,
  "endpointProtection": true,
  "officeApps": true
}
```





