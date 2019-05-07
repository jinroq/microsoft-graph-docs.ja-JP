---
title: Microsoft Graph におけるユーザーの概要
description: ユーザーは、Microsoft Graph における Azure Active Directory (Azure AD) の職場または学校のユーザー アカウント、または Microsoft アカウントの表現です。 Microsoft Graph の **user** リソースは、ユーザーと関連性のあるリレーションシップやリソースにアクセスする際に使用できるハブです。
author: dkershaw10
localization_priority: Priority
ms.openlocfilehash: 4b9af2e4c1a7b461f6b515b48aba75d6af77d1d9
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33599815"
---
# <a name="overview-of-users-in-microsoft-graph"></a><span data-ttu-id="e6784-104">Microsoft Graph におけるユーザーの概要</span><span class="sxs-lookup"><span data-stu-id="e6784-104">Overview of users in Microsoft Graph</span></span>

<span data-ttu-id="e6784-105">ユーザーは、Microsoft Graph における Azure Active Directory (Azure AD) の職場または学校のユーザー アカウント、または Microsoft アカウントの表現です。</span><span class="sxs-lookup"><span data-stu-id="e6784-105">Users are the representation of an Azure Active Directory (Azure AD) work or school user account or a Microsoft account in Microsoft Graph.</span></span> <span data-ttu-id="e6784-106">Microsoft Graph の **user** リソースは、ユーザーと関連性のあるリレーションシップやリソースにアクセスする際に使用できるハブです。</span><span class="sxs-lookup"><span data-stu-id="e6784-106">The **user** resource in Microsoft Graph is a hub from which you can access the relationships and resources that are relevant to your users.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/TUMPipN3UFI]

## <a name="develop-user-centric-applications"></a><span data-ttu-id="e6784-107">ユーザー中心のアプリケーションを開発する</span><span class="sxs-lookup"><span data-stu-id="e6784-107">Develop user-centric applications</span></span>

<span data-ttu-id="e6784-108">Microsoft Graph を使用して、サインインしているユーザーと文脈上関連性のあるリレーションシップ、ドキュメント、連絡先、およびユーザー設定にアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="e6784-108">You can use Microsoft Graph to access the relationships, documents, contacts, and preferences that are contextually relevant to the signed-in user.</span></span> <span data-ttu-id="e6784-109">**user** リソースを使用すると、追加の呼び出しを実行せずにユーザー リソースにアクセスして操作したり、特定の認証情報を調べたり、他の Microsoft Graph リソースに対して直接クエリを発行したりできます。</span><span class="sxs-lookup"><span data-stu-id="e6784-109">The **user** resource provides straightforward way for you to access and manipulate user resources without having to perform additional calls, look up specific authentication information, and directly issue queries against other Microsoft Graph resources.</span></span>

<span data-ttu-id="e6784-110">ユーザーの情報やデータにアクセスするには、[ユーザーの代わりにアクセスを取得する](auth-v2-user.md)必要があります。</span><span class="sxs-lookup"><span data-stu-id="e6784-110">To access a user's information and data, you'll need to [get access on their behalf](auth-v2-user.md).</span></span> <span data-ttu-id="e6784-111">[管理者の同意](permissions-reference.md)を得てアプリケーションを認証することにより、ユーザーに関連する幅広いエンティティを操作および更新できます。</span><span class="sxs-lookup"><span data-stu-id="e6784-111">Authenticating your application with [admin consent](permissions-reference.md) enables you to work with and update a wider range of entities associated with a user.</span></span>

### <a name="manage-your-organization"></a><span data-ttu-id="e6784-112">組織の管理</span><span class="sxs-lookup"><span data-stu-id="e6784-112">Manage your organization</span></span>

<span data-ttu-id="e6784-113">組織内に新しいユーザーを作成したり、既存のユーザーのリソースやリレーションシップを更新したりします。</span><span class="sxs-lookup"><span data-stu-id="e6784-113">Create new users in your organization or update the resources and relationships for existing users.</span></span> <span data-ttu-id="e6784-114">Microsoft Graph を使用して、次のユーザー管理タスクを実行できます。</span><span class="sxs-lookup"><span data-stu-id="e6784-114">You can use Microsoft Graph to perform the following user management tasks:</span></span> 

