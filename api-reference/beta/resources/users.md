---
title: Microsoft Graph でのユーザーとの作業
description: Microsoft Graph を使用し、ユーザー達、他のユーザーやグループとの関係、彼らのメール、予定表、およびファイルに基づいて、魅力的なアプリケーション体験を構築することができます。
localization_priority: Priority
ms.openlocfilehash: d9b699c008186f165a8be43ab4254213697710dc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860831"
---
# <a name="working-with-users-in-microsoft-graph"></a><span data-ttu-id="d6e5c-103">Microsoft Graph でのユーザーとの作業</span><span class="sxs-lookup"><span data-stu-id="d6e5c-103">Working with users in Microsoft Graph</span></span>

> <span data-ttu-id="d6e5c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6e5c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d6e5c-106">Microsoft Graph を使用し、ユーザー達、他のユーザーやグループとの関係、彼らのメール、予定表、およびファイルに基づいて、魅力的なアプリケーション体験を構築することができます。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-106">You can use Microsoft Graph to build compelling app experiences based on users, their relationships with other users and groups, and their mail, calendar, and files.</span></span>

<span data-ttu-id="d6e5c-107">Microsoft Graph を通じて、ふたつの方法で ユーザー にアクセスすることができます。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-107">You can access users through Microsoft Graph in two ways:</span></span>

- <span data-ttu-id="d6e5c-108">彼らの ID で、`/users/{id}`</span><span class="sxs-lookup"><span data-stu-id="d6e5c-108">By their ID, `/users/{id}`</span></span> 
- <span data-ttu-id="d6e5c-109">`/users/{signed-in user's id}` と同じである、サインインしているユーザーの `/me` エイリアス使用して</span><span class="sxs-lookup"><span data-stu-id="d6e5c-109">By using the `/me` alias for the signed-in user, which is the same as `/users/{signed-in user's id}`</span></span>

## <a name="authorization"></a><span data-ttu-id="d6e5c-110">承認</span><span class="sxs-lookup"><span data-stu-id="d6e5c-110">Authorization</span></span>
<span data-ttu-id="d6e5c-p102">ユーザー操作へのアクセスには、次のいずれかの [アクセス許可](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) が必要です。最初の 3 つのアクセス許可は、ユーザーがアプリケーションに付与できます。残りは管理者のみがアプリケーションに付与できます。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-p102">One of the following [permissions](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) is required to access user operations. The first three permissions can be granted to an app by a user. The rest can only be granted to an app by the administrator.</span></span>

- <span data-ttu-id="d6e5c-114">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="d6e5c-114">User.ReadBasic.All</span></span>
- <span data-ttu-id="d6e5c-115">User.Read</span><span class="sxs-lookup"><span data-stu-id="d6e5c-115">User.Read</span></span>
- <span data-ttu-id="d6e5c-116">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6e5c-116">User.ReadWrite</span></span>
- <span data-ttu-id="d6e5c-117">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d6e5c-117">User.Read.All</span></span>
- <span data-ttu-id="d6e5c-118">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6e5c-118">User.ReadWrite.All</span></span>
- <span data-ttu-id="d6e5c-119">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d6e5c-119">Directory.Read.All</span></span>
- <span data-ttu-id="d6e5c-120">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6e5c-120">Directory.ReadWrite.All</span></span>
- <span data-ttu-id="d6e5c-121">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d6e5c-121">Directory.AccessAsUser.All</span></span>

## <a name="common-properties"></a><span data-ttu-id="d6e5c-122">共通プロパティ</span><span class="sxs-lookup"><span data-stu-id="d6e5c-122">Common properties</span></span>

