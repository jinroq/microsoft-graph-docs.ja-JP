---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ドライブを取得する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 048c66f8a35477a08a2d317aae6750a0170a9714
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436607"
---
# <a name="get-drive"></a><span data-ttu-id="70230-102">ドライブを取得する</span><span class="sxs-lookup"><span data-stu-id="70230-102">Get Drive</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70230-103">[Drive](../resources/drive.md) リソースのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="70230-103">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="70230-104">ドライブとは、OneDrive または SharePoint のドキュメント ライブラリなど、ファイル システムの最上位コンテナーです。</span><span class="sxs-lookup"><span data-stu-id="70230-104">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="70230-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="70230-105">Permissions</span></span>

<span data-ttu-id="70230-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="70230-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70230-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="70230-108">Permission type</span></span>      | <span data-ttu-id="70230-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="70230-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70230-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="70230-110">Delegated (work or school account)</span></span> | <span data-ttu-id="70230-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70230-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="70230-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="70230-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70230-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70230-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="70230-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="70230-114">Application</span></span> | <span data-ttu-id="70230-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70230-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="70230-116">現在のユーザーの OneDrive を取得する</span><span class="sxs-lookup"><span data-stu-id="70230-116">Get current user's OneDrive</span></span>

<span data-ttu-id="70230-117">(委任された認証を使用する場合) `me` シングルトンから、サインイン ユーザーのドライブにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="70230-117">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="70230-118">ユーザーの OneDrive はプロビジョニングされていないものの、ユーザーが OneDrive を使用するライセンスを持っている場合、委任された認証を使用するときに、この要求によりユーザーのドライブは自動的にプロビジョニングされます。</span><span class="sxs-lookup"><span data-stu-id="70230-118">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="70230-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="70230-119">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="70230-120">プロトコル</span><span class="sxs-lookup"><span data-stu-id="70230-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read" } -->

```http
GET /me/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="70230-121">C#</span><span class="sxs-lookup"><span data-stu-id="70230-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="70230-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="70230-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="70230-123">目的-C</span><span class="sxs-lookup"><span data-stu-id="70230-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="get-a-users-onedrive"></a><span data-ttu-id="70230-124">ユーザーの OneDrive を取得する</span><span class="sxs-lookup"><span data-stu-id="70230-124">Get a user's OneDrive</span></span>

<span data-ttu-id="70230-125">ユーザーの OneDrive または OneDrive for Business にアクセスするには、User リソースについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="70230-125">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="70230-126">ユーザーの OneDrive はプロビジョニングされていないものの、ユーザーが OneDrive を使用するライセンスを持っている場合、委任された認証を使用するときに、この要求によりユーザーのドライブは自動的にプロビジョニングされます。</span><span class="sxs-lookup"><span data-stu-id="70230-126">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="70230-127">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="70230-127">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="70230-128">プロトコル</span><span class="sxs-lookup"><span data-stu-id="70230-128">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="70230-129">C#</span><span class="sxs-lookup"><span data-stu-id="70230-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="70230-130">Javascript</span><span class="sxs-lookup"><span data-stu-id="70230-130">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="70230-131">目的-C</span><span class="sxs-lookup"><span data-stu-id="70230-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="70230-132">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="70230-132">Path parameters</span></span>

| <span data-ttu-id="70230-133">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="70230-133">Parameter name</span></span> | <span data-ttu-id="70230-134">値</span><span class="sxs-lookup"><span data-stu-id="70230-134">Value</span></span>  | <span data-ttu-id="70230-135">説明</span><span class="sxs-lookup"><span data-stu-id="70230-135">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="70230-136">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="70230-136">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="70230-137">string</span><span class="sxs-lookup"><span data-stu-id="70230-137">string</span></span> | <span data-ttu-id="70230-138">必須です。</span><span class="sxs-lookup"><span data-stu-id="70230-138">Required.</span></span> <span data-ttu-id="70230-139">OneDrive を所有するユーザー オブジェクトの識別子。</span><span class="sxs-lookup"><span data-stu-id="70230-139">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="70230-140">グループに関連付けられたドキュメント ライブラリを取得する</span><span class="sxs-lookup"><span data-stu-id="70230-140">Get the document library associated with a group</span></span>

<span data-ttu-id="70230-141">グループの既定のドキュメント ライブラリにアクセスするには、そのグループについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="70230-141">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="70230-142">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="70230-142">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="70230-143">プロトコル</span><span class="sxs-lookup"><span data-stu-id="70230-143">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all" } -->

```http
GET /groups/{groupId}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="70230-144">C#</span><span class="sxs-lookup"><span data-stu-id="70230-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="70230-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="70230-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="70230-146">目的-C</span><span class="sxs-lookup"><span data-stu-id="70230-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="70230-147">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="70230-147">Path parameters</span></span>

