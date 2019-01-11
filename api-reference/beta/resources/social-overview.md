---
title: Microsoft グラフ API を使用して、アプリケーションでは、ソーシャル ・ インテリジェンスを統合するために
description: Graph では、コンテキストでは、ユーザーのソーシャル、ソーシャルのジェスチャをサポートしているし、便利な人や社会のデータにアクセスを提供します。
localization_priority: Priority
ms.openlocfilehash: b3b71cf1bad0d860978c75c88f0b77a32eab1a0c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862490"
---
# <a name="use-the-microsoft-graph-api-to-integrate-social-intelligence-in-an-app"></a><span data-ttu-id="63df9-103">Microsoft グラフ API を使用して、アプリケーションでは、ソーシャル ・ インテリジェンスを統合するために</span><span class="sxs-lookup"><span data-stu-id="63df9-103">Use the Microsoft Graph API to integrate social intelligence in an app</span></span>

> <span data-ttu-id="63df9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="63df9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="63df9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="63df9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="63df9-106">Graph では、コンテキストでは、ユーザーのソーシャル、ソーシャルのジェスチャをサポートしているし、便利な人や社会のデータにアクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="63df9-106">Microsoft Graph supports social gestures in a user's social context, and provides access to useful people and social data.</span></span>

## <a name="aggregate-and-extract-specific-information-about-people"></a><span data-ttu-id="63df9-107">集約し、他のユーザーに関する特定の情報を抽出</span><span class="sxs-lookup"><span data-stu-id="63df9-107">Aggregate and extract specific information about people</span></span>

<span data-ttu-id="63df9-108">メール、連絡先、およびソーシャル ネットワークの間で[ユーザー](../resources/person.md)リソースとユーザー API から、ある人物に関する情報を集約を使用します。</span><span class="sxs-lookup"><span data-stu-id="63df9-108">Use the [person](../resources/person.md) resource and the People API to aggregate information about a person from across mail, contacts, and social networks.</span></span> <span data-ttu-id="63df9-109">結果は、複数の通信、コラボレーション、および取引関係に基づく妥当性で並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="63df9-109">The results are ordered by their relevance based on multiple communication, collaboration, and business relationships.</span></span> <span data-ttu-id="63df9-110">API は、参照、並べ替え、選択、フィルター、またはの条件に基づいてユーザーを検索することができます。</span><span class="sxs-lookup"><span data-stu-id="63df9-110">The API lets you browse, sort, select, filter, or search for persons based on your criteria.</span></span>

- [<span data-ttu-id="63df9-111">ユーザーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="63df9-111">List people</span></span>](../api/user-list-people.md)

## <a name="manage--mentions"></a><span data-ttu-id="63df9-112">@-参照投稿を管理します。</span><span class="sxs-lookup"><span data-stu-id="63df9-112">Manage @-Mentions</span></span>

<span data-ttu-id="63df9-113">受信者に通知し、メッセージ内の受信者の注意を引くために呼び出すことは、一般的なソーシャル ジェスチャです。</span><span class="sxs-lookup"><span data-stu-id="63df9-113">Calling out a recipient to notify and get the recipient's attention in a message is a common social gesture.</span></span>
<span data-ttu-id="63df9-114">[説明](../resources/mention.md)リソースに関する API[メッセージ](../resources/message.md)の受信者を @ の説明を使用してユーザーに通知するすべてのメッセージを取得するには、軽量のメカニズムを提供やメッセージに記載されている各を取得します。</span><span class="sxs-lookup"><span data-stu-id="63df9-114">The [mention](../resources/mention.md) resource and the Mentions API provide a light-weight mechanism to call out a recipient in a [message](../resources/message.md), get all the messages in which a user is notified using an @-mention, or get each mention in a message.</span></span>

<!--
Include the next sentence when supporting events.

**Mention** is also supported by [Event](../resources/event.md).

-->

- <span data-ttu-id="63df9-115">新しいメッセージ内にメンションを作成する</span><span class="sxs-lookup"><span data-stu-id="63df9-115">Create mentions in a new message</span></span>

  - [<span data-ttu-id="63df9-116">新しいメッセージの一部としてメンションを作成および送信する</span><span class="sxs-lookup"><span data-stu-id="63df9-116">Create and send mentions as part of a new message</span></span>](../api/user-sendmail.md#request-2)
  - [<span data-ttu-id="63df9-117">下書きの一部としてメンションを作成する</span><span class="sxs-lookup"><span data-stu-id="63df9-117">Create mentions as part of a message draft</span></span>](../api/user-post-messages.md#request-2)

- <span data-ttu-id="63df9-118">メッセージのメンションに関する情報を取得する</span><span class="sxs-lookup"><span data-stu-id="63df9-118">Get information about mentions in a message</span></span>

  - [<span data-ttu-id="63df9-119">ユーザーに言及する、サインイン中のユーザーのメールボックス内のすべてのメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="63df9-119">Get all the messages in the signed-in user's mailbox that mention the user</span></span>](../api/user-list-messages.md#request-2)
  - [<span data-ttu-id="63df9-120">メッセージ内の各メンションの詳細の取得</span><span class="sxs-lookup"><span data-stu-id="63df9-120">Get details of each mention in a message</span></span>](../api/message-get.md#request-2)

- <span data-ttu-id="63df9-121">メッセージで[参照を削除](../api/message-delete.md#request-2)</span><span class="sxs-lookup"><span data-stu-id="63df9-121">[Delete a mention](../api/message-delete.md#request-2) in a message</span></span>

## <a name="access-social-data-around-and-about-a-user"></a><span data-ttu-id="63df9-122">周りと、ユーザーのソーシャル データにアクセス</span><span class="sxs-lookup"><span data-stu-id="63df9-122">Access social data around and about a user</span></span>

<span data-ttu-id="63df9-123">Office のグラフは、Office 365 内の別のエンティティ間の関係をカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="63df9-123">Office Graph encapsulates the relationships between different entities in Office 365.</span></span> <span data-ttu-id="63df9-124">Office 365 の間で個々 のユーザーのソーシャル洞察を取得するのにには、Office のグラフを使用します。</span><span class="sxs-lookup"><span data-stu-id="63df9-124">Use Office Graph to get social insights into individual users across Office 365.</span></span>

- <span data-ttu-id="63df9-125">アイテム[の周囲にトレンド ・](../api/insights-list-trending.md)ユーザーの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="63df9-125">List the items [trending around](../api/insights-list-trending.md) a user</span></span>
- <span data-ttu-id="63df9-126">[使用](../api/user-list-people.md)されているユーザーのユーザーを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="63df9-126">List users who have been [working with](../api/user-list-people.md) a user</span></span>
