---
title: Microsoft Graph 調整ガイド
description: 調整とは、リソースの使いすぎを防ぐために、サービスの同時呼び出し数を制限することをいいます。Microsoft Graph は、大量の要求を処理できるよう設計されています。過剰な数の要求が発生した場合、調整を行うことは Microsoft Graph サービスの最適なパフォーマンスと信頼性の維持に役立ちます。
author: piotrci
localization_priority: Priority
ms.openlocfilehash: 8b3b8c5b0ec5a5209ad96f87dc677f4331c24e0b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32580982"
---
# <a name="microsoft-graph-throttling-guidance"></a>Microsoft Graph 調整ガイド


調整とは、リソースの使いすぎを防ぐために、サービスの同時呼び出し数を制限することをいいます。Microsoft Graph は、大量の要求を処理できるよう設計されています。過剰な数の要求が発生した場合、調整を行うことは Microsoft Graph サービスの最適なパフォーマンスと信頼性の維持に役立ちます。

制限の調整はシナリオによって異なります。たとえば、大量の書き込みを行う際には、読み込みのみを行う場合に比べて調整が起こる可能性は高くなります。

## <a name="what-happens-when-throttling-occurs"></a>調整が発生すると、何が起こるのでしょうか

調整のしきい値を超えた場合、Microsoft Graph はそのクライアントの以降の要求を一定時間制限します。調整が発生した場合、Microsoft Graph は HTTP ステータス コード 429 (Too Many Requests) を返し、要求は失敗します。失敗した要求の応答ヘッダーで、推奨される待機時間を返します。調整の動作は要求の種類と数によります。たとえば、大量の要求があれば、すべての種類の要求が調整されます。しきい値は要求の種類によって異なります。そのため、書き込みは調整を受けるが、読み込みはそのままで許容されるシナリオが起こりえます。 

## <a name="common-throttling-scenarios"></a>一般的な調整のシナリオ

クライアントに対して調整が発生する最も一般的な原因は次のとおりです。

* あるテナントのすべてのアプリケーションから大量の要求がある。
* すべてのテナントで、特定のアプリケーションから大量の要求がある。

## <a name="best-practices-to-handle-throttling"></a>調整に対応するためのベスト プラクティス

調整に対応するためのベスト プラクティスには、次のようなものがあります。

* 要求あたりの操作の数を減らす。
* 呼び出しの頻度を減らす。
* すべての要求が使用量の制限に計上されるため、即時の再試行を避ける。

エラー処理を実装する場合は、HTTP エラー コード 429 を使用して調整の発生を検出します。失敗した要求への応答ヘッダーには、*Retry-After* フィールドが含まれています。Microsoft Graph はクライアントが調整による制限を受けている間でもリソースの使用量を記録しています。そのため、*Retry-After* の指示に従って要求を遅延させることが最も迅速に調整を解消できる方法です。

1. *Retry-After* フィールドに指定された秒数だけ待機してください。
2. 要求を再試行してください。
3. 要求が再度エラーコード 429 で失敗した場合は、依然として調整を受けています。Retry-After で推奨された遅延に引き続き従い、成功するまで再試行してください。

現在、次のリソースで Retry-After ヘッダーが提供されています。
- [ユーザー](/graph/api/resources/user?view=graph-rest-1.0)
- [写真](/graph/api/resources/profilephoto?view=graph-rest-1.0)
- [メール](/graph/api/resources/message?view=graph-rest-1.0)
- [カレンダー (ユーザーおよびグループ)](/graph/api/resources/event?view=graph-rest-1.0)
- [連絡先](/graph/api/resources/contact?view=graph-rest-1.0)
- [添付ファイル](/graph/api/resources/attachment?view=graph-rest-1.0)
- [グループ会話](/graph/api/resources/conversation?view=graph-rest-1.0)
- [ユーザーとソーシャル](/graph/api/resources/social-overview?view=graph-rest-beta)
- [ドライブ (OneDrive)](/graph/api/resources/drive?view=graph-rest-1.0)

Microsoft Cloud における調整についてのより幅広い議論については「[調整パターン](https://msdn.microsoft.com/library/office/dn589798.aspx)」を参照してください。
