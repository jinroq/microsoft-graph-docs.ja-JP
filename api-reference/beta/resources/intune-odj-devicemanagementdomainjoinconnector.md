---
title: deviceManagementDomainJoinConnector リソースの種類
description: ドメイン参加コネクタは、コンピューターアカウント blob の割り当て (および削除) を行うコネクタです。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0537d38d87a2cb574ca8984f895ed3796c33703a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "35001924"
---
# <a name="devicemanagementdomainjoinconnector-resource-type"></a>deviceManagementDomainJoinConnector リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ドメイン参加コネクタは、コンピューターアカウント blob の割り当て (および削除) を行うコネクタです。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[DeviceManagementDomainJoinConnectors を一覧表示する](../api/intune-odj-devicemanagementdomainjoinconnector-list.md)|[Devicemanagementdomainjoinconnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)コレクション|[Devicemanagementdomainjoinconnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[DeviceManagementDomainJoinConnector の取得](../api/intune-odj-devicemanagementdomainjoinconnector-get.md)|[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|[Devicemanagementdomainjoinconnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[DeviceManagementDomainJoinConnector の作成](../api/intune-odj-devicemanagementdomainjoinconnector-create.md)|[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|新しい[Devicemanagementdomainjoinconnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)オブジェクトを作成します。|
|[DeviceManagementDomainJoinConnector の削除](../api/intune-odj-devicemanagementdomainjoinconnector-delete.md)|None|[Devicemanagementdomainjoinconnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)を削除します。|
|[DeviceManagementDomainJoinConnector の更新](../api/intune-odj-devicemanagementdomainjoinconnector-update.md)|[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|[Devicemanagementdomainjoinconnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|コネクタを表す一意の識別子。|
|displayName|String|コネクタの表示名。|
|lastConnectionDateTime|DateTimeOffset|前回のコネクタが Intune に接続した時刻。|
|state|[Devicemanagementdomainjoinコネクタ状態](../resources/intune-odj-devicemanagementdomainjoinconnectorstate.md)|コネクタの状態です。 可能な値は、`active`、`error`、`inactive` です。|
|version|String|コネクタのバージョン。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementDomainJoinConnector"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementDomainJoinConnector",
  "id": "String (identifier)",
  "displayName": "String",
  "lastConnectionDateTime": "String (timestamp)",
  "state": "String",
  "version": "String"
}
```





