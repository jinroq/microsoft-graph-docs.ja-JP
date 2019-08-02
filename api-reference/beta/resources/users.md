---
title: Microsoft Graph でのユーザーとの作業
description: Microsoft Graph を使用し、ユーザー達、他のユーザーやグループとの関係、彼らのメール、予定表、およびファイルに基づいて、魅力的なアプリケーション体験を構築することができます。
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: a0a1959607e72397e24065a81b7d2362e05002ec
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007404"
---
# <a name="working-with-users-in-microsoft-graph"></a><span data-ttu-id="0db5c-103">Microsoft Graph でのユーザーの操作</span><span class="sxs-lookup"><span data-stu-id="0db5c-103">Working with users in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0db5c-104">Microsoft Graph を使用し、ユーザー達、他のユーザーやグループとの関係、彼らのメール、予定表、およびファイルに基づいて、魅力的なアプリケーション体験を構築することができます。</span><span class="sxs-lookup"><span data-stu-id="0db5c-104">You can use Microsoft Graph to build compelling app experiences based on users, their relationships with other users and groups, and their mail, calendar, and files.</span></span>

<span data-ttu-id="0db5c-105">Microsoft Graph から 2 つの方法でユーザーにアクセスすることができます。</span><span class="sxs-lookup"><span data-stu-id="0db5c-105">You can access users through Microsoft Graph in two ways:</span></span>

- <span data-ttu-id="0db5c-106">ユーザーの ID で、`/users/{id}`</span><span class="sxs-lookup"><span data-stu-id="0db5c-106">By their ID, `/users/{id}`</span></span> 
- <span data-ttu-id="0db5c-107">`/users/{signed-in user's id}` と同じである、サインインしているユーザーの `/me` エイリアス使用して</span><span class="sxs-lookup"><span data-stu-id="0db5c-107">By using the `/me` alias for the signed-in user, which is the same as `/users/{signed-in user's id}`</span></span>

## <a name="authorization"></a><span data-ttu-id="0db5c-108">承認</span><span class="sxs-lookup"><span data-stu-id="0db5c-108">Authorization</span></span>
<span data-ttu-id="0db5c-p101">ユーザー操作へのアクセスには、次のいずれかの [アクセス許可](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) が必要です。最初の 3 つのアクセス許可は、ユーザーがアプリケーションに付与できます。残りは管理者のみがアプリケーションに付与できます。</span><span class="sxs-lookup"><span data-stu-id="0db5c-p101">One of the following [permissions](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) is required to access user operations. The first three permissions can be granted to an app by a user. The rest can only be granted to an app by the administrator.</span></span>

- <span data-ttu-id="0db5c-112">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="0db5c-112">User.ReadBasic.All</span></span>
- <span data-ttu-id="0db5c-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="0db5c-113">User.Read</span></span>
- <span data-ttu-id="0db5c-114">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0db5c-114">User.ReadWrite</span></span>
- <span data-ttu-id="0db5c-115">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="0db5c-115">User.Read.All</span></span>
- <span data-ttu-id="0db5c-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0db5c-116">User.ReadWrite.All</span></span>
- <span data-ttu-id="0db5c-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0db5c-117">Directory.Read.All</span></span>
- <span data-ttu-id="0db5c-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0db5c-118">Directory.ReadWrite.All</span></span>
- <span data-ttu-id="0db5c-119">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0db5c-119">Directory.AccessAsUser.All</span></span>

## <a name="common-properties"></a><span data-ttu-id="0db5c-120">共通プロパティ</span><span class="sxs-lookup"><span data-stu-id="0db5c-120">Common properties</span></span>

