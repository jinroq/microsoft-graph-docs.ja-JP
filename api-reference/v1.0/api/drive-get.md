---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ドライブを取得する
localization_priority: Priority
ms.prod: sharepoint
description: Drive リソースのプロパティと関係を取得します。
doc_type: apiPageType
ms.openlocfilehash: 5118dedfde1126a01d445dd5a4c566ac8738902a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36365021"
---
# <a name="get-drive"></a><span data-ttu-id="f4399-103">ドライブを取得する</span><span class="sxs-lookup"><span data-stu-id="f4399-103">Get Drive</span></span>

<span data-ttu-id="f4399-104">[Drive](../resources/drive.md) リソースのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="f4399-104">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="f4399-105">ドライブとは、OneDrive または SharePoint のドキュメント ライブラリなど、ファイル システムの最上位コンテナーです。</span><span class="sxs-lookup"><span data-stu-id="f4399-105">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4399-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f4399-106">Permissions</span></span>

<span data-ttu-id="f4399-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f4399-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4399-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f4399-109">Permission type</span></span>      | <span data-ttu-id="f4399-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f4399-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4399-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f4399-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f4399-112">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4399-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f4399-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f4399-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4399-114">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4399-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="f4399-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f4399-115">Application</span></span> | <span data-ttu-id="f4399-116">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4399-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="f4399-117">現在のユーザーの OneDrive を取得する</span><span class="sxs-lookup"><span data-stu-id="f4399-117">Get current user's OneDrive</span></span>

<span data-ttu-id="f4399-118">(委任された認証を使用する場合) `me` シングルトンから、サインイン ユーザーのドライブにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="f4399-118">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="f4399-119">ユーザーの OneDrive はプロビジョニングされていないものの、ユーザーが OneDrive を使用するライセンスを持っている場合、委任された認証を使用するときに、この要求によりユーザーのドライブは自動的にプロビジョニングされます。</span><span class="sxs-lookup"><span data-stu-id="f4399-119">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="f4399-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f4399-120">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f4399-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="f4399-121">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f4399-122">C#</span><span class="sxs-lookup"><span data-stu-id="f4399-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f4399-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4399-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f4399-124">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f4399-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f4399-125">Java</span><span class="sxs-lookup"><span data-stu-id="f4399-125">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-default-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="get-a-users-onedrive"></a><span data-ttu-id="f4399-126">ユーザーの OneDrive を取得する</span><span class="sxs-lookup"><span data-stu-id="f4399-126">Get a user's OneDrive</span></span>

<span data-ttu-id="f4399-127">ユーザーの OneDrive または OneDrive for Business にアクセスするには、User リソースについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f4399-127">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="f4399-128">ユーザーの OneDrive はプロビジョニングされていないものの、ユーザーが OneDrive を使用するライセンスを持っている場合、委任された認証を使用するときに、この要求によりユーザーのドライブは自動的にプロビジョニングされます。</span><span class="sxs-lookup"><span data-stu-id="f4399-128">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="f4399-129">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f4399-129">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f4399-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="f4399-130">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all", "tags": "service.graph" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f4399-131">C#</span><span class="sxs-lookup"><span data-stu-id="f4399-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f4399-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4399-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f4399-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f4399-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f4399-134">Java</span><span class="sxs-lookup"><span data-stu-id="f4399-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="f4399-135">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="f4399-135">Path parameters</span></span>

| <span data-ttu-id="f4399-136">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="f4399-136">Parameter name</span></span> | <span data-ttu-id="f4399-137">値</span><span class="sxs-lookup"><span data-stu-id="f4399-137">Value</span></span>  | <span data-ttu-id="f4399-138">説明</span><span class="sxs-lookup"><span data-stu-id="f4399-138">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="f4399-139">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="f4399-139">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="f4399-140">string</span><span class="sxs-lookup"><span data-stu-id="f4399-140">string</span></span> | <span data-ttu-id="f4399-141">必須。</span><span class="sxs-lookup"><span data-stu-id="f4399-141">Required.</span></span> <span data-ttu-id="f4399-142">OneDrive を所有するユーザー オブジェクトの識別子。</span><span class="sxs-lookup"><span data-stu-id="f4399-142">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="f4399-143">グループに関連付けられたドキュメント ライブラリを取得する</span><span class="sxs-lookup"><span data-stu-id="f4399-143">Get the document library associated with a group</span></span>

<span data-ttu-id="f4399-144">グループの既定のドキュメント ライブラリにアクセスするには、そのグループについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f4399-144">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="f4399-145">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f4399-145">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f4399-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="f4399-146">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all", "tags": "service.graph" } -->

