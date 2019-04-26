---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ドライブを取得する
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 78d31fb584d345a401fddefac37399093c2d084b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551471"
---
# <a name="get-drive"></a><span data-ttu-id="8ad24-102">ドライブを取得する</span><span class="sxs-lookup"><span data-stu-id="8ad24-102">Get Drive</span></span>

<span data-ttu-id="8ad24-103">[Drive](../resources/drive.md) リソースのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="8ad24-103">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="8ad24-104">ドライブとは、OneDrive または SharePoint のドキュメント ライブラリなど、ファイル システムの最上位コンテナーです。</span><span class="sxs-lookup"><span data-stu-id="8ad24-104">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ad24-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8ad24-105">Permissions</span></span>

<span data-ttu-id="8ad24-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8ad24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ad24-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8ad24-108">Permission type</span></span>      | <span data-ttu-id="8ad24-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8ad24-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ad24-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8ad24-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8ad24-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ad24-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8ad24-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8ad24-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ad24-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ad24-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="8ad24-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8ad24-114">Application</span></span> | <span data-ttu-id="8ad24-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ad24-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="8ad24-116">現在のユーザーの OneDrive を取得する</span><span class="sxs-lookup"><span data-stu-id="8ad24-116">Get current user's OneDrive</span></span>

<span data-ttu-id="8ad24-117">(委任された認証を使用する場合) `me` シングルトンから、サインイン ユーザーのドライブにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="8ad24-117">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="8ad24-118">ユーザーの OneDrive はプロビジョニングされていないものの、ユーザーが OneDrive を使用するライセンスを持っている場合、委任された認証を使用するときに、この要求によりユーザーのドライブは自動的にプロビジョニングされます。</span><span class="sxs-lookup"><span data-stu-id="8ad24-118">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="8ad24-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8ad24-119">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive
```

## <a name="get-a-users-onedrive"></a><span data-ttu-id="8ad24-120">ユーザーの OneDrive を取得する</span><span class="sxs-lookup"><span data-stu-id="8ad24-120">Get a user's OneDrive</span></span>

<span data-ttu-id="8ad24-121">ユーザーの OneDrive または OneDrive for Business にアクセスするには、User リソースについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8ad24-121">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="8ad24-122">ユーザーの OneDrive はプロビジョニングされていないものの、ユーザーが OneDrive を使用するライセンスを持っている場合、委任された認証を使用するときに、この要求によりユーザーのドライブは自動的にプロビジョニングされます。</span><span class="sxs-lookup"><span data-stu-id="8ad24-122">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="8ad24-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8ad24-123">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all", "tags": "service.graph" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="8ad24-124">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="8ad24-124">Path parameters</span></span>

| <span data-ttu-id="8ad24-125">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="8ad24-125">Parameter name</span></span> | <span data-ttu-id="8ad24-126">値</span><span class="sxs-lookup"><span data-stu-id="8ad24-126">Value</span></span>  | <span data-ttu-id="8ad24-127">説明</span><span class="sxs-lookup"><span data-stu-id="8ad24-127">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="8ad24-128">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="8ad24-128">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="8ad24-129">string</span><span class="sxs-lookup"><span data-stu-id="8ad24-129">string</span></span> | <span data-ttu-id="8ad24-130">必須。</span><span class="sxs-lookup"><span data-stu-id="8ad24-130">Required.</span></span> <span data-ttu-id="8ad24-131">OneDrive を所有するユーザー オブジェクトの識別子。</span><span class="sxs-lookup"><span data-stu-id="8ad24-131">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="8ad24-132">グループに関連付けられたドキュメント ライブラリを取得する</span><span class="sxs-lookup"><span data-stu-id="8ad24-132">Get the document library associated with a group</span></span>

<span data-ttu-id="8ad24-133">グループの既定のドキュメント ライブラリにアクセスするには、そのグループについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8ad24-133">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="8ad24-134">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8ad24-134">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all", "tags": "service.graph" } -->

```http
GET /groups/{groupId}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="8ad24-135">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="8ad24-135">Path parameters</span></span>

