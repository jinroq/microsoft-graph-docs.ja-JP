---
title: OneNote REST API を使用する
description: 'Graph では、個人または組織のアカウントのユーザーの OneNote ノートブック、セクション、およびページへのアクセスの認証を取得するアプリを使用できます。 適切な委任またはアプリケーションのアクセス許可をアプリがサインインしているユーザーや、テナント内のユーザーの OneNote のデータにアクセスできます。 '
localization_priority: Normal
ms.openlocfilehash: 25817280fff570f0d87722fc8f3fadc9cf1c24d9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815238"
---
# <a name="use-the-onenote-rest-api"></a><span data-ttu-id="c9a9b-104">OneNote REST API を使用する</span><span class="sxs-lookup"><span data-stu-id="c9a9b-104">Use the OneNote REST API</span></span>

> <span data-ttu-id="c9a9b-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c9a9b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9a9b-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c9a9b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c9a9b-107">Graph では、個人または組織のアカウントのユーザーの OneNote ノートブック、セクション、およびページへのアクセスの認証を取得するアプリを使用できます。</span><span class="sxs-lookup"><span data-stu-id="c9a9b-107">Microsoft Graph lets your app get authorized access to a user's OneNote notebooks, sections, and pages in a personal or organization account.</span></span> <span data-ttu-id="c9a9b-108">アプリは、[委任、またはアプリケーションの適切なアクセス許可](/graph/permissions-reference#notes-permissions)では、サインイン中のユーザーや、テナント内のユーザーの OneNote のデータにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="c9a9b-108">With the [appropriate delegated or application permissions](/graph/permissions-reference#notes-permissions), your app can access the OneNote data of the signed-in user or any user in a tenant.</span></span> 

## <a name="root-url"></a><span data-ttu-id="c9a9b-109">ルート URL</span><span class="sxs-lookup"><span data-stu-id="c9a9b-109">Root URL</span></span>
<span data-ttu-id="c9a9b-110">OneNote サービスのルート URL は、OneNote API へのすべての呼び出しで次の形式を使用します。</span><span class="sxs-lookup"><span data-stu-id="c9a9b-110">The OneNote service root URL uses the following format for all calls to the OneNote API.</span></span>
```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="c9a9b-111">`version` 、URL 内のセグメントが使用する Microsoft Graph のバージョンを表します。</span><span class="sxs-lookup"><span data-stu-id="c9a9b-111">The `version` segment in the URL represents the version of Microsoft Graph that you want to use:</span></span>

- <span data-ttu-id="c9a9b-112">安定した運用コードには `v1.0` を使用します。</span><span class="sxs-lookup"><span data-stu-id="c9a9b-112">`v1.0` is for stable production code.</span></span>
- <span data-ttu-id="c9a9b-113">開発中の機能を試すには `beta` を使用します。</span><span class="sxs-lookup"><span data-stu-id="c9a9b-113">`beta` is to try out a feature that's in development.</span></span> <span data-ttu-id="c9a9b-114">ベータの終了点で機能が変わることがあります。実行コードで使用することはお勧めしません。</span><span class="sxs-lookup"><span data-stu-id="c9a9b-114">Features and functionality in the beta endpoint might change; we don't recommend that you use it in your production code.</span></span>

<span data-ttu-id="c9a9b-115">場所には、Office 365 またはコンシューマー OneDrive 上のユーザーのノートブック、ノートブックのグループ、または Office 365 で SharePoint サイトでホストされているチームのノートブックを指定できます。</span><span class="sxs-lookup"><span data-stu-id="c9a9b-115">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span> 

![OneNote の API の開発履歴](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

### <a name="user-notebooks"></a><span data-ttu-id="c9a9b-117">ユーザーのノートブック</span><span class="sxs-lookup"><span data-stu-id="c9a9b-117">User notebooks</span></span>
<span data-ttu-id="c9a9b-118">OneDrive または OneDrive ビジネスの消費者の個人のノートブックにアクセスするには、次の Url のいずれかを使用します。</span><span class="sxs-lookup"><span data-stu-id="c9a9b-118">To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- <span data-ttu-id="c9a9b-119">現在のユーザーがアクセスできる OneNote コンテンツには `me` を使用します (所有と共有)。</span><span class="sxs-lookup"><span data-stu-id="c9a9b-119">`me` is for OneNote content that the current user can access (owned and shared).</span></span>
- <span data-ttu-id="c9a9b-120">指定されたユーザー (URL 内) が現在のユーザーと共有している OneNote コンテンツには `users/{id}` を使用します。</span><span class="sxs-lookup"><span data-stu-id="c9a9b-120">`users/{id}` is for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="c9a9b-121">[ユーザー](users.md) API を使用します。</span><span class="sxs-lookup"><span data-stu-id="c9a9b-121">Use the [users](users.md) API.</span></span>
> <span data-ttu-id="c9a9b-122">**注:** GET 要求を行うと、ユーザー Id を取得することができます`https://graph.microsoft.com/v1.0/users`。</span><span class="sxs-lookup"><span data-stu-id="c9a9b-122">**Note:** You can get user IDs by making a GET request on `https://graph.microsoft.com/v1.0/users`.</span></span>

### <a name="group-notebooks"></a><span data-ttu-id="c9a9b-123">グループ ノートブック</span><span class="sxs-lookup"><span data-stu-id="c9a9b-123">Group notebooks</span></span>

<span data-ttu-id="c9a9b-124">グループによって所有されているノートブックにアクセスするには、次のサービスのルート URL を使用します。</span><span class="sxs-lookup"><span data-stu-id="c9a9b-124">To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
### <a name="sharepoint-site-notebooks"></a><span data-ttu-id="c9a9b-125">SharePoint サイトのノートブック</span><span class="sxs-lookup"><span data-stu-id="c9a9b-125">SharePoint site notebooks</span></span>
<span data-ttu-id="c9a9b-126">SharePoint チーム サイトによって所有されているノートブックにアクセスするには、次のサービスのルート URL を使用します。</span><span class="sxs-lookup"><span data-stu-id="c9a9b-126">To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
