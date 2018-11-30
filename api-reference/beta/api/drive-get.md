---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ドライブを取得する
ms.openlocfilehash: 620797ec453f9456f6ea6a6dcb90d396f43a7a4b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069229"
---
# <a name="get-drive"></a><span data-ttu-id="8a645-102">ドライブを取得する</span><span class="sxs-lookup"><span data-stu-id="8a645-102">Get Drive</span></span>

> <span data-ttu-id="8a645-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8a645-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8a645-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a645-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8a645-105">[Drive](../resources/drive.md) リソースのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="8a645-105">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="8a645-106">ドライブとは、OneDrive または SharePoint のドキュメント ライブラリなど、ファイル システムの最上位コンテナーです。</span><span class="sxs-lookup"><span data-stu-id="8a645-106">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a645-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8a645-107">Permissions</span></span>

<span data-ttu-id="8a645-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8a645-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a645-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8a645-110">Permission type</span></span>      | <span data-ttu-id="8a645-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8a645-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a645-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8a645-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8a645-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a645-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8a645-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8a645-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a645-115">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a645-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="8a645-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8a645-116">Application</span></span> | <span data-ttu-id="8a645-117">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a645-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="8a645-118">現在のユーザーの OneDrive を取得する</span><span class="sxs-lookup"><span data-stu-id="8a645-118">Get current user's OneDrive</span></span>

<span data-ttu-id="8a645-119">(委任された認証を使用する場合) `me` シングルトンから、サインイン ユーザーのドライブにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="8a645-119">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="8a645-120">ユーザーの OneDrive はプロビジョニングされていないものの、ユーザーが OneDrive を使用するライセンスを持っている場合、委任された認証を使用するときに、この要求によりユーザーのドライブは自動的にプロビジョニングされます。</span><span class="sxs-lookup"><span data-stu-id="8a645-120">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="8a645-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8a645-121">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read" } -->

```http
GET /me/drive
```

## <a name="get-a-users-onedrive"></a><span data-ttu-id="8a645-122">ユーザーの OneDrive を取得する</span><span class="sxs-lookup"><span data-stu-id="8a645-122">Get a user's OneDrive</span></span>

<span data-ttu-id="8a645-123">ユーザーの OneDrive または OneDrive for Business にアクセスするには、User リソースについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8a645-123">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="8a645-124">ユーザーの OneDrive はプロビジョニングされていないものの、ユーザーが OneDrive を使用するライセンスを持っている場合、委任された認証を使用するときに、この要求によりユーザーのドライブは自動的にプロビジョニングされます。</span><span class="sxs-lookup"><span data-stu-id="8a645-124">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="8a645-125">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8a645-125">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="8a645-126">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="8a645-126">Path parameters</span></span>

| <span data-ttu-id="8a645-127">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="8a645-127">Parameter name</span></span> | <span data-ttu-id="8a645-128">値</span><span class="sxs-lookup"><span data-stu-id="8a645-128">Value</span></span>  | <span data-ttu-id="8a645-129">説明</span><span class="sxs-lookup"><span data-stu-id="8a645-129">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="8a645-130">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="8a645-130">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="8a645-131">文字列</span><span class="sxs-lookup"><span data-stu-id="8a645-131">string</span></span> | <span data-ttu-id="8a645-132">必須。</span><span class="sxs-lookup"><span data-stu-id="8a645-132">Required.</span></span> <span data-ttu-id="8a645-133">OneDrive を所有するユーザー オブジェクトの識別子。</span><span class="sxs-lookup"><span data-stu-id="8a645-133">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="8a645-134">グループに関連付けられたドキュメント ライブラリを取得する</span><span class="sxs-lookup"><span data-stu-id="8a645-134">Get the document library associated with a group</span></span>

<span data-ttu-id="8a645-135">グループの既定のドキュメント ライブラリにアクセスするには、そのグループについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8a645-135">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="8a645-136">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8a645-136">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all" } -->

