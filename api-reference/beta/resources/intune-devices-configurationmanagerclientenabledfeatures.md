---
title: configurationManagerClientEnabledFeatures リソースの種類
description: 構成マネージャーのクライアントに対応した機能
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ed376bc616c26f1ad6e8a3ea06d3898c051e8d0b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148777"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a>configurationManagerClientEnabledFeatures リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

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
|endpointprotection|Boolean|エンドポイント保護が Intune によって管理されているかどうか|
|officeoffice|Boolean|Office アプリケーションが Intune によって管理されているかどうか|

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




