---
title: managedAppOperation リソースの種類
description: アプリ登録に対して適用される操作を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 52e511ca24f67a485ab289f48c25fa1ceb309910
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920479"
---
# <a name="managedappoperation-resource-type"></a>managedAppOperation リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

アプリ登録に対して適用される操作を表します。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List managedAppOperations](../api/intune-mam-managedappoperation-list.md)|[managedAppOperation](../resources/intune-mam-managedappoperation.md) コレクション|[managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get managedAppOperation](../api/intune-mam-managedappoperation-get.md)|[managedAppOperation](../resources/intune-mam-managedappoperation.md)|[managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create managedAppOperation](../api/intune-mam-managedappoperation-create.md)|[managedAppOperation](../resources/intune-mam-managedappoperation.md)|新しい [managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトを作成します。|
|[Delete managedAppOperation](../api/intune-mam-managedappoperation-delete.md)|なし|[managedAppOperation](../resources/intune-mam-managedappoperation.md) を削除します。|
|[Update managedAppOperation](../api/intune-mam-managedappoperation-update.md)|[managedAppOperation](../resources/intune-mam-managedappoperation.md)|[managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|displayName|String|操作名。|
|lastModifiedDateTime|DateTimeOffset|アプリ操作が変更された最終時刻。|
|state|String|操作の現在の状態。|
|id|String|エンティティのキー。|
|version|String|エンティティのバージョン。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppOperation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "state": "String",
  "id": "String (identifier)",
  "version": "String"
}
```



