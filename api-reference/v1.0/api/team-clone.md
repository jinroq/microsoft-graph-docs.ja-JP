---
title: チームのクローンを作成する
description: チームのコピーを作成します。 この操作では、対応するグループのコピーも作成されます。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c3b6b8e9615491275f981a759fabc4ed6a683373
ms.sourcegitcommit: a39db1154a07aa0dd7e96fb6f9d7e891a812207e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/16/2019
ms.locfileid: "31889927"
---
# <a name="clone-a-team"></a>チームのクローンを作成する



[チーム](../resources/team.md)のコピーを作成します。 この操作では、対応する[グループ](../resources/group.md)のコピーも作成されます。
チームのどの部分を複製するかを指定できます。

- **アプリ**-チームにインストールされている Microsoft Teams アプリをコピーします。 
- **** チャネル–チャネル構造をコピーします (チャネル内のメッセージはコピーしません)。
- **members** –グループのメンバーと所有者をコピーします。
- **設定**–主要なグループ設定と共に、チーム内のすべての設定をコピーします。
- **タブ**–チャネル内のタブをコピーします。

タブが複製されると、それらは未構成状態になります。これは、Microsoft Teams のタブバーに表示されます。これを最初に開いたときに、構成画面が表示されます。 (タブを開くユーザーがアプリを構成するためのアクセス許可を持っていない場合は、タブがまだ構成されていないことを示すメッセージが表示されます)。

複製は、長時間実行される操作です。
POST 複製が戻ると、"実行中" または "成功" または "失敗" のどちらであるかを確認するには、[操作](../resources/teamsasyncoperation.md)を取得する必要があります。 状態が "実行中" ではない状態になるまで、この操作を続行する必要があります。 推奨される遅延時間は、5秒です。

## <a name="permissions"></a>権限

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
|classification|String (省略可能)|グループの分類 (低、中、高のビジネスへの影響など) を記述します。 分類が指定されていない場合は、元のチーム/グループから分類がコピーされます。|
|説明|String (省略可能)|グループに関するオプションの説明。 このプロパティが指定されていない場合は、空白のままになります。|
|displayName|String|グループの表示名。このプロパティは、グループの作成時の必須プロパティであり、更新時にクリアすることはできません。$filter および $orderby をサポートします。|
|mailNickname|String|グループのメール エイリアスです (組織内で一意)。 このプロパティは、グループの作成時に指定する必要があります。 $filter をサポートします。 このプロパティが指定されていない場合は、displayName から計算されます。 既知の問題: このプロパティは現在無視されています。|
|partstoclone| [clonableTeamParts](../resources/clonableteamparts.md) |クローンするパーツのコンマ区切りのリスト。 法的パーツとは、「アプリ、タブ、設定、チャネル、メンバー」のことです。|
|visibility|[teamVisibilityType](../resources/teamvisibilitytype.md)オプション| グループを表示するかどうかを指定します。 可能な値は、 **Private**、 **Public**です。 visibility が指定されていない場合、表示は元のチーム/グループからコピーされます。 複製対象のチームが**educationClass**チームの場合、visibility パラメーターは無視され、新しいグループの表示が HiddenMembership に設定されます。|

## <a name="response"></a>応答

成功した場合、このメソッドは`202 Accepted` 、 [operation](../resources/teamsasyncoperation.md)リソースをポイントする Location: ヘッダーを持つ応答コードを返します。
操作が完了すると、作成されたチームの id が操作リソースに通知されます。

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
Location: /teams({id})/operations({opId})
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
