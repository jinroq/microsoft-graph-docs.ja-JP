---
title: Microsoft Graph でのユーザーとの作業
description: Microsoft Graph を使用し、ユーザー達、他のユーザーやグループとの関係、彼らのメール、予定表、およびファイルに基づいて、魅力的なアプリケーション体験を構築することができます。
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bfd7778d3fdc9675880b98a356dd690c4b1eaec8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966945"
---
# <a name="working-with-users-in-microsoft-graph"></a><span data-ttu-id="2bc4c-103">Microsoft Graph でのユーザーとの作業</span><span class="sxs-lookup"><span data-stu-id="2bc4c-103">Working with users in Microsoft Graph</span></span>

<span data-ttu-id="2bc4c-104">Microsoft Graph を使用し、ユーザー達、他のユーザーやグループとの関係、彼らのメール、予定表、およびファイルに基づいて、魅力的なアプリケーション体験を構築することができます。</span><span class="sxs-lookup"><span data-stu-id="2bc4c-104">You can use Microsoft Graph to build compelling app experiences based on users, their relationships with other users and groups, and their mail, calendar, and files.</span></span>

<span data-ttu-id="2bc4c-105">Microsoft Graph を通じて、ふたつの方法で [ユーザー](user.md) にアクセスすることができます。</span><span class="sxs-lookup"><span data-stu-id="2bc4c-105">You can access [users](user.md) through Microsoft Graph in two ways:</span></span>

- <span data-ttu-id="2bc4c-106">彼らの ID で、`/users/{id | userPrincipalName}`</span><span class="sxs-lookup"><span data-stu-id="2bc4c-106">By their ID, `/users/{id | userPrincipalName}`</span></span> 
- <span data-ttu-id="2bc4c-107">`/users/{signed-in user's id}` と同じである、サインインしているユーザーの `/me` エイリアス使用して</span><span class="sxs-lookup"><span data-stu-id="2bc4c-107">By using the `/me` alias for the signed-in user, which is the same as `/users/{signed-in user's id}`</span></span>

## <a name="authorization"></a><span data-ttu-id="2bc4c-108">承認</span><span class="sxs-lookup"><span data-stu-id="2bc4c-108">Authorization</span></span>

<span data-ttu-id="2bc4c-p101">ユーザー操作へのアクセスには、次のいずれかの [アクセス許可](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) が必要です。最初の 3 つのアクセス許可は、ユーザーがアプリケーションに付与できます。残りは管理者のみがアプリケーションに付与できます。</span><span class="sxs-lookup"><span data-stu-id="2bc4c-p101">One of the following [permissions](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) is required to access user operations. The first three permissions can be granted to an app by a user. The rest can only be granted to an app by the administrator.</span></span>

- <span data-ttu-id="2bc4c-112">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="2bc4c-112">User.ReadBasic.All</span></span>
- <span data-ttu-id="2bc4c-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="2bc4c-113">User.Read</span></span>
- <span data-ttu-id="2bc4c-114">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2bc4c-114">User.ReadWrite</span></span>
- <span data-ttu-id="2bc4c-115">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2bc4c-115">User.Read.All</span></span>
- <span data-ttu-id="2bc4c-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bc4c-116">User.ReadWrite.All</span></span>
- <span data-ttu-id="2bc4c-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2bc4c-117">Directory.Read.All</span></span>
- <span data-ttu-id="2bc4c-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bc4c-118">Directory.ReadWrite.All</span></span>
- <span data-ttu-id="2bc4c-119">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2bc4c-119">Directory.AccessAsUser.All</span></span>

## <a name="common-properties"></a><span data-ttu-id="2bc4c-120">共通プロパティ</span><span class="sxs-lookup"><span data-stu-id="2bc4c-120">Common properties</span></span>

<span data-ttu-id="2bc4c-121">以下は、ユーザーまたはユーザーの一覧を取得するときに返されるプロパティの既定のセットを表します。</span><span class="sxs-lookup"><span data-stu-id="2bc4c-121">The following represent the default set of properties that are returned when getting a user or listing users.</span></span> <span data-ttu-id="2bc4c-122">これらは、利用可能なすべてのプロパティのサブセットです。</span><span class="sxs-lookup"><span data-stu-id="2bc4c-122">These are a subset of all available properties.</span></span> <span data-ttu-id="2bc4c-123">より多くのユーザー プロパティを取得するには、`$select` クエリ パラメーターを使用します。</span><span class="sxs-lookup"><span data-stu-id="2bc4c-123">To get more user properties, use the `$select` query parameter.</span></span> 

