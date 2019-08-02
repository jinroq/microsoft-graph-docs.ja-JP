---
title: Microsoft Graph で通話とオンライン会議の API を使用する
description: Microsoft Graph の通話とオンライン会議の API により、音声機能とビデオ機能が使用可能になり、アプリおよびサービスとユーザーのインタラクションに新たな一面が加わります。 この API により、Microsoft Teams で通話を発信し、ユーザーとアプリケーションからの通話を受信することができます。 これらの API を使用して、通話や会議の参加者として動作するサービス アプリケーション (ボット) を作成できます。
author: VinodRavichandran
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: conceptualPageType
ms.openlocfilehash: dea588035e2f19361a36450bb49b4c5b2d9391b5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013011"
---
# <a name="working-with-the-calls-and-online-meetings-api-in-microsoft-graph"></a>Microsoft Graph で通話とオンライン会議の API を使用する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph の通話とオンライン会議の API により、音声機能とビデオ機能が使用可能になり、アプリおよびサービスとユーザーのインタラクションに新たな一面が加わります。 この API により、Microsoft Teams で通話を発信し、ユーザーとアプリケーションからの通話を受信することができます。 これらの API を使用して、通話や会議の参加者として動作するサービス アプリケーション (ボット) を作成できます。

## <a name="call-types"></a>通話の種類

通話はピアツーピア通話またはマルチパーティ通話に分類されます。 ユーザーは、ボットとのピアツーピア通話を開始するか、既存のマルチパーティ会議にボットを招待することができます。 ユーザーがボットをピアツーピア通話に招待するときには、アクセス許可は不要です。 ボットがマルチパーティ通話に参加するには、グループ通話に参加するためにテナント管理者からアクセス許可がボットに付与されている必要があります。

![ピアツーピア通話とマルチパーティ通話を示す画像](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/call-types.png)

ボットが通話を発信する場合、ボットには initiate または initiate-group-call アクセス許可のいずれかが必要です。 ボットには、ピアツーピア通話またはマルチパーティ通話を発信できるオプションがあります。

- ピアツーピア通話の場合、ボットはターゲットを 1 つだけ指定する必要があります。会議の調整は指定しません。 
- ボットが複数の参加者との通話を開始すると、バックグランドで臨時会議が設定され、全員がこの会議に参加できます。 会議の調整が指定されている場合、ターゲットが 1 つのみの場合でもマルチパーティ通話が設定されます。

通話はピアツーピアとして開始され、マルチパーティにエスカレートされます。 会議は自動的にプロビジョニングされ、メディアのターゲットがその会議に変更されます。 ボットに initiate-group-call アクセス許可が付与されている場合、ボットは他のユーザーを招待してエスカレーションを開始できます。 他の参加者がエスカレーションを開始し、ボットに join-group-call アクセス許可がない場合、ボットは通話から削除されます。

> **重要:** コールがピアツーピアからマルチパーティにエスカレートされる場合、一部のマルチパーティ機能が使用できません。 具体的には、ボットは参加者の更新情報を受信しません。

## <a name="signaling"></a>通知

### <a name="incoming-call"></a>着信通話

着信通話を受信するには、通話ボットを登録する必要があります。 ボットが着信通知を受け取るときには次のオプションがあります。

| メソッド                              | 説明                                  |
|:------------------------------------|:---------------------------------------------|
| [応答する (Answer)](../api/call-answer.md)     | 着信通話に応答します。                    |
| [拒否する (Reject)](../api/call-reject.md)     | 通話を拒否して切断します。                  |
| [リダイレクトする (Redirect)](../api/call-redirect.md) | 通話をリダイレクトします。                           |

ボットは別のユーザーまたはボットに通話をリダイレクトできます。 また、ボットはユーザーのボイスメールに通話をリダイレクトすることもできます。

![コールをボイスメールにリダイレクトするボットを示す画像](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/call-handling.png)

> **重要:** PSTN への発信通話のリダイレクトまたは発信は、現在サポートされていません。

### <a name="in-call"></a>通話中

通話オブジェクトではボットの操作を利用できます。 これらの操作は、通話の参加者であるボットに影響します。

| メソッド                                                            | 説明                                  |
|:------------------------------------------------------------------|:---------------------------------------------|
| [ミュートする (Mute)](../api/call-mute.md)                                       | 通話で自分をミュートします。                       |
| [ミュート解除する (Unmute)](../api/call-unmute.md)                                   | 通話で自分のミュートを解除します。                     |
| [UpdateMetadata](../api/call-updatemetadata.md)                   | 自分の名簿のメタデータを更新します。          |
| [ChangeScreenSharingRole](../api/call-changescreensharingrole.md) | 通話中に画面共有を開始および停止します。   |

