---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ドライブを取得する
ms.openlocfilehash: 6ff71104c18a5a9354d18689c62a96be72b7fe12
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021489"
---
# <a name="get-drive"></a><span data-ttu-id="2a4a8-102">ドライブを取得する</span><span class="sxs-lookup"><span data-stu-id="2a4a8-102">Get Drive</span></span>

<span data-ttu-id="2a4a8-103">[Drive](../resources/drive.md) リソースのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="2a4a8-103">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="2a4a8-104">ドライブとは、OneDrive または SharePoint のドキュメント ライブラリなど、ファイル システムの最上位コンテナーです。</span><span class="sxs-lookup"><span data-stu-id="2a4a8-104">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a4a8-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2a4a8-105">Permissions</span></span>

<span data-ttu-id="2a4a8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2a4a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a4a8-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2a4a8-108">Permission type</span></span>      | <span data-ttu-id="2a4a8-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2a4a8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2a4a8-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2a4a8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2a4a8-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a4a8-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2a4a8-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2a4a8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a4a8-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a4a8-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="2a4a8-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2a4a8-114">Application</span></span> | <span data-ttu-id="2a4a8-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a4a8-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="2a4a8-116">現在のユーザーの OneDrive を取得する</span><span class="sxs-lookup"><span data-stu-id="2a4a8-116">Get current user's OneDrive</span></span>

<span data-ttu-id="2a4a8-117">(委任された認証を使用する場合) `me` シングルトンから、サインイン ユーザーのドライブにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="2a4a8-117">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="2a4a8-118">ユーザーの OneDrive はプロビジョニングされていないものの、ユーザーが OneDrive を使用するライセンスを持っている場合、委任された認証を使用するときに、この要求によりユーザーのドライブは自動的にプロビジョニングされます。</span><span class="sxs-lookup"><span data-stu-id="2a4a8-118">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="2a4a8-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2a4a8-119">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive
```

## <a name="get-a-users-onedrive"></a><span data-ttu-id="2a4a8-120">ユーザーの OneDrive を取得する</span><span class="sxs-lookup"><span data-stu-id="2a4a8-120">Get a user's OneDrive</span></span>

<span data-ttu-id="2a4a8-121">ユーザーの OneDrive または OneDrive for Business にアクセスするには、User リソースについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2a4a8-121">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="2a4a8-122">ユーザーの OneDrive はプロビジョニングされていないものの、ユーザーが OneDrive を使用するライセンスを持っている場合、委任された認証を使用するときに、この要求によりユーザーのドライブは自動的にプロビジョニングされます。</span><span class="sxs-lookup"><span data-stu-id="2a4a8-122">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="2a4a8-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2a4a8-123">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all", "tags": "service.graph" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="2a4a8-124">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="2a4a8-124">Path parameters</span></span>

| <span data-ttu-id="2a4a8-125">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="2a4a8-125">Parameter name</span></span> | <span data-ttu-id="2a4a8-126">値</span><span class="sxs-lookup"><span data-stu-id="2a4a8-126">Value</span></span>  | <span data-ttu-id="2a4a8-127">説明</span><span class="sxs-lookup"><span data-stu-id="2a4a8-127">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="2a4a8-128">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="2a4a8-128">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="2a4a8-129">文字列</span><span class="sxs-lookup"><span data-stu-id="2a4a8-129">string</span></span> | <span data-ttu-id="2a4a8-130">必須。</span><span class="sxs-lookup"><span data-stu-id="2a4a8-130">Required.</span></span> <span data-ttu-id="2a4a8-131">OneDrive を所有するユーザー オブジェクトの識別子。</span><span class="sxs-lookup"><span data-stu-id="2a4a8-131">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="2a4a8-132">グループに関連付けられたドキュメント ライブラリを取得する</span><span class="sxs-lookup"><span data-stu-id="2a4a8-132">Get the document library associated with a group</span></span>

<span data-ttu-id="2a4a8-133">グループの既定のドキュメント ライブラリにアクセスするには、そのグループについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2a4a8-133">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="2a4a8-134">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2a4a8-134">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all", "tags": "service.graph" } -->

```http
GET /groups/{groupId}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="2a4a8-135">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="2a4a8-135">Path parameters</span></span>

