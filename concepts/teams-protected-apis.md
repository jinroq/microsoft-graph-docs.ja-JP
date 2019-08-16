---
title: Microsoft Teams の保護された API
description: 機密データにアクセスする Microsoft Graph の Microsoft Teams API は、保護された API であると見なされます。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 124a2f96f2c59909311fad605beeb1273193d8af
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364531"
---
# <a name="protected-apis-in-microsoft-teams"></a>Microsoft Teams の保護された API

機密データにアクセスする Microsoft Graph の Microsoft Teams API は、保護された API であると見なされます。 これらの API を使用する前に、この API では、アクセス許可および同意だけではなく、追加の検証を行う必要があります。

現在、保護されている API は次の通りです。
* [アプリケーション アクセス許可](auth/auth-concepts.md#microsoft-graph-permissions)を使用する[チャネル メッセージの一覧表示](/graph/api/channel-list-messages?view=graph-rest-beta) 
* [アプリケーション アクセス許可](auth/auth-concepts.md#microsoft-graph-permissions)を使用する[チャネル メッセージの取得](/graph/api/channel-get-message?view=graph-rest-beta)
* [アプリケーション アクセス許可](auth/auth-concepts.md#microsoft-graph-permissions)を使用する[メッセージへの返信の一覧表示](/graph/api/channel-list-messagereplies?view=graph-rest-beta)
* [アプリケーション アクセス許可](auth/auth-concepts.md#microsoft-graph-permissions)を使用する[メッセージへの返信の取得](/graph/api/channel-get-messagereply?view=graph-rest-beta)
* [アプリケーション アクセス許可](auth/auth-concepts.md#microsoft-graph-permissions)を使用する[チャット内のメッセージの一覧表示](/graph/api/chatmessage-list?view=graph-rest-beta) 
* [アプリケーション アクセス許可](auth/auth-concepts.md#microsoft-graph-permissions)を使用する[チャット内のメッセージの取得](/graph/api/chatmessage-get?view=graph-rest-beta) 

これらの保護された API へのアクセス権を要求するには、次の [要求フォーム](http://aka.ms/teamsgraph/requestaccess)の入力を完了します。 毎週水曜日にアクセス要求を確認し、毎週金曜日に承認を展開します。
要求フォーム以外の情報も提供したい場合は、[teamsAppPerms@microsoft.com](mailto:teamsAppPerms@microsoft.com) までご連絡ください。
