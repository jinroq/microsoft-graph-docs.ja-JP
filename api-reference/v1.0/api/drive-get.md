---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ドライブを取得する
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 3115e9a5b3312c6d357fc5c166abc7200ef5f546
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35279353"
---
# <a name="get-drive"></a><span data-ttu-id="a5d1c-102">ドライブを取得する</span><span class="sxs-lookup"><span data-stu-id="a5d1c-102">Get Drive</span></span>

<span data-ttu-id="a5d1c-103">[Drive](../resources/drive.md) リソースのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="a5d1c-103">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="a5d1c-104">ドライブとは、OneDrive または SharePoint のドキュメント ライブラリなど、ファイル システムの最上位コンテナーです。</span><span class="sxs-lookup"><span data-stu-id="a5d1c-104">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5d1c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a5d1c-105">Permissions</span></span>

<span data-ttu-id="a5d1c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a5d1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5d1c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a5d1c-108">Permission type</span></span>      | <span data-ttu-id="a5d1c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a5d1c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5d1c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a5d1c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a5d1c-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5d1c-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a5d1c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a5d1c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5d1c-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5d1c-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="a5d1c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a5d1c-114">Application</span></span> | <span data-ttu-id="a5d1c-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5d1c-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="a5d1c-116">現在のユーザーの OneDrive を取得する</span><span class="sxs-lookup"><span data-stu-id="a5d1c-116">Get current user's OneDrive</span></span>

<span data-ttu-id="a5d1c-117">(委任された認証を使用する場合) `me` シングルトンから、サインイン ユーザーのドライブにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="a5d1c-117">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="a5d1c-118">ユーザーの OneDrive はプロビジョニングされていないものの、ユーザーが OneDrive を使用するライセンスを持っている場合、委任された認証を使用するときに、この要求によりユーザーのドライブは自動的にプロビジョニングされます。</span><span class="sxs-lookup"><span data-stu-id="a5d1c-118">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="a5d1c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a5d1c-119">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a5d1c-120">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="a5d1c-120">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a5d1c-121">C#</span><span class="sxs-lookup"><span data-stu-id="a5d1c-121">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-default-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a5d1c-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="a5d1c-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-default-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a5d1c-123">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5d1c-123">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-drive-default-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="get-a-users-onedrive"></a><span data-ttu-id="a5d1c-124">ユーザーの OneDrive を取得する</span><span class="sxs-lookup"><span data-stu-id="a5d1c-124">Get a user's OneDrive</span></span>

<span data-ttu-id="a5d1c-125">ユーザーの OneDrive または OneDrive for Business にアクセスするには、User リソースについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a5d1c-125">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="a5d1c-126">ユーザーの OneDrive はプロビジョニングされていないものの、ユーザーが OneDrive を使用するライセンスを持っている場合、委任された認証を使用するときに、この要求によりユーザーのドライブは自動的にプロビジョニングされます。</span><span class="sxs-lookup"><span data-stu-id="a5d1c-126">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="a5d1c-127">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a5d1c-127">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all", "tags": "service.graph" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a5d1c-128">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="a5d1c-128">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a5d1c-129">C#</span><span class="sxs-lookup"><span data-stu-id="a5d1c-129">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a5d1c-130">Javascript</span><span class="sxs-lookup"><span data-stu-id="a5d1c-130">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-user-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a5d1c-131">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5d1c-131">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-drive-by-user-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="path-parameters"></a><span data-ttu-id="a5d1c-132">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="a5d1c-132">Path parameters</span></span>

| <span data-ttu-id="a5d1c-133">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="a5d1c-133">Parameter name</span></span> | <span data-ttu-id="a5d1c-134">値</span><span class="sxs-lookup"><span data-stu-id="a5d1c-134">Value</span></span>  | <span data-ttu-id="a5d1c-135">説明</span><span class="sxs-lookup"><span data-stu-id="a5d1c-135">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="a5d1c-136">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="a5d1c-136">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="a5d1c-137">string</span><span class="sxs-lookup"><span data-stu-id="a5d1c-137">string</span></span> | <span data-ttu-id="a5d1c-138">必須。</span><span class="sxs-lookup"><span data-stu-id="a5d1c-138">Required.</span></span> <span data-ttu-id="a5d1c-139">OneDrive を所有するユーザー オブジェクトの識別子。</span><span class="sxs-lookup"><span data-stu-id="a5d1c-139">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="a5d1c-140">グループに関連付けられたドキュメント ライブラリを取得する</span><span class="sxs-lookup"><span data-stu-id="a5d1c-140">Get the document library associated with a group</span></span>

<span data-ttu-id="a5d1c-141">グループの既定のドキュメント ライブラリにアクセスするには、そのグループについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a5d1c-141">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="a5d1c-142">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a5d1c-142">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all", "tags": "service.graph" } -->

