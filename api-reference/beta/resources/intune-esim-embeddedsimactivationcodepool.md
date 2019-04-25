---
title: embeddedSIMActivationCodePool リソースの種類
description: プールは、埋め込まれた SIM アクティブ化コードのグループを表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a1cecbcd21b878ea0cba5168d40444ece5937912
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32525314"
---
# <a name="embeddedsimactivationcodepool-resource-type"></a>embeddedSIMActivationCodePool リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

プールは、埋め込まれた SIM アクティブ化コードのグループを表します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト embeddedSIMActivationCodePools](../api/intune-esim-embeddedsimactivationcodepool-list.md)|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)コレクション|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[embeddedSIMActivationCodePool を取得する](../api/intune-esim-embeddedsimactivationcodepool-get.md)|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[embeddedSIMActivationCodePool を作成する](../api/intune-esim-embeddedsimactivationcodepool-create.md)|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)|新しい[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)オブジェクトを作成します。|
|[embeddedSIMActivationCodePool の削除](../api/intune-esim-embeddedsimactivationcodepool-delete.md)|なし|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)を削除します。|
|[embeddedSIMActivationCodePool の更新](../api/intune-esim-embeddedsimactivationcodepool-update.md)|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)オブジェクトのプロパティを更新します。|
|[assign アクション](../api/intune-esim-embeddedsimactivationcodepool-assign.md)|[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)コレクション|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|埋め込まれた SIM アクティブ化コードプールの一意識別子。 作成時に割り当てられたシステム生成値。|
|displayName|String|埋め込まれた SIM アクティブ化コードプールの管理者定義の名前。|
|createdDateTime|DateTimeOffset|埋め込まれた SIM ライセンス認証コードプールが作成された時刻。 サービス側を生成しました。|
|modifiedDateTime|DateTimeOffset|埋め込まれた SIM ライセンス認証コードプールが最後に変更された時刻。 サービス側を更新しました。|
|activationCodes|[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md)コレクション|このプールに属するアクティブ化コード。 このナビゲーションプロパティは、アクティブ化コードを intune に送信するために使用されますが、intune からのアクティブ化コードの読み取りには使用できません。|
|activationCodeCount|Int32|このプールに属するアクティブ化コードの合計数。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|assignments|[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)コレクション|このプールが割り当てられているターゲットのリストへのナビゲーションプロパティ。|
|deviceStates|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)コレクション|このプールのデバイス状態のリストへのナビゲーションプロパティ。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.embeddedSIMActivationCodePool"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "activationCodes": [
    {
      "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
      "integratedCircuitCardIdentifier": "String",
      "matchingIdentifier": "String",
      "smdpPlusServerAddress": "String"
    }
  ],
  "activationCodeCount": 1024
}
```