```http
GET /groups/{groupId}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="8a645-137">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="8a645-137">Path parameters</span></span>

| <span data-ttu-id="8a645-138">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="8a645-138">Parameter name</span></span> | <span data-ttu-id="8a645-139">値</span><span class="sxs-lookup"><span data-stu-id="8a645-139">Value</span></span>  | <span data-ttu-id="8a645-140">説明</span><span class="sxs-lookup"><span data-stu-id="8a645-140">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="8a645-141">_groupId_</span><span class="sxs-lookup"><span data-stu-id="8a645-141">_groupId_</span></span>      | <span data-ttu-id="8a645-142">文字列</span><span class="sxs-lookup"><span data-stu-id="8a645-142">string</span></span> | <span data-ttu-id="8a645-143">必須。</span><span class="sxs-lookup"><span data-stu-id="8a645-143">Required.</span></span> <span data-ttu-id="8a645-144">ドキュメント ライブラリを所有するグループの識別子。</span><span class="sxs-lookup"><span data-stu-id="8a645-144">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="8a645-145">サイトのドキュメント ライブラリを取得する</span><span class="sxs-lookup"><span data-stu-id="8a645-145">Get the document library for a site</span></span>

<span data-ttu-id="8a645-146">[サイトの](../resources/site.md)既定のドキュメント ライブラリにアクセスするには、そのサイトについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8a645-146">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="8a645-147">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8a645-147">HTTP request</span></span>

```http
GET /sites/{siteId}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="8a645-148">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="8a645-148">Path parameters</span></span>

| <span data-ttu-id="8a645-149">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="8a645-149">Parameter name</span></span> | <span data-ttu-id="8a645-150">値</span><span class="sxs-lookup"><span data-stu-id="8a645-150">Value</span></span>  | <span data-ttu-id="8a645-151">説明</span><span class="sxs-lookup"><span data-stu-id="8a645-151">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="8a645-152">_siteId_</span><span class="sxs-lookup"><span data-stu-id="8a645-152">_siteId_</span></span>       | <span data-ttu-id="8a645-153">文字列</span><span class="sxs-lookup"><span data-stu-id="8a645-153">string</span></span> | <span data-ttu-id="8a645-154">必須。</span><span class="sxs-lookup"><span data-stu-id="8a645-154">Required.</span></span> <span data-ttu-id="8a645-155">ドキュメント ライブラリを含むサイトの識別子。</span><span class="sxs-lookup"><span data-stu-id="8a645-155">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="8a645-156">ID によりドライブを取得する</span><span class="sxs-lookup"><span data-stu-id="8a645-156">Get a drive by ID</span></span>

<span data-ttu-id="8a645-157">ドライブの一意の識別子を持っている場合、最上位ドライブのコレクションから直接アクセスできます。</span><span class="sxs-lookup"><span data-stu-id="8a645-157">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="8a645-158">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8a645-158">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{driveId}
```

### <a name="path-parameters"></a><span data-ttu-id="8a645-159">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="8a645-159">Path parameters</span></span>

| <span data-ttu-id="8a645-160">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="8a645-160">Parameter name</span></span> | <span data-ttu-id="8a645-161">値</span><span class="sxs-lookup"><span data-stu-id="8a645-161">Value</span></span>  | <span data-ttu-id="8a645-162">説明</span><span class="sxs-lookup"><span data-stu-id="8a645-162">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="8a645-163">_driveId_</span><span class="sxs-lookup"><span data-stu-id="8a645-163">_driveId_</span></span>      | <span data-ttu-id="8a645-164">文字列</span><span class="sxs-lookup"><span data-stu-id="8a645-164">string</span></span> | <span data-ttu-id="8a645-165">必須。</span><span class="sxs-lookup"><span data-stu-id="8a645-165">Required.</span></span> <span data-ttu-id="8a645-166">要求されるドライブの識別子。</span><span class="sxs-lookup"><span data-stu-id="8a645-166">The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="8a645-167">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8a645-167">Optional query parameters</span></span>

<span data-ttu-id="8a645-168">応答を形成するため、これらのメソッドは [$select クエリ パラメーター][odata-query-parameters]をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="8a645-168">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="http-response"></a><span data-ttu-id="8a645-169">HTTP 応答</span><span class="sxs-lookup"><span data-stu-id="8a645-169">HTTP response</span></span>

<span data-ttu-id="8a645-170">各メソッドは、一致するドライブに応じた [Drive リソース][drive-resource]を応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="8a645-170">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

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

### <a name="error-response-codes"></a><span data-ttu-id="8a645-171">エラー応答コード</span><span class="sxs-lookup"><span data-stu-id="8a645-171">Error response codes</span></span>

<span data-ttu-id="8a645-172">(委任された認証を使用する場合) ドライブが存在しないために自動的にプロビジョニングできないなら、`HTTP 404` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="8a645-172">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

[drive-resource]: ../resources/drive.md
[odata-query-parameters]: /graph/query-parameters

<!-- {
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "tocPath": "Drives/Get drive"
} -->
