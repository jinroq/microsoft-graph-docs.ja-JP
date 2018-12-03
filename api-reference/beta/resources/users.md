---
title: Microsoft Graph でのユーザーとの作業
description: Microsoft Graph を使用し、ユーザー達、他のユーザーやグループとの関係、彼らのメール、予定表、およびファイルに基づいて、魅力的なアプリケーション体験を構築することができます。
ms.openlocfilehash: ee084bb52042b0c42f0308584ec6b3989b5b6114
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070020"
---
# <a name="working-with-users-in-microsoft-graph"></a><span data-ttu-id="8ea09-103">Microsoft Graph でのユーザーとの作業</span><span class="sxs-lookup"><span data-stu-id="8ea09-103">Working with users in Microsoft Graph</span></span>

> <span data-ttu-id="8ea09-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8ea09-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8ea09-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ea09-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8ea09-106">Microsoft Graph を使用し、ユーザー達、他のユーザーやグループとの関係、彼らのメール、予定表、およびファイルに基づいて、魅力的なアプリケーション体験を構築することができます。</span><span class="sxs-lookup"><span data-stu-id="8ea09-106">You can use Microsoft Graph to build compelling app experiences based on users, their relationships with other users and groups, and their mail, calendar, and files.</span></span>

<span data-ttu-id="8ea09-107">Microsoft Graph を通じて、ふたつの方法で ユーザー にアクセスすることができます。</span><span class="sxs-lookup"><span data-stu-id="8ea09-107">You can access users through Microsoft Graph in two ways:</span></span>

- <span data-ttu-id="8ea09-108">彼らの ID で、`/users/{id}`</span><span class="sxs-lookup"><span data-stu-id="8ea09-108">By their ID, `/users/{id}`</span></span> 
- <span data-ttu-id="8ea09-109">`/users/{signed-in user's id}` と同じである、サインインしているユーザーの `/me` エイリアス使用して</span><span class="sxs-lookup"><span data-stu-id="8ea09-109">By using the `/me` alias for the signed-in user, which is the same as `/users/{signed-in user's id}`</span></span>

## <a name="authorization"></a><span data-ttu-id="8ea09-110">承認</span><span class="sxs-lookup"><span data-stu-id="8ea09-110">Authorization</span></span>
<span data-ttu-id="8ea09-p102">ユーザー操作へのアクセスには、次のいずれかの [アクセス許可](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) が必要です。最初の 3 つのアクセス許可は、ユーザーがアプリケーションに付与できます。残りは管理者のみがアプリケーションに付与できます。</span><span class="sxs-lookup"><span data-stu-id="8ea09-p102">One of the following [permissions](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) is required to access user operations. The first three permissions can be granted to an app by a user. The rest can only be granted to an app by the administrator.</span></span>

- <span data-ttu-id="8ea09-114">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="8ea09-114">User.ReadBasic.All</span></span>
- <span data-ttu-id="8ea09-115">User.Read</span><span class="sxs-lookup"><span data-stu-id="8ea09-115">User.Read</span></span>
- <span data-ttu-id="8ea09-116">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ea09-116">User.ReadWrite</span></span>
- <span data-ttu-id="8ea09-117">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8ea09-117">User.Read.All</span></span>
- <span data-ttu-id="8ea09-118">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ea09-118">User.ReadWrite.All</span></span>
- <span data-ttu-id="8ea09-119">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="8ea09-119">Directory.Read.All</span></span>
- <span data-ttu-id="8ea09-120">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ea09-120">Directory.ReadWrite.All</span></span>
- <span data-ttu-id="8ea09-121">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8ea09-121">Directory.AccessAsUser.All</span></span>

## <a name="common-properties"></a><span data-ttu-id="8ea09-122">共通プロパティ</span><span class="sxs-lookup"><span data-stu-id="8ea09-122">Common properties</span></span>

