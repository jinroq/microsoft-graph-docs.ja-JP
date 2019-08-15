---
title: Microsoft Graph でのユーザーとの作業
description: Microsoft Graph を使用し、ユーザー達、他のユーザーやグループとの関係、彼らのメール、予定表、およびファイルに基づいて、魅力的なアプリケーション体験を構築することができます。
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 4d405dcc5e7881c7a404e5ca16f87c889cd5ccc7
ms.sourcegitcommit: 00959f992b9b77c98ec1fe2f185cc7fd098ab24b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36426413"
---
# <a name="working-with-users-in-microsoft-graph"></a>Microsoft Graph でのユーザーの操作

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph を使用し、ユーザー達、他のユーザーやグループとの関係、彼らのメール、予定表、およびファイルに基づいて、魅力的なアプリケーション体験を構築することができます。

Microsoft Graph から 2 つの方法でユーザーにアクセスすることができます。

- ユーザーの ID で、`/users/{id}`
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

| プロパティ | 説明 |
|----------|-------------|
| displayName | アドレス帳に表示されるユーザーの名前。|
|givenName| ユーザーの名。 |
|surname| ユーザーの姓。 |
|mail| ユーザーの電子メール アドレス。 |
|photo| ユーザーのプロフィール写真。 |

詳細と全プロパティの一覧は、[user](user.md) オブジェクトを参照してください。

## <a name="common-operations"></a>共通の操作

>**注:** これらの操作のいくつかは、追加のアクセス許可を必要とします。

| パス    | 説明 |
|---------|-------------|
|[`/users`](../api/user-list.md) | 組織内のユーザーを一覧表示します。 |
|[`/users/{id}`](../api/user-get.md) | Id で特定のユーザーを取得します。 |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| ユーザーのプロフィール写真を取得します。 |
|[`/users/{id}/manager`](../api/user-list-manager.md) | ユーザーの上司を取得します。 |
|[`/users/{id}/messages`](../api/user-list-messages.md)| プライマリ受信トレイ内のユーザーの電子メール メッセージを一覧表示します。 |
|[`/users/{id}/events`](../api/user-list-events.md) | ユーザーの予定表の今後のイベントを一覧表示します。 |
|[`/users/{id}/drive`](../api/drive-get.md)| ユーザーの OneDrive ファイル ストアを取得します。 |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| ユーザーがメンバーであるグループを一覧表示します。 |
|[`/users/{id}/joinedTeams`](../api/user-list-joinedteams.md)| ユーザーがメンバーである Microsoft Teams を一覧表示します。 |
