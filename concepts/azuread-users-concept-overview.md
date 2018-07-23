# <a name="overview-of-users-in-microsoft-graph"></a><span data-ttu-id="7d6e3-101">Microsoft Graph におけるユーザーの概要</span><span class="sxs-lookup"><span data-stu-id="7d6e3-101">Overview of users in Microsoft Graph</span></span>

<span data-ttu-id="7d6e3-102">ユーザーは、Microsoft Graph における Azure Active Directory (Azure AD) の職場または学校のユーザー アカウント、または Microsoft アカウントの表現です。</span><span class="sxs-lookup"><span data-stu-id="7d6e3-102">Users are the representation of an Azure Active Directory (Azure AD) work or school user account or a Microsoft account in Microsoft Graph.</span></span> <span data-ttu-id="7d6e3-103">Microsoft Graph の **user** リソースは、ユーザーと関連性のあるリレーションシップやリソースにアクセスする際に使用できるハブです。</span><span class="sxs-lookup"><span data-stu-id="7d6e3-103">The **user** resource in Microsoft Graph is a hub from which you can access the relationships and resources that are relevant to your users.</span></span>

![予定表、メール、連絡先、会議、タスク、サイト、およびドキュメントに接続されているユーザーを示す図](images/users.png)

## <a name="develop-user-centric-applications"></a><span data-ttu-id="7d6e3-105">ユーザー中心のアプリケーションを開発する</span><span class="sxs-lookup"><span data-stu-id="7d6e3-105">Develop user-centric applications</span></span>

<span data-ttu-id="7d6e3-106">Microsoft Graph を使用して、サインインしているユーザーと文脈上関連性のあるリレーションシップ、ドキュメント、連絡先、およびユーザー設定にアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="7d6e3-106">You can use Microsoft Graph to access the relationships, documents, contacts, and preferences that are contextually relevant to the signed-in user.</span></span> <span data-ttu-id="7d6e3-107">**user** リソースを使用すると、追加の呼び出しを実行せずにユーザー リソースにアクセスして操作したり、特定の認証情報を調べたり、他の Microsoft Graph リソースに対して直接クエリを発行したりできます。</span><span class="sxs-lookup"><span data-stu-id="7d6e3-107">The **user** resource provides straightforward way for you to access and manipulate user resources without having to perform additional calls, look up specific authentication information, and directly issue queries against other Microsoft Graph resources.</span></span>

