---
title: MailSearchFolder を作成します。
description: 指定されたユーザーのメールボックスに新しい mailSearchFolder を作成するのにには、この API を使用します。
localization_priority: Normal
ms.openlocfilehash: 07c6b96bc2dec35d06b5563673012ca0eafb3885
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840188"
---
# <a name="create-mailsearchfolder"></a>MailSearchFolder を作成します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

指定されたユーザーのメールボックスに新しい[mailSearchFolder](../resources/mailsearchfolder.md)を作成するのにには、この API を使用します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類 | アクセス許可 (特権の小さいものから大きいものへ) |
|:----------------|:--------------------------------------------|
|委任 (職場または学校のアカウント) | Mail.ReadWrite    |
|委任 (個人用 Microsoft アカウント) | Mail.ReadWrite    |
|アプリケーション | Mail.ReadWrite |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

フォルダー ID の場合、またはよく知られているフォルダー名とクエリの URL では、親フォルダーを指定します。 サポートされている既知のフォルダー名の一覧については、「[mailFolder リソースの種類](../resources/mailfolder.md)」を参照してください。

## <a name="request-headers"></a>要求ヘッダー

| ヘッダー | 値 |
|:-------|:------|
| Authorization | `Bearer {token}`. 必須。 |
| Content-Type | `application/json`. 必須。 |

## <a name="request-body"></a>要求本文

要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。

| パラメーター | Type | 説明 |
|:----------|:-----|:------------|
| @odata.type | String | 作成するフォルダーの種類。 "Microsoft.graph.mailSearchFolder"に設定します。 |
| displayName | String | 新しいフォルダーの表示名です。|
| includeNestedFolders | ブール型 | どのメールボックス フォルダー階層を走査する必要があります。 `true`詳細検索をする必要があることを意味時に`false`簡易検索を代わりに行う必要があることを意味します。 |
| sourceFolderIDs | String コレクション | メールボックス フォルダーをマイニングする必要があります。 |
| filterQuery | String | メッセージをフィルタ リングする OData クエリです。 |

## <a name="response"></a>応答

かどうかは成功すると、このメソッドを返します`201 Created`応答コードおよび応答の本文に[mailSearchFolder](../resources/mailsearchfolder.md)オブジェクトです。

## <a name="example"></a>例

#### <a name="request"></a>要求

要求の例を次に示します。
<!-- {
  "blockType": "request",
  "name": "create_mailsearchfolder"
}-->

```http
POST https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childfolders
Content-type: application/json
Content-length: 159

{
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "displayName": "Get MyAnalytics",
  "includeNestedFolders": true,
  "sourceFolderIDs": ["AAMkAGVmMDEzM"],
  "filterQuery": "contains(subject, 'MyAnalytics')"
}
```

#### <a name="response"></a>応答

応答の例を次に示します。

>**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。 実際の呼び出しではすべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.mailSearchFolder",
  "id": "AAMkAGVmMDEzMx",
  "displayName": "Get MyAnalytics",
  "parentFolderId": "AAMkAGVmMDEzMy",
  "childFolderCount": 0,
  "unreadItemCount": 0,
  "totalItemCount": 13,
  "wellKnownName": null,
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIDs": [
    "AAMkAGVmMDEzMi"
  ],
  "filterQuery": "contains(subject, 'MyAnalytics')"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create mailSearchFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