通話の他の参加者と対話するには、participants オブジェクトを使用します。

| メソッド                                                            | 説明                                  |
|:------------------------------------------------------------------|:---------------------------------------------|
| [参加者を一覧表示する (List participants)](../api/call-list-participants.md)             | participant オブジェクト コレクションを取得します。         |
| [参加者を招待する (Invite Participants)](../api/participant-invite.md)               | アクティブな通話に参加者を招待します。      |
| [すべての参加者をミュートする (Mute All Participants)](../api/participant-muteall.md)            | 通話ですべての参加者をミュートします。           |

## <a name="media"></a>メディア

メディアの処理は、Microsoft Real-time Media Platform から管理されます。 Real-time Media Platform により、ボットが Microsoft Teams の音声/ビデオ通話や会議に参加できるようになります。 リアルタイム ボットがピアツーピア通話とマルチパーティ通話の両方に参加できるようになります。

ボットが着信通話に応答するか、新規通話または既存の通話に参加する場合、ボットは Real-time Media Platform に対しメディアの処理方法を通知する必要があります。 対話型音声応答 (IVR) システムを構築する場合に Microsoft サービスによりホストされているメディア処理コンポーネントに、コストの高い音声処理をオフロードできます。 ボットがメディア ストリームに直接アクセスする必要がある場合は、Real-time Media SDK でアプリケーションによりホストされるメディアのオプションが提供されます。

### <a name="service-hosted-media"></a>サービスによりホストされるメディア

ボットはワークフローを管理し、音声処理を Microsoft Real-time Media Platform にオフロードできます。 サービスによりホストされるメディアを使用すると、ボットを実装、ホストするためのさまざまなオプションが使用できるようになります。 使用可能な [SDK](https://developer.microsoft.com/graph/code-samples-and-sdks) の 1 つを利用することを検討します。 サービスによりホストされるメディア ボットは、メディアをローカルで処理しないため、ステートレス サービスとして実装できます。

| メソッド                                                        | 説明                                             |
|:--------------------------------------------------------------|:--------------------------------------------------------|
| [PlayPrompt](../api/call-playprompt.md)                       | ユーザーに対してオーディオ クリップを再生します。                         |
| [録音する (Record)](../api/call-record.md)                               | 必要に応じてプロンプトを再生し、オーディオ クリップを録音します。      |
| [SubscribeToTone](../api/call-subscribetotone.md)             | ユーザーからの DTMF トーンを登録します。                  |
| [CancelMediaProcessing](../api/call-cancelmediaprocessing.md) | キューにすでに入れられているメディアの処理をキャンセルします。             |

### <a name="application-hosted-media"></a>アプリケーションによりホストされているメディア

ボットがメディアに直接アクセスできるようにするには、ボットに Access-Media アクセス許可が必要です。 Real-time Media ライブラリとステートフル SDK により、機能が豊富なリアルタイム メディア通話ボットを構築できます。 アプリケーションによりホストされるボットは、Windows 環境でホストされる必要があります。 「[アプリケーションでホストされているメディアの例](https://github.com/microsoftgraph/microsoft-graph-comms-samples)」に、さまざまな Azure Platform (Cloud Services や Service Fabric など) でボットを構築する方法を示します。

[Microsoft Graph Calls SDK](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/index.html) を使用してボットの作成を簡素化できます。 この SDK には、メモリ内のリソースの状態の管理やボット開発者のメディア スタックの抑制の機能があります。

Media SDK により、ボットは音声、ビデオ、およびビデオベースの画面共有コンテンツを送受信できます。 ビデオベースの画面共有は、ビデオ チャネルとしてモデル化されます。 ボットは、複合オーディオ チャネルと複数のビデオ チャネルを登録できます。 ビデオ チャネルでは、ボットはビデオをエンコード H.264 ストリームまたはデコードされた生フレームのいずれかとして送受信できます。

> **注:** Microsoft.Graph.Calls.Media API は、録音や、ボッドがアクセスする通話や会議のメディア コンテンツを保存することには使用できません。

## <a name="see-also"></a>関連項目

[通話とオンライン会議の API の例](https://github.com/microsoftgraph/microsoft-graph-comms-samples/)

[既知の問題](/graph/known-issues#calls-and-online-meetings)
