---
title: Microsoft Graph でのユーザーとの作業
description: Microsoft Graph を使用し、ユーザー達、他のユーザーやグループとの関係、彼らのメール、予定表、およびファイルに基づいて、魅力的なアプリケーション体験を構築することができます。
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b98bdd3f84171823942b3a48dd49a8993597a5ee
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572179"
---
# <a name="working-with-users-in-microsoft-graph"></a><span data-ttu-id="8b887-103">Microsoft Graph でのユーザーの操作</span><span class="sxs-lookup"><span data-stu-id="8b887-103">Working with users in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b887-104">Microsoft Graph を使用し、ユーザー達、他のユーザーやグループとの関係、彼らのメール、予定表、およびファイルに基づいて、魅力的なアプリケーション体験を構築することができます。</span><span class="sxs-lookup"><span data-stu-id="8b887-104">You can use Microsoft Graph to build compelling app experiences based on users, their relationships with other users and groups, and their mail, calendar, and files.</span></span>

<span data-ttu-id="8b887-105">Microsoft Graph から 2 つの方法でユーザーにアクセスすることができます。</span><span class="sxs-lookup"><span data-stu-id="8b887-105">You can access users through Microsoft Graph in two ways:</span></span>

- <span data-ttu-id="8b887-106">ユーザーの ID で、`/users/{id}`</span><span class="sxs-lookup"><span data-stu-id="8b887-106">By their ID, `/users/{id}`</span></span> 
- <span data-ttu-id="8b887-107">`/users/{signed-in user's id}` と同じである、サインインしているユーザーの `/me` エイリアス使用して</span><span class="sxs-lookup"><span data-stu-id="8b887-107">By using the `/me` alias for the signed-in user, which is the same as `/users/{signed-in user's id}`</span></span>

## <a name="authorization"></a><span data-ttu-id="8b887-108">承認</span><span class="sxs-lookup"><span data-stu-id="8b887-108">Authorization</span></span>
<span data-ttu-id="8b887-p101">ユーザー操作へのアクセスには、次のいずれかの [アクセス許可](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) が必要です。最初の 3 つのアクセス許可は、ユーザーがアプリケーションに付与できます。残りは管理者のみがアプリケーションに付与できます。</span><span class="sxs-lookup"><span data-stu-id="8b887-p101">One of the following [permissions](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) is required to access user operations. The first three permissions can be granted to an app by a user. The rest can only be granted to an app by the administrator.</span></span>

- <span data-ttu-id="8b887-112">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="8b887-112">User.ReadBasic.All</span></span>
- <span data-ttu-id="8b887-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="8b887-113">User.Read</span></span>
- <span data-ttu-id="8b887-114">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b887-114">User.ReadWrite</span></span>
- <span data-ttu-id="8b887-115">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b887-115">User.Read.All</span></span>
- <span data-ttu-id="8b887-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b887-116">User.ReadWrite.All</span></span>
- <span data-ttu-id="8b887-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b887-117">Directory.Read.All</span></span>
- <span data-ttu-id="8b887-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b887-118">Directory.ReadWrite.All</span></span>
- <span data-ttu-id="8b887-119">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8b887-119">Directory.AccessAsUser.All</span></span>

## <a name="common-properties"></a><span data-ttu-id="8b887-120">共通プロパティ</span><span class="sxs-lookup"><span data-stu-id="8b887-120">Common properties</span></span>

<span data-ttu-id="8b887-121">以下は、ユーザーまたはユーザーの一覧を取得するときに返されるプロパティの既定のセットを表します。</span><span class="sxs-lookup"><span data-stu-id="8b887-121">The following represent the default set of properties that are returned when getting a user or listing users.</span></span> <span data-ttu-id="8b887-122">これらは、利用可能なすべてのプロパティのサブセットです。</span><span class="sxs-lookup"><span data-stu-id="8b887-122">These are a subset of all available properties.</span></span> <span data-ttu-id="8b887-123">より多くのユーザー プロパティを取得するには、`$select` クエリ パラメーターを使用します。</span><span class="sxs-lookup"><span data-stu-id="8b887-123">To get more user properties, use the `$select` query parameter.</span></span> 