|<span data-ttu-id="2bc4c-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2bc4c-124">Property</span></span> |<span data-ttu-id="2bc4c-125">説明</span><span class="sxs-lookup"><span data-stu-id="2bc4c-125">Description</span></span> |
|:----------|:-------------|
|<span data-ttu-id="2bc4c-126">ID</span><span class="sxs-lookup"><span data-stu-id="2bc4c-126">id</span></span> | <span data-ttu-id="2bc4c-127">ユーザーの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="2bc4c-127">The unique identifier for the user.</span></span>|
|<span data-ttu-id="2bc4c-128">businessPhones</span><span class="sxs-lookup"><span data-stu-id="2bc4c-128">businessPhones</span></span> | <span data-ttu-id="2bc4c-129">ユーザーの電話番号。</span><span class="sxs-lookup"><span data-stu-id="2bc4c-129">The user's phone numbers.</span></span>|
|<span data-ttu-id="2bc4c-130">displayName</span><span class="sxs-lookup"><span data-stu-id="2bc4c-130">displayName</span></span> | <span data-ttu-id="2bc4c-131">アドレス帳に表示されるユーザーの名前。</span><span class="sxs-lookup"><span data-stu-id="2bc4c-131">The name displayed in the address book for the user.</span></span>|
|<span data-ttu-id="2bc4c-132">givenName</span><span class="sxs-lookup"><span data-stu-id="2bc4c-132">givenName</span></span>| <span data-ttu-id="2bc4c-133">ユーザーの名。</span><span class="sxs-lookup"><span data-stu-id="2bc4c-133">The first name of the user.</span></span> |
|<span data-ttu-id="2bc4c-134">jobTitle</span><span class="sxs-lookup"><span data-stu-id="2bc4c-134">jobTitle</span></span> | <span data-ttu-id="2bc4c-135">ユーザーの役職。</span><span class="sxs-lookup"><span data-stu-id="2bc4c-135">The user's job title.</span></span>|
|<span data-ttu-id="2bc4c-136">mail</span><span class="sxs-lookup"><span data-stu-id="2bc4c-136">mail</span></span>| <span data-ttu-id="2bc4c-137">ユーザーの電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="2bc4c-137">The user's email address.</span></span> |
|<span data-ttu-id="2bc4c-138">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="2bc4c-138">mobilePhone</span></span> | <span data-ttu-id="2bc4c-139">ユーザーの携帯電話番号。</span><span class="sxs-lookup"><span data-stu-id="2bc4c-139">The user's cellphone number.</span></span>|
|<span data-ttu-id="2bc4c-140">officeLocation</span><span class="sxs-lookup"><span data-stu-id="2bc4c-140">officeLocation</span></span> | <span data-ttu-id="2bc4c-141">ユーザーの物理的なオフィスの場所。</span><span class="sxs-lookup"><span data-stu-id="2bc4c-141">The user's physical office location.</span></span>|
|<span data-ttu-id="2bc4c-142">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="2bc4c-142">preferredLanguage</span></span> | <span data-ttu-id="2bc4c-143">ユーザーの選択言語。</span><span class="sxs-lookup"><span data-stu-id="2bc4c-143">The user's language of preference.</span></span>|
|<span data-ttu-id="2bc4c-144">surname</span><span class="sxs-lookup"><span data-stu-id="2bc4c-144">surname</span></span>| <span data-ttu-id="2bc4c-145">ユーザーの姓。</span><span class="sxs-lookup"><span data-stu-id="2bc4c-145">The last name of the user.</span></span> |
|<span data-ttu-id="2bc4c-146">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2bc4c-146">userPrincipalName</span></span>| <span data-ttu-id="2bc4c-147">ユーザーのプリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="2bc4c-147">The user's principal name.</span></span> |

<br/>

<span data-ttu-id="2bc4c-148">詳細と全プロパティの一覧は、[ユーザー](user.md) オブジェクトを参照してください。</span><span class="sxs-lookup"><span data-stu-id="2bc4c-148">For details and a list of all the properties, see the [user](user.md) object.</span></span>

## <a name="common-operations"></a><span data-ttu-id="2bc4c-149">共通の操作</span><span class="sxs-lookup"><span data-stu-id="2bc4c-149">Common operations</span></span>

> <span data-ttu-id="2bc4c-150">**注:** これらの操作のいくつかは、追加のアクセス許可を必要とします。</span><span class="sxs-lookup"><span data-stu-id="2bc4c-150">**Note:** Some of these operations require additional permissions.</span></span>

| <span data-ttu-id="2bc4c-151">パス</span><span class="sxs-lookup"><span data-stu-id="2bc4c-151">Path</span></span>    | <span data-ttu-id="2bc4c-152">説明</span><span class="sxs-lookup"><span data-stu-id="2bc4c-152">Description</span></span> |
|:---------|:-------------|
|[`/users`](../api/user-list.md) | <span data-ttu-id="2bc4c-153">組織内のユーザーを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="2bc4c-153">Lists users in the organization.</span></span> |
|[`/users/{id}`](../api/user-get.md) | <span data-ttu-id="2bc4c-154">Id で特定のユーザーを取得します。</span><span class="sxs-lookup"><span data-stu-id="2bc4c-154">Gets a specific user by id.</span></span> |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| <span data-ttu-id="2bc4c-155">ユーザーのプロフィール写真を取得します。</span><span class="sxs-lookup"><span data-stu-id="2bc4c-155">Gets the user's profile photo.</span></span> |
|[`/users/{id}/manager`](../api/user-list-manager.md) | <span data-ttu-id="2bc4c-156">ユーザーの上司を取得します。</span><span class="sxs-lookup"><span data-stu-id="2bc4c-156">Gets the user's manager.</span></span> |
|[`/users/{id}/messages`](../api/user-list-messages.md)| <span data-ttu-id="2bc4c-157">プライマリ受信トレイ内のユーザーの電子メール メッセージを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="2bc4c-157">Lists the user's email messages in their primary inbox.</span></span> |
|[`/users/{id}/events`](../api/user-list-events.md) | <span data-ttu-id="2bc4c-158">ユーザーの予定表の今後のイベントを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="2bc4c-158">Lists the user's upcoming events in their calendar.</span></span> |
|[`/users/{id}/drive`](../api/drive-get.md)| <span data-ttu-id="2bc4c-159">ユーザーの OneDrive ファイル ストアを取得します。</span><span class="sxs-lookup"><span data-stu-id="2bc4c-159">Gets the user's OneDrive file store.</span></span> |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| <span data-ttu-id="2bc4c-160">ユーザーがメンバーであるグループを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="2bc4c-160">Lists the groups that the user is a member of.</span></span> |
