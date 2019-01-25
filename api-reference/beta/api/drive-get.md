---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ドライブを取得する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 58f0a7f302aa41f286d949a4cbae56d6ff1cd62f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518171"
---
# <a name="get-drive"></a><span data-ttu-id="3107b-102">ドライブを取得する</span><span class="sxs-lookup"><span data-stu-id="3107b-102">Get Drive</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3107b-103">[Drive](../resources/drive.md) リソースのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="3107b-103">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="3107b-104">ドライブとは、OneDrive または SharePoint のドキュメント ライブラリなど、ファイル システムの最上位コンテナーです。</span><span class="sxs-lookup"><span data-stu-id="3107b-104">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="3107b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3107b-105">Permissions</span></span>

<span data-ttu-id="3107b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3107b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3107b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3107b-108">Permission type</span></span>      | <span data-ttu-id="3107b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3107b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3107b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3107b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3107b-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3107b-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="3107b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3107b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3107b-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3107b-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="3107b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3107b-114">Application</span></span> | <span data-ttu-id="3107b-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3107b-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="3107b-116">現在のユーザーの OneDrive を取得する</span><span class="sxs-lookup"><span data-stu-id="3107b-116">Get current user's OneDrive</span></span>

<span data-ttu-id="3107b-117">(委任された認証を使用する場合) `me` シングルトンから、サインイン ユーザーのドライブにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="3107b-117">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="3107b-118">ユーザーの OneDrive はプロビジョニングされていないものの、ユーザーが OneDrive を使用するライセンスを持っている場合、委任された認証を使用するときに、この要求によりユーザーのドライブは自動的にプロビジョニングされます。</span><span class="sxs-lookup"><span data-stu-id="3107b-118">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="3107b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3107b-119">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read" } -->

```http
GET /me/drive
```

## <a name="get-a-users-onedrive"></a><span data-ttu-id="3107b-120">ユーザーの OneDrive を取得する</span><span class="sxs-lookup"><span data-stu-id="3107b-120">Get a user's OneDrive</span></span>

<span data-ttu-id="3107b-121">ユーザーの OneDrive または OneDrive for Business にアクセスするには、User リソースについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3107b-121">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="3107b-122">ユーザーの OneDrive はプロビジョニングされていないものの、ユーザーが OneDrive を使用するライセンスを持っている場合、委任された認証を使用するときに、この要求によりユーザーのドライブは自動的にプロビジョニングされます。</span><span class="sxs-lookup"><span data-stu-id="3107b-122">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="3107b-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3107b-123">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="3107b-124">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="3107b-124">Path parameters</span></span>

| <span data-ttu-id="3107b-125">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="3107b-125">Parameter name</span></span> | <span data-ttu-id="3107b-126">値</span><span class="sxs-lookup"><span data-stu-id="3107b-126">Value</span></span>  | <span data-ttu-id="3107b-127">説明</span><span class="sxs-lookup"><span data-stu-id="3107b-127">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="3107b-128">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="3107b-128">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="3107b-129">string</span><span class="sxs-lookup"><span data-stu-id="3107b-129">string</span></span> | <span data-ttu-id="3107b-130">必須。</span><span class="sxs-lookup"><span data-stu-id="3107b-130">Required.</span></span> <span data-ttu-id="3107b-131">OneDrive を所有するユーザー オブジェクトの識別子。</span><span class="sxs-lookup"><span data-stu-id="3107b-131">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="3107b-132">グループに関連付けられたドキュメント ライブラリを取得する</span><span class="sxs-lookup"><span data-stu-id="3107b-132">Get the document library associated with a group</span></span>

<span data-ttu-id="3107b-133">グループの既定のドキュメント ライブラリにアクセスするには、そのグループについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3107b-133">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="3107b-134">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3107b-134">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all" } -->

