---
title: localizedNotificationMessage リソースの種類
description: 指定されたロケールの通知メッセージ テンプレートのテキスト コンテンツ。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7bf21828e69cd6365143bdc7c27b2b9bbf495a27
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418058"
---
# <a name="localizednotificationmessage-resource-type"></a>localizedNotificationMessage リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

指定されたロケールの通知メッセージ テンプレートのテキスト コンテンツ。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List localizedNotificationMessages](../api/intune-notification-localizednotificationmessage-list.md)|[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) コレクション|[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get localizedNotificationMessage](../api/intune-notification-localizednotificationmessage-get.md)|[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)|[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create localizedNotificationMessage](../api/intune-notification-localizednotificationmessage-create.md)|[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)|新しい [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトを作成します。|
|[Delete localizedNotificationMessage](../api/intune-notification-localizednotificationmessage-delete.md)|なし|[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) を削除します。|
|[Update localizedNotificationMessage](../api/intune-notification-localizednotificationmessage-update.md)|[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)|[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|lastModifiedDateTime|DateTimeOffset|オブジェクトの最終更新の DateTime。|
|locale|String|対象メッセージの送信先ロケール。|
|subject|String|メッセージ テンプレートの件名。|
|messageTemplate|String|メッセージ テンプレートのコンテンツ。|
|isDefault|Boolean|言語フォールバック用の既定ロケールかどうかを示すフラグ。 このフラグは設定のみ可能です。 設定解除するには、このプロパティを別のローカライズされた通知メッセージで有効にします。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.localizedNotificationMessage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "locale": "String",
  "subject": "String",
  "messageTemplate": "String",
  "isDefault": true
}
```




