---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ドライブを取得する
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: f1fd3b48646c0df4a982652545e8494839f40c02
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33589647"
---
# <a name="get-drive"></a><span data-ttu-id="154d1-102">ドライブを取得する</span><span class="sxs-lookup"><span data-stu-id="154d1-102">Get Drive</span></span>

<span data-ttu-id="154d1-103">[Drive](../resources/drive.md) リソースのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="154d1-103">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="154d1-104">ドライブとは、OneDrive または SharePoint のドキュメント ライブラリなど、ファイル システムの最上位コンテナーです。</span><span class="sxs-lookup"><span data-stu-id="154d1-104">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="154d1-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="154d1-105">Permissions</span></span>

<span data-ttu-id="154d1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="154d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="154d1-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="154d1-108">Permission type</span></span>      | <span data-ttu-id="154d1-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="154d1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="154d1-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="154d1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="154d1-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="154d1-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="154d1-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="154d1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="154d1-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="154d1-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="154d1-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="154d1-114">Application</span></span> | <span data-ttu-id="154d1-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="154d1-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="154d1-116">現在のユーザーの OneDrive を取得する</span><span class="sxs-lookup"><span data-stu-id="154d1-116">Get current user's OneDrive</span></span>

<span data-ttu-id="154d1-117">(委任された認証を使用する場合) `me` シングルトンから、サインイン ユーザーのドライブにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="154d1-117">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="154d1-118">ユーザーの OneDrive はプロビジョニングされていないものの、ユーザーが OneDrive を使用するライセンスを持っている場合、委任された認証を使用するときに、この要求によりユーザーのドライブは自動的にプロビジョニングされます。</span><span class="sxs-lookup"><span data-stu-id="154d1-118">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="154d1-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="154d1-119">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="154d1-120">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="154d1-120">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="154d1-121">Visual</span><span class="sxs-lookup"><span data-stu-id="154d1-121">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-default-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="154d1-122">Java</span><span class="sxs-lookup"><span data-stu-id="154d1-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-default-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="get-a-users-onedrive"></a><span data-ttu-id="154d1-123">ユーザーの OneDrive を取得する</span><span class="sxs-lookup"><span data-stu-id="154d1-123">Get a user's OneDrive</span></span>

<span data-ttu-id="154d1-124">ユーザーの OneDrive または OneDrive for Business にアクセスするには、User リソースについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="154d1-124">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="154d1-125">ユーザーの OneDrive はプロビジョニングされていないものの、ユーザーが OneDrive を使用するライセンスを持っている場合、委任された認証を使用するときに、この要求によりユーザーのドライブは自動的にプロビジョニングされます。</span><span class="sxs-lookup"><span data-stu-id="154d1-125">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="154d1-126">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="154d1-126">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all", "tags": "service.graph" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="154d1-127">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="154d1-127">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="154d1-128">Visual</span><span class="sxs-lookup"><span data-stu-id="154d1-128">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="154d1-129">Java</span><span class="sxs-lookup"><span data-stu-id="154d1-129">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-user-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="path-parameters"></a><span data-ttu-id="154d1-130">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="154d1-130">Path parameters</span></span>

| <span data-ttu-id="154d1-131">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="154d1-131">Parameter name</span></span> | <span data-ttu-id="154d1-132">値</span><span class="sxs-lookup"><span data-stu-id="154d1-132">Value</span></span>  | <span data-ttu-id="154d1-133">説明</span><span class="sxs-lookup"><span data-stu-id="154d1-133">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="154d1-134">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="154d1-134">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="154d1-135">string</span><span class="sxs-lookup"><span data-stu-id="154d1-135">string</span></span> | <span data-ttu-id="154d1-136">必須です。</span><span class="sxs-lookup"><span data-stu-id="154d1-136">Required.</span></span> <span data-ttu-id="154d1-137">OneDrive を所有するユーザー オブジェクトの識別子。</span><span class="sxs-lookup"><span data-stu-id="154d1-137">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="154d1-138">グループに関連付けられたドキュメント ライブラリを取得する</span><span class="sxs-lookup"><span data-stu-id="154d1-138">Get the document library associated with a group</span></span>

<span data-ttu-id="154d1-139">グループの既定のドキュメント ライブラリにアクセスするには、そのグループについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="154d1-139">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="154d1-140">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="154d1-140">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all", "tags": "service.graph" } -->

