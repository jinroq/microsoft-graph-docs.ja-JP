---
author: JeremyKelley
description: Drive リソースのプロパティと関係を取得します。
ms.date: 09/10/2017
title: ドライブを取得する
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: e564303b4d4ac1ad937c10e20c55ee21205947f4
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417039"
---
# <a name="get-drive"></a><span data-ttu-id="aebb5-103">ドライブを取得する</span><span class="sxs-lookup"><span data-stu-id="aebb5-103">Get Drive</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aebb5-104">[Drive](../resources/drive.md) リソースのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="aebb5-104">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="aebb5-105">ドライブとは、OneDrive または SharePoint のドキュメント ライブラリなど、ファイル システムの最上位コンテナーです。</span><span class="sxs-lookup"><span data-stu-id="aebb5-105">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="aebb5-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="aebb5-106">Permissions</span></span>

<span data-ttu-id="aebb5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aebb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aebb5-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="aebb5-109">Permission type</span></span>      | <span data-ttu-id="aebb5-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="aebb5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aebb5-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="aebb5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="aebb5-112">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aebb5-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="aebb5-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="aebb5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aebb5-114">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aebb5-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="aebb5-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="aebb5-115">Application</span></span> | <span data-ttu-id="aebb5-116">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aebb5-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="aebb5-117">現在のユーザーの OneDrive を取得する</span><span class="sxs-lookup"><span data-stu-id="aebb5-117">Get current user's OneDrive</span></span>

<span data-ttu-id="aebb5-118">(委任された認証を使用する場合) `me` シングルトンから、サインイン ユーザーのドライブにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="aebb5-118">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="aebb5-119">ユーザーの OneDrive はプロビジョニングされていないものの、ユーザーが OneDrive を使用するライセンスを持っている場合、委任された認証を使用するときに、この要求によりユーザーのドライブは自動的にプロビジョニングされます。</span><span class="sxs-lookup"><span data-stu-id="aebb5-119">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="aebb5-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="aebb5-120">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="aebb5-121">プロトコル</span><span class="sxs-lookup"><span data-stu-id="aebb5-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read" } -->

```http
GET /me/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="aebb5-122">C#</span><span class="sxs-lookup"><span data-stu-id="aebb5-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aebb5-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aebb5-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="aebb5-124">目的-C</span><span class="sxs-lookup"><span data-stu-id="aebb5-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="get-a-users-onedrive"></a><span data-ttu-id="aebb5-125">ユーザーの OneDrive を取得する</span><span class="sxs-lookup"><span data-stu-id="aebb5-125">Get a user's OneDrive</span></span>

<span data-ttu-id="aebb5-126">ユーザーの OneDrive または OneDrive for Business にアクセスするには、User リソースについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="aebb5-126">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="aebb5-127">ユーザーの OneDrive はプロビジョニングされていないものの、ユーザーが OneDrive を使用するライセンスを持っている場合、委任された認証を使用するときに、この要求によりユーザーのドライブは自動的にプロビジョニングされます。</span><span class="sxs-lookup"><span data-stu-id="aebb5-127">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="aebb5-128">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="aebb5-128">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="aebb5-129">プロトコル</span><span class="sxs-lookup"><span data-stu-id="aebb5-129">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="aebb5-130">C#</span><span class="sxs-lookup"><span data-stu-id="aebb5-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aebb5-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aebb5-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="aebb5-132">目的-C</span><span class="sxs-lookup"><span data-stu-id="aebb5-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="aebb5-133">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="aebb5-133">Path parameters</span></span>

| <span data-ttu-id="aebb5-134">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="aebb5-134">Parameter name</span></span> | <span data-ttu-id="aebb5-135">値</span><span class="sxs-lookup"><span data-stu-id="aebb5-135">Value</span></span>  | <span data-ttu-id="aebb5-136">説明</span><span class="sxs-lookup"><span data-stu-id="aebb5-136">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="aebb5-137">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="aebb5-137">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="aebb5-138">string</span><span class="sxs-lookup"><span data-stu-id="aebb5-138">string</span></span> | <span data-ttu-id="aebb5-139">必須です。</span><span class="sxs-lookup"><span data-stu-id="aebb5-139">Required.</span></span> <span data-ttu-id="aebb5-140">OneDrive を所有するユーザー オブジェクトの識別子。</span><span class="sxs-lookup"><span data-stu-id="aebb5-140">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="aebb5-141">グループに関連付けられたドキュメント ライブラリを取得する</span><span class="sxs-lookup"><span data-stu-id="aebb5-141">Get the document library associated with a group</span></span>

<span data-ttu-id="aebb5-142">グループの既定のドキュメント ライブラリにアクセスするには、そのグループについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="aebb5-142">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="aebb5-143">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="aebb5-143">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="aebb5-144">プロトコル</span><span class="sxs-lookup"><span data-stu-id="aebb5-144">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all" } -->

```http
GET /groups/{groupId}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="aebb5-145">C#</span><span class="sxs-lookup"><span data-stu-id="aebb5-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aebb5-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aebb5-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="aebb5-147">目的-C</span><span class="sxs-lookup"><span data-stu-id="aebb5-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="aebb5-148">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="aebb5-148">Path parameters</span></span>