| <span data-ttu-id="2a4a8-136">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="2a4a8-136">Parameter name</span></span> | <span data-ttu-id="2a4a8-137">値</span><span class="sxs-lookup"><span data-stu-id="2a4a8-137">Value</span></span>  | <span data-ttu-id="2a4a8-138">説明</span><span class="sxs-lookup"><span data-stu-id="2a4a8-138">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="2a4a8-139">_groupId_</span><span class="sxs-lookup"><span data-stu-id="2a4a8-139">_groupId_</span></span>      | <span data-ttu-id="2a4a8-140">文字列</span><span class="sxs-lookup"><span data-stu-id="2a4a8-140">string</span></span> | <span data-ttu-id="2a4a8-141">必須。</span><span class="sxs-lookup"><span data-stu-id="2a4a8-141">Required.</span></span> <span data-ttu-id="2a4a8-142">ドキュメント ライブラリを所有するグループの識別子。</span><span class="sxs-lookup"><span data-stu-id="2a4a8-142">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="2a4a8-143">サイトのドキュメント ライブラリを取得する</span><span class="sxs-lookup"><span data-stu-id="2a4a8-143">Get the document library for a site</span></span>

<span data-ttu-id="2a4a8-144">[サイトの](../resources/site.md)既定のドキュメント ライブラリにアクセスするには、そのサイトについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2a4a8-144">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="2a4a8-145">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2a4a8-145">HTTP request</span></span>

```http
GET /sites/{siteId}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="2a4a8-146">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="2a4a8-146">Path parameters</span></span>

| <span data-ttu-id="2a4a8-147">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="2a4a8-147">Parameter name</span></span> | <span data-ttu-id="2a4a8-148">値</span><span class="sxs-lookup"><span data-stu-id="2a4a8-148">Value</span></span>  | <span data-ttu-id="2a4a8-149">説明</span><span class="sxs-lookup"><span data-stu-id="2a4a8-149">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="2a4a8-150">_siteId_</span><span class="sxs-lookup"><span data-stu-id="2a4a8-150">_siteId_</span></span>       | <span data-ttu-id="2a4a8-151">文字列</span><span class="sxs-lookup"><span data-stu-id="2a4a8-151">string</span></span> | <span data-ttu-id="2a4a8-152">必須。</span><span class="sxs-lookup"><span data-stu-id="2a4a8-152">Required.</span></span> <span data-ttu-id="2a4a8-153">ドキュメント ライブラリを含むサイトの識別子。</span><span class="sxs-lookup"><span data-stu-id="2a4a8-153">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="2a4a8-154">ID によりドライブを取得する</span><span class="sxs-lookup"><span data-stu-id="2a4a8-154">Get a drive by ID</span></span>

<span data-ttu-id="2a4a8-155">ドライブの一意の識別子を持っている場合、最上位ドライブのコレクションから直接アクセスできます。</span><span class="sxs-lookup"><span data-stu-id="2a4a8-155">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="2a4a8-156">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2a4a8-156">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}
```

### <a name="path-parameters"></a><span data-ttu-id="2a4a8-157">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="2a4a8-157">Path parameters</span></span>

| <span data-ttu-id="2a4a8-158">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="2a4a8-158">Parameter name</span></span> | <span data-ttu-id="2a4a8-159">値</span><span class="sxs-lookup"><span data-stu-id="2a4a8-159">Value</span></span>  | <span data-ttu-id="2a4a8-160">説明</span><span class="sxs-lookup"><span data-stu-id="2a4a8-160">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="2a4a8-161">_driveId_</span><span class="sxs-lookup"><span data-stu-id="2a4a8-161">_driveId_</span></span>      | <span data-ttu-id="2a4a8-162">文字列</span><span class="sxs-lookup"><span data-stu-id="2a4a8-162">string</span></span> | <span data-ttu-id="2a4a8-163">必須。</span><span class="sxs-lookup"><span data-stu-id="2a4a8-163">Required.</span></span> <span data-ttu-id="2a4a8-164">要求されるドライブの識別子。</span><span class="sxs-lookup"><span data-stu-id="2a4a8-164">The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="2a4a8-165">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2a4a8-165">Optional query parameters</span></span>

<span data-ttu-id="2a4a8-166">応答を形成するため、これらのメソッドは [$select クエリ パラメーター][odata-query-parameters]をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="2a4a8-166">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="http-response"></a><span data-ttu-id="2a4a8-167">HTTP 応答</span><span class="sxs-lookup"><span data-stu-id="2a4a8-167">HTTP response</span></span>

<span data-ttu-id="2a4a8-168">各メソッドは、一致するドライブに応じた [Drive リソース][drive-resource]を応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="2a4a8-168">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

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

### <a name="error-response-codes"></a><span data-ttu-id="2a4a8-169">エラー応答コード</span><span class="sxs-lookup"><span data-stu-id="2a4a8-169">Error response codes</span></span>

<span data-ttu-id="2a4a8-170">(委任された認証を使用する場合) ドライブが存在しないために自動的にプロビジョニングできないなら、`HTTP 404` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="2a4a8-170">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

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
