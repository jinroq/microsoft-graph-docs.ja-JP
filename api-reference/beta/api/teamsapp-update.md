---
title: アクセス許可
description: '以前に Microsoft Teams アプリカタログに発行したアプリを更新します。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 48bf1682821578c786ad9e52b00409f35b6fab66
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33330670"
---
# <a name="update-apps-published-to-your-organizations-app-catalog"></a><span data-ttu-id="0a57d-103">組織のアプリカタログに発行されたアプリを更新する</span><span class="sxs-lookup"><span data-stu-id="0a57d-103">Update apps published to your organization's app catalog</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a57d-104">以前に Microsoft Teams アプリカタログに発行した[アプリ](../resources/teamsapp.md)を更新します。</span><span class="sxs-lookup"><span data-stu-id="0a57d-104">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span> <span data-ttu-id="0a57d-105">この API は、組織のアプリカタログ (テナントのアプリカタログ) に公開されたアプリを特に更新します。</span><span class="sxs-lookup"><span data-stu-id="0a57d-105">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="0a57d-106">組織のアプリカタログに発行するには、 `organization` teamsCatalogApp リソース\*\*\*\* の " [](../resources/teamsapp.md) " としてを指定します。</span><span class="sxs-lookup"><span data-stu-id="0a57d-106">To publish to your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a57d-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0a57d-107">Permissions</span></span>

<span data-ttu-id="0a57d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0a57d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="0a57d-110">**注:** この API は、グローバル管理者のみが呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="0a57d-110">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="0a57d-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0a57d-111">Permission Type</span></span>                        | <span data-ttu-id="0a57d-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0a57d-112">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="0a57d-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0a57d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="0a57d-114">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a57d-114">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="0a57d-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0a57d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a57d-116">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="0a57d-116">Not supported</span></span>|
| <span data-ttu-id="0a57d-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0a57d-117">Application</span></span>                            | <span data-ttu-id="0a57d-118">非サポート</span><span class="sxs-lookup"><span data-stu-id="0a57d-118">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a57d-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0a57d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0a57d-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0a57d-120">Request headers</span></span>

| <span data-ttu-id="0a57d-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0a57d-121">Header</span></span>        | <span data-ttu-id="0a57d-122">値</span><span class="sxs-lookup"><span data-stu-id="0a57d-122">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="0a57d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a57d-123">Authorization</span></span> | <span data-ttu-id="0a57d-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0a57d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0a57d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0a57d-126">Content-Type</span></span>  | <span data-ttu-id="0a57d-127">アプリケーション/zip</span><span class="sxs-lookup"><span data-stu-id="0a57d-127">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="0a57d-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="0a57d-128">Request body</span></span>

<span data-ttu-id="0a57d-129">teams zip マニフェストペイロード: teams アプリケーション zip ファイルについ[ては、「アプリパッケージを作成する」を参照してください](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)。</span><span class="sxs-lookup"><span data-stu-id="0a57d-129">Teams Zip Manifest Payload: For Teams application zip file [see Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

><span data-ttu-id="0a57d-130">**注:** の[発行済みアプリの一覧](./teamsapp-list.md)から返された ID を使用して、更新するアプリを参照します。</span><span class="sxs-lookup"><span data-stu-id="0a57d-130">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="0a57d-131">zip アプリパッケージのマニフェストからの ID は使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="0a57d-131">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="0a57d-132">応答</span><span class="sxs-lookup"><span data-stu-id="0a57d-132">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="0a57d-133">例</span><span class="sxs-lookup"><span data-stu-id="0a57d-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a57d-134">要求</span><span class="sxs-lookup"><span data-stu-id="0a57d-134">Request</span></span>

```
PUT https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="0a57d-135">Teams アプリケーションの zip ファイルについては、 [「アプリパッケージの作成」を参照してください](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)。</span><span class="sxs-lookup"><span data-stu-id="0a57d-135">For Teams application zip file [see Create app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

### <a name="response"></a><span data-ttu-id="0a57d-136">応答</span><span class="sxs-lookup"><span data-stu-id="0a57d-136">Response</span></span>

```
HTTP/1.1 204 No Content
```