- <span data-ttu-id="e6784-115">作成または Azure AD 組織内のユーザーを作成または削除する。</span><span class="sxs-lookup"><span data-stu-id="e6784-115">Create or delete users in your Azure AD organization.</span></span>
- <span data-ttu-id="e6784-116">ユーザーのグループ メンバーシップを一覧表示し、ユーザーがグループのメンバーであるかどうかを確認する。</span><span class="sxs-lookup"><span data-stu-id="e6784-116">List a user's group memberships and determine whether a user is a member of a group.</span></span>
- <span data-ttu-id="e6784-117">ユーザーへの報告やユーザーへの管理者の割り当てを行うユーザーを一覧表示する。</span><span class="sxs-lookup"><span data-stu-id="e6784-117">List the users who report to a user and assign managers to a user.</span></span>
- <span data-ttu-id="e6784-118">ユーザーの写真をアップロードまたは取得する。</span><span class="sxs-lookup"><span data-stu-id="e6784-118">Upload or retrieve a photo for the user.</span></span>

### <a name="work-with-calendars-and-tasks"></a><span data-ttu-id="e6784-119">予定表とタスクの操作</span><span class="sxs-lookup"><span data-stu-id="e6784-119">Work with calendars and tasks</span></span>

<span data-ttu-id="e6784-120">ユーザーの予定表やユーザーに関連付けられている予定表グループを表示、照会、更新できます。次のような操作が含まれます。</span><span class="sxs-lookup"><span data-stu-id="e6784-120">You can view, query, and update user calendar and calendar groups associated with a user, including:</span></span>

- <span data-ttu-id="e6784-121">ユーザーの予定表でイベントを一覧表示し、作成する。</span><span class="sxs-lookup"><span data-stu-id="e6784-121">List and create events on a users calendar.</span></span>
- <span data-ttu-id="e6784-122">ユーザーに割り当てられたタスクを表示する。</span><span class="sxs-lookup"><span data-stu-id="e6784-122">View tasks assigned to a user.</span></span>
- <span data-ttu-id="e6784-123">一連のユーザーのために空いている会議時間を検索する。</span><span class="sxs-lookup"><span data-stu-id="e6784-123">Find free meeting times for a set of users.</span></span>
- <span data-ttu-id="e6784-124">ユーザーの予定表に設定されたリマインダーの一覧を取得する。</span><span class="sxs-lookup"><span data-stu-id="e6784-124">Get a list of reminders set on a user's calendar.</span></span>

### <a name="administer-mail-and-handle-contacts"></a><span data-ttu-id="e6784-125">メールの管理と連絡先の処理</span><span class="sxs-lookup"><span data-stu-id="e6784-125">Administer mail and handle contacts</span></span>

<span data-ttu-id="e6784-126">ユーザーのメール設定と連絡先リストを構成し、ユーザーの代わりにメールを送信できます。次のような操作が含まれます。</span><span class="sxs-lookup"><span data-stu-id="e6784-126">You can configure user mail settings and contact lists and send mail on a user's behalf, including:</span></span>

- <span data-ttu-id="e6784-127">メール メッセージを一覧表示し、新しいメールを送信する。</span><span class="sxs-lookup"><span data-stu-id="e6784-127">List mail messages and send new mail.</span></span>
- <span data-ttu-id="e6784-128">ユーザーの連絡先を作成および一覧表示し、連絡先をフォルダーに整理する。</span><span class="sxs-lookup"><span data-stu-id="e6784-128">Create and list user contacts and organize contacts in folders.</span></span>
- <span data-ttu-id="e6784-129">メールボックスのフォルダーと設定を取得し、更新する。</span><span class="sxs-lookup"><span data-stu-id="e6784-129">Retrieve and update mailbox folders and settings.</span></span>

### <a name="enrich-your-app-with-user-insights"></a><span data-ttu-id="e6784-130">ユーザーのインサイトを使用したアプリの強化</span><span class="sxs-lookup"><span data-stu-id="e6784-130">Enrich your app with user insights</span></span>

