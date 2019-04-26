---
title: 'serviceprincipal: delta'
description: リソースコレクション全体の完全な読み取りを実行せずに、新しく作成、更新、または削除されたサービスプリンシパルを取得します。 詳細については、「デルタクエリの使用」を参照してください。
localization_priority: Normal
ms.openlocfilehash: f405dec49de75789d015988b0043c1ea57973cfb
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331384"
---
# <a name="serviceprincipal-delta"></a>serviceprincipal: delta

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

リソースコレクション全体の完全な読み取りを実行せずに、新しく作成、更新、または削除されたサービスプリンシパルを取得します。 詳細については、「[デルタクエリの使用](/graph/delta-query-overview)」を参照してください。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。


|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | Application.ReadWrite.All、Directory.Read.All |

## <a name="http-request"></a>HTTP 要求

変更の追跡を開始するには、serviceprincipal リソースにデルタ関数を含む要求を行います。 

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/delta
```

### <a name="query-parameters"></a>クエリ パラメーター

変更の追跡では、1回以上の**デルタ**関数呼び出しが発生します。 クエリパラメーター ( `$deltatoken`および`$skiptoken`以外) を使用する場合は、最初の**デルタ**要求で指定する必要があります。 Microsoft Graph は、指定されたパラメーターを、 `nextLink`応答で指定`deltaLink`されたまたは URL のトークン部分に自動的にエンコードします。 必要なクエリ パラメーターを前もって 1 回指定しておくだけで済みます。 その後の要求では、前の応答で得られた `nextLink` や `deltaLink` の URL をコピーして適用します。エンコード済みの必要なパラメーターがこの URL に既に含まれているためです。

| クエリ パラメーター      | 種類   |説明|
|:---------------|:--------|:----------|
| $deltatoken | string | 同じリソースコレクションに対する前`deltaLink`の**デルタ**関数呼び出しの URL で返された[状態トークン](/graph/delta-query-overview)。変更追跡のラウンドが終了したことを示します。 そのコレクションの次の`deltaLink`ラウンドの変更追跡の最初の要求で、このトークンを含む URL 全体を保存して適用します。|
| $skiptoken | string | 前の**デルタ**関数呼び出しの`nextLink` URL で[状態トークン](/graph/delta-query-overview)が返され、同じリソースコレクションに追跡すべき変更が他にもあることを示します。 |

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター

このメソッドは、応答をカスタマイズするための OData クエリ パラメーターをサポートします。

- 任意の GET リクエストと同様に `$select` クエリ パラメーターを使用して、最善のパフォーマンスを得るために必要なプロパティのみを指定することができます。_Id_ プロパティは常に返されます。 

- 次のサポートに`$filter`制限があります。
  * サポートされ`$filter`ている唯一の式は、id: `$filter=id+eq+{value}`または`$filter=id+eq+{value1}+or+id+eq+{value2}`を使用して特定のリソースの変更を追跡することです。 指定できる id の数は、URL の最大の長さによって制限されます。


## <a name="request-headers"></a>要求ヘッダー
| 名前       | 説明|
|:---------------|:----------|
| Authorization  | Bearer &lt;token&gt;|
| Content-Type  | application/json |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

### <a name="response"></a>応答

成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[serviceprincipal](../resources/serviceprincipal.md)コレクションオブジェクトを返します。 応答には、nextlink url または deltaLink url も含まれます。 

- URL が返される場合は、セッションに取得するデータの追加ページがあります。`nextLink` アプリケーションは、応答に`nextLink` `deltaLink` url が含まれるまで、url を使用して要求を引き続き行います。

- URL が返される場合、返されるリソースの既存の状態に関するデータはありません。 今後のリソースの`deltaLink`変更点については、URL を永続化して使用してください。

参照先:</br>
- 詳細については、「[デルタ クエリの使用](/graph/delta-query-overview)」をご覧ください</br>
- 要求の例については、「[ユーザーに対する増分の変更の取得](/graph/delta-query-users)」をご覧ください。</br>

### <a name="example"></a>例
##### <a name="request"></a>要求
<!-- {
  "blockType": "request",
  "name": "servicePrincipal_delta"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/delta
```

##### <a name="response"></a>応答
注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#servicePrincipals",
  "@odata.nextLink":"https://graph.microsoft.com/beta/servicePrincipals/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
     {
      "accountEnabled": true,
      "addIns": [
        {
          "id": "id-value",
          "type": "type-value",
          "properties": [
            {
              "key": "key-value",
              "value": "value-value"
            }
          ]
        }
      ],
      "appDisplayName": "appDisplayName-value",
      "appId": "appId-value",
      "appOwnerOrganizationId": "appOwnerOrganizationId-value",
      "appRoleAssignmentRequired": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "servicePrincipal: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
