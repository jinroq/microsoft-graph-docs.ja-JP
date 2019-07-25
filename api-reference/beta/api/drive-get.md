---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ドライブを取得する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 818923b6c8f72a972d6979813e5e0365359c42d2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861641"
---
# <a name="get-drive"></a><span data-ttu-id="0c8df-102">ドライブを取得する</span><span class="sxs-lookup"><span data-stu-id="0c8df-102">Get Drive</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c8df-103">[Drive](../resources/drive.md) リソースのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="0c8df-103">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="0c8df-104">ドライブとは、OneDrive または SharePoint のドキュメント ライブラリなど、ファイル システムの最上位コンテナーです。</span><span class="sxs-lookup"><span data-stu-id="0c8df-104">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="0c8df-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0c8df-105">Permissions</span></span>

<span data-ttu-id="0c8df-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0c8df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c8df-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0c8df-108">Permission type</span></span>      | <span data-ttu-id="0c8df-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0c8df-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c8df-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0c8df-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0c8df-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c8df-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="0c8df-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0c8df-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c8df-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c8df-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="0c8df-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0c8df-114">Application</span></span> | <span data-ttu-id="0c8df-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c8df-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="0c8df-116">現在のユーザーの OneDrive を取得する</span><span class="sxs-lookup"><span data-stu-id="0c8df-116">Get current user's OneDrive</span></span>

<span data-ttu-id="0c8df-117">(委任された認証を使用する場合) `me` シングルトンから、サインイン ユーザーのドライブにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="0c8df-117">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="0c8df-118">ユーザーの OneDrive はプロビジョニングされていないものの、ユーザーが OneDrive を使用するライセンスを持っている場合、委任された認証を使用するときに、この要求によりユーザーのドライブは自動的にプロビジョニングされます。</span><span class="sxs-lookup"><span data-stu-id="0c8df-118">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="0c8df-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0c8df-119">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0c8df-120">プロトコル</span><span class="sxs-lookup"><span data-stu-id="0c8df-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read" } -->

```http
GET /me/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0c8df-121">C#</span><span class="sxs-lookup"><span data-stu-id="0c8df-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0c8df-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="0c8df-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0c8df-123">目的-C</span><span class="sxs-lookup"><span data-stu-id="0c8df-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0c8df-124">Java</span><span class="sxs-lookup"><span data-stu-id="0c8df-124">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-default-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="get-a-users-onedrive"></a><span data-ttu-id="0c8df-125">ユーザーの OneDrive を取得する</span><span class="sxs-lookup"><span data-stu-id="0c8df-125">Get a user's OneDrive</span></span>

<span data-ttu-id="0c8df-126">ユーザーの OneDrive または OneDrive for Business にアクセスするには、User リソースについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0c8df-126">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="0c8df-127">ユーザーの OneDrive はプロビジョニングされていないものの、ユーザーが OneDrive を使用するライセンスを持っている場合、委任された認証を使用するときに、この要求によりユーザーのドライブは自動的にプロビジョニングされます。</span><span class="sxs-lookup"><span data-stu-id="0c8df-127">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="0c8df-128">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0c8df-128">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0c8df-129">プロトコル</span><span class="sxs-lookup"><span data-stu-id="0c8df-129">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0c8df-130">C#</span><span class="sxs-lookup"><span data-stu-id="0c8df-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0c8df-131">Javascript</span><span class="sxs-lookup"><span data-stu-id="0c8df-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0c8df-132">目的-C</span><span class="sxs-lookup"><span data-stu-id="0c8df-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0c8df-133">Java</span><span class="sxs-lookup"><span data-stu-id="0c8df-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="0c8df-134">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="0c8df-134">Path parameters</span></span>

| <span data-ttu-id="0c8df-135">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="0c8df-135">Parameter name</span></span> | <span data-ttu-id="0c8df-136">値</span><span class="sxs-lookup"><span data-stu-id="0c8df-136">Value</span></span>  | <span data-ttu-id="0c8df-137">説明</span><span class="sxs-lookup"><span data-stu-id="0c8df-137">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="0c8df-138">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="0c8df-138">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="0c8df-139">string</span><span class="sxs-lookup"><span data-stu-id="0c8df-139">string</span></span> | <span data-ttu-id="0c8df-140">必須です。</span><span class="sxs-lookup"><span data-stu-id="0c8df-140">Required.</span></span> <span data-ttu-id="0c8df-141">OneDrive を所有するユーザー オブジェクトの識別子。</span><span class="sxs-lookup"><span data-stu-id="0c8df-141">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="0c8df-142">グループに関連付けられたドキュメント ライブラリを取得する</span><span class="sxs-lookup"><span data-stu-id="0c8df-142">Get the document library associated with a group</span></span>

<span data-ttu-id="0c8df-143">グループの既定のドキュメント ライブラリにアクセスするには、そのグループについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0c8df-143">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="0c8df-144">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0c8df-144">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0c8df-145">プロトコル</span><span class="sxs-lookup"><span data-stu-id="0c8df-145">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all" } -->

```http
GET /groups/{groupId}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0c8df-146">C#</span><span class="sxs-lookup"><span data-stu-id="0c8df-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0c8df-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="0c8df-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0c8df-148">目的-C</span><span class="sxs-lookup"><span data-stu-id="0c8df-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0c8df-149">Java</span><span class="sxs-lookup"><span data-stu-id="0c8df-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="0c8df-150">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="0c8df-150">Path parameters</span></span>

