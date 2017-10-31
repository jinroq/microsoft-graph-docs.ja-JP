# <a name="working-with-users-in-microsoft-graph"></a><span data-ttu-id="694a7-101">Microsoft Graph でのユーザーとの作業</span><span class="sxs-lookup"><span data-stu-id="694a7-101">Working with users in Microsoft Graph</span></span>

<span data-ttu-id="694a7-102">Microsoft Graph を使用し、ユーザー達、他のユーザーやグループとの関係、彼らのメール、予定表、およびファイルに基づいて、魅力的なアプリケーション体験を構築することができます。</span><span class="sxs-lookup"><span data-stu-id="694a7-102">You can use Microsoft Graph to build compelling app experiences based on users, their relationships with other users and groups, and their mail, calendar, and files.</span></span>

<span data-ttu-id="694a7-103">Microsoft Graph を通じて、ふたつの方法で [ユーザー](user.md) にアクセスすることができます。</span><span class="sxs-lookup"><span data-stu-id="694a7-103">You can access [users](user.md) through Microsoft Graph in two ways:</span></span>

- <span data-ttu-id="694a7-104">彼らの ID で、`/users/{id | userPrincipalName}`</span><span class="sxs-lookup"><span data-stu-id="694a7-104">By their ID, `/users/{id | userPrincipalName}`</span></span> 
- <span data-ttu-id="694a7-105">`/users/{signed-in user's id}` と同じである、サインインしているユーザーの `/me` エイリアス使用して</span><span class="sxs-lookup"><span data-stu-id="694a7-105">By using the `/me` alias for the signed-in user, which is the same as `/users/{signed-in user's id}`</span></span>

## <a name="authorization"></a><span data-ttu-id="694a7-106">承認</span><span class="sxs-lookup"><span data-stu-id="694a7-106">Authorization</span></span>

