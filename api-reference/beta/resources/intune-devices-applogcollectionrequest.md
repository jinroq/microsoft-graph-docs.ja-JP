---
title: appLogCollectionRequest リソースの種類
description: AppLogCollectionRequest エンティティ。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cb715113e45477738faba70e9cd1e4f6c10a4ad8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36319252"
---
# <a name="applogcollectionrequest-resource-type"></a>appLogCollectionRequest リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

AppLogCollectionRequest エンティティ。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト appLogCollectionRequests](../api/intune-devices-applogcollectionrequest-list.md)|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)コレクション|[AppLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[AppLogCollectionRequest を取得する](../api/intune-devices-applogcollectionrequest-get.md)|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|[AppLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[AppLogCollectionRequest を作成する](../api/intune-devices-applogcollectionrequest-create.md)|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|新しい[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)オブジェクトを作成します。|
|[AppLogCollectionRequest の削除](../api/intune-devices-applogcollectionrequest-delete.md)|None|[AppLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)を削除します。|
|[AppLogCollectionRequest の更新](../api/intune-devices-applogcollectionrequest-update.md)|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|[AppLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)オブジェクトのプロパティを更新します。|
|[createDownloadUrl アクション](../api/intune-devices-applogcollectionrequest-createdownloadurl.md)|[appLogCollectionDownloadDetails](../resources/intune-devices-applogcollectiondownloaddetails.md)|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|一意の識別子。 これは userId_DeviceId_AppId id です。|
|status|[appLogUploadState](../resources/intune-devices-apploguploadstate.md)|ログのアップロードの状態。 可能な値は、`pending`、`completed`、`failed` です。|
|errorMessage|String|アップロードプロセス中にエラーメッセージが表示される場合|
|customLogFolders|文字列コレクション|ログフォルダーの一覧。 |
|CompletedDateTime|DateTimeOffset|アップロードログ要求がターミナル状態に達した時刻|

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