|<span data-ttu-id="8b887-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8b887-124">Property</span></span> |<span data-ttu-id="8b887-125">説明</span><span class="sxs-lookup"><span data-stu-id="8b887-125">Description</span></span> |
|:----------|:-------------|
|<span data-ttu-id="8b887-126">id</span><span class="sxs-lookup"><span data-stu-id="8b887-126">id</span></span> | <span data-ttu-id="8b887-127">ユーザーの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="8b887-127">The unique identifier for the user.</span></span>|
|<span data-ttu-id="8b887-128">businessPhones</span><span class="sxs-lookup"><span data-stu-id="8b887-128">businessPhones</span></span> | <span data-ttu-id="8b887-129">ユーザーの電話番号。</span><span class="sxs-lookup"><span data-stu-id="8b887-129">The user's phone numbers.</span></span>|
|<span data-ttu-id="8b887-130">displayName</span><span class="sxs-lookup"><span data-stu-id="8b887-130">displayName</span></span> | <span data-ttu-id="8b887-131">アドレス帳に表示されるユーザーの名前。</span><span class="sxs-lookup"><span data-stu-id="8b887-131">The name displayed in the address book for the user.</span></span>|
|<span data-ttu-id="8b887-132">givenName</span><span class="sxs-lookup"><span data-stu-id="8b887-132">givenName</span></span>| <span data-ttu-id="8b887-133">ユーザーの名。</span><span class="sxs-lookup"><span data-stu-id="8b887-133">The first name of the user.</span></span> |
|<span data-ttu-id="8b887-134">jobTitle</span><span class="sxs-lookup"><span data-stu-id="8b887-134">jobTitle</span></span> | <span data-ttu-id="8b887-135">ユーザーの役職。</span><span class="sxs-lookup"><span data-stu-id="8b887-135">The user's job title.</span></span>|
|<span data-ttu-id="8b887-136">mail</span><span class="sxs-lookup"><span data-stu-id="8b887-136">mail</span></span>| <span data-ttu-id="8b887-137">ユーザーの電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="8b887-137">The user's email address.</span></span> |
|<span data-ttu-id="8b887-138">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="8b887-138">mobilePhone</span></span> | <span data-ttu-id="8b887-139">ユーザーの携帯電話番号。</span><span class="sxs-lookup"><span data-stu-id="8b887-139">The user's cellphone number.</span></span>|
|<span data-ttu-id="8b887-140">officeLocation</span><span class="sxs-lookup"><span data-stu-id="8b887-140">officeLocation</span></span> | <span data-ttu-id="8b887-141">ユーザーの物理的なオフィスの場所。</span><span class="sxs-lookup"><span data-stu-id="8b887-141">The user's physical office location.</span></span>|
|<span data-ttu-id="8b887-142">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="8b887-142">preferredLanguage</span></span> | <span data-ttu-id="8b887-143">ユーザーの選択言語。</span><span class="sxs-lookup"><span data-stu-id="8b887-143">The user's language of preference.</span></span>|
|<span data-ttu-id="8b887-144">surname</span><span class="sxs-lookup"><span data-stu-id="8b887-144">surname</span></span>| <span data-ttu-id="8b887-145">ユーザーの姓。</span><span class="sxs-lookup"><span data-stu-id="8b887-145">The last name of the user.</span></span> |
|<span data-ttu-id="8b887-146">mail</span><span class="sxs-lookup"><span data-stu-id="8b887-146">mail</span></span>| <span data-ttu-id="8b887-147">ユーザーの電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="8b887-147">The user's email address.</span></span> |
|<span data-ttu-id="8b887-148">photo</span><span class="sxs-lookup"><span data-stu-id="8b887-148">photo</span></span>| <span data-ttu-id="8b887-149">ユーザーのプロフィール写真。</span><span class="sxs-lookup"><span data-stu-id="8b887-149">The user's profile photo. Read-only.</span></span> |
|<span data-ttu-id="8b887-150">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8b887-150">userPrincipalName</span></span>| <span data-ttu-id="8b887-151">ユーザーのプリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="8b887-151">The user's principal name.</span></span> |

<span data-ttu-id="8b887-152">詳細と全プロパティの一覧は、[ユーザー](user.md) オブジェクトを参照してください。</span><span class="sxs-lookup"><span data-stu-id="8b887-152">For details and a list of all the properties, see the [user](user.md) object.</span></span>

## <a name="common-operations"></a><span data-ttu-id="8b887-153">共通の操作</span><span class="sxs-lookup"><span data-stu-id="8b887-153">Common operations</span></span>
><span data-ttu-id="8b887-154">**注:** これらの操作のいくつかは、追加のアクセス許可を必要とします。</span><span class="sxs-lookup"><span data-stu-id="8b887-154">**Note:** Some of these operations require additional permissions.</span></span>

| <span data-ttu-id="8b887-155">パス</span><span class="sxs-lookup"><span data-stu-id="8b887-155">Path</span></span>    | <span data-ttu-id="8b887-156">説明</span><span class="sxs-lookup"><span data-stu-id="8b887-156">Description</span></span> |
|:---------|:-------------|
|[`/users`](../api/user-list.md) | <span data-ttu-id="8b887-157">組織内のユーザーを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="8b887-157">Lists users in the organization.</span></span> |
|[`/users/{id}`](../api/user-get.md) | <span data-ttu-id="8b887-158">Id で特定のユーザーを取得します。</span><span class="sxs-lookup"><span data-stu-id="8b887-158">Gets a specific user by id.</span></span> |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| <span data-ttu-id="8b887-159">ユーザーのプロフィール写真を取得します。</span><span class="sxs-lookup"><span data-stu-id="8b887-159">Gets the user's profile photo.</span></span> |
|[`/users/{id}/manager`](../api/user-list-manager.md) | <span data-ttu-id="8b887-160">ユーザーの上司を取得します。</span><span class="sxs-lookup"><span data-stu-id="8b887-160">Gets the user's manager.</span></span> |
|[`/users/{id}/messages`](../api/user-list-messages.md)| <span data-ttu-id="8b887-161">プライマリ受信トレイ内のユーザーの電子メール メッセージを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="8b887-161">Lists the user's email messages in their primary inbox.</span></span> |
|[`/users/{id}/events`](../api/user-list-events.md) | <span data-ttu-id="8b887-162">ユーザーの予定表の今後のイベントを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="8b887-162">Lists the user's upcoming events in their calendar.</span></span> |
|[`/users/{id}/drive`](../api/drive-get.md)| <span data-ttu-id="8b887-163">ユーザーの OneDrive ファイル ストアを取得します。</span><span class="sxs-lookup"><span data-stu-id="8b887-163">Gets the user's OneDrive file store.</span></span> |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| <span data-ttu-id="8b887-164">ユーザーがメンバーであるグループを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="8b887-164">Lists the groups that the user is a member of.</span></span> |
|[`/users/{id}/joinedTeams`](../api/user-list-joinedteams.md)| <span data-ttu-id="8b887-165">ユーザーがメンバーである Microsoft Teams を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="8b887-165">Get the Microsoft Teams that the user is a direct member of.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/users.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
