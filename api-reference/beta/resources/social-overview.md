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
# <a name="use-the-microsoft-graph-api-to-integrate-social-intelligence-in-an-app"></a><span data-ttu-id="0bd0d-103">Microsoft Graph API を使用してアプリにソーシャル インテリジェンスを統合する</span><span class="sxs-lookup"><span data-stu-id="0bd0d-103">Use the Microsoft Graph API to integrate social intelligence in an app</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0bd0d-104">Microsoft Graph では、コンテキストにおけるユーザーのソーシャル ジェスチャをサポートし、ユーザーとソーシャルに関する役立つデータにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="0bd0d-104">Microsoft Graph supports social gestures in a user's social context, and provides access to useful people and social data.</span></span>

## <a name="aggregate-and-extract-specific-information-about-people"></a><span data-ttu-id="0bd0d-105">ユーザーに関する特有の情報を集約して抽出する</span><span class="sxs-lookup"><span data-stu-id="0bd0d-105">Aggregate and extract specific information about people</span></span>

<span data-ttu-id="0bd0d-106">[person](../resources/person.md) リソースと People API を使用して、メール、連絡先、およびソーシャル ネットワークから、個人に関する情報を集約することができます。</span><span class="sxs-lookup"><span data-stu-id="0bd0d-106">Use the [person](../resources/person.md) resource and the People API to aggregate information about a person from across mail, contacts, and social networks.</span></span> <span data-ttu-id="0bd0d-107">結果は、複数のコミュニケーション、コラボレーション、およびビジネスのリレーションシップを基に、関連性によって並べられます。</span><span class="sxs-lookup"><span data-stu-id="0bd0d-107">The results are ordered by their relevance, which is determined by the criteria specified in the request and ranked based on multiple communication, collaboration and business relationships.</span></span> <span data-ttu-id="0bd0d-108">API を使用すると、条件に基づいて、個人の閲覧、並べ替え、選択、フィルター、または検索を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="0bd0d-108">The API lets you browse, sort, select, filter, or search for persons based on your criteria.</span></span>

- [<span data-ttu-id="0bd0d-109">ユーザーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="0bd0d-109">List people</span></span>](../api/user-list-people.md)

## <a name="manage--mentions"></a><span data-ttu-id="0bd0d-110">@- メンションを管理する</span><span class="sxs-lookup"><span data-stu-id="0bd0d-110">Manage @-Mentions (preview)</span></span>

<span data-ttu-id="0bd0d-111">ソーシャルの世界では、メッセージ内で受信者に通知して注意を引くために受信者に呼びかけることが一般的に行われています。</span><span class="sxs-lookup"><span data-stu-id="0bd0d-111">Calling out a recipient to notify and get the recipient's attention in a message is a common social gesture.</span></span>
<span data-ttu-id="0bd0d-112">[mention](../resources/mention.md) リソースと Mentions API には、[メッセージ](../resources/message.md)内で受信者に呼びかけたり、ユーザーが @-メンションを使用して通知しているすべてのメッセージを取得したり、メッセージの内の各メンションを取得したりする軽量のメカニズムが備わっています。</span><span class="sxs-lookup"><span data-stu-id="0bd0d-112">The [mention](../resources/mention.md) resource and the Mentions API provide a light-weight mechanism to call out a recipient in a [message](../resources/message.md), get all the messages in which a user is notified using an @-mention, or get each mention in a message.</span></span>

<!--
Include the next sentence when supporting events.

**Mention** is also supported by [Event](../resources/event.md).

-->

- <span data-ttu-id="0bd0d-113">新しいメッセージ内にメンションを作成する</span><span class="sxs-lookup"><span data-stu-id="0bd0d-113">Create mentions in a new message</span></span>

  - [<span data-ttu-id="0bd0d-114">新しいメッセージの一部としてメンションを作成および送信する</span><span class="sxs-lookup"><span data-stu-id="0bd0d-114">Create and send mentions as part of a new message</span></span>](../api/user-sendmail.md#request-2)
  - [<span data-ttu-id="0bd0d-115">下書きの一部としてメンションを作成する</span><span class="sxs-lookup"><span data-stu-id="0bd0d-115">Create mentions as part of a message draft</span></span>](../api/user-post-messages.md#request-2)

- <span data-ttu-id="0bd0d-116">メッセージのメンションに関する情報を取得する</span><span class="sxs-lookup"><span data-stu-id="0bd0d-116">Get information about mentions in a message</span></span>

  - [<span data-ttu-id="0bd0d-117">対象ユーザーについてメンションしている、サインイン ユーザーのメールボックス内のすべてのメッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="0bd0d-117">Get all the messages in the signed-in user's mailbox.</span></span>](../api/user-list-messages.md#request-2)
  - [<span data-ttu-id="0bd0d-118">特定のメッセージ内の各メンションの詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="0bd0d-118">Get details of each mention in a message</span></span>](../api/message-get.md#request-2)

- <span data-ttu-id="0bd0d-119">特定のメッセージ内の[メンションを削除する](../api/message-delete.md#request-2)</span><span class="sxs-lookup"><span data-stu-id="0bd0d-119">[Delete a mention in a message](../api/message-delete.md#request-2)</span></span>

## <a name="access-social-data-around-and-about-a-user"></a><span data-ttu-id="0bd0d-120">ユーザーに関するソーシャル データにアクセスする</span><span class="sxs-lookup"><span data-stu-id="0bd0d-120">Access social data around and about a user</span></span>

<span data-ttu-id="0bd0d-121">Office Graph は、Office 365 の各種エンティティ間のリレーションシップをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="0bd0d-121">Office Graph encapsulates the relationships between different entities in Office 365.</span></span> <span data-ttu-id="0bd0d-122">Office Graph を使用して、Office 365 全体における各ユーザーのソーシャル インサイトを取得できます。</span><span class="sxs-lookup"><span data-stu-id="0bd0d-122">Use Office Graph to get social insights into individual users across Office 365.</span></span>

- <span data-ttu-id="0bd0d-123">ユーザーの[周りで人気急上昇中](../api/insights-list-trending.md)の項目を取得する</span><span class="sxs-lookup"><span data-stu-id="0bd0d-123">List the items [trending around](../api/insights-list-trending.md) a user</span></span>
- <span data-ttu-id="0bd0d-124">ユーザーと[仕事をしている](../api/user-list-people.md)ユーザーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="0bd0d-124">List users who have been [working with](../api/user-list-people.md) a user</span></span>
