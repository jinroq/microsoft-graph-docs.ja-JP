---
title: OneNote REST API を使用する
description: 'Microsoft Graph を使用すると、アプリは個人または組織のアカウントでユーザーの OneNote ノートブック、セクション、および画面に正当にアクセスできます。 適切な代理アクセス許可またはアプリケーション アクセス許可を使用すると、アプリはサインインしているユーザーまたはテナント内のユーザーの OneNote データにアクセスできます。 '
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: ceb5ac30786ecfd207a2076d471e9d004b60f8d3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462957"
---
# <a name="use-the-onenote-rest-api"></a><span data-ttu-id="4a0af-104">OneNote REST API を使用する</span><span class="sxs-lookup"><span data-stu-id="4a0af-104">Use the OneNote REST API</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a0af-105">Microsoft Graph を使用すると、アプリは個人または組織のアカウントでユーザーの OneNote ノートブック、セクション、および画面に正当にアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="4a0af-105">Microsoft Graph lets your app get authorized access to a user's Outlook mail data in a personal or organization account.</span></span> <span data-ttu-id="4a0af-106">[適切な代理アクセス許可またはアプリケーション アクセス許可を使用すると](/graph/permissions-reference#notes-permissions)、アプリはサインインしているユーザーまたはテナント内のユーザーの OneNote データにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="4a0af-106">With the [appropriate delegated or application permissions](/graph/permissions-reference#notes-permissions), your app can access the OneNote data of the signed-in user or any user in a tenant.</span></span> 

## <a name="root-url"></a><span data-ttu-id="4a0af-107">ルート URL</span><span class="sxs-lookup"><span data-stu-id="4a0af-107">Root URL</span></span>
<span data-ttu-id="4a0af-108">OneNote サービスのルート URL は、OneNote API へのすべての呼び出しで次の形式を使用します。</span><span class="sxs-lookup"><span data-stu-id="4a0af-108">The OneNote service root URL uses the following format for all calls to the OneNote API.</span></span>
```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="4a0af-109">URL の `version` セグメントは、使用する Microsoft Graph のバージョンを示しています。</span><span class="sxs-lookup"><span data-stu-id="4a0af-109">The `version` segment in the URL represents the version of Microsoft Graph that you want to use.</span></span>

- <span data-ttu-id="4a0af-110">安定した運用コードには `v1.0` を使用します。</span><span class="sxs-lookup"><span data-stu-id="4a0af-110">`v1.0` is for stable production code.</span></span>
- <span data-ttu-id="4a0af-111">開発中の機能を試すには `beta` を使用します。</span><span class="sxs-lookup"><span data-stu-id="4a0af-111">`beta` is to try out a feature that's in development.</span></span> <span data-ttu-id="4a0af-112">ベータ版のエンドポイントの特徴と機能は予告なしに変更されることがあります。運用コード内で使用することはお勧めしません。</span><span class="sxs-lookup"><span data-stu-id="4a0af-112">Features and functionality in the beta endpoint might change; we don't recommend that you use it in your production code.</span></span>

<span data-ttu-id="4a0af-113">Office 365 またはコンシューマー OneDrive のユーザー ノートブック、Office 365 のグループ ノートブック、または SharePoint サイトでホストされているチームのノートブックを場所として指定できます。</span><span class="sxs-lookup"><span data-stu-id="4a0af-113">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span> 

![OneNote API 開発スタック](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

### <a name="user-notebooks"></a><span data-ttu-id="4a0af-115">ユーザー ノートブック</span><span class="sxs-lookup"><span data-stu-id="4a0af-115">User notebooks</span></span>
<span data-ttu-id="4a0af-116">コンシューマー OneDrive または OneDrive for Business の個人用ノートブックにアクセスするには、次の URL のいずれかを使用します。</span><span class="sxs-lookup"><span data-stu-id="4a0af-116">To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- <span data-ttu-id="4a0af-117">現在のユーザーがアクセスできる OneNote コンテンツには `me` を使用します (所有と共有)。</span><span class="sxs-lookup"><span data-stu-id="4a0af-117">`me` is for OneNote content that the current user can access (owned and shared).</span></span>
- <span data-ttu-id="4a0af-118">指定されたユーザー (URL 内) が現在のユーザーと共有している OneNote コンテンツには `users/{id}` を使用します。</span><span class="sxs-lookup"><span data-stu-id="4a0af-118">`users/{id}` is for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="4a0af-119">[ユーザー](users.md) API を使用します。</span><span class="sxs-lookup"><span data-stu-id="4a0af-119">[](users.md)Use the Windows API</span></span>
> <span data-ttu-id="4a0af-120">**注:** `https://graph.microsoft.com/v1.0/users` で GET 要求を行うことにより、ユーザー ID を取得できます。</span><span class="sxs-lookup"><span data-stu-id="4a0af-120">**Note:** You can get user ids by making a GET request on `https://graph.microsoft.com/v1.0/users`.</span></span>

### <a name="group-notebooks"></a><span data-ttu-id="4a0af-121">グループ ノートブック</span><span class="sxs-lookup"><span data-stu-id="4a0af-121">Group notebooks</span></span>

<span data-ttu-id="4a0af-122">グループによって所有されているノートブックにアクセスするには、次のサービス ルート URL を使用します。</span><span class="sxs-lookup"><span data-stu-id="4a0af-122">To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
### <a name="sharepoint-site-notebooks"></a><span data-ttu-id="4a0af-123">SharePoint サイト ノートブック</span><span class="sxs-lookup"><span data-stu-id="4a0af-123">SharePoint site notebooks</span></span>
<span data-ttu-id="4a0af-124">SharePoint チーム サイトによって所有されているノートブックにアクセスするには、次のサービス ルート URL を使用します。</span><span class="sxs-lookup"><span data-stu-id="4a0af-124">To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/onenote-api-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
