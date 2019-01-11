---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ドライブを取得する
localization_priority: Normal
ms.openlocfilehash: d18ee7191747b2c625b62bdecec6d3bffdf0f57e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859659"
---
# <a name="get-drive"></a><span data-ttu-id="be5a8-102">ドライブを取得する</span><span class="sxs-lookup"><span data-stu-id="be5a8-102">Get Drive</span></span>

> <span data-ttu-id="be5a8-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="be5a8-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="be5a8-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be5a8-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="be5a8-105">[Drive](../resources/drive.md) リソースのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="be5a8-105">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="be5a8-106">ドライブとは、OneDrive または SharePoint のドキュメント ライブラリなど、ファイル システムの最上位コンテナーです。</span><span class="sxs-lookup"><span data-stu-id="be5a8-106">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="be5a8-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="be5a8-107">Permissions</span></span>

<span data-ttu-id="be5a8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="be5a8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be5a8-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="be5a8-110">Permission type</span></span>      | <span data-ttu-id="be5a8-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="be5a8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be5a8-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="be5a8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="be5a8-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be5a8-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="be5a8-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="be5a8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be5a8-115">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be5a8-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="be5a8-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="be5a8-116">Application</span></span> | <span data-ttu-id="be5a8-117">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be5a8-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="be5a8-118">現在のユーザーの OneDrive を取得する</span><span class="sxs-lookup"><span data-stu-id="be5a8-118">Get current user's OneDrive</span></span>

<span data-ttu-id="be5a8-119">(委任された認証を使用する場合) `me` シングルトンから、サインイン ユーザーのドライブにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="be5a8-119">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="be5a8-120">ユーザーの OneDrive はプロビジョニングされていないものの、ユーザーが OneDrive を使用するライセンスを持っている場合、委任された認証を使用するときに、この要求によりユーザーのドライブは自動的にプロビジョニングされます。</span><span class="sxs-lookup"><span data-stu-id="be5a8-120">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="be5a8-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="be5a8-121">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read" } -->

```http
GET /me/drive
```

## <a name="get-a-users-onedrive"></a><span data-ttu-id="be5a8-122">ユーザーの OneDrive を取得する</span><span class="sxs-lookup"><span data-stu-id="be5a8-122">Get a user's OneDrive</span></span>

<span data-ttu-id="be5a8-123">ユーザーの OneDrive または OneDrive for Business にアクセスするには、User リソースについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="be5a8-123">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="be5a8-124">ユーザーの OneDrive はプロビジョニングされていないものの、ユーザーが OneDrive を使用するライセンスを持っている場合、委任された認証を使用するときに、この要求によりユーザーのドライブは自動的にプロビジョニングされます。</span><span class="sxs-lookup"><span data-stu-id="be5a8-124">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="be5a8-125">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="be5a8-125">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="be5a8-126">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="be5a8-126">Path parameters</span></span>

| <span data-ttu-id="be5a8-127">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="be5a8-127">Parameter name</span></span> | <span data-ttu-id="be5a8-128">値</span><span class="sxs-lookup"><span data-stu-id="be5a8-128">Value</span></span>  | <span data-ttu-id="be5a8-129">説明</span><span class="sxs-lookup"><span data-stu-id="be5a8-129">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="be5a8-130">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="be5a8-130">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="be5a8-131">文字列</span><span class="sxs-lookup"><span data-stu-id="be5a8-131">string</span></span> | <span data-ttu-id="be5a8-132">必須。</span><span class="sxs-lookup"><span data-stu-id="be5a8-132">Required.</span></span> <span data-ttu-id="be5a8-133">OneDrive を所有するユーザー オブジェクトの識別子。</span><span class="sxs-lookup"><span data-stu-id="be5a8-133">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="be5a8-134">グループに関連付けられたドキュメント ライブラリを取得する</span><span class="sxs-lookup"><span data-stu-id="be5a8-134">Get the document library associated with a group</span></span>

<span data-ttu-id="be5a8-135">グループの既定のドキュメント ライブラリにアクセスするには、そのグループについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="be5a8-135">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="be5a8-136">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="be5a8-136">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all" } -->

