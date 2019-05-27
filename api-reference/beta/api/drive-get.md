---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ドライブを取得する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 34a3b2a772f225a4b4806f0e8b305bd036bd03f7
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34434278"
---
# <a name="get-drive"></a><span data-ttu-id="66244-102">ドライブを取得する</span><span class="sxs-lookup"><span data-stu-id="66244-102">Get Drive</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66244-103">[Drive](../resources/drive.md) リソースのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="66244-103">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="66244-104">ドライブとは、OneDrive または SharePoint のドキュメント ライブラリなど、ファイル システムの最上位コンテナーです。</span><span class="sxs-lookup"><span data-stu-id="66244-104">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="66244-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="66244-105">Permissions</span></span>

<span data-ttu-id="66244-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="66244-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66244-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="66244-108">Permission type</span></span>      | <span data-ttu-id="66244-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="66244-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66244-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="66244-110">Delegated (work or school account)</span></span> | <span data-ttu-id="66244-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66244-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="66244-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="66244-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66244-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66244-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="66244-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="66244-114">Application</span></span> | <span data-ttu-id="66244-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66244-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="66244-116">現在のユーザーの OneDrive を取得する</span><span class="sxs-lookup"><span data-stu-id="66244-116">Get current user's OneDrive</span></span>

<span data-ttu-id="66244-117">(委任された認証を使用する場合) `me` シングルトンから、サインイン ユーザーのドライブにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="66244-117">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="66244-118">ユーザーの OneDrive はプロビジョニングされていないものの、ユーザーが OneDrive を使用するライセンスを持っている場合、委任された認証を使用するときに、この要求によりユーザーのドライブは自動的にプロビジョニングされます。</span><span class="sxs-lookup"><span data-stu-id="66244-118">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="66244-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="66244-119">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read" } -->

```http
GET /me/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="66244-120">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="66244-120">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="66244-121">C#</span><span class="sxs-lookup"><span data-stu-id="66244-121">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-default-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="66244-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="66244-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-default-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="get-a-users-onedrive"></a><span data-ttu-id="66244-123">ユーザーの OneDrive を取得する</span><span class="sxs-lookup"><span data-stu-id="66244-123">Get a user's OneDrive</span></span>

<span data-ttu-id="66244-124">ユーザーの OneDrive または OneDrive for Business にアクセスするには、User リソースについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="66244-124">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="66244-125">ユーザーの OneDrive はプロビジョニングされていないものの、ユーザーが OneDrive を使用するライセンスを持っている場合、委任された認証を使用するときに、この要求によりユーザーのドライブは自動的にプロビジョニングされます。</span><span class="sxs-lookup"><span data-stu-id="66244-125">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="66244-126">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="66244-126">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="66244-127">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="66244-127">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="66244-128">C#</span><span class="sxs-lookup"><span data-stu-id="66244-128">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="66244-129">Javascript</span><span class="sxs-lookup"><span data-stu-id="66244-129">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-user-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="path-parameters"></a><span data-ttu-id="66244-130">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="66244-130">Path parameters</span></span>

| <span data-ttu-id="66244-131">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="66244-131">Parameter name</span></span> | <span data-ttu-id="66244-132">値</span><span class="sxs-lookup"><span data-stu-id="66244-132">Value</span></span>  | <span data-ttu-id="66244-133">説明</span><span class="sxs-lookup"><span data-stu-id="66244-133">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="66244-134">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="66244-134">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="66244-135">string</span><span class="sxs-lookup"><span data-stu-id="66244-135">string</span></span> | <span data-ttu-id="66244-136">必須です。</span><span class="sxs-lookup"><span data-stu-id="66244-136">Required.</span></span> <span data-ttu-id="66244-137">OneDrive を所有するユーザー オブジェクトの識別子。</span><span class="sxs-lookup"><span data-stu-id="66244-137">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="66244-138">グループに関連付けられたドキュメント ライブラリを取得する</span><span class="sxs-lookup"><span data-stu-id="66244-138">Get the document library associated with a group</span></span>

<span data-ttu-id="66244-139">グループの既定のドキュメント ライブラリにアクセスするには、そのグループについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="66244-139">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="66244-140">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="66244-140">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all" } -->

```http
GET /groups/{groupId}/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="66244-141">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="66244-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="66244-142">C#</span><span class="sxs-lookup"><span data-stu-id="66244-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="66244-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="66244-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="path-parameters"></a><span data-ttu-id="66244-144">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="66244-144">Path parameters</span></span>