| <span data-ttu-id="0c8df-151">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="0c8df-151">Parameter name</span></span> | <span data-ttu-id="0c8df-152">値</span><span class="sxs-lookup"><span data-stu-id="0c8df-152">Value</span></span>  | <span data-ttu-id="0c8df-153">説明</span><span class="sxs-lookup"><span data-stu-id="0c8df-153">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="0c8df-154">_groupId_</span><span class="sxs-lookup"><span data-stu-id="0c8df-154">_groupId_</span></span>      | <span data-ttu-id="0c8df-155">string</span><span class="sxs-lookup"><span data-stu-id="0c8df-155">string</span></span> | <span data-ttu-id="0c8df-156">必須です。</span><span class="sxs-lookup"><span data-stu-id="0c8df-156">Required.</span></span> <span data-ttu-id="0c8df-157">ドキュメント ライブラリを所有するグループの識別子。</span><span class="sxs-lookup"><span data-stu-id="0c8df-157">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="0c8df-158">サイトのドキュメント ライブラリを取得する</span><span class="sxs-lookup"><span data-stu-id="0c8df-158">Get the document library for a site</span></span>

<span data-ttu-id="0c8df-159">[サイトの](../resources/site.md)既定のドキュメント ライブラリにアクセスするには、そのサイトについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0c8df-159">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="0c8df-160">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0c8df-160">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0c8df-161">プロトコル</span><span class="sxs-lookup"><span data-stu-id="0c8df-161">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-site-id", "scopes": "group.read.all" } -->

```http
GET /sites/{siteId}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0c8df-162">C#</span><span class="sxs-lookup"><span data-stu-id="0c8df-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-site-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0c8df-163">Javascript</span><span class="sxs-lookup"><span data-stu-id="0c8df-163">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-site-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0c8df-164">目的-C</span><span class="sxs-lookup"><span data-stu-id="0c8df-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-site-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0c8df-165">Java</span><span class="sxs-lookup"><span data-stu-id="0c8df-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-site-id-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="0c8df-166">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="0c8df-166">Path parameters</span></span>

| <span data-ttu-id="0c8df-167">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="0c8df-167">Parameter name</span></span> | <span data-ttu-id="0c8df-168">値</span><span class="sxs-lookup"><span data-stu-id="0c8df-168">Value</span></span>  | <span data-ttu-id="0c8df-169">説明</span><span class="sxs-lookup"><span data-stu-id="0c8df-169">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="0c8df-170">_siteId_</span><span class="sxs-lookup"><span data-stu-id="0c8df-170">_siteId_</span></span>       | <span data-ttu-id="0c8df-171">string</span><span class="sxs-lookup"><span data-stu-id="0c8df-171">string</span></span> | <span data-ttu-id="0c8df-172">必須。</span><span class="sxs-lookup"><span data-stu-id="0c8df-172">Required.</span></span> <span data-ttu-id="0c8df-173">ドキュメント ライブラリを含むサイトの識別子。</span><span class="sxs-lookup"><span data-stu-id="0c8df-173">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="0c8df-174">ID によりドライブを取得する</span><span class="sxs-lookup"><span data-stu-id="0c8df-174">Get a drive by ID</span></span>

<span data-ttu-id="0c8df-175">ドライブの一意の識別子を持っている場合、最上位ドライブのコレクションから直接アクセスできます。</span><span class="sxs-lookup"><span data-stu-id="0c8df-175">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="0c8df-176">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0c8df-176">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0c8df-177">プロトコル</span><span class="sxs-lookup"><span data-stu-id="0c8df-177">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{driveId}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0c8df-178">C#</span><span class="sxs-lookup"><span data-stu-id="0c8df-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0c8df-179">Javascript</span><span class="sxs-lookup"><span data-stu-id="0c8df-179">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0c8df-180">目的-C</span><span class="sxs-lookup"><span data-stu-id="0c8df-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0c8df-181">Java</span><span class="sxs-lookup"><span data-stu-id="0c8df-181">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-id-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="0c8df-182">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="0c8df-182">Path parameters</span></span>

| <span data-ttu-id="0c8df-183">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="0c8df-183">Parameter name</span></span> | <span data-ttu-id="0c8df-184">値</span><span class="sxs-lookup"><span data-stu-id="0c8df-184">Value</span></span>  | <span data-ttu-id="0c8df-185">説明</span><span class="sxs-lookup"><span data-stu-id="0c8df-185">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="0c8df-186">_driveId_</span><span class="sxs-lookup"><span data-stu-id="0c8df-186">_driveId_</span></span>      | <span data-ttu-id="0c8df-187">string</span><span class="sxs-lookup"><span data-stu-id="0c8df-187">string</span></span> | <span data-ttu-id="0c8df-p105">必須。 要求されるドライブの識別子。</span><span class="sxs-lookup"><span data-stu-id="0c8df-p105">Required. The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="0c8df-190">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="0c8df-190">Optional query parameters</span></span>

<span data-ttu-id="0c8df-191">応答を形成するため、これらのメソッドは [$select クエリ パラメーター][odata-query-parameters]をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="0c8df-191">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="0c8df-192">応答</span><span class="sxs-lookup"><span data-stu-id="0c8df-192">Response</span></span>

<span data-ttu-id="0c8df-193">各メソッドは、一致するドライブに応じた [Drive リソース][drive-resource]を応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="0c8df-193">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

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

### <a name="error-response-codes"></a><span data-ttu-id="0c8df-194">エラー応答コード</span><span class="sxs-lookup"><span data-stu-id="0c8df-194">Error response codes</span></span>

<span data-ttu-id="0c8df-195">(委任された認証を使用する場合) ドライブが存在しないために自動的にプロビジョニングできないなら、`HTTP 404` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="0c8df-195">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

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
