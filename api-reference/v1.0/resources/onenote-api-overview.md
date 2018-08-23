# <a name="use-the-onenote-rest-api"></a><span data-ttu-id="8c95e-101">OneNote REST API を使用する</span><span class="sxs-lookup"><span data-stu-id="8c95e-101">Use the OneNote REST API</span></span>

<span data-ttu-id="8c95e-102">Microsoft Graph では、個人または組織のアカウントのユーザーの OneNote ノートブック、セクション、およびページにアプリからアクセスする権限を取得できます。</span><span class="sxs-lookup"><span data-stu-id="8c95e-102">Microsoft Graph lets your app get authorized access to a user's OneNote notebooks, sections, and pages in a personal or organization account.</span></span> <span data-ttu-id="8c95e-103">[適切な代理アクセス許可またはアプリケーション アクセス許可](../../../concepts/permissions_reference.md#notes-permissions)を使用すると、アプリはサインインしているユーザーまたはテナント内のユーザーの OneNote データにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="8c95e-103">With the [appropriate delegated or application permissions](../../../concepts/permissions_reference.md#notes-permissions), your app can access the OneNote data of the signed-in user or any user in a tenant.</span></span>

## <a name="root-url"></a><span data-ttu-id="8c95e-104">ルート URL</span><span class="sxs-lookup"><span data-stu-id="8c95e-104">Root URL</span></span>
<span data-ttu-id="8c95e-105">OneNote サービスのルート URL は、OneNote API へのすべての呼び出しで次の形式を使用します。</span><span class="sxs-lookup"><span data-stu-id="8c95e-105">The OneNote service root URL uses the following format for all calls to the OneNote API.</span></span>
```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```
<span data-ttu-id="8c95e-106">URL の `version` セグメントは、使用する Microsoft Graph のバージョンを示しています。</span><span class="sxs-lookup"><span data-stu-id="8c95e-106">The `version` segment in the URL represents the version of Microsoft Graph that you want to use.</span></span>

- <span data-ttu-id="8c95e-107">`v1.0`  は、安定した製品コード用です。</span><span class="sxs-lookup"><span data-stu-id="8c95e-107">`v1.0` is for stable production code.</span></span>
- <span data-ttu-id="8c95e-108">`beta`  は、開発中の機能を試すのに使用します。</span><span class="sxs-lookup"><span data-stu-id="8c95e-108">`beta` is to try out a feature that's in development.</span></span> <span data-ttu-id="8c95e-109">ベータのエンドポイントで機能が変わることがあります。製品コードで使用することはお勧めしません。</span><span class="sxs-lookup"><span data-stu-id="8c95e-109">Features and functionality in the beta endpoint might change; we don't recommend that you use it in your production code.</span></span>

<span data-ttu-id="8c95e-110">Office 365 またはコンシューマー OneDrive のユーザー ノートブック、Office 365 のグループ ノートブック、または SharePoint サイトでホストされているチームのノートブックを場所として指定できます。</span><span class="sxs-lookup"><span data-stu-id="8c95e-110">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks or SharePoint site-hosted team notebooks on Office 365.</span></span> 

![OneNote API の開発スタック](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

### <a name="user-notebooks"></a><span data-ttu-id="8c95e-112">ユーザーのノートブック</span><span class="sxs-lookup"><span data-stu-id="8c95e-112">User notebooks</span></span>
<span data-ttu-id="8c95e-113">コンシューマー OneDrive または OneDrive for Business の個人用ノートブックにアクセスするには、次の URL のいずれかを使用します。</span><span class="sxs-lookup"><span data-stu-id="8c95e-113">User notebooks To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- <span data-ttu-id="8c95e-114">`me` は、現在のユーザーがアクセスできる OneNote コンテンツのためのものです (所有と共有)。</span><span class="sxs-lookup"><span data-stu-id="8c95e-114">`me` is for OneNote content that the current user can access (owned and shared).</span></span>
- <span data-ttu-id="8c95e-115">`users/{id}` は、指定されたユーザー (URL 内) が現在のユーザーと共有している OneNote コンテンツのためのものです。</span><span class="sxs-lookup"><span data-stu-id="8c95e-115">`users/{id}` is for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="8c95e-116">[ユーザー](users.md) API を使用します。</span><span class="sxs-lookup"><span data-stu-id="8c95e-116">[Use the Planner API](users.md)</span></span>
> <span data-ttu-id="8c95e-117">**注:** `https://graph.microsoft.com/v1.0/users`で GET 要求を行うことにより、ユーザー ID を取得できます。</span><span class="sxs-lookup"><span data-stu-id="8c95e-117">**Note:** You can get user ids by making a GET request on `https://graph.microsoft.com/v1.0/users`.</span></span>

### <a name="group-notebooks"></a><span data-ttu-id="8c95e-118">グループ ノートブック</span><span class="sxs-lookup"><span data-stu-id="8c95e-118">Group notebooks</span></span>
<span data-ttu-id="8c95e-119">グループによって所有されているノートブックにアクセスするには、次のサービス ルート URL を使用します。</span><span class="sxs-lookup"><span data-stu-id="8c95e-119">Group notebooks To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
### <a name="sharepoint-site-notebooks"></a><span data-ttu-id="8c95e-120">SharePoint サイトのノートブック</span><span class="sxs-lookup"><span data-stu-id="8c95e-120">SharePoint site notebooks</span></span>

<span data-ttu-id="8c95e-121">SharePoint チーム サイトによって所有されているノートブックにアクセスするには、次のサービス ルート URL を使用します。</span><span class="sxs-lookup"><span data-stu-id="8c95e-121">SharePoint site notebooks To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

