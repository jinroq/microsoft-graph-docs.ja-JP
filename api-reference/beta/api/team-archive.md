---
title: チームをアーカイブする
description: '指定したチームをアーカイブします。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a009dc7214627575b00b2537875e5561b0515d32
ms.sourcegitcommit: a39db1154a07aa0dd7e96fb6f9d7e891a812207e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/16/2019
ms.locfileid: "31889920"
---
# <a name="archive-team"></a>チームをアーカイブする

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定した[チーム](../resources/team.md)をアーカイブします。 チームがアーカイブされている場合、ユーザーはチーム内のチャネルでメッセージを送信したり、チームの名前、説明、その他の設定を編集したり、通常はチームにほとんど変更を加えたりすることができなくなります。
チームに対するメンバーシップの変更は引き続き許可されます。

アーカイブは、非同期操作です。 非同期操作が正常に完了すると、この API からの応答によって発生する可能性があるチームがアーカイブされます。

チームをアーカイブするためには、チームと[グループ](../resources/group.md)に所有者が必要です。

チームをアーカイブされた状態から復元するには、API を使用して[アーカイブ](team-unarchive.md)を解除します。

## <a name="permissions"></a>権限
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
要求では、必要に_応じ_て、 `shouldSetSpoSiteReadOnlyForMembers`次のように JSON 本文にパラメーターを含めることができます。
```JSON
{
    "shouldSetSpoSiteReadOnlyForMembers": true
}
```
このオプションのパラメーターは、チームに関連付けられた Sharepoint Online サイトでチームメンバーのアクセス許可を読み取り専用に設定するかどうかを定義します。 false に設定するか、または本文を完全に省略すると、この手順はスキップされます。

## <a name="response"></a>応答

アーカイブが正常に開始された場合、 `202 Accepted`このメソッドは応答コードを返します。 応答には、チームの`Location`アーカイブを処理するために作成された[teamsAsyncOperation](../resources/teamsasyncoperation.md)の場所を含むヘッダーも含まれます。 この場所に GET 要求を行うことによって、アーカイブ操作の状態を確認します。

## <a name="example"></a>例
#### <a name="request"></a>要求
要求の例を次に示します。
<!-- {
  "blockType": "ignored",
  "name": "archive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/archive
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
<!--
{
  "type": "#page.annotation",
  "description": "Archive team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/team-archive.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