| <span data-ttu-id="aebb5-149">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="aebb5-149">Parameter name</span></span> | <span data-ttu-id="aebb5-150">値</span><span class="sxs-lookup"><span data-stu-id="aebb5-150">Value</span></span>  | <span data-ttu-id="aebb5-151">説明</span><span class="sxs-lookup"><span data-stu-id="aebb5-151">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="aebb5-152">_groupId_</span><span class="sxs-lookup"><span data-stu-id="aebb5-152">_groupId_</span></span>      | <span data-ttu-id="aebb5-153">string</span><span class="sxs-lookup"><span data-stu-id="aebb5-153">string</span></span> | <span data-ttu-id="aebb5-154">必須です。</span><span class="sxs-lookup"><span data-stu-id="aebb5-154">Required.</span></span> <span data-ttu-id="aebb5-155">ドキュメント ライブラリを所有するグループの識別子。</span><span class="sxs-lookup"><span data-stu-id="aebb5-155">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="aebb5-156">サイトのドキュメント ライブラリを取得する</span><span class="sxs-lookup"><span data-stu-id="aebb5-156">Get the document library for a site</span></span>

<span data-ttu-id="aebb5-157">[サイトの](../resources/site.md)既定のドキュメント ライブラリにアクセスするには、そのサイトについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="aebb5-157">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="aebb5-158">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="aebb5-158">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="aebb5-159">プロトコル</span><span class="sxs-lookup"><span data-stu-id="aebb5-159">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-site-id", "scopes": "group.read.all" } -->

```http
GET /sites/{siteId}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="aebb5-160">C#</span><span class="sxs-lookup"><span data-stu-id="aebb5-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-site-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aebb5-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aebb5-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-site-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="aebb5-162">目的-C</span><span class="sxs-lookup"><span data-stu-id="aebb5-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-site-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="aebb5-163">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="aebb5-163">Path parameters</span></span>

| <span data-ttu-id="aebb5-164">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="aebb5-164">Parameter name</span></span> | <span data-ttu-id="aebb5-165">値</span><span class="sxs-lookup"><span data-stu-id="aebb5-165">Value</span></span>  | <span data-ttu-id="aebb5-166">説明</span><span class="sxs-lookup"><span data-stu-id="aebb5-166">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="aebb5-167">_siteId_</span><span class="sxs-lookup"><span data-stu-id="aebb5-167">_siteId_</span></span>       | <span data-ttu-id="aebb5-168">string</span><span class="sxs-lookup"><span data-stu-id="aebb5-168">string</span></span> | <span data-ttu-id="aebb5-169">必須。</span><span class="sxs-lookup"><span data-stu-id="aebb5-169">Required.</span></span> <span data-ttu-id="aebb5-170">ドキュメント ライブラリを含むサイトの識別子。</span><span class="sxs-lookup"><span data-stu-id="aebb5-170">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="aebb5-171">ID によりドライブを取得する</span><span class="sxs-lookup"><span data-stu-id="aebb5-171">Get a drive by ID</span></span>

<span data-ttu-id="aebb5-172">ドライブの一意の識別子を持っている場合、最上位ドライブのコレクションから直接アクセスできます。</span><span class="sxs-lookup"><span data-stu-id="aebb5-172">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="aebb5-173">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="aebb5-173">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="aebb5-174">プロトコル</span><span class="sxs-lookup"><span data-stu-id="aebb5-174">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{driveId}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="aebb5-175">C#</span><span class="sxs-lookup"><span data-stu-id="aebb5-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aebb5-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aebb5-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="aebb5-177">目的-C</span><span class="sxs-lookup"><span data-stu-id="aebb5-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="aebb5-178">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="aebb5-178">Path parameters</span></span>

| <span data-ttu-id="aebb5-179">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="aebb5-179">Parameter name</span></span> | <span data-ttu-id="aebb5-180">値</span><span class="sxs-lookup"><span data-stu-id="aebb5-180">Value</span></span>  | <span data-ttu-id="aebb5-181">説明</span><span class="sxs-lookup"><span data-stu-id="aebb5-181">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="aebb5-182">_driveId_</span><span class="sxs-lookup"><span data-stu-id="aebb5-182">_driveId_</span></span>      | <span data-ttu-id="aebb5-183">string</span><span class="sxs-lookup"><span data-stu-id="aebb5-183">string</span></span> | <span data-ttu-id="aebb5-p105">必須。 要求されるドライブの識別子。</span><span class="sxs-lookup"><span data-stu-id="aebb5-p105">Required. The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="aebb5-186">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="aebb5-186">Optional query parameters</span></span>

<span data-ttu-id="aebb5-187">応答を形成するため、これらのメソッドは [$select クエリ パラメーター][odata-query-parameters]をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="aebb5-187">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="aebb5-188">応答</span><span class="sxs-lookup"><span data-stu-id="aebb5-188">Response</span></span>

<span data-ttu-id="aebb5-189">各メソッドは、一致するドライブに応じた [Drive リソース][drive-resource]を応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="aebb5-189">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

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

### <a name="error-response-codes"></a><span data-ttu-id="aebb5-190">エラー応答コード</span><span class="sxs-lookup"><span data-stu-id="aebb5-190">Error response codes</span></span>

<span data-ttu-id="aebb5-191">(委任された認証を使用する場合) ドライブが存在しないために自動的にプロビジョニングできないなら、`HTTP 404` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="aebb5-191">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

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