```http
GET /groups/{groupId}/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a5d1c-143">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="a5d1c-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a5d1c-144">C#</span><span class="sxs-lookup"><span data-stu-id="a5d1c-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a5d1c-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="a5d1c-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a5d1c-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5d1c-146">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-drive-by-group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="path-parameters"></a><span data-ttu-id="a5d1c-147">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="a5d1c-147">Path parameters</span></span>

| <span data-ttu-id="a5d1c-148">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="a5d1c-148">Parameter name</span></span> | <span data-ttu-id="a5d1c-149">値</span><span class="sxs-lookup"><span data-stu-id="a5d1c-149">Value</span></span>  | <span data-ttu-id="a5d1c-150">説明</span><span class="sxs-lookup"><span data-stu-id="a5d1c-150">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="a5d1c-151">_groupId_</span><span class="sxs-lookup"><span data-stu-id="a5d1c-151">_groupId_</span></span>      | <span data-ttu-id="a5d1c-152">string</span><span class="sxs-lookup"><span data-stu-id="a5d1c-152">string</span></span> | <span data-ttu-id="a5d1c-153">必須。</span><span class="sxs-lookup"><span data-stu-id="a5d1c-153">Required.</span></span> <span data-ttu-id="a5d1c-154">ドキュメント ライブラリを所有するグループの識別子。</span><span class="sxs-lookup"><span data-stu-id="a5d1c-154">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="a5d1c-155">サイトのドキュメント ライブラリを取得する</span><span class="sxs-lookup"><span data-stu-id="a5d1c-155">Get the document library for a site</span></span>

<span data-ttu-id="a5d1c-156">[サイトの](../resources/site.md)既定のドキュメント ライブラリにアクセスするには、そのサイトについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a5d1c-156">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="a5d1c-157">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a5d1c-157">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-site-id", "scopes": "group.read.all" } -->

```http
GET /sites/{siteId}/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a5d1c-158">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="a5d1c-158">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a5d1c-159">C#</span><span class="sxs-lookup"><span data-stu-id="a5d1c-159">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-site-id-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a5d1c-160">Javascript</span><span class="sxs-lookup"><span data-stu-id="a5d1c-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-site-id-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a5d1c-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5d1c-161">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-drive-by-site-id-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="path-parameters"></a><span data-ttu-id="a5d1c-162">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="a5d1c-162">Path parameters</span></span>

| <span data-ttu-id="a5d1c-163">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="a5d1c-163">Parameter name</span></span> | <span data-ttu-id="a5d1c-164">値</span><span class="sxs-lookup"><span data-stu-id="a5d1c-164">Value</span></span>  | <span data-ttu-id="a5d1c-165">説明</span><span class="sxs-lookup"><span data-stu-id="a5d1c-165">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="a5d1c-166">_siteId_</span><span class="sxs-lookup"><span data-stu-id="a5d1c-166">_siteId_</span></span>       | <span data-ttu-id="a5d1c-167">string</span><span class="sxs-lookup"><span data-stu-id="a5d1c-167">string</span></span> | <span data-ttu-id="a5d1c-168">必須。</span><span class="sxs-lookup"><span data-stu-id="a5d1c-168">Required.</span></span> <span data-ttu-id="a5d1c-169">ドキュメント ライブラリを含むサイトの識別子。</span><span class="sxs-lookup"><span data-stu-id="a5d1c-169">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="a5d1c-170">ID によりドライブを取得する</span><span class="sxs-lookup"><span data-stu-id="a5d1c-170">Get a drive by ID</span></span>

<span data-ttu-id="a5d1c-171">ドライブの一意の識別子を持っている場合、最上位ドライブのコレクションから直接アクセスできます。</span><span class="sxs-lookup"><span data-stu-id="a5d1c-171">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="a5d1c-172">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a5d1c-172">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}
```

### <a name="path-parameters"></a><span data-ttu-id="a5d1c-173">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="a5d1c-173">Path parameters</span></span>

| <span data-ttu-id="a5d1c-174">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="a5d1c-174">Parameter name</span></span> | <span data-ttu-id="a5d1c-175">値</span><span class="sxs-lookup"><span data-stu-id="a5d1c-175">Value</span></span>  | <span data-ttu-id="a5d1c-176">説明</span><span class="sxs-lookup"><span data-stu-id="a5d1c-176">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="a5d1c-177">_driveId_</span><span class="sxs-lookup"><span data-stu-id="a5d1c-177">_driveId_</span></span>      | <span data-ttu-id="a5d1c-178">string</span><span class="sxs-lookup"><span data-stu-id="a5d1c-178">string</span></span> | <span data-ttu-id="a5d1c-p105">必須。 要求されるドライブの識別子。</span><span class="sxs-lookup"><span data-stu-id="a5d1c-p105">Required. The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="a5d1c-181">省略可能なクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a5d1c-181">Optional query parameters</span></span>

<span data-ttu-id="a5d1c-182">応答を形成するため、これらのメソッドは [$select クエリ パラメーター][odata-query-parameters]をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="a5d1c-182">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="a5d1c-183">応答</span><span class="sxs-lookup"><span data-stu-id="a5d1c-183">Response</span></span>

<span data-ttu-id="a5d1c-184">各メソッドは、一致するドライブに応じた [Drive リソース][drive-resource]を応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="a5d1c-184">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="a5d1c-185">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="a5d1c-185">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a5d1c-186">C#</span><span class="sxs-lookup"><span data-stu-id="a5d1c-186">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-id-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a5d1c-187">Javascript</span><span class="sxs-lookup"><span data-stu-id="a5d1c-187">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-id-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a5d1c-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5d1c-188">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-drive-by-id-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="error-response-codes"></a><span data-ttu-id="a5d1c-189">エラー応答コード</span><span class="sxs-lookup"><span data-stu-id="a5d1c-189">Error response codes</span></span>

<span data-ttu-id="a5d1c-190">(委任された認証を使用する場合) ドライブが存在しないために自動的にプロビジョニングできないなら、`HTTP 404` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="a5d1c-190">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

[drive-resource]: ../resources/drive.md
[odata-query-parameters]: /graph/query-parameters

<!-- {
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "suppressions": [
    "Error: /api-reference/v1.0/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
      "Warning: /api-reference/v1.0/api/drive-get.md:
        Unable to map some markdown elements into schema.
            Unmapped methods:
        get-drive-default, get-drive-by-user, get-drive-by-group, get-drive-by-id
            Unmapped tables:
        Permissions - AuthScopes, Path parameters - PathParameters, Path parameters - PathParameters, Path parameters - PathParameters, Path parameters - PathParameters"
  ],
  "tocPath": "Drives/Get drive"
} -->
