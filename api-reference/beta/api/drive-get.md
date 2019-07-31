---
author: JeremyKelley
description: Drive リソースのプロパティと関係を取得します。
ms.date: 09/10/2017
title: ドライブを取得する
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: d4d4f548eb5deffd307bffbeb78cb42a414ff87c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35957375"
---
# <a name="get-drive"></a><span data-ttu-id="3faa0-103">ドライブを取得する</span><span class="sxs-lookup"><span data-stu-id="3faa0-103">Get Drive</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3faa0-104">[Drive](../resources/drive.md) リソースのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="3faa0-104">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="3faa0-105">ドライブとは、OneDrive または SharePoint のドキュメント ライブラリなど、ファイル システムの最上位コンテナーです。</span><span class="sxs-lookup"><span data-stu-id="3faa0-105">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="3faa0-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3faa0-106">Permissions</span></span>

<span data-ttu-id="3faa0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3faa0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3faa0-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3faa0-109">Permission type</span></span>      | <span data-ttu-id="3faa0-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3faa0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3faa0-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3faa0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3faa0-112">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3faa0-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="3faa0-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3faa0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3faa0-114">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3faa0-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="3faa0-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3faa0-115">Application</span></span> | <span data-ttu-id="3faa0-116">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3faa0-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="3faa0-117">現在のユーザーの OneDrive を取得する</span><span class="sxs-lookup"><span data-stu-id="3faa0-117">Get current user's OneDrive</span></span>

<span data-ttu-id="3faa0-118">(委任された認証を使用する場合) `me` シングルトンから、サインイン ユーザーのドライブにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="3faa0-118">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="3faa0-119">ユーザーの OneDrive はプロビジョニングされていないものの、ユーザーが OneDrive を使用するライセンスを持っている場合、委任された認証を使用するときに、この要求によりユーザーのドライブは自動的にプロビジョニングされます。</span><span class="sxs-lookup"><span data-stu-id="3faa0-119">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="3faa0-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3faa0-120">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3faa0-121">プロトコル</span><span class="sxs-lookup"><span data-stu-id="3faa0-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read" } -->

```http
GET /me/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3faa0-122">C#</span><span class="sxs-lookup"><span data-stu-id="3faa0-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3faa0-123">Javascript</span><span class="sxs-lookup"><span data-stu-id="3faa0-123">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3faa0-124">目的-C</span><span class="sxs-lookup"><span data-stu-id="3faa0-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3faa0-125">Java</span><span class="sxs-lookup"><span data-stu-id="3faa0-125">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-default-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="get-a-users-onedrive"></a><span data-ttu-id="3faa0-126">ユーザーの OneDrive を取得する</span><span class="sxs-lookup"><span data-stu-id="3faa0-126">Get a user's OneDrive</span></span>

<span data-ttu-id="3faa0-127">ユーザーの OneDrive または OneDrive for Business にアクセスするには、User リソースについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3faa0-127">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="3faa0-128">ユーザーの OneDrive はプロビジョニングされていないものの、ユーザーが OneDrive を使用するライセンスを持っている場合、委任された認証を使用するときに、この要求によりユーザーのドライブは自動的にプロビジョニングされます。</span><span class="sxs-lookup"><span data-stu-id="3faa0-128">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="3faa0-129">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3faa0-129">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3faa0-130">プロトコル</span><span class="sxs-lookup"><span data-stu-id="3faa0-130">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3faa0-131">C#</span><span class="sxs-lookup"><span data-stu-id="3faa0-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3faa0-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="3faa0-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3faa0-133">目的-C</span><span class="sxs-lookup"><span data-stu-id="3faa0-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3faa0-134">Java</span><span class="sxs-lookup"><span data-stu-id="3faa0-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="3faa0-135">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="3faa0-135">Path parameters</span></span>

| <span data-ttu-id="3faa0-136">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="3faa0-136">Parameter name</span></span> | <span data-ttu-id="3faa0-137">値</span><span class="sxs-lookup"><span data-stu-id="3faa0-137">Value</span></span>  | <span data-ttu-id="3faa0-138">説明</span><span class="sxs-lookup"><span data-stu-id="3faa0-138">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="3faa0-139">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="3faa0-139">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="3faa0-140">string</span><span class="sxs-lookup"><span data-stu-id="3faa0-140">string</span></span> | <span data-ttu-id="3faa0-141">必須です。</span><span class="sxs-lookup"><span data-stu-id="3faa0-141">Required.</span></span> <span data-ttu-id="3faa0-142">OneDrive を所有するユーザー オブジェクトの識別子。</span><span class="sxs-lookup"><span data-stu-id="3faa0-142">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="3faa0-143">グループに関連付けられたドキュメント ライブラリを取得する</span><span class="sxs-lookup"><span data-stu-id="3faa0-143">Get the document library associated with a group</span></span>

<span data-ttu-id="3faa0-144">グループの既定のドキュメント ライブラリにアクセスするには、そのグループについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3faa0-144">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="3faa0-145">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3faa0-145">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3faa0-146">プロトコル</span><span class="sxs-lookup"><span data-stu-id="3faa0-146">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all" } -->

```http
GET /groups/{groupId}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3faa0-147">C#</span><span class="sxs-lookup"><span data-stu-id="3faa0-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3faa0-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="3faa0-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3faa0-149">目的-C</span><span class="sxs-lookup"><span data-stu-id="3faa0-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3faa0-150">Java</span><span class="sxs-lookup"><span data-stu-id="3faa0-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="3faa0-151">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="3faa0-151">Path parameters</span></span>