```http
GET /groups/{groupId}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="3107b-135">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="3107b-135">Path parameters</span></span>

| <span data-ttu-id="3107b-136">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="3107b-136">Parameter name</span></span> | <span data-ttu-id="3107b-137">値</span><span class="sxs-lookup"><span data-stu-id="3107b-137">Value</span></span>  | <span data-ttu-id="3107b-138">説明</span><span class="sxs-lookup"><span data-stu-id="3107b-138">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="3107b-139">_groupId_</span><span class="sxs-lookup"><span data-stu-id="3107b-139">_groupId_</span></span>      | <span data-ttu-id="3107b-140">string</span><span class="sxs-lookup"><span data-stu-id="3107b-140">string</span></span> | <span data-ttu-id="3107b-141">必須。</span><span class="sxs-lookup"><span data-stu-id="3107b-141">Required.</span></span> <span data-ttu-id="3107b-142">ドキュメント ライブラリを所有するグループの識別子。</span><span class="sxs-lookup"><span data-stu-id="3107b-142">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="3107b-143">サイトのドキュメント ライブラリを取得する</span><span class="sxs-lookup"><span data-stu-id="3107b-143">Get the document library for a site</span></span>

<span data-ttu-id="3107b-144">[サイトの](../resources/site.md)既定のドキュメント ライブラリにアクセスするには、そのサイトについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3107b-144">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="3107b-145">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3107b-145">HTTP request</span></span>

```http
GET /sites/{siteId}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="3107b-146">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="3107b-146">Path parameters</span></span>

| <span data-ttu-id="3107b-147">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="3107b-147">Parameter name</span></span> | <span data-ttu-id="3107b-148">値</span><span class="sxs-lookup"><span data-stu-id="3107b-148">Value</span></span>  | <span data-ttu-id="3107b-149">説明</span><span class="sxs-lookup"><span data-stu-id="3107b-149">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="3107b-150">_siteId_</span><span class="sxs-lookup"><span data-stu-id="3107b-150">_siteId_</span></span>       | <span data-ttu-id="3107b-151">string</span><span class="sxs-lookup"><span data-stu-id="3107b-151">string</span></span> | <span data-ttu-id="3107b-152">必須。</span><span class="sxs-lookup"><span data-stu-id="3107b-152">Required.</span></span> <span data-ttu-id="3107b-153">ドキュメント ライブラリを含むサイトの識別子。</span><span class="sxs-lookup"><span data-stu-id="3107b-153">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="3107b-154">ID によりドライブを取得する</span><span class="sxs-lookup"><span data-stu-id="3107b-154">Get a drive by ID</span></span>

<span data-ttu-id="3107b-155">ドライブの一意の識別子を持っている場合、最上位ドライブのコレクションから直接アクセスできます。</span><span class="sxs-lookup"><span data-stu-id="3107b-155">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="3107b-156">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3107b-156">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{driveId}
```

### <a name="path-parameters"></a><span data-ttu-id="3107b-157">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="3107b-157">Path parameters</span></span>

| <span data-ttu-id="3107b-158">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="3107b-158">Parameter name</span></span> | <span data-ttu-id="3107b-159">値</span><span class="sxs-lookup"><span data-stu-id="3107b-159">Value</span></span>  | <span data-ttu-id="3107b-160">説明</span><span class="sxs-lookup"><span data-stu-id="3107b-160">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="3107b-161">_driveId_</span><span class="sxs-lookup"><span data-stu-id="3107b-161">_driveId_</span></span>      | <span data-ttu-id="3107b-162">string</span><span class="sxs-lookup"><span data-stu-id="3107b-162">string</span></span> | <span data-ttu-id="3107b-163">必須。</span><span class="sxs-lookup"><span data-stu-id="3107b-163">Required.</span></span> <span data-ttu-id="3107b-164">要求されるドライブの識別子。</span><span class="sxs-lookup"><span data-stu-id="3107b-164">The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="3107b-165">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3107b-165">Optional query parameters</span></span>

<span data-ttu-id="3107b-166">応答を形成するため、これらのメソッドは [$select クエリ パラメーター][odata-query-parameters]をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="3107b-166">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="3107b-167">応答</span><span class="sxs-lookup"><span data-stu-id="3107b-167">Response</span></span>

<span data-ttu-id="3107b-168">各メソッドは、一致するドライブに応じた [Drive リソース][drive-resource]を応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="3107b-168">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

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

### <a name="error-response-codes"></a><span data-ttu-id="3107b-169">エラー応答コード</span><span class="sxs-lookup"><span data-stu-id="3107b-169">Error response codes</span></span>

<span data-ttu-id="3107b-170">(委任された認証を使用する場合) ドライブが存在しないために自動的にプロビジョニングできないなら、`HTTP 404` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="3107b-170">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

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
    "Error: /api-reference/beta/api/drive-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
