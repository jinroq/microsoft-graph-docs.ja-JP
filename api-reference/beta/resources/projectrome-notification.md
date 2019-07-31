---
title: 通知リソースの種類
description: '指定したユーザーを対象とするアプリサーバーによって発行される通知を表します。 通知は Microsoft Graph に格納され、ユーザーが所有する異なるデバイスエンドポイントに配布されます。 '
localization_priority: Normal
ms.prod: project-rome
doc_type: resourcePageType
author: ''
ms.openlocfilehash: f9d9a4ff77190e18b8c090cf9c976decb4edfc3d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965580"
---
# <a name="notification-resource-type"></a>通知リソースの種類
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定したユーザーを対象とするアプリサーバーによって発行される通知を表します。 通知は Microsoft Graph に格納され、ユーザーが所有する異なるデバイスエンドポイントに配布されます。 

通知は、Windows、Android、iOS のプラットフォームを含む、オペレーティングシステムによって解釈可能な視覚的な通知のペイロードである場合があります。 また、アプリクライアントによって配信および処理されるデータペイロードを使用して、各デバイスで対応するユーザーの動作を決定します。通常は、生成された元のデータペイロードのコンテンツに対応するビジュアル通知 UI を示します。マシン. 

ユーザーが視覚的な通知を処理すると、アプリクライアントはクライアント側のプロジェクトローマ SDK を使用して、通知を非表示としてマークするなど、Microsoft Graph で対応する通知フィードの状態を更新することができます。 その後、その更新は他のすべてのアプリクライアントエンドポイントに配布され、クライアントは、ユーザーが冗長情報を表示できないようにするために、その変更をそれに応じて処理します。 アプリクライアントは、 [Project ローマ SDK](https://github.com/Microsoft/project-rome)を介して、通知履歴として、(非表示とマークされた後でも) 有効期限が切れる前に、後で同じ通知リソースにアクセスできます。 

## <a name="methods"></a>メソッド
|メソッド | 戻り値の型 | 説明|
|:------|:------------|:-----------|
|[通知の作成](../api/notifications-post.md) | [お知らせ](projectrome-notification.md) |通知を作成し、送信します。 |

## <a name="properties"></a>プロパティ
|名前 | 型 | 説明|
|:----|:-----|:-----------|
| targetHostName | String | 指定されたユーザーについて、呼び出し元サービスが通知を投稿するアプリケーションのホスト名を表します。 |
| appNotificationId | String | 通知のアプリサーバーによって設定された一意の id。個別の通知を識別して対象にします。 |
| expirationDateTime | DateTimeOffset | ユーザー通知の UTC 有効期限を設定します。時間が経過すると、通知は Microsoft Graph 通知フィードストアから完全に削除され、通知履歴の一部ではなくなります。 最大値は30日です。 |
| payload | Edm ComplexType、JSON オブジェクト | これは、この通知を受信するアプリクライアントによって配信および消費される生または視覚的なユーザー通知のデータの内容です。 |
| ペイロードコンテンツ | String | この通知を受信するアプリクライアントによって配信および消費される生のユーザー通知の通知の内容。 POST 通知要求に対しては、少なくとも1つの Content-type コンテンツとペイロードコンテンツが有効である必要があります。 |
| ペイロード | Edm ComplexType、JSON オブジェクト | 各モバイルプラットフォームの通知プラットフォームによって使用され、ユーザーに対してレンダリングされる、ビジュアルユーザー通知のビジュアルコンテンツ。 POST 通知要求に対して、少なくとも1つのコンテンツおよび VisualContent が有効である必要があります。 |
| ペイロード | String | ビジュアルユーザー通知のタイトル。 Title または body のいずれかを指定する必要があります。 |
| ペイロード | String | ビジュアルユーザー通知の本文。 Title または body のいずれかを指定する必要があります。 |
| displayTimeToLive | Int | この通知コンテンツを各プラットフォームの通知ビューアーに保持する時間 (秒単位) を設定します。 たとえば、Windows デバイスに通知が配信されると、このプロパティの値が ToastNotification に渡されます。この値によって、トースト通知がユーザーの Windows アクションセンターに保持される期間が決まります。 |
| priority | EnumType | 生のユーザー通知の優先度を示します。 既定では、視覚通知は高優先度で送信されます。 有効な値は High と Low です。 |
| groupName | String | この通知が属するグループの名前。 これは、通知をグループ化するための開発者によって設定されます。 |
| targetPolicy | Edm ComplexType、JSON オブジェクト | ターゲットポリシーオブジェクトは、対象とする必要があるエンドポイントの種類 (Windows、iOS、および Android) と、対象とする必要がある特定のエンドポイント (サブスクリプション id で識別される) の2つの異なるレベルで通知配信ポリシーを処理します。 |
| targetPolicy の種類 | Edm ComplexType、コレクション (EnumType) | 特定のプラットフォームまたはプラットフォームに対して通知配布をフィルター処理するために使用します。 既定では、すべてのプッシュエンドポイントの種類 (iOS、Windows、および Android) が有効になっています。 |

## <a name="relationships"></a>リレーションシップ
なし。

## <a name="json-representation"></a>JSON 表記
次に示すのは、移行先のオペレーティングシステムに配信される直接の視覚的な通知を発行するときのリソースの JSON 表記です。

```json
{   
  "targetHostName": "String",
  "appNotificationId": "String",
  "expirationDateTime": "DateTimeOffset",
  "payload":  
  {
    "visualContent": 
    {
      "title": "String",
      "body": "String"
    },
  },
  "displayTimeToLive": "Int",
  "priority": "Enum",
  "groupName": "String",
  "targetPolicy":
  {
    "platformTypes": [ 
      "Enum"
    ]
  }
}
```

アプリクライアントに配信される生データ通知を発行するときの、リソースの JSON 表記を次に示します。
```json
{   
  "targetHostName": "String",
  "appNotificationId": "String",
  "expirationDateTime": "DateTimeOffset",
  "payload":  
  {
    "rawContent": "String"
  },
  "displayTimeToLive": "Int",
  "priority": "Enum",
  "groupName": "String",
  "targetPolicy":
  {
    "platformTypes": [ 
      "Enum"
    ]
  }
}
```