| <span data-ttu-id="3faa0-152">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="3faa0-152">Parameter name</span></span> | <span data-ttu-id="3faa0-153">値</span><span class="sxs-lookup"><span data-stu-id="3faa0-153">Value</span></span>  | <span data-ttu-id="3faa0-154">説明</span><span class="sxs-lookup"><span data-stu-id="3faa0-154">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="3faa0-155">_groupId_</span><span class="sxs-lookup"><span data-stu-id="3faa0-155">_groupId_</span></span>      | <span data-ttu-id="3faa0-156">string</span><span class="sxs-lookup"><span data-stu-id="3faa0-156">string</span></span> | <span data-ttu-id="3faa0-157">必須です。</span><span class="sxs-lookup"><span data-stu-id="3faa0-157">Required.</span></span> <span data-ttu-id="3faa0-158">ドキュメント ライブラリを所有するグループの識別子。</span><span class="sxs-lookup"><span data-stu-id="3faa0-158">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="3faa0-159">サイトのドキュメント ライブラリを取得する</span><span class="sxs-lookup"><span data-stu-id="3faa0-159">Get the document library for a site</span></span>

<span data-ttu-id="3faa0-160">[サイトの](../resources/site.md)既定のドキュメント ライブラリにアクセスするには、そのサイトについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3faa0-160">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="3faa0-161">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3faa0-161">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3faa0-162">プロトコル</span><span class="sxs-lookup"><span data-stu-id="3faa0-162">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-site-id", "scopes": "group.read.all" } -->

