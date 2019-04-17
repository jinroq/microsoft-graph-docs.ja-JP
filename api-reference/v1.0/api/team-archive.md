---
title: チームをアーカイブする
description: '指定されたチームをアーカイブします。 '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 28c1ea9d96d55587f95af85c9aba50a43fe08d60
ms.sourcegitcommit: a39db1154a07aa0dd7e96fb6f9d7e891a812207e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/16/2019
ms.locfileid: "31890025"
---
# <a name="archive-team"></a>チームをアーカイブする



指定された[チーム](../resources/team.md)をアーカイブします。 チームをアーカイブすると、ユーザーはチームのチャネルでメッセージを送信したり、いいねしたり、チームの名前、説明、またはその他の設定、通常、チームへの変更がほとんどできなくなります。
チームへのメンバーシップの変更はそのまま許可されます。

アーカイブは非同期操作です。 非同期操作が正常に完了すると、チームがアーカイブされます。この API の応答に続いて発生する可能性があります。

チームをアーカイブできるのは、チームと[グループ](../resources/group.md)が所有者の場合です。

アーカイブした状態からチームを復元するには、API を使用して[アーカイブを解除](team-unarchive.md)します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Group.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | Group.ReadWrite.All    |

> **注**: この API は、管理者のアクセス許可をサポートします。 グローバル管理者と Microsoft Teams サービス管理者は、メンバーではないチームにアクセスできます。

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/archive
```
## <a name="request-headers"></a>要求ヘッダー
| ヘッダー       | 値 |
|:---------------|:--------|
| Authorization  | ベアラー {トークン}。必須。  |

## <a name="request-body"></a>要求本文
次のように、リクエストでは_オプションで_ JSON の本文に`shouldSetSpoSiteReadOnlyForMembers`パラメーターを入力できます。
```JSON
{
    "shouldSetSpoSiteReadOnlyForMembers": true
}
```
このオプションのパラメーターは、チーム メンバーのアクセス許可を、チームに関連付けられている Sharepoint Online サイトで読み取り専用に設定するかどうかを定義します。 False に設定したり、本文を完全に省略したりすると、この手順がスキップされます。

## <a name="response"></a>応答

アーカイブが正常に開始された場合、このメソッドは`202 Accepted`応答コードを返します。 応答には、チームのアーカイブを処理するのに作成された [teamsAsyncOperation](../resources/teamsasyncoperation.md) の場所を含む`Location`ヘッダーも含まれます。 この場所に GET 要求を作成して、アーカイブ操作の状態を確認します。

## <a name="example"></a>例
#### <a name="request"></a>要求
要求の例を次に示します。
<!-- {
  "blockType": "ignored",
  "name": "archive_team"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/archive
```
#### <a name="response"></a>応答
応答の例を次に示します。
```http
HTTP/1.1 202 Accepted
Location: /teams({id})/operations({opId})
Content-Type: text/plain
Content-Length: 0
```
<!-- uuid: e848414b-4669-4484-ac36-1504c58a3fb8
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Archive team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
