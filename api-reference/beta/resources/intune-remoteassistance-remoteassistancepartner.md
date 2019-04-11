---
title: remoteAssistancePartner リソースの種類
description: RemoteAssistPartner リソースは、指定されたリモートアシスタンスパートナーサービスのメタデータと状態を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3343d0e9d68c76db91f1153704176d70b06a7483
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31805489"
---
# <a name="remoteassistancepartner-resource-type"></a>remoteAssistancePartner リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

RemoteAssistPartner リソースは、指定されたリモートアシスタンスパートナーサービスのメタデータと状態を表します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[remoteAssistancePartners のリスト](../api/intune-remoteassistance-remoteassistancepartner-list.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) コレクション|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-get.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[remoteAssistancePartner の作成](../api/intune-remoteassistance-remoteassistancepartner-create.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|新しい [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトを作成します。|
|[remoteAssistancePartner の削除](../api/intune-remoteassistance-remoteassistancepartner-delete.md)|なし|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) を削除します。|
|[remoteAssistancePartner の更新](../api/intune-remoteassistance-remoteassistancepartner-update.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトのプロパティを更新します。|
|[beginOnboarding アクション](../api/intune-remoteassistance-remoteassistancepartner-beginonboarding.md)|なし|オンボードを開始する要求。  適切な TeamViewer アカウント情報と組み合わせる必要があります。|
|[切断アクション](../api/intune-remoteassistance-remoteassistancepartner-disconnect.md)|なし|アクティブな TeamViewer connector を削除する要求|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|パートナーの一意識別子。|
|displayName|String|パートナーの表示名。|
|onboardingUrl|String|パートナーのオンボーディング ポータルの URL。このポータルでは、管理者がパートナーのリモート アシスタンス サービスを構成できます。|
|onboardingStatus|[remoteAssistanceOnboardingStatus](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|現在の TeamViewer connector の状態のわかりやすい説明。 使用可能な値は、`notOnboarded`、`onboarding`、`onboarded` です。|
|lastConnectionDateTime|DateTimeOffset|TEM パートナーによって Intune に対して最後に送信された要求のタイムスタンプ。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.remoteAssistancePartner"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "id": "String (identifier)",
  "displayName": "String",
  "onboardingUrl": "String",
  "onboardingStatus": "String",
  "lastConnectionDateTime": "String (timestamp)"
}
```





