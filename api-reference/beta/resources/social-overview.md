---
title: Microsoft Graph API を使用してアプリにソーシャル インテリジェンスを統合する
description: Microsoft Graph では、コンテキストにおけるユーザーのソーシャル ジェスチャをサポートし、ユーザーとソーシャルに関する役立つデータにアクセスできます。
localization_priority: Priority
author: simonhult
ms.prod: insights
ms.openlocfilehash: 45482d2e47c97b6c09302ab60ff9c031cef1e92a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345710"
---
# <a name="use-the-microsoft-graph-api-to-integrate-social-intelligence-in-an-app"></a>Microsoft Graph API を使用してアプリにソーシャル インテリジェンスを統合する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph では、コンテキストにおけるユーザーのソーシャル ジェスチャをサポートし、ユーザーとソーシャルに関する役立つデータにアクセスできます。

## <a name="aggregate-and-extract-specific-information-about-people"></a>ユーザーに関する特有の情報を集約して抽出する

[person](../resources/person.md) リソースと People API を使用して、メール、連絡先、およびソーシャル ネットワークから、個人に関する情報を集約することができます。 結果は、複数のコミュニケーション、コラボレーション、およびビジネスのリレーションシップを基に、関連性によって並べられます。 API を使用すると、条件に基づいて、個人の閲覧、並べ替え、選択、フィルター、または検索を行うことができます。

- [ユーザーを一覧表示する](../api/user-list-people.md)

## <a name="manage--mentions"></a>@- メンションを管理する

ソーシャルの世界では、メッセージ内で受信者に通知して注意を引くために受信者に呼びかけることが一般的に行われています。
[mention](../resources/mention.md) リソースと Mentions API には、[メッセージ](../resources/message.md)内で受信者に呼びかけたり、ユーザーが @-メンションを使用して通知しているすべてのメッセージを取得したり、メッセージの内の各メンションを取得したりする軽量のメカニズムが備わっています。

<!--
Include the next sentence when supporting events.

**Mention** is also supported by [Event](../resources/event.md).

-->

- 新しいメッセージ内にメンションを作成する

  - [新しいメッセージの一部としてメンションを作成および送信する](../api/user-sendmail.md#request-2)
  - [下書きの一部としてメンションを作成する](../api/user-post-messages.md#request-2)

- メッセージのメンションに関する情報を取得する

  - [対象ユーザーについてメンションしている、サインイン ユーザーのメールボックス内のすべてのメッセージを取得する](../api/user-list-messages.md#request-2)
  - [特定のメッセージ内の各メンションの詳細を取得する](../api/message-get.md#request-2)

- 特定のメッセージ内の[メンションを削除する](../api/message-delete.md#request-2)

## <a name="access-social-data-around-and-about-a-user"></a>ユーザーに関するソーシャル データにアクセスする

Office Graph は、Office 365 の各種エンティティ間のリレーションシップをカプセル化します。 Office Graph を使用して、Office 365 全体における各ユーザーのソーシャル インサイトを取得できます。

- ユーザーの[周りで人気急上昇中](../api/insights-list-trending.md)の項目を取得する
- ユーザーと[仕事をしている](../api/user-list-people.md)ユーザーを一覧表示する
