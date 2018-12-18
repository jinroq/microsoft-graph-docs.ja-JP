---
title: embeddedSIMActivationCodePoolAssignment リソースの種類
description: 埋め込み SIM アクティベーション コード プール割り当てエンティティには、AAD のデバイス ・ グループに特定の embeddedSIMActivationCodePool が割り当てられます。
author: tfitzmac
ms.openlocfilehash: 67d563a630fb1c1092416f1081c4decda0d9eaf4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337437"
---
# <a name="embeddedsimactivationcodepoolassignment-resource-type"></a>embeddedSIMActivationCodePoolAssignment リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

埋め込み SIM アクティベーション コード プール割り当てエンティティには、AAD のデバイス ・ グループに特定の embeddedSIMActivationCodePool が割り当てられます。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト embeddedSIMActivationCodePoolAssignments](../api/intune-esim-embeddedsimactivationcodepoolassignment-list.md)|[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)コレクション|[EmbeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)オブジェクトのプロパティと関係を一覧表示します。|
|[EmbeddedSIMActivationCodePoolAssignment を取得します。](../api/intune-esim-embeddedsimactivationcodepoolassignment-get.md)|[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|[EmbeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)オブジェクトのプロパティと関係を参照してください。|
|[EmbeddedSIMActivationCodePoolAssignment を作成します。](../api/intune-esim-embeddedsimactivationcodepoolassignment-create.md)|[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|新しい[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)オブジェクトを作成します。|
|[EmbeddedSIMActivationCodePoolAssignment を削除します。](../api/intune-esim-embeddedsimactivationcodepoolassignment-delete.md)|なし|の[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)を削除します。|
|[EmbeddedSIMActivationCodePoolAssignment を更新します。](../api/intune-esim-embeddedsimactivationcodepoolassignment-update.md)|[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|[EmbeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>Properties
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|埋め込み SIM アクティベーション コードのプール割り当ての一意の識別子です。 システムでは、作成時に割り当てられた値が生成されます。|
|ターゲット|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|SIM のアクティブ化コードの埋め込み、プールの対象となるグループの種類。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.embeddedSIMActivationCodePoolAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





