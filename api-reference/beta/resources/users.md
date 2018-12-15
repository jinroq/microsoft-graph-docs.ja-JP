---
title: Microsoft Graph でのユーザーとの作業
description: Microsoft Graph を使用し、ユーザー達、他のユーザーやグループとの関係、彼らのメール、予定表、およびファイルに基づいて、魅力的なアプリケーション体験を構築することができます。
ms.openlocfilehash: 0bc1e0b045703c73a22568912db978d50c5a0c15
ms.sourcegitcommit: f3d479edf03935d0edbbc7668a65f7cde2a56c92
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/15/2018
ms.locfileid: "27283648"
---
# <a name="working-with-users-in-microsoft-graph"></a>Microsoft Graph でのユーザーとの作業

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

Microsoft Graph を使用し、ユーザー達、他のユーザーやグループとの関係、彼らのメール、予定表、およびファイルに基づいて、魅力的なアプリケーション体験を構築することができます。

Microsoft Graph を通じて、ふたつの方法で ユーザー にアクセスすることができます。

- 彼らの ID で、`/users/{id}` 
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
|photo| ユーザーのプロフィールの写真です。 |

詳細と全プロパティの一覧は、[ユーザー](user.md) オブジェクトを参照してください。

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
|[`/users/{id}/joinedTeams`](../api/user-list-joinedteams.md)| マイクロソフトのチームのメンバーであるユーザーの一覧を表示します。 |