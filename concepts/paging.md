---
title: 'アプリで Microsoft Graph データをページングする '
description: "応答内の、結果の次のページへの URL を含む odata.nextLink' プロパティ。 "
author: piotrci
localization_priority: Priority
ms.openlocfilehash: 8c39ff697de2d6afdb2f24c1ec99d2ce5a89b32c
ms.sourcegitcommit: 7c03131291113c343a98bb0234d31bd4535a4050
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/22/2019
ms.locfileid: "35133804"
---
# <a name="paging-microsoft-graph-data-in-your-app"></a>アプリで Microsoft Graph データをページングする 

Microsoft Graph に対するクエリの中には、サーバー側のページングを使用したり、1 つの要求におけるページ サイズを限定するために `$top` クエリ パラメーターを使用したりすることによって、複数のデータ ページを返すものがあります。要求セットが複数ページにまたがる場合、Microsoft Graph は、結果の次のページへの URL が含まれる `@odata.nextLink` プロパティを応答で返します。 

たとえば、次の URL の場合、組織内のすべてのユーザーのうち、`$top` クエリ パラメーターで指定されたページ サイズ 5 のユーザーを要求します。

```html
https://graph.microsoft.com/v1.0/users?$top=5
```

結果に 5 人を超えるユーザーが含まれる場合、Microsoft Graph は、最初のページのユーザーに加えて、次のような `@odata:nextLink` プロパティを返します。

```json
"@odata.nextLink": "https://graph.microsoft.com/v1.0/users?$top=5&$skiptoken=X%274453707 ... 6633B900000000000000000000%27"
```

この `@odata:nextLink` プロパティの URL 値を Microsoft Graph に送信することによって、結果の次のページを取得できます。 

```html
https://graph.microsoft.com/v1.0/users?$top=5&$skiptoken=X%274453707 ... 6633B900000000000000000000%27
```

その後、Microsoft Graph はすべての結果ページが読み取られるまで、それぞれの応答の `@odata:nextLink` プロパティ内の次のページのデータへの参照を返します。

>**重要:** 結果の次のページの要求には、`@odata:nextLink` プロパティの URL 全体を含める必要があります。 クエリの実行対象の API によって、`@odata:nextLink` URL 値には `$skiptoken` と `$skip` のいずれかのクエリ パラメーターが入ります。 また、URL には、元の要求にある他のクエリ パラメーターすべても含まれます。 `$skiptoken` 値または `$skip` 値を抽出して、別の要求で使用しないでください。 

ページング動作は、それぞれの Microsoft Graph API によって異なります。 ページングされたデータを扱う場合には、以下の事柄を考慮してください。

- API によって、既定および最大のページ サイズが異なる場合があります。
- (`$top` クエリ パラメーターを使用して) 対象の API の最大ページ サイズを超えるページ サイズを指定する場合には、API によって動作が異なる可能性があります。 API によっては要求されたページ サイズが無視されることがあります。対象 API の最大ページ サイズに既定で設定されたり、Microsoft Graph によってエラーが返されたりする場合があります。 
- すべてのリソースまたはリレーションシップでページングがサポートされているわけではありません。たとえば、[directoryRoles](/graph/api/resources/directoryrole?view=graph-rest-1.0) に対するクエリではページングはサポートされていません。これにはロール メンバーおよびロール オブジェクト自体の読み取りも含まれます。

## <a name="learn-more-about-paging"></a>ページングの詳細
次のビデオでは、Microsoft Graph でのページングについて説明します。

> [!VIDEO https://www.youtube-nocookie.com/embed/DB_NoC9a1JI]