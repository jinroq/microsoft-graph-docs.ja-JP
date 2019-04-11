---
title: deviceManagementExchangeConnector リソースの種類
description: Exchange 環境との接続を表すエンティティです。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 703a2458cc91014ceda5e0fa26353901d06342ca
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31781051"
---
# <a name="devicemanagementexchangeconnector-resource-type"></a>deviceManagementExchangeConnector リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Exchange 環境との接続を表すエンティティです。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[deviceManagementExchangeConnectors のリスト](../api/intune-onboarding-devicemanagementexchangeconnector-list.md)|[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) コレクション|[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get deviceManagementExchangeConnector](../api/intune-onboarding-devicemanagementexchangeconnector-get.md)|[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)|[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[deviceManagementExchangeConnector の作成](../api/intune-onboarding-devicemanagementexchangeconnector-create.md)|[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)|新しい [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) オブジェクトを作成します。|
|[deviceManagementExchangeConnector の削除](../api/intune-onboarding-devicemanagementexchangeconnector-delete.md)|なし|[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) を削除します。|
|[deviceManagementExchangeConnector の更新](../api/intune-onboarding-devicemanagementexchangeconnector-update.md)|[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)|[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) オブジェクトのプロパティを更新します。|
|[同期アクション](../api/intune-onboarding-devicemanagementexchangeconnector-sync.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|まだ文書化されていません|
|lastSyncDateTime|DateTimeOffset|Exchange Connector の最終同期日時|
|status|[deviceManagementExchangeConnectorStatus](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|Exchange Connector の状態。 可能な値は、`none`、`connectionPending`、`connected`、`disconnected` です。|
|primarySmtpAddress|文字列|サービス間の Exchange Connector を構成するときに使用するメール アドレス。|
|serverName|文字列|Exchange サーバーの名前。|
|コネクタ servername|文字列|Exchange Connector をホストするサーバーの名前。|
|exchangeConnectorType|[deviceManagementExchangeConnectorType](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|構成されている Exchange Connector の種類。 可能な値は、`onPremises`、`hosted`、`serviceToService`、`dedicated` です。|
|version|文字列|ExchangeConnectorAgent のバージョン|
|exchangeAlias|文字列|Exchange Server に割り当てられているエイリアス。|
|exchangeOrganization|String|Exchange Server に対する Exchange 組織|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementExchangeConnector"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "id": "String (identifier)",
  "lastSyncDateTime": "String (timestamp)",
  "status": "String",
  "primarySmtpAddress": "String",
  "serverName": "String",
  "connectorServerName": "String",
  "exchangeConnectorType": "String",
  "version": "String",
  "exchangeAlias": "String",
  "exchangeOrganization": "String"
}
```