| <span data-ttu-id="8ea09-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8ea09-123">Property</span></span> | <span data-ttu-id="8ea09-124">説明</span><span class="sxs-lookup"><span data-stu-id="8ea09-124">Description</span></span> |
|----------|-------------|
| <span data-ttu-id="8ea09-125">displayName</span><span class="sxs-lookup"><span data-stu-id="8ea09-125">displayName</span></span> | <span data-ttu-id="8ea09-126">アドレス帳に表示されるユーザーの名前。</span><span class="sxs-lookup"><span data-stu-id="8ea09-126">The name displayed in the address book for the user.</span></span>|
|<span data-ttu-id="8ea09-127">givenName</span><span class="sxs-lookup"><span data-stu-id="8ea09-127">givenName</span></span>| <span data-ttu-id="8ea09-128">ユーザーの名。</span><span class="sxs-lookup"><span data-stu-id="8ea09-128">The first name of the user.</span></span> |
|<span data-ttu-id="8ea09-129">surname</span><span class="sxs-lookup"><span data-stu-id="8ea09-129">surname</span></span>| <span data-ttu-id="8ea09-130">ユーザーの姓。</span><span class="sxs-lookup"><span data-stu-id="8ea09-130">The last name of the user.</span></span> |
|<span data-ttu-id="8ea09-131">mail</span><span class="sxs-lookup"><span data-stu-id="8ea09-131">mail</span></span>| <span data-ttu-id="8ea09-132">ユーザーの電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="8ea09-132">The user's email address.</span></span> |
|<span data-ttu-id="8ea09-133">photo</span><span class="sxs-lookup"><span data-stu-id="8ea09-133">photo</span></span>| <span data-ttu-id="8ea09-134">ユーザーのプロフィールの写真です。</span><span class="sxs-lookup"><span data-stu-id="8ea09-134">The user's profile photo.</span></span> |

<span data-ttu-id="8ea09-135">詳細と全プロパティの一覧は、[ユーザー](user.md) オブジェクトを参照してください。</span><span class="sxs-lookup"><span data-stu-id="8ea09-135">For details and a list of all the properties, see the [user](user.md) object.</span></span>

## <a name="common-operations"></a><span data-ttu-id="8ea09-136">共通の操作</span><span class="sxs-lookup"><span data-stu-id="8ea09-136">Common operations</span></span>
><span data-ttu-id="8ea09-137">**注:** これらの操作のいくつかは、追加のアクセス許可を必要とします。</span><span class="sxs-lookup"><span data-stu-id="8ea09-137">**Note:** Some of these operations require additional permissions.</span></span>

| <span data-ttu-id="8ea09-138">パス</span><span class="sxs-lookup"><span data-stu-id="8ea09-138">Path</span></span>    | <span data-ttu-id="8ea09-139">説明</span><span class="sxs-lookup"><span data-stu-id="8ea09-139">Description</span></span> |
|---------|-------------|
|[`/users`](../api/user-list.md) | <span data-ttu-id="8ea09-140">組織内のユーザーを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="8ea09-140">Lists users in the organization.</span></span> |
|[`/users/{id}`](../api/user-get.md) | <span data-ttu-id="8ea09-141">Id で特定のユーザーを取得します。</span><span class="sxs-lookup"><span data-stu-id="8ea09-141">Gets a specific user by id.</span></span> |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| <span data-ttu-id="8ea09-142">ユーザーのプロフィール写真を取得します。</span><span class="sxs-lookup"><span data-stu-id="8ea09-142">Gets the user's profile photo.</span></span> |
|[`/users/{id}/manager`](../api/user-list-manager.md) | <span data-ttu-id="8ea09-143">ユーザーの上司を取得します。</span><span class="sxs-lookup"><span data-stu-id="8ea09-143">Gets the user's manager.</span></span> |
|[`/users/{id}/messages`](../api/user-list-messages.md)| <span data-ttu-id="8ea09-144">プライマリ受信トレイ内のユーザーの電子メール メッセージを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="8ea09-144">Lists the user's email messages in their primary inbox.</span></span> |
|[`/users/{id}/events`](../api/user-list-events.md) | <span data-ttu-id="8ea09-145">ユーザーの予定表の今後のイベントを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="8ea09-145">Lists the user's upcoming events in their calendar.</span></span> |
|[`/users/{id}/drive`](../api/drive-get.md)| <span data-ttu-id="8ea09-146">ユーザーの OneDrive ファイル ストアを取得します。</span><span class="sxs-lookup"><span data-stu-id="8ea09-146">Gets the user's OneDrive file store.</span></span> |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| <span data-ttu-id="8ea09-147">ユーザーがメンバーであるグループを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="8ea09-147">Lists the groups that the user is a member of.</span></span> |
|[`/users/{id}/joinedTeams`](../api/user-list-joinedteams.md)| <span data-ttu-id="8ea09-148">マイクロソフトのチームのメンバーであるユーザーの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="8ea09-148">Lists the Microsoft Teams that the user is a member of.</span></span> |
