---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: パスで SharePoint サイトを取得する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 146a3c80bd3cd4cae53766c19206dc79930f7edf
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33330384"
---
# <a name="get-a-site-resource-by-path"></a>パスを使用したサイト リソースの取得

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[サイト][] リソースのプロパティとリレーションシップを取得します。**サイト** リソースは、SharePoint のチーム サイトを表します。

[サイト]: ../resources/site.md

[ID を使用したサイト](site-get.md)の取得のほかに、サーバーの相対 URL パスに基づいてサイトを取得できます。

* サイト コレクションのホスト名 (contoso.sharepoint.com)
* サーバーのホスト名を基準にしたサイトのパス。

予約済みのサイト識別子 `root` もあります。これは次に示すように、常にターゲットのルート サイトを参照します。

* `/sites/root`:テナントのルート サイト。
* `/groups/{group-id}/sites/root`:グループのチーム サイト。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Sites.Read.All、Sites.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | Sites.Read.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求

相対パスを使用してルートの SharePoint サイトにアクセスするには、次のようにします。

<!-- { "blockType": "request", "name": "get-site-by-hostname-and-path", "scopes": "service.sharepoint sites.read.all" } -->

```http
GET /sites/{hostname}:/{relative-path}
```

## <a name="response"></a>応答

このメソッドは、一意の識別子によって参照されるサイトの[サイト][] リソースを返します。

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.site" } -->

```http
HTTP/1.1 200 OK

{
  "id": "contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE",
  "owner": {
    "user": { 
      "displayName": "Daron Spektor",
      "id": "5280E7FE-DC7A-4486-9490-E790D81DFEB3"
    }
  },
  "displayName": "OneDrive Team Site",
  "name": "1drvteam",
  "createdDateTime": "2017-05-09T20:56:00Z",
  "lastModifiedDateTime": "2017-05-09T20:56:01Z",
  "webUrl": "https://contoso.sharepoint.com/teams/1drvteam"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Get by path",
  "suppressions": []
}
-->