| <span data-ttu-id="66244-145">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="66244-145">Parameter name</span></span> | <span data-ttu-id="66244-146">値</span><span class="sxs-lookup"><span data-stu-id="66244-146">Value</span></span>  | <span data-ttu-id="66244-147">説明</span><span class="sxs-lookup"><span data-stu-id="66244-147">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="66244-148">_groupId_</span><span class="sxs-lookup"><span data-stu-id="66244-148">_groupId_</span></span>      | <span data-ttu-id="66244-149">string</span><span class="sxs-lookup"><span data-stu-id="66244-149">string</span></span> | <span data-ttu-id="66244-150">必須です。</span><span class="sxs-lookup"><span data-stu-id="66244-150">Required.</span></span> <span data-ttu-id="66244-151">ドキュメント ライブラリを所有するグループの識別子。</span><span class="sxs-lookup"><span data-stu-id="66244-151">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="66244-152">サイトのドキュメント ライブラリを取得する</span><span class="sxs-lookup"><span data-stu-id="66244-152">Get the document library for a site</span></span>

<span data-ttu-id="66244-153">[サイトの](../resources/site.md)既定のドキュメント ライブラリにアクセスするには、そのサイトについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="66244-153">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="66244-154">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="66244-154">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-site-id", "scopes": "group.read.all" } -->

```http
GET /sites/{siteId}/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="66244-155">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="66244-155">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="66244-156">C#</span><span class="sxs-lookup"><span data-stu-id="66244-156">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-site-id-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="66244-157">Javascript</span><span class="sxs-lookup"><span data-stu-id="66244-157">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-site-id-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="path-parameters"></a><span data-ttu-id="66244-158">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="66244-158">Path parameters</span></span>

| <span data-ttu-id="66244-159">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="66244-159">Parameter name</span></span> | <span data-ttu-id="66244-160">値</span><span class="sxs-lookup"><span data-stu-id="66244-160">Value</span></span>  | <span data-ttu-id="66244-161">説明</span><span class="sxs-lookup"><span data-stu-id="66244-161">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="66244-162">_siteId_</span><span class="sxs-lookup"><span data-stu-id="66244-162">_siteId_</span></span>       | <span data-ttu-id="66244-163">string</span><span class="sxs-lookup"><span data-stu-id="66244-163">string</span></span> | <span data-ttu-id="66244-164">必須。</span><span class="sxs-lookup"><span data-stu-id="66244-164">Required.</span></span> <span data-ttu-id="66244-165">ドキュメント ライブラリを含むサイトの識別子。</span><span class="sxs-lookup"><span data-stu-id="66244-165">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="66244-166">ID によりドライブを取得する</span><span class="sxs-lookup"><span data-stu-id="66244-166">Get a drive by ID</span></span>

<span data-ttu-id="66244-167">ドライブの一意の識別子を持っている場合、最上位ドライブのコレクションから直接アクセスできます。</span><span class="sxs-lookup"><span data-stu-id="66244-167">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="66244-168">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="66244-168">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{driveId}
```

### <a name="path-parameters"></a><span data-ttu-id="66244-169">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="66244-169">Path parameters</span></span>

| <span data-ttu-id="66244-170">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="66244-170">Parameter name</span></span> | <span data-ttu-id="66244-171">値</span><span class="sxs-lookup"><span data-stu-id="66244-171">Value</span></span>  | <span data-ttu-id="66244-172">説明</span><span class="sxs-lookup"><span data-stu-id="66244-172">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="66244-173">_driveId_</span><span class="sxs-lookup"><span data-stu-id="66244-173">_driveId_</span></span>      | <span data-ttu-id="66244-174">string</span><span class="sxs-lookup"><span data-stu-id="66244-174">string</span></span> | <span data-ttu-id="66244-p105">必須。 要求されるドライブの識別子。</span><span class="sxs-lookup"><span data-stu-id="66244-p105">Required. The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="66244-177">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="66244-177">Optional query parameters</span></span>

<span data-ttu-id="66244-178">応答を形成するため、これらのメソッドは [$select クエリ パラメーター][odata-query-parameters]をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="66244-178">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="66244-179">応答</span><span class="sxs-lookup"><span data-stu-id="66244-179">Response</span></span>

<span data-ttu-id="66244-180">各メソッドは、一致するドライブに応じた [Drive リソース][drive-resource]を応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="66244-180">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="66244-181">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="66244-181">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="66244-182">C#</span><span class="sxs-lookup"><span data-stu-id="66244-182">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-id-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="66244-183">Javascript</span><span class="sxs-lookup"><span data-stu-id="66244-183">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-id-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="error-response-codes"></a><span data-ttu-id="66244-184">エラー応答コード</span><span class="sxs-lookup"><span data-stu-id="66244-184">Error response codes</span></span>

<span data-ttu-id="66244-185">(委任された認証を使用する場合) ドライブが存在しないために自動的にプロビジョニングできないなら、`HTTP 404` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="66244-185">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

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
    "Error: /api-reference/beta/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
