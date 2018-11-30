---
title: Permissions
description: '前にチームの Microsoft アプリケーションのカタログを発行したアプリケーションを更新します。 '
ms.openlocfilehash: 38dd5cdbdb64c31d47c6d7e5b0c4bb27da8ad6e7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020856"
---
# <a name="update-apps-published-to-your-organizations-app-catalog"></a><span data-ttu-id="e08a0-103">組織のアプリケーションのカタログに公開するアプリケーションを更新します。</span><span class="sxs-lookup"><span data-stu-id="e08a0-103">Update apps published to your organization's app catalog</span></span>



<span data-ttu-id="e08a0-104">[アプリケーション](../resources/teamsapp.md)の更新プログラムは、以前マイクロソフト チーム アプリケーション カタログに公開します。</span><span class="sxs-lookup"><span data-stu-id="e08a0-104">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span> <span data-ttu-id="e08a0-105">この API は、具体的には、組織のアプリケーション カタログ (テナント アプリケーション カタログ) に公開されたアプリケーションを更新します。</span><span class="sxs-lookup"><span data-stu-id="e08a0-105">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="e08a0-106">組織のアプリケーションのカタログを公開するには、指定`organization` [teamsCatalogApp](../resources/teamsapp.md)リソースで**distributionMethod**とします。</span><span class="sxs-lookup"><span data-stu-id="e08a0-106">To publish to your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="e08a0-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e08a0-107">Permissions</span></span>

<span data-ttu-id="e08a0-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e08a0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="e08a0-110">**注:** グローバル管理者だけでは、この API を呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="e08a0-110">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="e08a0-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e08a0-111">Permission Type</span></span>                        | <span data-ttu-id="e08a0-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e08a0-112">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="e08a0-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e08a0-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="e08a0-114">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e08a0-114">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="e08a0-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e08a0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e08a0-116">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="e08a0-116">Not supported</span></span>|
| <span data-ttu-id="e08a0-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e08a0-117">Application</span></span>                            | <span data-ttu-id="e08a0-118">非サポート</span><span class="sxs-lookup"><span data-stu-id="e08a0-118">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="e08a0-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e08a0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e08a0-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e08a0-120">Request headers</span></span>

| <span data-ttu-id="e08a0-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e08a0-121">Header</span></span>        | <span data-ttu-id="e08a0-122">値</span><span class="sxs-lookup"><span data-stu-id="e08a0-122">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="e08a0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e08a0-123">Authorization</span></span> | <span data-ttu-id="e08a0-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e08a0-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e08a0-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e08a0-126">Content-Type</span></span>  | <span data-ttu-id="e08a0-127">アプリケーション/zip</span><span class="sxs-lookup"><span data-stu-id="e08a0-127">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="e08a0-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="e08a0-128">Request body</span></span>

<span data-ttu-id="e08a0-129">チーム Zip のマニフェスト ペイロード: チームのアプリケーションの zip 形式で圧縮ファイルは[、アプリケーション パッケージの作成を参照してください。](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="e08a0-129">Teams Zip Manifest Payload: For Teams application zip file [see Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

><span data-ttu-id="e08a0-130">**注:** 更新するにはアプリケーションを参照するための[リストには、アプリケーションが公開されて](./teamsapp-list.md)呼び出しから返された ID を使用します。</span><span class="sxs-lookup"><span data-stu-id="e08a0-130">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="e08a0-131">Zip アプリケーション パッケージのマニフェストの ID を使用しません。</span><span class="sxs-lookup"><span data-stu-id="e08a0-131">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="e08a0-132">応答</span><span class="sxs-lookup"><span data-stu-id="e08a0-132">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="e08a0-133">例</span><span class="sxs-lookup"><span data-stu-id="e08a0-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e08a0-134">要求</span><span class="sxs-lookup"><span data-stu-id="e08a0-134">Request</span></span>

```
PUT https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="e08a0-135">チームのアプリケーションの zip ファイルは[アプリケーション パッケージ作成を参照していますください。](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="e08a0-135">For Teams application zip file [see Create app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

### <a name="response"></a><span data-ttu-id="e08a0-136">応答</span><span class="sxs-lookup"><span data-stu-id="e08a0-136">Response</span></span>

```
HTTP/1.1 204 No Content
```