```http
GET /groups/{groupId}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="154d1-141">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="154d1-141">Path parameters</span></span>

| <span data-ttu-id="154d1-142">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="154d1-142">Parameter name</span></span> | <span data-ttu-id="154d1-143">値</span><span class="sxs-lookup"><span data-stu-id="154d1-143">Value</span></span>  | <span data-ttu-id="154d1-144">説明</span><span class="sxs-lookup"><span data-stu-id="154d1-144">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="154d1-145">_groupId_</span><span class="sxs-lookup"><span data-stu-id="154d1-145">_groupId_</span></span>      | <span data-ttu-id="154d1-146">string</span><span class="sxs-lookup"><span data-stu-id="154d1-146">string</span></span> | <span data-ttu-id="154d1-147">必須です。</span><span class="sxs-lookup"><span data-stu-id="154d1-147">Required.</span></span> <span data-ttu-id="154d1-148">ドキュメント ライブラリを所有するグループの識別子。</span><span class="sxs-lookup"><span data-stu-id="154d1-148">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="154d1-149">サイトのドキュメント ライブラリを取得する</span><span class="sxs-lookup"><span data-stu-id="154d1-149">Get the document library for a site</span></span>

<span data-ttu-id="154d1-150">[サイトの](../resources/site.md)既定のドキュメント ライブラリにアクセスするには、そのサイトについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="154d1-150">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="154d1-151">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="154d1-151">HTTP request</span></span>

```http
GET /sites/{siteId}/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="154d1-152">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="154d1-152">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="154d1-153">Visual</span><span class="sxs-lookup"><span data-stu-id="154d1-153">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="154d1-154">Java</span><span class="sxs-lookup"><span data-stu-id="154d1-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="path-parameters"></a><span data-ttu-id="154d1-155">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="154d1-155">Path parameters</span></span>

| <span data-ttu-id="154d1-156">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="154d1-156">Parameter name</span></span> | <span data-ttu-id="154d1-157">値</span><span class="sxs-lookup"><span data-stu-id="154d1-157">Value</span></span>  | <span data-ttu-id="154d1-158">説明</span><span class="sxs-lookup"><span data-stu-id="154d1-158">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="154d1-159">_siteId_</span><span class="sxs-lookup"><span data-stu-id="154d1-159">_siteId_</span></span>       | <span data-ttu-id="154d1-160">string</span><span class="sxs-lookup"><span data-stu-id="154d1-160">string</span></span> | <span data-ttu-id="154d1-161">必須。</span><span class="sxs-lookup"><span data-stu-id="154d1-161">Required.</span></span> <span data-ttu-id="154d1-162">ドキュメント ライブラリを含むサイトの識別子。</span><span class="sxs-lookup"><span data-stu-id="154d1-162">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="154d1-163">ID によりドライブを取得する</span><span class="sxs-lookup"><span data-stu-id="154d1-163">Get a drive by ID</span></span>

<span data-ttu-id="154d1-164">ドライブの一意の識別子を持っている場合、最上位ドライブのコレクションから直接アクセスできます。</span><span class="sxs-lookup"><span data-stu-id="154d1-164">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="154d1-165">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="154d1-165">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}
```

### <a name="path-parameters"></a><span data-ttu-id="154d1-166">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="154d1-166">Path parameters</span></span>

| <span data-ttu-id="154d1-167">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="154d1-167">Parameter name</span></span> | <span data-ttu-id="154d1-168">値</span><span class="sxs-lookup"><span data-stu-id="154d1-168">Value</span></span>  | <span data-ttu-id="154d1-169">説明</span><span class="sxs-lookup"><span data-stu-id="154d1-169">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="154d1-170">_driveId_</span><span class="sxs-lookup"><span data-stu-id="154d1-170">_driveId_</span></span>      | <span data-ttu-id="154d1-171">string</span><span class="sxs-lookup"><span data-stu-id="154d1-171">string</span></span> | <span data-ttu-id="154d1-p105">必須。 要求されるドライブの識別子。</span><span class="sxs-lookup"><span data-stu-id="154d1-p105">Required. The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="154d1-174">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="154d1-174">Optional query parameters</span></span>

<span data-ttu-id="154d1-175">応答を形成するため、これらのメソッドは [$select クエリ パラメーター][odata-query-parameters]をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="154d1-175">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="154d1-176">応答</span><span class="sxs-lookup"><span data-stu-id="154d1-176">Response</span></span>

<span data-ttu-id="154d1-177">各メソッドは、一致するドライブに応じた [Drive リソース][drive-resource]を応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="154d1-177">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.drive", "truncated": true, "name": ["get-drive-by-id", "get-drive-by-group", "get-drive-by-user", "get-drive-default"] } -->

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="154d1-178">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="154d1-178">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="154d1-179">Visual</span><span class="sxs-lookup"><span data-stu-id="154d1-179">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-id-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="154d1-180">Java</span><span class="sxs-lookup"><span data-stu-id="154d1-180">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-id-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="error-response-codes"></a><span data-ttu-id="154d1-181">エラー応答コード</span><span class="sxs-lookup"><span data-stu-id="154d1-181">Error response codes</span></span>

<span data-ttu-id="154d1-182">(委任された認証を使用する場合) ドライブが存在しないために自動的にプロビジョニングできないなら、`HTTP 404` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="154d1-182">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

[drive-resource]: ../resources/drive.md
[odata-query-parameters]: /graph/query-parameters

<!-- {
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "suppressions": [
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