<span data-ttu-id="7d6e3-108">ユーザーの情報やデータにアクセスするには、[ユーザーの代わりにアクセスを取得する](https://developer.microsoft.com/graph/docs/concepts/auth_v2_user)必要があります。</span><span class="sxs-lookup"><span data-stu-id="7d6e3-108">To access a user's information and data, you'll need to [get access on their behalf](https://developer.microsoft.com/graph/docs/concepts/auth_v2_user).</span></span> <span data-ttu-id="7d6e3-109">[管理者の同意](https://developer.microsoft.com/en-us/graph/docs/concepts/permissions_reference)を得てアプリケーションを認証することにより、ユーザーに関連する幅広いエンティティを操作および更新できます。</span><span class="sxs-lookup"><span data-stu-id="7d6e3-109">Authenticating your application with [admin consent](https://developer.microsoft.com/en-us/graph/docs/concepts/permissions_reference) enables you to work with and update a wider range of entities associated with a user.</span></span>

### <a name="manage-your-organization"></a><span data-ttu-id="7d6e3-110">組織の管理</span><span class="sxs-lookup"><span data-stu-id="7d6e3-110">Manage your organization</span></span>

<span data-ttu-id="7d6e3-111">組織内に新しいユーザーを作成したり、既存のユーザーのリソースやリレーションシップを更新したりします。</span><span class="sxs-lookup"><span data-stu-id="7d6e3-111">Create new users in your organization or update the resources and relationships for existing users.</span></span> <span data-ttu-id="7d6e3-112">Microsoft Graph を使用して、次のユーザー管理タスクを実行できます。</span><span class="sxs-lookup"><span data-stu-id="7d6e3-112">You can use Microsoft Graph to perform the following user management tasks:</span></span> 

- <span data-ttu-id="7d6e3-113">作成または Azure AD 組織内のユーザーを作成または削除する。</span><span class="sxs-lookup"><span data-stu-id="7d6e3-113">Create or delete users in your Azure AD organization.</span></span>
- <span data-ttu-id="7d6e3-114">ユーザーのグループ メンバーシップを一覧表示し、ユーザーがグループのメンバーであるかどうかを確認する。</span><span class="sxs-lookup"><span data-stu-id="7d6e3-114">List a user's group memberships and determine whether a user is a member of a group.</span></span>
- <span data-ttu-id="7d6e3-115">ユーザーへの報告やユーザーへの管理者の割り当てを行うユーザーを一覧表示する。</span><span class="sxs-lookup"><span data-stu-id="7d6e3-115">List the users who report to a user and assign managers to a user.</span></span>
- <span data-ttu-id="7d6e3-116">ユーザーの写真をアップロードまたは取得する。</span><span class="sxs-lookup"><span data-stu-id="7d6e3-116">Upload or retrieve a photo for the user.</span></span>

### <a name="work-with-calendars-and-tasks"></a><span data-ttu-id="7d6e3-117">予定表とタスクの操作</span><span class="sxs-lookup"><span data-stu-id="7d6e3-117">Work with calendars and tasks</span></span>

<span data-ttu-id="7d6e3-118">ユーザーの予定表やユーザーに関連付けられている予定表グループを表示、照会、更新できます。次のような操作が含まれます。</span><span class="sxs-lookup"><span data-stu-id="7d6e3-118">You can view, query, and update user calendar and calendar groups associated with a user, including:</span></span>

- <span data-ttu-id="7d6e3-119">ユーザーの予定表でイベントを一覧表示し、作成する。</span><span class="sxs-lookup"><span data-stu-id="7d6e3-119">List and create events on a users calendar.</span></span>
- <span data-ttu-id="7d6e3-120">ユーザーに割り当てられたタスクを表示する。</span><span class="sxs-lookup"><span data-stu-id="7d6e3-120">View tasks assigned to a user.</span></span>
- <span data-ttu-id="7d6e3-121">一連のユーザーのために空いている会議時間を検索する。</span><span class="sxs-lookup"><span data-stu-id="7d6e3-121">Find free meeting times for a set of users.</span></span>
- <span data-ttu-id="7d6e3-122">ユーザーの予定表に設定されたリマインダーの一覧を取得する。</span><span class="sxs-lookup"><span data-stu-id="7d6e3-122">Get a list of reminders set on a user's calendar.</span></span>

### <a name="administer-mail-and-handle-contacts"></a><span data-ttu-id="7d6e3-123">メールの管理と連絡先の処理</span><span class="sxs-lookup"><span data-stu-id="7d6e3-123">Administer mail and handle contacts</span></span>

<span data-ttu-id="7d6e3-124">ユーザーのメール設定と連絡先リストを構成し、ユーザーの代わりにメールを送信できます。次のような操作が含まれます。</span><span class="sxs-lookup"><span data-stu-id="7d6e3-124">You can configure user mail settings and contact lists and send mail on a user's behalf, including:</span></span>

- <span data-ttu-id="7d6e3-125">メール メッセージを一覧表示し、新しいメールを送信する。</span><span class="sxs-lookup"><span data-stu-id="7d6e3-125">List mail messages and send new mail.</span></span>
- <span data-ttu-id="7d6e3-126">ユーザーの連絡先を作成および一覧表示し、連絡先をフォルダーに整理する。</span><span class="sxs-lookup"><span data-stu-id="7d6e3-126">Create and list user contacts and organize contacts in folders.</span></span>
- <span data-ttu-id="7d6e3-127">メールボックスのフォルダーと設定を取得し、更新する。</span><span class="sxs-lookup"><span data-stu-id="7d6e3-127">Retrieve and update mailbox folders and settings.</span></span>

### <a name="enrich-your-app-with-user-insights"></a><span data-ttu-id="7d6e3-128">ユーザーのインサイトを使用したアプリの強化</span><span class="sxs-lookup"><span data-stu-id="7d6e3-128">Enrich your app with user insights</span></span>

<span data-ttu-id="7d6e3-129">ユーザーに関連するドキュメントや連絡先のうち、最近使用したものや人気上昇中のものを奨励することで、アプリケーションの関連性を最大化します。</span><span class="sxs-lookup"><span data-stu-id="7d6e3-129">Maximize relevance in your application by promoting recently used or trending documents and contacts associated with a user.</span></span> <span data-ttu-id="7d6e3-130">Microsoft Graph を使用して次のことができます。</span><span class="sxs-lookup"><span data-stu-id="7d6e3-130">You can use Microsoft Graph to:</span></span>

- <span data-ttu-id="7d6e3-131">ユーザーが最近表示および変更したドキュメントを返す。</span><span class="sxs-lookup"><span data-stu-id="7d6e3-131">Return documents recently viewed and modified by a user.</span></span>
- <span data-ttu-id="7d6e3-132">ユーザーのアクティビティで人気上昇中のドキュメントやサイトを返す。</span><span class="sxs-lookup"><span data-stu-id="7d6e3-132">Return documents and sites trending around a user's activity.</span></span>
- <span data-ttu-id="7d6e3-133">ユーザーがメールや OneDrive for Business で共有しているドキュメントを一覧表示する。</span><span class="sxs-lookup"><span data-stu-id="7d6e3-133">List documents shared with a user through email or OneDrive for Business.</span></span>

## <a name="next-steps"></a><span data-ttu-id="7d6e3-134">次の手順</span><span class="sxs-lookup"><span data-stu-id="7d6e3-134">Next steps</span></span>

- <span data-ttu-id="7d6e3-135">[ユーザーの操作](../api-reference/v1.0/resources/users.md)方法の詳細を確認する</span><span class="sxs-lookup"><span data-stu-id="7d6e3-135">Learn more about how to [work with users](../api-reference/v1.0/resources/users.md).</span></span>
- <span data-ttu-id="7d6e3-136">[Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)の **user** リソースを使用して自分自身のデータを調べる</span><span class="sxs-lookup"><span data-stu-id="7d6e3-136">Explore your own data from the **user** resource in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="7d6e3-137">[ユーザーの代わりに](auth_v2_user.md)、または[管理者の同意を得てデーモンまたはサービスとして](auth_v2_service.md) Microsoft Graph を使用して認証します。</span><span class="sxs-lookup"><span data-stu-id="7d6e3-137">Authenticate with Microsoft Graph [on behalf of a user](auth_v2_user.md) or [as a daemon or service by consent of an administator](auth_v2_service.md).</span></span>
- <span data-ttu-id="7d6e3-138">[Azure AD API](../api-reference/v1.0/resources/azure_ad_overview.md) を使用してユーザーのアクセス制御とポリシーを設定する</span><span class="sxs-lookup"><span data-stu-id="7d6e3-138">Set access control and policies for users with the [Azure AD API](../api-reference/v1.0/resources/azure_ad_overview.md).</span></span>
- <span data-ttu-id="7d6e3-139">アプリからユーザー データにアクセスするために必要な[権限](permissions_reference.md)を確認する</span><span class="sxs-lookup"><span data-stu-id="7d6e3-139">Review the [permissions](permissions_reference.md) your app will need to access user data.</span></span> 
<!-- This isn't really a next step; let's remove to keep the list of links concise.>
- Stay up to date with Microsoft Graph [changelog](https://developer.microsoft.com/graph/docs/concepts/changelog).
-->
