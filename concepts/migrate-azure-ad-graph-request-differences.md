---
title: Azure AD Graph と Microsoft Graph の間の相違を要求する
description: Microsoft Graph 要求と Azure AD 要求との相違について説明します。これは、アプリを新しいサービスに移行する際に役に立ちます。.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f046043b6a30d66cef96bb6eb6192bddd90d2f5f
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630210"
---
# <a name="request-differences-between-azure-ad-graph-and-microsoft-graph"></a>Azure AD Graph と Microsoft Graph の間の相違を要求する

この記事は、*手順 1:* [アプリを移行するプロセス](migrate-azure-ad-graph-planning-checklist.md)の API の相違点を確認します。

Microsoft Graph および Azure AD Graph API はどちらも REST Api であり、それぞれがクエリパラメーターの ODATA 規則をサポートしています。 ただし、この2つの Api の構文は異なります。

[グラフエクスプローラー](https://aka.ms/ge)を使用して、要求と応答の違いについて理解するための最適な方法として、自分のデータに対してこれらの要求パターンを試してみてください。

## <a name="basic-requests"></a>基本的な要求

次の表は、2つの Api の主な要求の違いを示しています。

|| Azure AD Graph | Microsoft Graph |
|---|---|---|
|要求の構文| `https://graph.windows.net/{tenant_id}/` <br> `{resource}?{version}&query-parameters` | `https://graph.microsoft.com/`<br>`{version}/{resource}?query-parameters`|
|サービス&nbsp;エンドポイント:||
|-&nbsp;全体|`https://graph.windows.net`|`https://graph.microsoft.com`|
|-&nbsp;US&nbsp;Gov&nbsp;L4|`https://graph.microsoftazure.us`|`https://graph.microsoft.us`|
|-&nbsp;US&nbsp;Gov&nbsp;L5&nbsp;(DOD)|`https://graph.microsoftazure.us`|`https://dod-graph.microsoft.us`|
|-&nbsp;ドイツ|`https://graph.cloudapi.de`|`https://graph.microsoft.de`|
|-&nbsp;中国&nbsp;(21vianet)| `https://graph.chinacloudapi.cn`|`https://microsoftgraph.chinacloudapi.cn`|
|{tenant_id}|要求内のテナントの ID を指定します。|要求では、アクセストークンから推論されるときに、テナント ID を指定することはオプションです。<br><br>テナント ID を指定する`{version}`と、はとの間`{resource}`で要求 URL になります。|
|4.0|必要なクエリパラメーターを使用して、要求に Azure AD Graph のリリースバージョンを指定します。|要求では、サービスエンドポイントの直後の URL パスの一部として、Microsoft Graph のリリースバージョンを指定します。|

Microsoft Graph では、Azure AD Graph と同じクエリパラメーターを引き続き使用できます。

### <a name="example-request-comparison"></a>要求の比較の例

"Dan" で始まる名前を持つすべてのユーザーの一覧を作成するとします。

Azure AD Graph では、次の要求を使用できます。

`https://graph.windows.net/contoso.com/users?$filter=startswith(givenName,'Dan')&api-version=1.6`

この要求:

- Azure AD Graph のバージョン1.6 を対象としています。  
- テナント`contoso.com` ID としてを指定します。  
- ユーザーリソースを呼び出します。  
- は、 `$filter`クエリパラメーターを使用して、指定された名前`Dan`ので始まる応答を制限します。  

結果には、Daniel、Danforth、Danielle、Danerys などの名前を持つユーザーが含まれます。

Microsoft Graph については、次のような要求があります。

`https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName,'Dan')`

ここは：

- バージョンは`v1.0`です。  
- テナント ID は、アクセストークンから推論されます (ここでは示されていません)。  
- Resource パラメーターと`$filter` query パラメーターは Azure AD クエリと同じです。  

> **注**: Azure AD Graph .net クライアントライブラリを使用している場合は、詳細については「 [.net クライアントライブラリ](migrate-azure-ad-graph-client-libraries.md)」を参照し、Microsoft Graph .net クライアントライブラリに移動する方法について参照してください。

### <a name="key-identifiers-objectid-vs-id"></a>キー識別子: objectId vs id

Azure AD Graph では、すべてのエンティティのリソース型には、 **objectId**という一意の識別子 (またはキー) があります。  ほとんどの場合 (特に明記されていない限り)、同じ識別子が Microsoft Graph では**id**と呼ばれます。

## <a name="default-properties-and-select"></a>既定のプロパティと $select

GET 要求`$select`でクエリパラメーターを使用して、アプリが必要とするすべてのプロパティを含むように応答をカスタマイズします。

Microsoft Graph の**get**または**list**操作ユーザーまたはグループのリソースは、すべてのプロパティのサブセットを返します (_既定のプロパティ_と呼ばれます)。 既定のプロパティは、リソースでよく使用されるプロパティを表します。 一方、Azure AD Graph は、それぞれのリソースのすべてのプロパティの完全なセットを返します。

V 1.0 のその他のプロパティを取得するには、 `$select`クエリパラメーターを使用して、アプリで明示的に要求する必要があります。 これには、アプリが使用している可能性のあるディレクトリスキーマの拡張機能が含まれます。 アプリに実際に必要なプロパティのみを要求することをお勧めします。

違いを説明するために、Graph エクスプローラーを使用して次の要求を実行し、異なる応答を比較します。

```http
GET https://graph.microsoft.com/v1.0/me/
GET https://graph.microsoft.com/beta/me/
```

各クエリからの応答を確認します。 アドレス情報は、ベータ版では返されますが、/v1.0 のバージョンでは返されないことに注意してください。  これは、アドレスプロパティが既定のプロパティセットに含まれていないためです。

アプリがアドレスプロパティに依存している場合は、次の`$select`ように、version 1.0 要求を更新してクエリパラメーターを含める必要があります。

```http
https://graph.microsoft.com/v1.0/me/?$select=displayName,streetAddress,city,state,postalCode
```

この要求に対する応答には、アドレスのプロパティが含まれます。  **DisplayName**プロパティも含まれていますが、クエリパラメーターで指定されているためです。

詳細については、次の情報を参照してください。

- ユーザーの既定のプロパティ。「[ユーザー](/graph/api/resources/users?view=graph-rest-1.0) 」を参照
- `$select`パラメーターおよびその他のサポートされる ODATA クエリパラメーターについては、「[クエリパラメーターを使用して応答をカスタマイズする](/graph/query-parameters)」を参照してください。
- この他の推奨される最適化については、「[ベストプラクティス](/graph/best-practices-concept)」を参照してください。

## <a name="relationships-and-navigation-properties"></a>リレーションシップとナビゲーションプロパティ

リレーションシップ (またはナビゲーションプロパティ) は、Azure AD Graph と Microsoft Graph の重要な概念であり、関連するリソースのネットワークを作成します。 たとえば、**マネージャー**および**directreports**プロパティは、ユーザーリソースを拡張して組織階層を提供します。  

また、関係は、ユーザーが属するグループ、グループまたはディレクトリの役割に属するメンバーなどのメンバーシップも定義します。

Azure AD Graph 要求は`$link` 、リソース間の関係を示すために使用します。  Microsoft Graph では、代わりに ODATA 4.01 `$ref`表記を使用します。

次の表は、いくつかの例を示しています。

| タスク | Azure AD Graph | Microsoft Graph |
|------|----------------|-----------------|
| メンバーを追加する        | ```POST /groups/{id}/$link/members```        | ```POST /groups/{id}/members/$ref```        |
| メンバーリンクの一覧表示 | ```GET /groups/{id}/$link/members```         | ```GET /groups/{id}/members/$ref```         |
| メンバーを一覧表示する      | ```GET /groups/{id}/members```                | ```GET /groups/{id}/members```               |
| メンバーを削除する     | ```DELETE /groups/{id}/$link/members/{id}``` | ```DELETE /groups/{id}/members/{id}/$ref``` |

アプリを Microsoft Graph に移行する場合は、リソースの関連付け`$link`に使用する要求を探します。代わりにを使用`$ref`するように変更します。

## <a name="next-steps"></a>次のステップ

- Azure AD Graph と Microsoft Graph の[サービス機能の違い](migrate-azure-ad-graph-feature-differences.md)について説明します。
- [Microsoft Graph](/graph/overview)の概念とプラクティスについて説明します。
- [Graph エクスプローラー](https://aka.ms/ge)を使用して、Microsoft graph を試してみてください。
