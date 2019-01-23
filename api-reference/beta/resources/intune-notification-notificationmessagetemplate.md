---
title: notificationMessageTemplate リソース タイプ
description: 通知メッセージは、管理者が定義したコンプライアンス ポリシーに準拠していないと判断されたエンド ユーザーに送信されるメッセージです。 管理者は通知を選択し、Intune 管理コンソールで、コンプライアンス ポリシー作成ページの [コンプライアンス非対応に対するアクション] セクションを使用して通知を構成します。 notificationMessageTemplate オブジェクトを使用して、管理者が非準拠のアクションを構成する際に選択する、独自のカスタム通知を作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5b76ddbc9f55f1129cb186b23022812c84ce32a7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394783"
---
# <a name="notificationmessagetemplate-resource-type"></a>notificationMessageTemplate リソース タイプ

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

通知メッセージは、管理者が定義したコンプライアンス ポリシーに準拠していないと判断されたエンド ユーザーに送信されるメッセージです。 管理者は通知を選択し、Intune 管理コンソールで、コンプライアンス ポリシー作成ページの [コンプライアンス非対応に対するアクション] セクションを使用して通知を構成します。 notificationMessageTemplate オブジェクトを使用して、管理者が非準拠のアクションを構成する際に選択する、独自のカスタム通知を作成します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List notificationMessageTemplates](../api/intune-notification-notificationmessagetemplate-list.md)|[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) コレクション|[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get notificationMessageTemplate](../api/intune-notification-notificationmessagetemplate-get.md)|[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)|[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create notificationMessageTemplate](../api/intune-notification-notificationmessagetemplate-create.md)|[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)|新しい [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) を作成します。|
|[Delete notificationMessageTemplate](../api/intune-notification-notificationmessagetemplate-delete.md)|なし|[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) を削除します。|
|[Update notificationMessageTemplate](../api/intune-notification-notificationmessagetemplate-update.md)|[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)|[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) オブジェクトのプロパティを更新します。|
|[sendTestMessage action](../api/intune-notification-notificationmessagetemplate-sendtestmessage.md)|なし|既定のロケールで、指定された notificationMessageTemplate を使用して、テスト メッセージを送信します|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。|
|displayName|String|通知メッセージ テンプレートの表示名。|
|defaultLocale|String|要求されたロケールが使用できないときにフォールバックする既定のロケール。|
|brandingOptions|[notificationTemplateBrandingOptions](../resources/intune-notification-notificationtemplatebrandingoptions.md)|メッセージ テンプレートのブランド化オプション。 ブランド化は、Intune 管理コンソールで定義されます。 可能な値は、`none`、`includeCompanyLogo`、`includeCompanyName`、`includeContactInformation` です。|
|roleScopeTagIds|String コレクション|このエンティティ インスタンスのスコープのタグのリストです。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|localizedNotificationMessages|[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) コレクション|この通知メッセージ テンプレート用にローカライズされたメッセージのリスト。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.notificationMessageTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "defaultLocale": "String",
  "brandingOptions": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```




