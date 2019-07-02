---
title: Microsoft Graph API を使用して、アプリにソーシャル インテリジェンスとワークプレイス インテリジェンスを統合する
description: Microsoft Graph では、コンテキストにおけるユーザーのソーシャル ジェスチャをサポートし、ユーザーとソーシャルに関する役立つデータにアクセスできます。
localization_priority: Priority
author: simonhult
ms.prod: insights
ms.openlocfilehash: 0118902f42984a541c750f34db945bc0e7ede5f2
ms.sourcegitcommit: ee710ff556f4a7907181df5c323e345f52808ce2
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35417676"
---
# <a name="use-the-microsoft-graph-api-to-integrate-social-and-workplace-intelligence-in-an-app"></a><span data-ttu-id="26e56-103">Microsoft Graph API を使用して、アプリにソーシャル インテリジェンスとワークプレイス インテリジェンスを統合する</span><span class="sxs-lookup"><span data-stu-id="26e56-103">Use the Microsoft Graph API to integrate social intelligence in an app</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26e56-104">Microsoft Graph では、コンテキストにおけるユーザーのソーシャル ジェスチャをサポートし、ユーザーとソーシャルに関する役立つデータにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="26e56-104">Microsoft Graph supports social gestures in a user's social context, and provides access to useful people and social data.</span></span>

## <a name="aggregate-and-extract-specific-information-about-people"></a><span data-ttu-id="26e56-105">ユーザーに関する特有の情報を集約して抽出する</span><span class="sxs-lookup"><span data-stu-id="26e56-105">Aggregate and extract specific information about people</span></span>

<span data-ttu-id="26e56-106">[person](../resources/person.md) リソースと People API を使用して、メール、連絡先、およびソーシャル ネットワークから、個人に関する情報を集約することができます。</span><span class="sxs-lookup"><span data-stu-id="26e56-106">Use the [person](../resources/person.md) resource and the People API to aggregate information about a person from across mail, contacts, and social networks.</span></span> <span data-ttu-id="26e56-107">結果は、複数のコミュニケーション、コラボレーション、およびビジネスのリレーションシップを基に、関連性によって並べられます。</span><span class="sxs-lookup"><span data-stu-id="26e56-107">The results are ordered by their relevance based on multiple communication, collaboration, and business relationships.</span></span> <span data-ttu-id="26e56-108">API を使用すると、条件に基づいて、個人の閲覧、並べ替え、選択、フィルター、または検索を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="26e56-108">The API lets you browse, sort, select, filter, or search for persons based on your criteria.</span></span>

- [<span data-ttu-id="26e56-109">ユーザーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="26e56-109">List people</span></span>](../api/user-list-people.md)

## <a name="help-users-get-the-most-relevant-documents-for-their-work"></a><span data-ttu-id="26e56-110">ユーザーの仕事に最適なドキュメントの取得に役立つ</span><span class="sxs-lookup"><span data-stu-id="26e56-110">Help users get the most relevant documents for their work</span></span>

<span data-ttu-id="26e56-111">Insights API を使用して、ユーザーに最適なドキュメントを特定する:</span><span class="sxs-lookup"><span data-stu-id="26e56-111">Use the insights API to identify the most relevant documents for a user:</span></span> 

- <span data-ttu-id="26e56-112">ユーザーの[周りで人気急上昇中](../api/insights-list-trending.md)のドキュメントを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="26e56-112">List the items [trending around](../api/insights-list-trending.md) a user</span></span>
- <span data-ttu-id="26e56-113">ユーザーによって[使用される](../api/insights-list-used.md)ドキュメントを一覧表示する </span><span class="sxs-lookup"><span data-stu-id="26e56-113">List documents [used by](../api/insights-list-used.md) a user</span></span>
- <span data-ttu-id="26e56-114">ユーザーが[共有先または共有元](../api/insights-list-shared.md)のドキュメントを一覧表示する </span><span class="sxs-lookup"><span data-stu-id="26e56-114">List documents [shared with or shared by](../api/insights-list-shared.md) a user</span></span>

## <a name="manage--mentions"></a><span data-ttu-id="26e56-115">@- メンションを管理する</span><span class="sxs-lookup"><span data-stu-id="26e56-115">Manage @-Mentions</span></span>

<span data-ttu-id="26e56-116">ソーシャルの世界では、メッセージ内で受信者に通知して注意を引くために受信者に呼びかけることが一般的に行われています。</span><span class="sxs-lookup"><span data-stu-id="26e56-116">Calling out a recipient to notify and get the recipient's attention in a message is a common social gesture.</span></span>
<span data-ttu-id="26e56-117">[mention](../resources/mention.md) リソースと Mentions API には、[メッセージ](../resources/message.md)内で受信者に呼びかけたり、ユーザーが @-メンションを使用して通知しているすべてのメッセージを取得したり、メッセージの内の各メンションを取得したりする軽量のメカニズムが備わっています。</span><span class="sxs-lookup"><span data-stu-id="26e56-117">The [mention](../resources/mention.md) resource and the Mentions API provide a light-weight mechanism to call out a recipient in a [message](../resources/message.md), get all the messages in which a user is notified using an @-mention, or get each mention in a message.</span></span>

<!--
Include the next sentence when supporting events.

**Mention** is also supported by [Event](../resources/event.md).

-->

- <span data-ttu-id="26e56-118">新しいメッセージ内にメンションを作成する</span><span class="sxs-lookup"><span data-stu-id="26e56-118">Create mentions in a new message</span></span>

  - [<span data-ttu-id="26e56-119">新しいメッセージの一部としてメンションを作成および送信する</span><span class="sxs-lookup"><span data-stu-id="26e56-119">Create and send mentions as part of a new message</span></span>](../api/user-sendmail.md#request-2)
  - [<span data-ttu-id="26e56-120">下書きの一部としてメンションを作成する</span><span class="sxs-lookup"><span data-stu-id="26e56-120">Create mentions as part of a message draft</span></span>](../api/user-post-messages.md#request-2)

- <span data-ttu-id="26e56-121">メッセージのメンションに関する情報を取得する</span><span class="sxs-lookup"><span data-stu-id="26e56-121">Get information about mentions in a message</span></span>

  - [<span data-ttu-id="26e56-122">対象ユーザーについてメンションしている、サインイン ユーザーのメールボックス内のすべてのメッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="26e56-122">Get all the messages in the signed-in user's mailbox that mention the user</span></span>](../api/user-list-messages.md#request-2)
  - [<span data-ttu-id="26e56-123">特定のメッセージ内の各メンションの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="26e56-123">Get details of each mention in a message</span></span>](../api/message-get.md#request-2)

- <span data-ttu-id="26e56-124">特定のメッセージ内の[メンションを削除する](../api/message-delete.md#request-2)</span><span class="sxs-lookup"><span data-stu-id="26e56-124">[Delete a mention](../api/message-delete.md#request-2) in a message</span></span>