```http
GET /groups/{groupId}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="be5a8-137">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="be5a8-137">Path parameters</span></span>

| <span data-ttu-id="be5a8-138">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="be5a8-138">Parameter name</span></span> | <span data-ttu-id="be5a8-139">値</span><span class="sxs-lookup"><span data-stu-id="be5a8-139">Value</span></span>  | <span data-ttu-id="be5a8-140">説明</span><span class="sxs-lookup"><span data-stu-id="be5a8-140">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="be5a8-141">_groupId_</span><span class="sxs-lookup"><span data-stu-id="be5a8-141">_groupId_</span></span>      | <span data-ttu-id="be5a8-142">文字列</span><span class="sxs-lookup"><span data-stu-id="be5a8-142">string</span></span> | <span data-ttu-id="be5a8-143">必須。</span><span class="sxs-lookup"><span data-stu-id="be5a8-143">Required.</span></span> <span data-ttu-id="be5a8-144">ドキュメント ライブラリを所有するグループの識別子。</span><span class="sxs-lookup"><span data-stu-id="be5a8-144">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="be5a8-145">サイトのドキュメント ライブラリを取得する</span><span class="sxs-lookup"><span data-stu-id="be5a8-145">Get the document library for a site</span></span>

<span data-ttu-id="be5a8-146">[サイトの](../resources/site.md)既定のドキュメント ライブラリにアクセスするには、そのサイトについての**ドライブ** リレーションシップをアプリが要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="be5a8-146">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="be5a8-147">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="be5a8-147">HTTP request</span></span>

```http
GET /sites/{siteId}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="be5a8-148">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="be5a8-148">Path parameters</span></span>

| <span data-ttu-id="be5a8-149">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="be5a8-149">Parameter name</span></span> | <span data-ttu-id="be5a8-150">値</span><span class="sxs-lookup"><span data-stu-id="be5a8-150">Value</span></span>  | <span data-ttu-id="be5a8-151">説明</span><span class="sxs-lookup"><span data-stu-id="be5a8-151">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="be5a8-152">_siteId_</span><span class="sxs-lookup"><span data-stu-id="be5a8-152">_siteId_</span></span>       | <span data-ttu-id="be5a8-153">文字列</span><span class="sxs-lookup"><span data-stu-id="be5a8-153">string</span></span> | <span data-ttu-id="be5a8-154">必須。</span><span class="sxs-lookup"><span data-stu-id="be5a8-154">Required.</span></span> <span data-ttu-id="be5a8-155">ドキュメント ライブラリを含むサイトの識別子。</span><span class="sxs-lookup"><span data-stu-id="be5a8-155">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="be5a8-156">ID によりドライブを取得する</span><span class="sxs-lookup"><span data-stu-id="be5a8-156">Get a drive by ID</span></span>

<span data-ttu-id="be5a8-157">ドライブの一意の識別子を持っている場合、最上位ドライブのコレクションから直接アクセスできます。</span><span class="sxs-lookup"><span data-stu-id="be5a8-157">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="be5a8-158">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="be5a8-158">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{driveId}
```

### <a name="path-parameters"></a><span data-ttu-id="be5a8-159">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="be5a8-159">Path parameters</span></span>

| <span data-ttu-id="be5a8-160">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="be5a8-160">Parameter name</span></span> | <span data-ttu-id="be5a8-161">値</span><span class="sxs-lookup"><span data-stu-id="be5a8-161">Value</span></span>  | <span data-ttu-id="be5a8-162">説明</span><span class="sxs-lookup"><span data-stu-id="be5a8-162">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="be5a8-163">_driveId_</span><span class="sxs-lookup"><span data-stu-id="be5a8-163">_driveId_</span></span>      | <span data-ttu-id="be5a8-164">文字列</span><span class="sxs-lookup"><span data-stu-id="be5a8-164">string</span></span> | <span data-ttu-id="be5a8-165">必須。</span><span class="sxs-lookup"><span data-stu-id="be5a8-165">Required.</span></span> <span data-ttu-id="be5a8-166">要求されるドライブの識別子。</span><span class="sxs-lookup"><span data-stu-id="be5a8-166">The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="be5a8-167">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="be5a8-167">Optional query parameters</span></span>

<span data-ttu-id="be5a8-168">応答を形成するため、これらのメソッドは [$select クエリ パラメーター][odata-query-parameters]をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="be5a8-168">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="be5a8-169">応答</span><span class="sxs-lookup"><span data-stu-id="be5a8-169">Response</span></span>

<span data-ttu-id="be5a8-170">各メソッドは、一致するドライブに応じた [Drive リソース][drive-resource]を応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="be5a8-170">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

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

### <a name="error-response-codes"></a><span data-ttu-id="be5a8-171">エラー応答コード</span><span class="sxs-lookup"><span data-stu-id="be5a8-171">Error response codes</span></span>

<span data-ttu-id="be5a8-172">(委任された認証を使用する場合) ドライブが存在しないために自動的にプロビジョニングできないなら、`HTTP 404` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="be5a8-172">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

[drive-resource]: ../resources/drive.md
[odata-query-parameters]: /graph/query-parameters

<!-- {
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "tocPath": "Drives/Get drive"
} -->
