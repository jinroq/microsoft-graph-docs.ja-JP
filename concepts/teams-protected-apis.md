---
title: Microsoft Teams の保護された API
description: 機密データにアクセスする Microsoft Graph の Microsoft Teams API は、保護された API であると見なされます。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: ebf0bbda324f62c6413bbe3d70ade33a5052da0d
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778762"
---
# <a name="protected-apis-in-microsoft-teams"></a><span data-ttu-id="38713-103">Microsoft Teams の保護された API</span><span class="sxs-lookup"><span data-stu-id="38713-103">Protected APIs in Microsoft Teams</span></span>

<span data-ttu-id="38713-104">機密データにアクセスする Microsoft Graph の Microsoft Teams API は、保護された API であると見なされます。</span><span class="sxs-lookup"><span data-stu-id="38713-104">Microsoft Teams APIs in Microsoft Graph that access sensitive data are considered protected APIs.</span></span> <span data-ttu-id="38713-105">これらの API を使用する前に、この API では、アクセス許可および同意だけではなく、追加の検証を行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="38713-105">These APIs require that you have additional validation, beyond permissions and consent, before you can use them.</span></span>

<span data-ttu-id="38713-106">現在、保護されている API は次の通りです。</span><span class="sxs-lookup"><span data-stu-id="38713-106">The following APIs are currently protected:</span></span>
* <span data-ttu-id="38713-107">[アプリケーション アクセス許可](auth/auth-concepts.md#microsoft-graph-permissions)を使用する[チャネル メッセージの一覧表示](/graph/api/channel-list-messages?view=graph-rest-beta) </span><span class="sxs-lookup"><span data-stu-id="38713-107">[List channel messages](/graph/api/channel-list-messages?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="38713-108">[アプリケーション アクセス許可](auth/auth-concepts.md#microsoft-graph-permissions)を使用する[チャネル メッセージの取得](/graph/api/channel-get-message?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="38713-108">[Get channel message](/graph/api/channel-get-message?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="38713-109">[アプリケーション アクセス許可](auth/auth-concepts.md#microsoft-graph-permissions)を使用する[メッセージへの返信の一覧表示](/graph/api/channel-list-messagereplies?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="38713-109">[List replies to a message](/graph/api/channel-list-messagereplies?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="38713-110">[アプリケーション アクセス許可](auth/auth-concepts.md#microsoft-graph-permissions)を使用する[メッセージへの返信の取得](/graph/api/channel-get-messagereply?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="38713-110">[Get a reply to a message](/graph/api/channel-get-messagereply?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="38713-111">[アプリケーション アクセス許可](auth/auth-concepts.md#microsoft-graph-permissions)を使用する[チャット内のメッセージの一覧表示](/graph/api/chatmessage-list?view=graph-rest-beta) </span><span class="sxs-lookup"><span data-stu-id="38713-111">[List messages in a chat](/graph/api/chatmessage-list?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>
* <span data-ttu-id="38713-112">[アプリケーション アクセス許可](auth/auth-concepts.md#microsoft-graph-permissions)を使用する[チャット内のメッセージの取得](/graph/api/chatmessage-get?view=graph-rest-beta) </span><span class="sxs-lookup"><span data-stu-id="38713-112">[Get message in chat](/graph/api/chatmessage-get?view=graph-rest-beta) using [application permissions](auth/auth-concepts.md#microsoft-graph-permissions)</span></span>

<span data-ttu-id="38713-113">これらの保護された API へのアクセス権を要求するには、次の [要求フォーム](http://aka.ms/teamsgraph/requestaccess)の入力を完了します。</span><span class="sxs-lookup"><span data-stu-id="38713-113">To request access to these protected APIs, complete the following [request form](http://aka.ms/teamsgraph/requestaccess).</span></span> <span data-ttu-id="38713-114">毎週アクセス権の要求を確認しています。</span><span class="sxs-lookup"><span data-stu-id="38713-114">We review access requests weekly.</span></span> <span data-ttu-id="38713-115">要求フォーム以外の情報も提供したい場合は、[teamsAppPerms@microsoft.com](mailto:teamsAppPerms@microsoft.com)までご連絡ください。</span><span class="sxs-lookup"><span data-stu-id="38713-115">If you would like to provide information in addition to the form, you can contact [teamsAppPerms@microsoft.com](mailto:teamsAppPerms@microsoft.com).</span></span>
