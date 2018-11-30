---
title: 通知リソースの種類
description: '指定したユーザーを対象とするアプリケーション ・ サーバによって提供される通知を表します。 通知は、Microsoft Graph で格納され、ユーザーによって所有されている端点を別のデバイスに配布されます。 '
ms.openlocfilehash: dfcff69fd51ffa8993c0d570883e04a69371fb85
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073216"
---
# <a name="notification-resource-type"></a>通知リソースの種類
> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

指定したユーザーを対象とするアプリケーション ・ サーバによって提供される通知を表します。 通知は、Microsoft Graph で格納され、ユーザーによって所有されている端点を別のデバイスに配布されます。 

通知には、Windows、Android、iOS プラットフォームを含む、オペレーティング システムによって解釈可能なメッセージ ボックスによる通知のペイロードを指定できます。 通常、視覚的に通知が生成される元のデータ ペイロードのコンテンツに対応する UI の – すべてのデバイスに、app のクライアントは、対応するユーザーを決定し、データ ペイロードに配信し、処理が発生することもできます。ローカルにします。 

ユーザーは、視覚的に通知の動作と、アプリケーション クライアントことができますし、SDK を使用クライアント側プロジェクト ローマを閉じるよう通知をマークすることによって、graph のフィード対応する通知の状態を更新します。 更新プログラムはアプリケーションのクライアント エンドポイントでは、配布して、クライアントこの変化に対応などの冗長な情報を見ることからユーザーを防ぐために通知を無視すれば。 後で (非表示としてマークされます) の後も期限切れ前に、アプリケーションのクライアントを同じ通知リソースにアクセスできる[プロジェクトのローマの SDK](https://github.com/Microsoft/project-rome)を使用して、通知の履歴とします。 

## <a name="methods"></a>メソッド
|メソッド | 戻り値の型 | 説明|
|:------|:------------|:-----------|
|[通知を作成します。](../api/projectrome-notification-post.md) | [通知](projectrome-notification.md) |作成し、通知を送信します。 |

## <a name="properties"></a>プロパティ
|名前 | 型 | 説明|
|:----|:-----|:-----------|
| targetHostName | String | 呼び出し元のサービスが特定のユーザーに対して、通知を投稿するのにはアプリケーションのホスト名を表します。 |
| appNotificationId | String | 識別し、個々 の通知を対象に使用する通知のアプリケーション サーバで設定する一意の id。 |
| expirationDateTime | DateTimeOffset | 有効期限の時刻を設定、ユーザーへの通知の上、時間は、通知 Graph フィード通知ストアから完全に削除され、通知履歴の一部ではありません。 最大値は、30 日間です。 |
| payload | Edm.ComplexType、JSON オブジェクト | 提供され、この通知を受け取るアプリケーションのクライアントによって消費される raw またはビジュアルのユーザーの通知のデータ コンテンツです。 |
| payload.rawContent | String | 提供され、この通知を受け取るアプリケーションのクライアントによって消費されることを示す生のユーザー通知の通知の内容です。 投稿の通知要求を有効にする Payload.RawContent と Payload.VisualContent の少なくとも 1 つ必要があります。 |
| payload.visual | Edm.ComplexType、JSON オブジェクト | モバイル プラットフォームごとに通知のプラットフォームで使用され、ユーザーに表示する、ビジュアルなユーザー通知のビジュアルのコンテンツです。 投稿の通知要求を有効にするコンテンツと VisualContent の少なくとも 1 つ必要があります。 |
| payload.visual.title | String | ビジュアルなユーザー通知のタイトル。 タイトルまたは本文のいずれかが必要です。 |
| payload.visual.body | String | ビジュアルなユーザー通知の本文です。 タイトルまたは本文のいずれかが必要です。 |
| displayTimeToLive | 整数型 (Int) | 時間 (秒) この通知の内容のままで各プラットフォームの通知のビューアーを設定します。 たとえば、通知が配信されると Windows のデバイスに、このプロパティの値に渡されます ToastNotification.ExpirationTime は、どのくらいの時間、トースト通知は常にユーザーの Windows アクション センターで決定します。 |
| priority | EnumType | 生のユーザーの通知の優先順位を示します。 既定で優先度の高い視覚的な通知が送信されます。 有効な値は、最低額です。 |
| グループ名 | String | この通知が所属するグループの名前。 通知をグループ化するための開発者によって設定されます。 |
| targetPolicy | Edm.ComplexType、JSON オブジェクト | ターゲット ポリシー オブジェクトは、さまざまなレベルの 2 つのエンドポイントの種類 (Windows、iOS および Android) の対象とする、および対象とする、(サブスクリプションの id によって識別される) 特定のエンドポイントに配信ポリシーを通知を処理します。 |
| targetPolicy.platformTypes | Edm.ComplexType、コレクション (EnumType) | フィルター通知の配布を特定のプラットフォームまたはプラットフォームを使用します。 既定では、プッシュ エンドポイントのすべての種類 (iOS、ウィンドウ、および Android) が有効になります。 |

## <a name="relationships"></a>リレーションシップ
なし。

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表現は、ターゲット ・ オペレーティング ・ システムに配信する直接視覚的に通知を発行するとき。

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

次は JSON 表現です、リソースのアプリケーションのクライアントに配信される生データの通知を発行するとき。
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
