---
title: appLogCollectionRequest リソースの種類
description: AppLogCollectionRequest エンティティです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 795b80b0194f2c3a1d314cbb317af954fb675063
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431618"
---
# <a name="applogcollectionrequest-resource-type"></a>appLogCollectionRequest リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

AppLogCollectionRequest エンティティです。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト appLogCollectionRequests](../api/intune-devices-applogcollectionrequest-list.md)|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)コレクション|[AppLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)オブジェクトのプロパティと関係を一覧表示します。|
|[AppLogCollectionRequest を取得します。](../api/intune-devices-applogcollectionrequest-get.md)|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|[AppLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)オブジェクトのプロパティと関係を参照してください。|
|[AppLogCollectionRequest を作成します。](../api/intune-devices-applogcollectionrequest-create.md)|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|新しい[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)オブジェクトを作成します。|
|[AppLogCollectionRequest を削除します。](../api/intune-devices-applogcollectionrequest-delete.md)|なし|の[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)を削除します。|
|[AppLogCollectionRequest を更新します。](../api/intune-devices-applogcollectionrequest-update.md)|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|[AppLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)オブジェクトのプロパティを更新します。|
|[createDownloadUrl アクション](../api/intune-devices-applogcollectionrequest-createdownloadurl.md)|[appLogCollectionDownloadDetails](../resources/intune-devices-applogcollectiondownloaddetails.md)|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|一意の識別子です。 これは、userId_DeviceId_AppId の id です。|
|status|[appLogUploadState](../resources/intune-devices-apploguploadstate.md)|ログのアップロードの状態です。 可能な値は、`pending`、`completed`、`failed` です。|
|エラー メッセージ|String|アップロード プロセス中に存在する場合のエラー メッセージ|
|customLogFolders|String コレクション|ログのフォルダーの一覧です。 |
|CompletedDateTime|DateTimeOffset|までに時間のアップロードのログ要求が終了状態|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appLogCollectionRequest"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appLogCollectionRequest",
  "id": "String (identifier)",
  "status": "String",
  "errorMessage": "String",
  "customLogFolders": [
    "String"
  ],
  "completedDateTime": "String (timestamp)"
}
```




