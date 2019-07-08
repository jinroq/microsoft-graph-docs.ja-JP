---
title: Microsoft Graph で OneNote API を使用する場合のベスト プラクティス
description: この記事では、Microsoft Graph で OneNote API を使用するための推奨事項を提供します。 これらの推奨事項は、Stack Overflow と Twitter でよく寄せられる質問への回答に基づいています。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 95c135ec405764a53f06fed2f9ac2dde6b4138bd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32560915"
---
# <a name="best-practices-for-working-with-the-onenote-api-in-microsoft-graph"></a>Microsoft Graph で OneNote API を使用する場合の推奨事項

この記事では、Microsoft Graph で OneNote API を使用するための推奨事項を提供します。 これらの推奨事項は、Stack Overflow と Twitter でよく寄せられる質問への回答に基づいています。

## <a name="use-select-to-select-the-minimum-set-of-properties-you-need"></a>$Select を使用して、必要なプロパティの最小限のセットを選択する

リソース (たとえば、ノートブック内のセクション) のクエリを実行するときには、次のような要求を行います。

```http
GET ~/notebooks/{id}/sections
```

これは、セクションのすべてのプロパティを取得します。 ただし、すべてのプロパティが必要とは限りません。 次の例のように、`$select` クエリ パラメーターを使用して、必要なプロパティだけを返すことができます。

```http
GET ~/notebooks/{id}/sections?$select=id,displayName
```

同じアプローチは、他の OneNote API に適用されます。

## <a name="use-expand-instead-of-making-multiple-api-calls"></a>複数の API 呼び出しを実行するのではなく、$expand を使用します。

ユーザーのノートブック、セクション、およびセクション グループのすべてを階層的なビューで取得します。 次の方法でこれを行います。

* `GET ~/notebooks` を呼び出して、ノートブックの一覧を取得します。

* 取得したすべてのノートブックについて、`GET ~/notebooks/{notebookId}/sections` を呼び出してセクションの一覧を取得します。

* 取得したすべてのノートブックについて、`GET ~/notebooks/{notebookId}/sectionGroups` を呼び出してセクション グループの一覧を取得します。

* 必要に応じて、セクション グループを再帰的に反復処理できます。

この方法 (サービスへ何回かの連続した余分なラウンドトリップを実行) でも可能ですが、より優れたアプローチは、`$expand` クエリ パラメーターを使用することです。 

```http
GET ~/notebooks?$expand=sections,sectionGroups($expand=sections)
```

これにより、1 回のネットワーク ラウンドトリップで同じ結果が得られ、より良いパフォーマンスが得られます。

## <a name="when-getting-all-pages-for-a-user-do-so-for-each-section-separately"></a>ユーザーに対してすべてのページを取得する場合は、セクションごとに個別に行ってください。

Microsoft Graph はすべてのページを取得するためにエンドポイントを公開しますが、これはユーザーがアクセス権を持っているすべてのページを取得する最良の方法ではありません。 ユーザーが持つセクションが多すぎると、これによりタイムアウトやパフォーマンスの低下を招きます。 各セクションを反復処理して、個別にそれぞれのページを取得することをお勧めします。

たとえば、この呼び出しを使用する代わりに、(この API はページ化されているので、すべてのページを一度にフェッチすることはできません):

```http
GET ~/pages
```

(特にすべてのセクションが必要ない場合は) 次の呼び出しを何回か使用することをお勧めします。

```http
GET ~/sections/{id}/pages
```

ページのメタデータを取得するには、既定値 `lastModifiedDateTime` の順序付けを上書きします。 それらを `lastModifiedDateTime` で並べ替える必要がないときには、より速くページを取得できます。 これを行うには、たとえば他の任意のプロパティで並べ替えることができます。

```http
GET ~/sections/{id}/pages?$select=id,title,createdDateTime&$orderby=createdDateTime
```