| <span data-ttu-id="0db5c-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0db5c-121">Property</span></span> | <span data-ttu-id="0db5c-122">説明</span><span class="sxs-lookup"><span data-stu-id="0db5c-122">Description</span></span> |
|----------|-------------|
| <span data-ttu-id="0db5c-123">displayName</span><span class="sxs-lookup"><span data-stu-id="0db5c-123">displayName</span></span> | <span data-ttu-id="0db5c-124">アドレス帳に表示されるユーザーの名前。</span><span class="sxs-lookup"><span data-stu-id="0db5c-124">The name displayed in the address book for the user.</span></span>|
|<span data-ttu-id="0db5c-125">givenName</span><span class="sxs-lookup"><span data-stu-id="0db5c-125">givenName</span></span>| <span data-ttu-id="0db5c-126">ユーザーの名。</span><span class="sxs-lookup"><span data-stu-id="0db5c-126">The first name of the user.</span></span> |
|<span data-ttu-id="0db5c-127">surname</span><span class="sxs-lookup"><span data-stu-id="0db5c-127">surname</span></span>| <span data-ttu-id="0db5c-128">ユーザーの姓。</span><span class="sxs-lookup"><span data-stu-id="0db5c-128">The last name of the user.</span></span> |
|<span data-ttu-id="0db5c-129">mail</span><span class="sxs-lookup"><span data-stu-id="0db5c-129">mail</span></span>| <span data-ttu-id="0db5c-130">ユーザーの電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="0db5c-130">The user's email address.</span></span> |
|<span data-ttu-id="0db5c-131">photo</span><span class="sxs-lookup"><span data-stu-id="0db5c-131">photo</span></span>| <span data-ttu-id="0db5c-132">ユーザーのプロフィール写真。</span><span class="sxs-lookup"><span data-stu-id="0db5c-132">The user's profile photo.</span></span> |

<span data-ttu-id="0db5c-133">詳細と全プロパティの一覧は、[user](user.md) オブジェクトを参照してください。</span><span class="sxs-lookup"><span data-stu-id="0db5c-133">For details and a list of all the properties, see the [user](user.md) object.</span></span>

## <a name="common-operations"></a><span data-ttu-id="0db5c-134">共通の操作</span><span class="sxs-lookup"><span data-stu-id="0db5c-134">Common operations</span></span>
><span data-ttu-id="0db5c-135">**注:** これらの操作のいくつかは、追加のアクセス許可を必要とします。</span><span class="sxs-lookup"><span data-stu-id="0db5c-135">**Note:** Some of these operations require additional permissions.</span></span>

| <span data-ttu-id="0db5c-136">パス</span><span class="sxs-lookup"><span data-stu-id="0db5c-136">Path</span></span>    | <span data-ttu-id="0db5c-137">説明</span><span class="sxs-lookup"><span data-stu-id="0db5c-137">Description</span></span> |
|---------|-------------|
|[`/users`](../api/user-list.md) | <span data-ttu-id="0db5c-138">組織内のユーザーを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="0db5c-138">Lists users in the organization.</span></span> |
|[`/users/{id}`](../api/user-get.md) | <span data-ttu-id="0db5c-139">Id で特定のユーザーを取得します。</span><span class="sxs-lookup"><span data-stu-id="0db5c-139">Gets a specific user by id.</span></span> |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| <span data-ttu-id="0db5c-140">ユーザーのプロフィール写真を取得します。</span><span class="sxs-lookup"><span data-stu-id="0db5c-140">Gets the user's profile photo.</span></span> |
|[`/users/{id}/manager`](../api/user-list-manager.md) | <span data-ttu-id="0db5c-141">ユーザーの上司を取得します。</span><span class="sxs-lookup"><span data-stu-id="0db5c-141">Gets the user's manager.</span></span> |
|[`/users/{id}/messages`](../api/user-list-messages.md)| <span data-ttu-id="0db5c-142">プライマリ受信トレイ内のユーザーの電子メール メッセージを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="0db5c-142">Lists the user's email messages in their primary inbox.</span></span> |
|[`/users/{id}/events`](../api/user-list-events.md) | <span data-ttu-id="0db5c-143">ユーザーの予定表の今後のイベントを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="0db5c-143">Lists the user's upcoming events in their calendar.</span></span> |
|[`/users/{id}/drive`](../api/drive-get.md)| <span data-ttu-id="0db5c-144">ユーザーの OneDrive ファイル ストアを取得します。</span><span class="sxs-lookup"><span data-stu-id="0db5c-144">Gets the user's OneDrive file store.</span></span> |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| <span data-ttu-id="0db5c-145">ユーザーがメンバーであるグループを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="0db5c-145">Lists the groups that the user is a member of.</span></span> |
|[`/users/{id}/joinedTeams`](../api/user-list-joinedteams.md)| <span data-ttu-id="0db5c-146">ユーザーがメンバーである Microsoft Teams を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="0db5c-146">Lists the Microsoft Teams that the user is a member of.</span></span> |
