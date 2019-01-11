---
title: windowsManagementApp リソースの種類
description: Windows 管理アプリケーションのエンティティです。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 47262f93e619690352cac9ae3f9a500d0dc77c20
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833413"
---
# <a name="windowsmanagementapp-resource-type"></a>windowsManagementApp リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Windows 管理アプリケーションのエンティティです。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[WindowsManagementApp を取得します。](../api/intune-devices-windowsmanagementapp-get.md)|[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)|[WindowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)オブジェクトのプロパティと関係を参照してください。|
|[WindowsManagementApp を更新します。](../api/intune-devices-windowsmanagementapp-update.md)|[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)|[WindowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|Windows 管理アプリケーションの一意の識別子|
|availableVersion|String|Windows 管理アプリケーションの使用可能なバージョンです。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|healthSummary|[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)|Windows 管理アプリケーションの概要の状態です。|
|healthStates|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)コレクション|インストールされている Windows の管理アプリケーションの稼働状態の一覧です。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "id": "String (identifier)",
  "availableVersion": "String"
}
```