| <span data-ttu-id="d6e5c-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d6e5c-123">Property</span></span> | <span data-ttu-id="d6e5c-124">説明</span><span class="sxs-lookup"><span data-stu-id="d6e5c-124">Description</span></span> |
|----------|-------------|
| <span data-ttu-id="d6e5c-125">displayName</span><span class="sxs-lookup"><span data-stu-id="d6e5c-125">displayName</span></span> | <span data-ttu-id="d6e5c-126">アドレス帳に表示されるユーザーの名前。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-126">The name displayed in the address book for the user.</span></span>|
|<span data-ttu-id="d6e5c-127">givenName</span><span class="sxs-lookup"><span data-stu-id="d6e5c-127">givenName</span></span>| <span data-ttu-id="d6e5c-128">ユーザーの名。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-128">The first name of the user.</span></span> |
|<span data-ttu-id="d6e5c-129">surname</span><span class="sxs-lookup"><span data-stu-id="d6e5c-129">surname</span></span>| <span data-ttu-id="d6e5c-130">ユーザーの姓。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-130">The last name of the user.</span></span> |
|<span data-ttu-id="d6e5c-131">mail</span><span class="sxs-lookup"><span data-stu-id="d6e5c-131">mail</span></span>| <span data-ttu-id="d6e5c-132">ユーザーの電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-132">The user's email address.</span></span> |
|<span data-ttu-id="d6e5c-133">photo</span><span class="sxs-lookup"><span data-stu-id="d6e5c-133">photo</span></span>| <span data-ttu-id="d6e5c-134">ユーザーのプロフィールの写真です。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-134">The user's profile photo.</span></span> |

<span data-ttu-id="d6e5c-135">詳細と全プロパティの一覧は、[ユーザー](user.md) オブジェクトを参照してください。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-135">For details and a list of all the properties, see the [user](user.md) object.</span></span>

## <a name="common-operations"></a><span data-ttu-id="d6e5c-136">共通の操作</span><span class="sxs-lookup"><span data-stu-id="d6e5c-136">Common operations</span></span>
><span data-ttu-id="d6e5c-137">**注:** これらの操作のいくつかは、追加のアクセス許可を必要とします。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-137">**Note:** Some of these operations require additional permissions.</span></span>

| <span data-ttu-id="d6e5c-138">パス</span><span class="sxs-lookup"><span data-stu-id="d6e5c-138">Path</span></span>    | <span data-ttu-id="d6e5c-139">説明</span><span class="sxs-lookup"><span data-stu-id="d6e5c-139">Description</span></span> |
|---------|-------------|
|[`/users`](../api/user-list.md) | <span data-ttu-id="d6e5c-140">組織内のユーザーを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-140">Lists users in the organization.</span></span> |
|[`/users/{id}`](../api/user-get.md) | <span data-ttu-id="d6e5c-141">Id で特定のユーザーを取得します。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-141">Gets a specific user by id.</span></span> |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| <span data-ttu-id="d6e5c-142">ユーザーのプロフィール写真を取得します。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-142">Gets the user's profile photo.</span></span> |
|[`/users/{id}/manager`](../api/user-list-manager.md) | <span data-ttu-id="d6e5c-143">ユーザーの上司を取得します。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-143">Gets the user's manager.</span></span> |
|[`/users/{id}/messages`](../api/user-list-messages.md)| <span data-ttu-id="d6e5c-144">プライマリ受信トレイ内のユーザーの電子メール メッセージを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-144">Lists the user's email messages in their primary inbox.</span></span> |
|[`/users/{id}/events`](../api/user-list-events.md) | <span data-ttu-id="d6e5c-145">ユーザーの予定表の今後のイベントを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-145">Lists the user's upcoming events in their calendar.</span></span> |
|[`/users/{id}/drive`](../api/drive-get.md)| <span data-ttu-id="d6e5c-146">ユーザーの OneDrive ファイル ストアを取得します。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-146">Gets the user's OneDrive file store.</span></span> |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| <span data-ttu-id="d6e5c-147">ユーザーがメンバーであるグループを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-147">Lists the groups that the user is a member of.</span></span> |
|[`/users/{id}/joinedTeams`](../api/user-list-joinedteams.md)| <span data-ttu-id="d6e5c-148">マイクロソフトのチームのメンバーであるユーザーの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-148">Lists the Microsoft Teams that the user is a member of.</span></span> |
