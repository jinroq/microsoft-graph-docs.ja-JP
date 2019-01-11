---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ドライブを取得する
localization_priority: Normal
ms.openlocfilehash: d18ee7191747b2c625b62bdecec6d3bffdf0f57e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859659"
---
# <a name="get-drive"></a>ドライブを取得する

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[Drive](../resources/drive.md) リソースのプロパティとリレーションシップを取得します。

ドライブとは、OneDrive または SharePoint のドキュメント ライブラリなど、ファイル システムの最上位コンテナーです。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All    |
|アプリケーション | Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All |

## <a name="get-current-users-onedrive"></a>現在のユーザーの OneDrive を取得する

(委任された認証を使用する場合) `me` シングルトンから、サインイン ユーザーのドライブにアクセスできます。

ユーザーの OneDrive はプロビジョニングされていないものの、ユーザーが OneDrive を使用するライセンスを持っている場合、委任された認証を使用するときに、この要求によりユーザーのドライブは自動的にプロビジョニングされます。

### <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read" } -->

```http
GET /me/drive
```

## <a name="get-a-users-onedrive"></a>ユーザーの OneDrive を取得する

ユーザーの OneDrive または OneDrive for Business にアクセスするには、User リソースについての**ドライブ** リレーションシップをアプリが要求する必要があります。

ユーザーの OneDrive はプロビジョニングされていないものの、ユーザーが OneDrive を使用するライセンスを持っている場合、委任された認証を使用するときに、この要求によりユーザーのドライブは自動的にプロビジョニングされます。

### <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```

### <a name="path-parameters"></a>パス パラメーター

| パラメーター名 | 値  | 説明                                       |
|:---------------|:-------|:--------------------------------------------------|
| _idOrUserPrincipalName_     | 文字列 | 必須。 OneDrive を所有するユーザー オブジェクトの識別子。 |

## <a name="get-the-document-library-associated-with-a-group"></a>グループに関連付けられたドキュメント ライブラリを取得する

グループの既定のドキュメント ライブラリにアクセスするには、そのグループについての**ドライブ** リレーションシップをアプリが要求する必要があります。

### <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all" } -->

```http
GET /groups/{groupId}/drive
```

### <a name="path-parameters"></a>パス パラメーター

| パラメーター名 | 値  | 説明                                       |
|:---------------|:-------|:--------------------------------------------------|
| _groupId_      | 文字列 | 必須。 ドキュメント ライブラリを所有するグループの識別子。 |

## <a name="get-the-document-library-for-a-site"></a>サイトのドキュメント ライブラリを取得する

[サイトの](../resources/site.md)既定のドキュメント ライブラリにアクセスするには、そのサイトについての**ドライブ** リレーションシップをアプリが要求する必要があります。

### <a name="http-request"></a>HTTP 要求

```http
GET /sites/{siteId}/drive
```

### <a name="path-parameters"></a>パス パラメーター

| パラメーター名 | 値  | 説明                                       |
|:---------------|:-------|:--------------------------------------------------|
| _siteId_       | 文字列 | 必須。 ドキュメント ライブラリを含むサイトの識別子。 |

## <a name="get-a-drive-by-id"></a>ID によりドライブを取得する

ドライブの一意の識別子を持っている場合、最上位ドライブのコレクションから直接アクセスできます。

### <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{driveId}
```

### <a name="path-parameters"></a>パス パラメーター

| パラメーター名 | 値  | 説明                                       |
|:---------------|:-------|:--------------------------------------------------|
| _driveId_      | 文字列 | 必須。 要求されるドライブの識別子。 |

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター

応答を形成するため、これらのメソッドは [$select クエリ パラメーター][odata-query-parameters]をサポートしています。

## <a name="response"></a>応答

各メソッドは、一致するドライブに応じた [Drive リソース][drive-resource]を応答本文で返します。

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.drive", "truncated": true, "name": ["get-drive-by-id", "get-drive-by-group", "get-drive-by-user", "get-drive-default"] } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "b!t18F8ybsHUq1z3LTz8xvZqP8zaSWjkFNhsME-Fepo75dTf9vQKfeRblBZjoSQrd7",
    "driveType": "business",
    "owner": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "Ryan Gregg"
        }
    },
    "quota": {
        "deleted": 256938,
        "remaining": 1099447353539,
        "state": "normal",
        "total": 1099511627776
    }
}
```

### <a name="error-response-codes"></a>エラー応答コード

(委任された認証を使用する場合) ドライブが存在しないために自動的にプロビジョニングできないなら、`HTTP 404` 応答が返されます。

[drive-resource]: ../resources/drive.md
[odata-query-parameters]: /graph/query-parameters

<!-- {
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "tocPath": "Drives/Get drive"
} -->