<span data-ttu-id="694a7-107">ユーザー操作へのアクセスには、次のいずれかの[アクセス許可](https://developer.microsoft.com/en-us/graph/docs/authorization/permission_scopes)が必要です。</span><span class="sxs-lookup"><span data-stu-id="694a7-107">One of the following [permissions](https://developer.microsoft.com/en-us/graph/docs/authorization/permission_scopes) is required to access user operations.</span></span> <span data-ttu-id="694a7-108">最初の 3 つのアクセス許可は、ユーザーがアプリケーションに付与できます。</span><span class="sxs-lookup"><span data-stu-id="694a7-108">The first three permissions can be granted to an app by a user.</span></span> <span data-ttu-id="694a7-109">残りは管理者のみがアプリケーションに付与できます。</span><span class="sxs-lookup"><span data-stu-id="694a7-109">The rest can only be granted to an app by the administrator.</span></span>

- <span data-ttu-id="694a7-110">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="694a7-110">User.ReadBasic.All</span></span>
- <span data-ttu-id="694a7-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="694a7-111">User.Read</span></span>
- <span data-ttu-id="694a7-112">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="694a7-112">User.ReadWrite</span></span>
- <span data-ttu-id="694a7-113">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="694a7-113">User.Read.All</span></span>
- <span data-ttu-id="694a7-114">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="694a7-114">User.ReadWrite.All</span></span>
- <span data-ttu-id="694a7-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="694a7-115">Directory.Read.All</span></span>
- <span data-ttu-id="694a7-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="694a7-116">Directory.ReadWrite.All</span></span>
- <span data-ttu-id="694a7-117">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="694a7-117">Directory.AccessAsUser.All</span></span>

## <a name="common-properties"></a><span data-ttu-id="694a7-118">共通プロパティ</span><span class="sxs-lookup"><span data-stu-id="694a7-118">Common properties</span></span>

<span data-ttu-id="694a7-119">以下は、ユーザーまたはユーザーの一覧を取得するときに返されるプロパティの既定のセットを表します。</span><span class="sxs-lookup"><span data-stu-id="694a7-119">The following represent the default set of properties that are returned when getting a user or listing users.  These are a subset of all available properties. To get more user properties, use the  query parameter.</span></span> <span data-ttu-id="694a7-120">これらは、利用可能なすべてのプロパティのサブセットです。</span><span class="sxs-lookup"><span data-stu-id="694a7-120">These are a subset of all available properties.</span></span> <span data-ttu-id="694a7-121">より多くのユーザー プロパティを取得するには、`$select` クエリ パラメーターを使用します。</span><span class="sxs-lookup"><span data-stu-id="694a7-121">To get more user properties, use the `$select` query parameter.</span></span> 

|<span data-ttu-id="694a7-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="694a7-122">Property</span></span> |<span data-ttu-id="694a7-123">説明</span><span class="sxs-lookup"><span data-stu-id="694a7-123">Description</span></span> |
|:----------|:-------------|
|<span data-ttu-id="694a7-124">id</span><span class="sxs-lookup"><span data-stu-id="694a7-124">id</span></span> | <span data-ttu-id="694a7-125">ユーザーの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="694a7-125">The unique identifier for the user.</span></span>|
|<span data-ttu-id="694a7-126">businessPhones</span><span class="sxs-lookup"><span data-stu-id="694a7-126">businessPhones</span></span> | <span data-ttu-id="694a7-127">ユーザーの電話番号。</span><span class="sxs-lookup"><span data-stu-id="694a7-127">The user's phone numbers.</span></span>|
|<span data-ttu-id="694a7-128">displayName</span><span class="sxs-lookup"><span data-stu-id="694a7-128">displayName</span></span> | <span data-ttu-id="694a7-129">アドレス帳に表示されるユーザーの名前。</span><span class="sxs-lookup"><span data-stu-id="694a7-129">The name displayed in the address book for the user.</span></span>|
|<span data-ttu-id="694a7-130">givenName</span><span class="sxs-lookup"><span data-stu-id="694a7-130">givenName</span></span>| <span data-ttu-id="694a7-131">ユーザーの名。</span><span class="sxs-lookup"><span data-stu-id="694a7-131">The first name of the user.</span></span> |
|<span data-ttu-id="694a7-132">jobTitle</span><span class="sxs-lookup"><span data-stu-id="694a7-132">jobTitle</span></span> | <span data-ttu-id="694a7-133">ユーザーの役職。</span><span class="sxs-lookup"><span data-stu-id="694a7-133">The user's job title.</span></span>|
|<span data-ttu-id="694a7-134">mail</span><span class="sxs-lookup"><span data-stu-id="694a7-134">mail</span></span>| <span data-ttu-id="694a7-135">ユーザーの電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="694a7-135">The user's email address.</span></span> |
|<span data-ttu-id="694a7-136">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="694a7-136">mobilePhone</span></span> | <span data-ttu-id="694a7-137">ユーザーの携帯電話番号。</span><span class="sxs-lookup"><span data-stu-id="694a7-137">The user's cellphone number.</span></span>|
|<span data-ttu-id="694a7-138">officeLocation</span><span class="sxs-lookup"><span data-stu-id="694a7-138">officeLocation</span></span> | <span data-ttu-id="694a7-139">ユーザーの物理的なオフィスの場所。</span><span class="sxs-lookup"><span data-stu-id="694a7-139">The user's physical office location.</span></span>|
|<span data-ttu-id="694a7-140">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="694a7-140">preferredLanguage</span></span> | <span data-ttu-id="694a7-141">ユーザーの選択言語。</span><span class="sxs-lookup"><span data-stu-id="694a7-141">The user's language of preference.</span></span>|
|<span data-ttu-id="694a7-142">surname</span><span class="sxs-lookup"><span data-stu-id="694a7-142">surname</span></span>| <span data-ttu-id="694a7-143">ユーザーの姓。</span><span class="sxs-lookup"><span data-stu-id="694a7-143">The last name of the user.</span></span> |
|<span data-ttu-id="694a7-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="694a7-144">userPrincipalName</span></span>| <span data-ttu-id="694a7-145">ユーザーのプリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="694a7-145">The user's principal name.</span></span> |

<br/>

<span data-ttu-id="694a7-146">詳細と全プロパティの一覧は、[ユーザー](user.md) オブジェクトを参照してください。</span><span class="sxs-lookup"><span data-stu-id="694a7-146">For details and a list of all the properties, see the [user](user.md) object.</span></span>

## <a name="common-operations"></a><span data-ttu-id="694a7-147">共通の操作</span><span class="sxs-lookup"><span data-stu-id="694a7-147">Common operations</span></span>

> <span data-ttu-id="694a7-148">**注:**これらの操作のいくつかは、追加のアクセス許可を必要とします。</span><span class="sxs-lookup"><span data-stu-id="694a7-148">**Note:** Some of these operations require additional permissions.</span></span>

| <span data-ttu-id="694a7-149">パス</span><span class="sxs-lookup"><span data-stu-id="694a7-149">Path</span></span>    | <span data-ttu-id="694a7-150">説明</span><span class="sxs-lookup"><span data-stu-id="694a7-150">Description</span></span> |
|:---------|:-------------|
|[`/users`](../api/user_list.md) | <span data-ttu-id="694a7-151">組織内のユーザーを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="694a7-151">Lists users in the organization.</span></span> |
|[`/users/{id}`](../api/user_get.md) | <span data-ttu-id="694a7-152">Id で特定のユーザーを取得します。</span><span class="sxs-lookup"><span data-stu-id="694a7-152">Gets a specific user by id.</span></span> |
|[`/users/{id}/photo/$value`](../api/profilephoto_get.md)| <span data-ttu-id="694a7-153">ユーザーのプロフィール写真を取得します。</span><span class="sxs-lookup"><span data-stu-id="694a7-153">Gets the user's profile photo.</span></span> |
|[`/users/{id}/manager`](../api/user_list_manager.md) | <span data-ttu-id="694a7-154">ユーザーの上司を取得します。</span><span class="sxs-lookup"><span data-stu-id="694a7-154">Gets the user's manager.</span></span> |
|[`/users/{id}/messages`](../api/user_list_messages.md)| <span data-ttu-id="694a7-155">プライマリ受信トレイ内のユーザーの電子メール メッセージを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="694a7-155">Lists the user's email messages in their primary inbox.</span></span> |
|[`/users/{id}/events`](../api/user_list_events.md) | <span data-ttu-id="694a7-156">ユーザーの予定表の今後のイベントを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="694a7-156">Lists the user's upcoming events in their calendar.</span></span> |
|[`/users/{id}/drive`](../api/drive_get.md)| <span data-ttu-id="694a7-157">ユーザーの OneDrive ファイル ストアを取得します。</span><span class="sxs-lookup"><span data-stu-id="694a7-157">Gets the user's OneDrive file store.</span></span> |
|[`/users/{id}/memberOf`](../api/user_list_memberof.md)| <span data-ttu-id="694a7-158">ユーザーがメンバーであるグループを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="694a7-158">Lists the groups that the user is a member of.</span></span> |
