---
title: Permissions
description: '前にチームの Microsoft アプリケーションのカタログを発行したアプリケーションを更新します。 '
ms.openlocfilehash: f63b75fe3373ad89148b2901b828dcc0ae1f95a3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073353"
---
# <a name="update-apps-published-to-your-organizations-app-catalog"></a><span data-ttu-id="19fc9-103">組織のアプリケーションのカタログに公開するアプリケーションを更新します。</span><span class="sxs-lookup"><span data-stu-id="19fc9-103">Update apps published to your organization's app catalog</span></span>

> <span data-ttu-id="19fc9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="19fc9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19fc9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="19fc9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="19fc9-106">[アプリケーション](../resources/teamsapp.md)の更新プログラムは、以前マイクロソフト チーム アプリケーション カタログに公開します。</span><span class="sxs-lookup"><span data-stu-id="19fc9-106">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span> <span data-ttu-id="19fc9-107">この API は、具体的には、組織のアプリケーション カタログ (テナント アプリケーション カタログ) に公開されたアプリケーションを更新します。</span><span class="sxs-lookup"><span data-stu-id="19fc9-107">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="19fc9-108">組織のアプリケーションのカタログを公開するには、指定`organization` [teamsCatalogApp](../resources/teamsapp.md)リソースで**distributionMethod**とします。</span><span class="sxs-lookup"><span data-stu-id="19fc9-108">To publish to your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="19fc9-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="19fc9-109">Permissions</span></span>

<span data-ttu-id="19fc9-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="19fc9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="19fc9-112">**注:** グローバル管理者だけでは、この API を呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="19fc9-112">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="19fc9-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="19fc9-113">Permission Type</span></span>                        | <span data-ttu-id="19fc9-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="19fc9-114">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="19fc9-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="19fc9-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="19fc9-116">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19fc9-116">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="19fc9-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="19fc9-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19fc9-118">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="19fc9-118">Not supported</span></span>|
| <span data-ttu-id="19fc9-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="19fc9-119">Application</span></span>                            | <span data-ttu-id="19fc9-120">非サポート</span><span class="sxs-lookup"><span data-stu-id="19fc9-120">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="19fc9-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="19fc9-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="19fc9-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="19fc9-122">Request headers</span></span>

| <span data-ttu-id="19fc9-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="19fc9-123">Header</span></span>        | <span data-ttu-id="19fc9-124">値</span><span class="sxs-lookup"><span data-stu-id="19fc9-124">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="19fc9-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="19fc9-125">Authorization</span></span> | <span data-ttu-id="19fc9-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="19fc9-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="19fc9-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="19fc9-128">Content-Type</span></span>  | <span data-ttu-id="19fc9-129">アプリケーション/zip</span><span class="sxs-lookup"><span data-stu-id="19fc9-129">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="19fc9-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="19fc9-130">Request body</span></span>

<span data-ttu-id="19fc9-131">チーム Zip のマニフェスト ペイロード: チームのアプリケーションの zip 形式で圧縮ファイルは[、アプリケーション パッケージの作成を参照してください。](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="19fc9-131">Teams Zip Manifest Payload: For Teams application zip file [see Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

><span data-ttu-id="19fc9-132">**注:** 更新するにはアプリケーションを参照するための[リストには、アプリケーションが公開されて](./teamsapp-list.md)呼び出しから返された ID を使用します。</span><span class="sxs-lookup"><span data-stu-id="19fc9-132">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="19fc9-133">Zip アプリケーション パッケージのマニフェストの ID を使用しません。</span><span class="sxs-lookup"><span data-stu-id="19fc9-133">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="19fc9-134">応答</span><span class="sxs-lookup"><span data-stu-id="19fc9-134">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="19fc9-135">例</span><span class="sxs-lookup"><span data-stu-id="19fc9-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="19fc9-136">要求</span><span class="sxs-lookup"><span data-stu-id="19fc9-136">Request</span></span>

```
PUT https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="19fc9-137">チームのアプリケーションの zip ファイルは[アプリケーション パッケージ作成を参照していますください。](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="19fc9-137">For Teams application zip file [see Create app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

### <a name="response"></a><span data-ttu-id="19fc9-138">応答</span><span class="sxs-lookup"><span data-stu-id="19fc9-138">Response</span></span>

```
HTTP/1.1 204 No Content
```