| <span data-ttu-id="8ad24-136">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="8ad24-136">Parameter name</span></span> | <span data-ttu-id="8ad24-137">値</span><span class="sxs-lookup"><span data-stu-id="8ad24-137">Value</span></span>  | <span data-ttu-id="8ad24-138">説明</span><span class="sxs-lookup"><span data-stu-id="8ad24-138">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="8ad24-139">_groupId_</span><span class="sxs-lookup"><span data-stu-id="8ad24-139">_groupId_</span></span>      | <span data-ttu-id="8ad24-140">string</span><span class="sxs-lookup"><span data-stu-id="8ad24-140">string</span></span> | <span data-ttu-id="8ad24-141">必須。</span><span class="sxs-lookup"><span data-stu-id="8ad24-141">Required.</span></span> <span data-ttu-id="8ad24-142">ドキュメント ライブラリを所有するグループの識別子。</span><span class="sxs-lookup"><span data-stu-id="8ad24-142">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="8ad24-143">サイトのドキュメント ライブラリを取得する</span><span class="sxs-lookup"><span data-stu-id="8ad24-143">Get the document library for a site</span></span>

<span data-ttu-id="8ad24-144">[サイトの](../resources/site.md)既定のドキュメント ライブラリにアクセスするには、そのサイトについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8ad24-144">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="8ad24-145">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8ad24-145">HTTP request</span></span>

```http
GET /sites/{siteId}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="8ad24-146">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="8ad24-146">Path parameters</span></span>

| <span data-ttu-id="8ad24-147">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="8ad24-147">Parameter name</span></span> | <span data-ttu-id="8ad24-148">値</span><span class="sxs-lookup"><span data-stu-id="8ad24-148">Value</span></span>  | <span data-ttu-id="8ad24-149">説明</span><span class="sxs-lookup"><span data-stu-id="8ad24-149">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="8ad24-150">_siteId_</span><span class="sxs-lookup"><span data-stu-id="8ad24-150">_siteId_</span></span>       | <span data-ttu-id="8ad24-151">string</span><span class="sxs-lookup"><span data-stu-id="8ad24-151">string</span></span> | <span data-ttu-id="8ad24-152">必須。</span><span class="sxs-lookup"><span data-stu-id="8ad24-152">Required.</span></span> <span data-ttu-id="8ad24-153">ドキュメント ライブラリを含むサイトの識別子。</span><span class="sxs-lookup"><span data-stu-id="8ad24-153">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="8ad24-154">ID によりドライブを取得する</span><span class="sxs-lookup"><span data-stu-id="8ad24-154">Get a drive by ID</span></span>

<span data-ttu-id="8ad24-155">ドライブの一意の識別子を持っている場合、最上位ドライブのコレクションから直接アクセスできます。</span><span class="sxs-lookup"><span data-stu-id="8ad24-155">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="8ad24-156">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8ad24-156">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}
```

### <a name="path-parameters"></a><span data-ttu-id="8ad24-157">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="8ad24-157">Path parameters</span></span>

| <span data-ttu-id="8ad24-158">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="8ad24-158">Parameter name</span></span> | <span data-ttu-id="8ad24-159">値</span><span class="sxs-lookup"><span data-stu-id="8ad24-159">Value</span></span>  | <span data-ttu-id="8ad24-160">説明</span><span class="sxs-lookup"><span data-stu-id="8ad24-160">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="8ad24-161">_driveId_</span><span class="sxs-lookup"><span data-stu-id="8ad24-161">_driveId_</span></span>      | <span data-ttu-id="8ad24-162">string</span><span class="sxs-lookup"><span data-stu-id="8ad24-162">string</span></span> | <span data-ttu-id="8ad24-p105">必須。 要求されるドライブの識別子。</span><span class="sxs-lookup"><span data-stu-id="8ad24-p105">Required. The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="8ad24-165">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8ad24-165">Optional query parameters</span></span>

<span data-ttu-id="8ad24-166">応答を形成するため、これらのメソッドは [$select クエリ パラメーター][odata-query-parameters]をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="8ad24-166">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="8ad24-167">応答</span><span class="sxs-lookup"><span data-stu-id="8ad24-167">Response</span></span>

<span data-ttu-id="8ad24-168">各メソッドは、一致するドライブに応じた [Drive リソース][drive-resource]を応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="8ad24-168">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

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

### <a name="error-response-codes"></a><span data-ttu-id="8ad24-169">エラー応答コード</span><span class="sxs-lookup"><span data-stu-id="8ad24-169">Error response codes</span></span>

<span data-ttu-id="8ad24-170">(委任された認証を使用する場合) ドライブが存在しないために自動的にプロビジョニングできないなら、`HTTP 404` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="8ad24-170">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

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
