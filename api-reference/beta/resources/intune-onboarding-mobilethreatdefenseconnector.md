---
title: mobileThreatDefenseConnector リソースの種類
description: Mobile Threat Defense パートナーとの接続を表すエンティティです。
ms.openlocfilehash: ee832f8e3acce151d51483522aa0c76b181e93d6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070107"
---
# <a name="mobilethreatdefenseconnector-resource-type"></a>mobileThreatDefenseConnector リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Mobile Threat Defense パートナーとの接続を表すエンティティです。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[mobileThreatDefenseConnectors のリスト](../api/intune-onboarding-mobilethreatdefenseconnector-list.md)|[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) コレクション|[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[mobileThreatDefenseConnector の取得](../api/intune-onboarding-mobilethreatdefenseconnector-get.md)|[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md)|[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[mobileThreatDefenseConnector の作成](../api/intune-onboarding-mobilethreatdefenseconnector-create.md)|[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md)|新しい [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) オブジェクトを作成します。|
|[mobileThreatDefenseConnector の削除](../api/intune-onboarding-mobilethreatdefenseconnector-delete.md)|なし|[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) を削除します。|
|[mobileThreatDefenseConnector の更新](../api/intune-onboarding-mobilethreatdefenseconnector-update.md)|[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md)|[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|まだ文書化されていません|
|lastHeartbeatDateTime|DateTimeOffset|データ同期パートナーから受信した最後のハートビートの日時|
|partnerState|[mobileThreatPartnerTenantState](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|このアカウントのデータの同期パートナーの状態です。 可能な値は、`unavailable`、`available`、`enabled`、`unresponsive` です。|
|androidEnabled|ブール型|Android において、準拠評価時にデータ同期パートナーからのデータを使用するかどうかを設定します|
|iosEnabled|ブール型|IOS において、準拠評価時にデータ同期パートナーからのデータを使用するかどうかを取得または設定します|
|windowsEnabled|ブール値|ウィンドウを取得または設定するコンプライアンスの評価中にデータの同期パートナーからのデータを使用する必要があるかどうか|
|macEnabled|ブール値|For Mac を取得または設定するコンプライアンスの評価中にデータの同期パートナーからのデータを使用する必要があるかどうか|
|androidDeviceBlockedOnMissingPartnerData|ブール型|Android において、デバイスを準拠させる前に Intune がデータ同期パートナーからデータを受信する必要があるかどうかを設定します|
|iosDeviceBlockedOnMissingPartnerData|ブール型|IOS において、デバイスを準拠させる前に Intune がデータ同期パートナーからデータを受信する必要があるかどうかを設定します|
|windowsDeviceBlockedOnMissingPartnerData|ブール値|Windows Intune は、準拠デバイスをマークする前にデータの同期パートナーからデータを受信する必要があるかどうかを設定します。|
|macDeviceBlockedOnMissingPartnerData|ブール値|For Mac を取得または設定する Intune 準拠デバイスをマークする前にデータの同期パートナーからデータを受信する必要があるかどうか|
|partnerUnsupportedOsVersionBlocked|ブール型|データ同期パートナーの最小バージョンの要件を満たさない、有効なプラットフォーム上のデバイスをブロックするかどうかを取得または設定します|
|partnerUnresponsivenessThresholdInDays|Int32|このパートナー統合に関する、テナントごとの無応答への許容日数の取得または設定を行います|
|allowPartnerToCollectIOSApplicationMetadata|ブール値|IOS デバイスでは、データの同期パートナー Intune からインストールされているアプリケーションについてのメタデータの収集もあるかどうかを構成するのには管理者では、します。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileThreatDefenseConnector"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "String (identifier)",
  "lastHeartbeatDateTime": "String (timestamp)",
  "partnerState": "String",
  "androidEnabled": true,
  "iosEnabled": true,
  "windowsEnabled": true,
  "macEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "windowsDeviceBlockedOnMissingPartnerData": true,
  "macDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 1024,
  "allowPartnerToCollectIOSApplicationMetadata": true
}
```





