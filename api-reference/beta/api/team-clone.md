---
title: チームのクローンを作成します。
description: チームのコピーを作成します。 この操作では、対応するグループのコピーも作成します。
ms.openlocfilehash: b49fa4262fe65be03b99f2107e9ef1b2799bfeb3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074404"
---
# <a name="clone-a-team"></a>チームのクローンを作成します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[チーム](../resources/team.md)のコピーを作成します。 この操作では、対応する[グループ](../resources/group.md)のコピーも作成します。
クローンを作成するチームのどの部分を指定できます。

- **アプリケーション**・ チームにインストールされているアプリケーションをマイクロソフト チームのコピーです。 
- **チャネル**は、チャネルの構造 (ただし、チャネル内のメッセージではない) をコピーします。
- **メンバー** -メンバーをコピーし、グループの所有者です。
- **設定**– は、キーのグループの設定と、チーム内のすべての設定をコピーします。
- **タブ**– は、チャネル内のタブにコピーします。

タブがクローン化されると、未構成の状態に移動する:、マイクロソフト チームのタブ バーに表示され、構成] 画面で移動します] をクリックします。 (タブを開いた人がアプリケーションを構成するのにはアクセス許可を持たない場合が表示されるタブが構成されていないことを説明するメッセージです。)

クローン作成は、時間のかかる操作です。
投稿クローンが返されるは、「実行中」または「成功」または「失敗」を表示する[操作](../resources/teamsasyncoperation.md)を取得する必要があります。 ステータスが「動作していない」まで取得を続行してください。 取得の推奨される間隔は、5 秒間です。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント)     | Group.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション                            | Group.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/clone
```

## <a name="request-headers"></a>要求ヘッダー
| ヘッダー       | 値 |
|:---------------|:--------|
| Authorization  | ベアラー {トークン}。必須。  |
| Content-Type  | application/json  |

## <a name="request-body"></a>要求本文

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|分類|文字列 (省略可能)|(低、中、または高のビジネス ・ インパクト) などのグループの分類について説明します。 このプロパティの有効値は、[テンプレートの定義](../resources/directorysettingtemplate.md)に基づいて、ClassificationList の[設定](../resources/directorysetting.md)値を作成することによって定義されます。 分類を指定しない場合、分類は、元のチームまたはグループからコピーされます。|
|description|文字列 (省略可能)|グループに関するオプションの説明。 このプロパティを指定しない場合、空白のままにします。|
|displayName|String|グループの表示名。このプロパティは、グループの作成時の必須プロパティであり、更新時にクリアすることはできません。$filter および $orderby をサポートします。|
|mailNickname|String|グループ、組織内で一意の電子メール エイリアス。 グループが作成されるとき、このプロパティを指定する必要があります。 $filter をサポートします。 このプロパティが指定されていない場合に、表示名から計算されます。 既知の問題: 現在、このプロパティは無視されます。|
|partsToClone| [clonableTeamParts](../resources/clonableteamparts.md) |クローンを作成する部品のコンマで区切られたリスト。 法的な部分は、「アプリケーション、タブ、設定、チャネル、メンバー"です。|
|visibility|[teamVisibilityType](../resources/teamvisibilitytype.md)(省略可能)| グループの可視性を指定します。 使用可能な値:**パブリック**、**プライベート**です。 可視性が指定されていない場合、元のチームまたはグループの表示と非表示がコピーされます。 **EducationClass**チームは、チームのクローンが作成されている場合、可視性パラメーターは無視されます、および新しいグループの表示/非表示を HiddenMembership に設定されます。|

## <a name="response"></a>応答

かどうかは成功すると、このメソッドは、`202 Accepted`の場所で応答コード: ヘッダーの[処理](../resources/teamsasyncoperation.md)リソースを指します。
操作が完了すると、処理リソースが送信されます作成したチームの id。

## <a name="example"></a>例
#### <a name="request"></a>要求
要求の例を次に示します。
<!-- {
  "blockType": "ignored",
  "name": "create_team"
}-->
```http
POST /teams/{id}/clone
Content-Type: application/json

{  
     "displayName": "Library Assist",
     "description": "Self help community for library",
     "mailNickname": "libassist",
     "partsToClone": "apps,tabs,settings,channels,members",
     "visibility": "public"
}
```

#### <a name="response"></a>応答
応答の例を次に示します。 注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。 実際の呼び出しではすべてのプロパティが返されます。
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 202 Accepted
Location: /teams{id}/operations({opId})
Content-Type: text/plain
Content-Length: 0
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
