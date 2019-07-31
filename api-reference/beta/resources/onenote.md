---
title: OneNote リソースの種類
description: OneNote リソースのエントリ ポイントです。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 215cf68cbf2efffacd6259aa64b0a00d5700b842
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009385"
---
# <a name="onenote-resource-type"></a>OneNote リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

OneNote リソースのエントリ ポイントです。

Microsoft Graph API を介しての OneNote サービスに対する呼び出しすべては、次のサービス ルート URL を使用します。

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

Office 365 またはコンシューマー OneDrive のユーザー ノートブック、Office 365 のグループ ノートブック、または SharePoint サイトでホストされているチームのノートブックを場所として指定できます。 

**ユーザー ノートブック** コンシューマー OneDrive または OneDrive for Business の個人用ノートブックにアクセスするには、次の URL のいずれかを使用します。

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

**グループ ノートブック** グループによって所有されているノートブックにアクセスするには、次のサービス ルート URL を使用します。

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
**SharePoint サイト ノートブック** SharePoint チーム サイトによって所有されているノートブックにアクセスするには、次のサービス ルート URL を使用します。

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

## <a name="authorization"></a>承認

OneNote API で動作するために必要なアクセス許可については、「[メモのアクセス許可](/graph/permissions-reference#notes-permissions)」を参照してください。

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|notebooks|[ノートブック](notebook.md) コレクション|ユーザーまたはグループが所有している OneNote ノートブックのコレクションです。 読み取り専用。 Null 許容型。|
|operations|[onenoteOperation](onenoteoperation.md)コレクション |OneNote の操作の状態です。 操作のコレクションを取得することはサポートされていませんが、応答で `Operation-Location` ヘッダーが返される場合には長時間実行処理の状態を取得できます。 読み取り専用。 Null 許容型。|
|ページ|[onenotePage](onenotepage.md)コレクション|ユーザーまたはグループが所有しているすべての OneNote ノートブックのページです。  読み取り専用。 Null 許容型。|
|リソース|[onenoteResource](onenoteresource.md)コレクション |OneNote ページの画像リソースおよび他のファイル リソースです。 リソース コレクションを取得することはサポートされていませんが、[特定のリソースのバイナリ コンテンツを取得](onenoteresource.md)できます。 読み取り専用。 Null 許容型。|
|sectionGroups|[sectionGroup](sectiongroup.md)コレクション|ユーザーまたはグループが所有しているすべての OneNote ノートブックのセクション グループです。  読み取り専用。 Null 許容型。|
|セクション|[onenoteSection](onenotesection.md)コレクション|ユーザーまたはグループが所有しているすべての OneNote ノートブック内のセクションです。  読み取り専用。 Null 許容型。|

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Create notebook](../api/onenote-post-notebooks.md) |[ノートブック](notebook.md)| ノートブックのコレクションに投稿してノートブックを作成します。|
|[List notebooks](../api/onenote-list-notebooks.md) |[ノートブック](notebook.md) コレクション| ノートブックのコレクションを取得します。|
|[Create page](../api/onenote-post-pages.md) |[onenotePage](onenotepage.md) | ページのコレクションに投稿してページを作成します。|
|[List pages](../api/onenote-list-pages.md) |[onenotePage](onenotepage.md)コレクション| ページのコレクションを取得します。|
|[List section groups](../api/onenote-list-sectiongroups.md) |[sectionGroup](sectiongroup.md)コレクション| セクション グループのコレクションを取得します。|
|[List sections](../api/onenote-list-sections.md) |[onenoteSection](onenotesection.md)コレクション| セクションのコレクションを取得します。|
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.onenote"
}-->
``` json
{
  "notebooks": [{ "@odata.type": "microsoft.graph.notebook" }],
  "operations": [{ "@odata.type": "microsoft.graph.onenoteOperation" }],
  "pages": [{ "@odata.type": "microsoft.graph.onenotePage" }],
  "resources": [ { "@odata.type": "microsoft.graph.onenoteResource" } ],
  "sectionGroups": [ { "@odata.type": "microsoft.graph.sectionGroup" } ],
  "sections": [ { "@odata.type": "microsoft.graph.onenoteSection" } ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenote resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