<span data-ttu-id="e6784-131">ユーザーに関連するドキュメントや連絡先のうち、最近使用したものや人気上昇中のものを奨励することで、アプリケーションの関連性を最大化します。</span><span class="sxs-lookup"><span data-stu-id="e6784-131">Maximize relevance in your application by promoting recently used or trending documents and contacts associated with a user.</span></span> <span data-ttu-id="e6784-132">Microsoft Graph を使用して次のことができます。</span><span class="sxs-lookup"><span data-stu-id="e6784-132">You can use Microsoft Graph to:</span></span>

- <span data-ttu-id="e6784-133">ユーザーが最近表示および変更したドキュメントを返す。</span><span class="sxs-lookup"><span data-stu-id="e6784-133">Return documents recently viewed and modified by a user.</span></span>
- <span data-ttu-id="e6784-134">ユーザーのアクティビティで人気上昇中のドキュメントやサイトを返す。</span><span class="sxs-lookup"><span data-stu-id="e6784-134">Return documents and sites trending around a user's activity.</span></span>
- <span data-ttu-id="e6784-135">ユーザーがメールや OneDrive for Business で共有しているドキュメントを一覧表示する。</span><span class="sxs-lookup"><span data-stu-id="e6784-135">List documents shared with a user through email or OneDrive for Business.</span></span>

## <a name="api-reference"></a><span data-ttu-id="e6784-136">API リファレンス</span><span class="sxs-lookup"><span data-stu-id="e6784-136">API reference</span></span>
<span data-ttu-id="e6784-137">このサービスの API リファレンスをお探しですか?</span><span class="sxs-lookup"><span data-stu-id="e6784-137">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="e6784-138">Microsoft Graph v1.0 の Users API</span><span class="sxs-lookup"><span data-stu-id="e6784-138">Users API in Microsoft Graph v1.0</span></span>](/graph/api/resources/users?view=graph-rest-1.0)
- [<span data-ttu-id="e6784-139">Microsoft Graph ベータ版の Users API</span><span class="sxs-lookup"><span data-stu-id="e6784-139">Users API in Microsoft Graph beta</span></span>](/graph/api/resources/users?view=graph-rest-beta)

## <a name="next-steps"></a><span data-ttu-id="e6784-140">次のステップ</span><span class="sxs-lookup"><span data-stu-id="e6784-140">Next steps</span></span>

- <span data-ttu-id="e6784-141">[ユーザーの操作](/graph/api/resources/users?view=graph-rest-1.0)方法の詳細を確認する</span><span class="sxs-lookup"><span data-stu-id="e6784-141">Learn more about how to [work with users](/graph/api/resources/users?view=graph-rest-1.0).</span></span>
- <span data-ttu-id="e6784-142">[Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)の **user** リソースを使用して自分自身のデータを調べる</span><span class="sxs-lookup"><span data-stu-id="e6784-142">Explore your own data from the **user** resource in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="e6784-143">[ユーザーの代わり](auth-v2-user.md)、または[管理者の同意を得たデーモンまたはサービスとして](auth-v2-service.md) Microsoft Graph を使用して認証します。</span><span class="sxs-lookup"><span data-stu-id="e6784-143">Authenticate with Microsoft Graph [on behalf of a user](auth-v2-user.md) or [as a daemon or service by consent of an administrator](auth-v2-service.md).</span></span>
- <span data-ttu-id="e6784-144">[Azure AD API](/graph/api/resources/azure-ad-overview?view=graph-rest-1.0) を使用してユーザーのアクセス制御とポリシーを設定する</span><span class="sxs-lookup"><span data-stu-id="e6784-144">Set access control and policies for users with the [Azure AD API](/graph/api/resources/azure-ad-overview?view=graph-rest-1.0).</span></span>
- <span data-ttu-id="e6784-145">アプリからユーザー データにアクセスするために必要な[権限](permissions-reference.md)を確認する</span><span class="sxs-lookup"><span data-stu-id="e6784-145">Review the [permissions](permissions-reference.md) your app will need to access user data.</span></span> 
<!-- This isn't really a next step; let's remove to keep the list of links concise.>
- Stay up to date with Microsoft Graph [changelog](changelog.md).
-->