```http
GET /groups/{groupId}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f4399-147">C#</span><span class="sxs-lookup"><span data-stu-id="f4399-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f4399-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4399-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f4399-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f4399-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f4399-150">Java</span><span class="sxs-lookup"><span data-stu-id="f4399-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="f4399-151">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="f4399-151">Path parameters</span></span>

| <span data-ttu-id="f4399-152">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="f4399-152">Parameter name</span></span> | <span data-ttu-id="f4399-153">値</span><span class="sxs-lookup"><span data-stu-id="f4399-153">Value</span></span>  | <span data-ttu-id="f4399-154">説明</span><span class="sxs-lookup"><span data-stu-id="f4399-154">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="f4399-155">_groupId_</span><span class="sxs-lookup"><span data-stu-id="f4399-155">_groupId_</span></span>      | <span data-ttu-id="f4399-156">string</span><span class="sxs-lookup"><span data-stu-id="f4399-156">string</span></span> | <span data-ttu-id="f4399-157">必須。</span><span class="sxs-lookup"><span data-stu-id="f4399-157">Required.</span></span> <span data-ttu-id="f4399-158">ドキュメント ライブラリを所有するグループの識別子。</span><span class="sxs-lookup"><span data-stu-id="f4399-158">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="f4399-159">サイトのドキュメント ライブラリを取得する</span><span class="sxs-lookup"><span data-stu-id="f4399-159">Get the document library for a site</span></span>

<span data-ttu-id="f4399-160">[サイトの](../resources/site.md)既定のドキュメント ライブラリにアクセスするには、そのサイトについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f4399-160">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="f4399-161">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f4399-161">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f4399-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="f4399-162">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-site-id", "scopes": "group.read.all" } -->

```http
GET /sites/{siteId}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f4399-163">C#</span><span class="sxs-lookup"><span data-stu-id="f4399-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-site-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f4399-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4399-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-site-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f4399-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f4399-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-site-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f4399-166">Java</span><span class="sxs-lookup"><span data-stu-id="f4399-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-site-id-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="f4399-167">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="f4399-167">Path parameters</span></span>

| <span data-ttu-id="f4399-168">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="f4399-168">Parameter name</span></span> | <span data-ttu-id="f4399-169">値</span><span class="sxs-lookup"><span data-stu-id="f4399-169">Value</span></span>  | <span data-ttu-id="f4399-170">説明</span><span class="sxs-lookup"><span data-stu-id="f4399-170">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="f4399-171">_siteId_</span><span class="sxs-lookup"><span data-stu-id="f4399-171">_siteId_</span></span>       | <span data-ttu-id="f4399-172">string</span><span class="sxs-lookup"><span data-stu-id="f4399-172">string</span></span> | <span data-ttu-id="f4399-173">必須。</span><span class="sxs-lookup"><span data-stu-id="f4399-173">Required.</span></span> <span data-ttu-id="f4399-174">ドキュメント ライブラリを含むサイトの識別子。</span><span class="sxs-lookup"><span data-stu-id="f4399-174">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="f4399-175">ID によりドライブを取得する</span><span class="sxs-lookup"><span data-stu-id="f4399-175">Get a drive by ID</span></span>

<span data-ttu-id="f4399-176">ドライブの一意の識別子を持っている場合、最上位ドライブのコレクションから直接アクセスできます。</span><span class="sxs-lookup"><span data-stu-id="f4399-176">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="f4399-177">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f4399-177">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f4399-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="f4399-178">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f4399-179">C#</span><span class="sxs-lookup"><span data-stu-id="f4399-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f4399-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4399-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f4399-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f4399-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f4399-182">Java</span><span class="sxs-lookup"><span data-stu-id="f4399-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-id-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="f4399-183">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="f4399-183">Path parameters</span></span>

| <span data-ttu-id="f4399-184">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="f4399-184">Parameter name</span></span> | <span data-ttu-id="f4399-185">値</span><span class="sxs-lookup"><span data-stu-id="f4399-185">Value</span></span>  | <span data-ttu-id="f4399-186">説明</span><span class="sxs-lookup"><span data-stu-id="f4399-186">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="f4399-187">_driveId_</span><span class="sxs-lookup"><span data-stu-id="f4399-187">_driveId_</span></span>      | <span data-ttu-id="f4399-188">string</span><span class="sxs-lookup"><span data-stu-id="f4399-188">string</span></span> | <span data-ttu-id="f4399-p105">必須。 要求されるドライブの識別子。</span><span class="sxs-lookup"><span data-stu-id="f4399-p105">Required. The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="f4399-191">省略可能なクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f4399-191">Optional query parameters</span></span>

<span data-ttu-id="f4399-192">応答を形成するため、これらのメソッドは [$select クエリ パラメーター][odata-query-parameters]をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="f4399-192">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="f4399-193">応答</span><span class="sxs-lookup"><span data-stu-id="f4399-193">Response</span></span>

<span data-ttu-id="f4399-194">各メソッドは、一致するドライブに応じた [Drive リソース][drive-resource]を応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="f4399-194">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.drive", "truncated": true, "name": ["get-drive-by-id", "get-drive-by-group", "get-drive-by-user", "get-drive-default" , "get-drive-by-site-id"] } -->

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

### <a name="error-response-codes"></a><span data-ttu-id="f4399-195">エラー応答コード</span><span class="sxs-lookup"><span data-stu-id="f4399-195">Error response codes</span></span>

<span data-ttu-id="f4399-196">(委任された認証を使用する場合) ドライブが存在しないために自動的にプロビジョニングできないなら、`HTTP 404` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="f4399-196">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

[drive-resource]: ../resources/drive.md
[odata-query-parameters]: /graph/query-parameters

<!-- {
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "suppressions": [
      "Warning: /api-reference/v1.0/api/drive-get.md:
        Unable to map some markdown elements into schema.
            Unmapped methods:
        get-drive-default, get-drive-by-user, get-drive-by-group, get-drive-by-id
            Unmapped tables:
        Permissions - AuthScopes, Path parameters - PathParameters, Path parameters - PathParameters, Path parameters - PathParameters, Path parameters - PathParameters"
  ],
  "tocPath": "Drives/Get drive"
} -->