```http
GET /sites/{siteId}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3faa0-163">C#</span><span class="sxs-lookup"><span data-stu-id="3faa0-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-site-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3faa0-164">Javascript</span><span class="sxs-lookup"><span data-stu-id="3faa0-164">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-site-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3faa0-165">目的-C</span><span class="sxs-lookup"><span data-stu-id="3faa0-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-site-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3faa0-166">Java</span><span class="sxs-lookup"><span data-stu-id="3faa0-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-site-id-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="3faa0-167">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="3faa0-167">Path parameters</span></span>

| <span data-ttu-id="3faa0-168">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="3faa0-168">Parameter name</span></span> | <span data-ttu-id="3faa0-169">値</span><span class="sxs-lookup"><span data-stu-id="3faa0-169">Value</span></span>  | <span data-ttu-id="3faa0-170">説明</span><span class="sxs-lookup"><span data-stu-id="3faa0-170">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="3faa0-171">_siteId_</span><span class="sxs-lookup"><span data-stu-id="3faa0-171">_siteId_</span></span>       | <span data-ttu-id="3faa0-172">string</span><span class="sxs-lookup"><span data-stu-id="3faa0-172">string</span></span> | <span data-ttu-id="3faa0-173">必須。</span><span class="sxs-lookup"><span data-stu-id="3faa0-173">Required.</span></span> <span data-ttu-id="3faa0-174">ドキュメント ライブラリを含むサイトの識別子。</span><span class="sxs-lookup"><span data-stu-id="3faa0-174">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="3faa0-175">ID によりドライブを取得する</span><span class="sxs-lookup"><span data-stu-id="3faa0-175">Get a drive by ID</span></span>

<span data-ttu-id="3faa0-176">ドライブの一意の識別子を持っている場合、最上位ドライブのコレクションから直接アクセスできます。</span><span class="sxs-lookup"><span data-stu-id="3faa0-176">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="3faa0-177">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3faa0-177">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3faa0-178">プロトコル</span><span class="sxs-lookup"><span data-stu-id="3faa0-178">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{driveId}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3faa0-179">C#</span><span class="sxs-lookup"><span data-stu-id="3faa0-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3faa0-180">Javascript</span><span class="sxs-lookup"><span data-stu-id="3faa0-180">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3faa0-181">目的-C</span><span class="sxs-lookup"><span data-stu-id="3faa0-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3faa0-182">Java</span><span class="sxs-lookup"><span data-stu-id="3faa0-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-id-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="3faa0-183">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="3faa0-183">Path parameters</span></span>

| <span data-ttu-id="3faa0-184">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="3faa0-184">Parameter name</span></span> | <span data-ttu-id="3faa0-185">値</span><span class="sxs-lookup"><span data-stu-id="3faa0-185">Value</span></span>  | <span data-ttu-id="3faa0-186">説明</span><span class="sxs-lookup"><span data-stu-id="3faa0-186">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="3faa0-187">_driveId_</span><span class="sxs-lookup"><span data-stu-id="3faa0-187">_driveId_</span></span>      | <span data-ttu-id="3faa0-188">string</span><span class="sxs-lookup"><span data-stu-id="3faa0-188">string</span></span> | <span data-ttu-id="3faa0-p105">必須。 要求されるドライブの識別子。</span><span class="sxs-lookup"><span data-stu-id="3faa0-p105">Required. The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="3faa0-191">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3faa0-191">Optional query parameters</span></span>

<span data-ttu-id="3faa0-192">応答を形成するため、これらのメソッドは [$select クエリ パラメーター][odata-query-parameters]をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="3faa0-192">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="3faa0-193">応答</span><span class="sxs-lookup"><span data-stu-id="3faa0-193">Response</span></span>

<span data-ttu-id="3faa0-194">各メソッドは、一致するドライブに応じた [Drive リソース][drive-resource]を応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="3faa0-194">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.drive", "truncated": true, "name": ["get-drive-by-id", "get-drive-by-group", "get-drive-by-user", "get-drive-default" , "get-drive-by-site-id",] } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "b!t18F8ybsHUq1z3LTz8xvZqP8zaSWjkFNhsME-Fepo75dTf9vQKfeRblBZjoSQrd7",
    "driveType": "business",
    "owner": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "Ryan Gregg"
        }
    },
    "quota": {
        "deleted": 256938,
        "remaining": 1099447353539,
        "state": "normal",
        "total": 1099511627776
    }
}
```

### <a name="error-response-codes"></a><span data-ttu-id="3faa0-195">エラー応答コード</span><span class="sxs-lookup"><span data-stu-id="3faa0-195">Error response codes</span></span>

<span data-ttu-id="3faa0-196">(委任された認証を使用する場合) ドライブが存在しないために自動的にプロビジョニングできないなら、`HTTP 404` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="3faa0-196">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

[drive-resource]: ../resources/drive.md
[odata-query-parameters]: /graph/query-parameters

<!--
{
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "tocPath": "Drives/Get drive",
  "suppressions": [
  ]
}
-->