| <span data-ttu-id="70230-148">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="70230-148">Parameter name</span></span> | <span data-ttu-id="70230-149">値</span><span class="sxs-lookup"><span data-stu-id="70230-149">Value</span></span>  | <span data-ttu-id="70230-150">説明</span><span class="sxs-lookup"><span data-stu-id="70230-150">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="70230-151">_groupId_</span><span class="sxs-lookup"><span data-stu-id="70230-151">_groupId_</span></span>      | <span data-ttu-id="70230-152">string</span><span class="sxs-lookup"><span data-stu-id="70230-152">string</span></span> | <span data-ttu-id="70230-153">必須です。</span><span class="sxs-lookup"><span data-stu-id="70230-153">Required.</span></span> <span data-ttu-id="70230-154">ドキュメント ライブラリを所有するグループの識別子。</span><span class="sxs-lookup"><span data-stu-id="70230-154">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="70230-155">サイトのドキュメント ライブラリを取得する</span><span class="sxs-lookup"><span data-stu-id="70230-155">Get the document library for a site</span></span>

<span data-ttu-id="70230-156">[サイトの](../resources/site.md)既定のドキュメント ライブラリにアクセスするには、そのサイトについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="70230-156">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="70230-157">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="70230-157">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="70230-158">プロトコル</span><span class="sxs-lookup"><span data-stu-id="70230-158">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-site-id", "scopes": "group.read.all" } -->

```http
GET /sites/{siteId}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="70230-159">C#</span><span class="sxs-lookup"><span data-stu-id="70230-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-site-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="70230-160">Javascript</span><span class="sxs-lookup"><span data-stu-id="70230-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-site-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="70230-161">目的-C</span><span class="sxs-lookup"><span data-stu-id="70230-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-site-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="70230-162">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="70230-162">Path parameters</span></span>

| <span data-ttu-id="70230-163">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="70230-163">Parameter name</span></span> | <span data-ttu-id="70230-164">値</span><span class="sxs-lookup"><span data-stu-id="70230-164">Value</span></span>  | <span data-ttu-id="70230-165">説明</span><span class="sxs-lookup"><span data-stu-id="70230-165">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="70230-166">_siteId_</span><span class="sxs-lookup"><span data-stu-id="70230-166">_siteId_</span></span>       | <span data-ttu-id="70230-167">string</span><span class="sxs-lookup"><span data-stu-id="70230-167">string</span></span> | <span data-ttu-id="70230-168">必須。</span><span class="sxs-lookup"><span data-stu-id="70230-168">Required.</span></span> <span data-ttu-id="70230-169">ドキュメント ライブラリを含むサイトの識別子。</span><span class="sxs-lookup"><span data-stu-id="70230-169">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="70230-170">ID によりドライブを取得する</span><span class="sxs-lookup"><span data-stu-id="70230-170">Get a drive by ID</span></span>

<span data-ttu-id="70230-171">ドライブの一意の識別子を持っている場合、最上位ドライブのコレクションから直接アクセスできます。</span><span class="sxs-lookup"><span data-stu-id="70230-171">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="70230-172">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="70230-172">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="70230-173">プロトコル</span><span class="sxs-lookup"><span data-stu-id="70230-173">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{driveId}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="70230-174">C#</span><span class="sxs-lookup"><span data-stu-id="70230-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="70230-175">Javascript</span><span class="sxs-lookup"><span data-stu-id="70230-175">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="70230-176">目的-C</span><span class="sxs-lookup"><span data-stu-id="70230-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="70230-177">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="70230-177">Path parameters</span></span>

| <span data-ttu-id="70230-178">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="70230-178">Parameter name</span></span> | <span data-ttu-id="70230-179">値</span><span class="sxs-lookup"><span data-stu-id="70230-179">Value</span></span>  | <span data-ttu-id="70230-180">説明</span><span class="sxs-lookup"><span data-stu-id="70230-180">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="70230-181">_driveId_</span><span class="sxs-lookup"><span data-stu-id="70230-181">_driveId_</span></span>      | <span data-ttu-id="70230-182">string</span><span class="sxs-lookup"><span data-stu-id="70230-182">string</span></span> | <span data-ttu-id="70230-p105">必須。 要求されるドライブの識別子。</span><span class="sxs-lookup"><span data-stu-id="70230-p105">Required. The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="70230-185">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="70230-185">Optional query parameters</span></span>

<span data-ttu-id="70230-186">応答を形成するため、これらのメソッドは [$select クエリ パラメーター][odata-query-parameters]をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="70230-186">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="70230-187">応答</span><span class="sxs-lookup"><span data-stu-id="70230-187">Response</span></span>

<span data-ttu-id="70230-188">各メソッドは、一致するドライブに応じた [Drive リソース][drive-resource]を応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="70230-188">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

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

### <a name="error-response-codes"></a><span data-ttu-id="70230-189">エラー応答コード</span><span class="sxs-lookup"><span data-stu-id="70230-189">Error response codes</span></span>

<span data-ttu-id="70230-190">(委任された認証を使用する場合) ドライブが存在しないために自動的にプロビジョニングできないなら、`HTTP 404` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="70230-190">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

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
