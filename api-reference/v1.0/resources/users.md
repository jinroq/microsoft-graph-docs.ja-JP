---
title: Microsoft Graph でのユーザーとの作業
description: Microsoft Graph を使用し、ユーザー達、他のユーザーやグループとの関係、彼らのメール、予定表、およびファイルに基づいて、魅力的なアプリケーション体験を構築することができます。
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: d171a247b980ef2f1b1d762df696699eae7a1890
ms.sourcegitcommit: 00959f992b9b77c98ec1fe2f185cc7fd098ab24b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36426406"
---
# <a name="working-with-users-in-microsoft-graph"></a>Microsoft Graph でのユーザーの操作

Microsoft Graph を使用し、ユーザー達、他のユーザーやグループとの関係、彼らのメール、予定表、およびファイルに基づいて、魅力的なアプリケーション体験を構築することができます。

Microsoft Graph を通じて、ふたつの方法で [ユーザー](user.md) にアクセスすることができます。

- 彼らの ID で、`/users/{id | userPrincipalName}`
- `/users/{signed-in user's id}` と同じである、サインインしているユーザーの `/me` エイリアス使用して

## <a name="authorization"></a>承認

ユーザー操作へのアクセスには、次のいずれかの [アクセス許可](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) が必要です。最初の 3 つのアクセス許可は、ユーザーがアプリケーションに付与できます。残りは管理者のみがアプリケーションに付与できます。

- User.ReadBasic.All
- User.Read
- User.ReadWrite
- User.Read.All
- User.ReadWrite.All
- Directory.Read.All
- Directory.ReadWrite.All
- Directory.AccessAsUser.All

## <a name="common-properties"></a>共通プロパティ

以下は、ユーザーまたはユーザーの一覧を取得するときに返されるプロパティの既定のセットを表します。 これらは、利用可能なすべてのプロパティのサブセットです。 より多くのユーザー プロパティを取得するには、`$select` クエリ パラメーターを使用します。

|プロパティ |説明 |
|:----------|:-------------|
|id | ユーザーの一意の識別子。|
|businessPhones | ユーザーの電話番号。|
|displayName | アドレス帳に表示されるユーザーの名前。|
|givenName| ユーザーの名。 |
|jobTitle | ユーザーの役職。|
|mail| ユーザーの電子メール アドレス。 |
|mobilePhone | ユーザーの携帯電話番号。|
|officeLocation | ユーザーの物理的なオフィスの場所。|
|preferredLanguage | ユーザーの選択言語。|
|surname| ユーザーの姓。 |
|userPrincipalName| ユーザーのプリンシパル名。 |

詳細と全プロパティの一覧は、[ユーザー](user.md) オブジェクトを参照してください。

## <a name="common-operations"></a>共通の操作

> **注:** これらの操作のいくつかは、追加のアクセス許可を必要とします。

| パス    | 説明 |
|:---------|:-------------|
|[`/users`](../api/user-list.md) | 組織内のユーザーを一覧表示します。 |
|[`/users/{id}`](../api/user-get.md) | Id で特定のユーザーを取得します。 |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| ユーザーのプロフィール写真を取得します。 |
|[`/users/{id}/manager`](../api/user-list-manager.md) | ユーザーの上司を取得します。 |
|[`/users/{id}/messages`](../api/user-list-messages.md)| プライマリ受信トレイ内のユーザーの電子メール メッセージを一覧表示します。 |
|[`/users/{id}/events`](../api/user-list-events.md) | ユーザーの予定表の今後のイベントを一覧表示します。 |
|[`/users/{id}/drive`](../api/drive-get.md)| ユーザーの OneDrive ファイル ストアを取得します。 |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| ユーザーがメンバーであるグループを一覧表示します。 |
