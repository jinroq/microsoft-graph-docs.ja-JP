---
title: アクセス許可
description: 'マイクロソフト チーム アプリケーション カタログにアプリケーションを発行します。 '
author: nkramer
ms.openlocfilehash: 01d552a013b3d1324893bd775611e797253ff261
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27335197"
---
# <a name="publish-apps-to-your-organizations-app-catalog"></a><span data-ttu-id="cdcee-103">アプリケーションを組織のアプリケーションのカタログに発行します。</span><span class="sxs-lookup"><span data-stu-id="cdcee-103">Publish apps to your organization's app catalog</span></span>

> <span data-ttu-id="cdcee-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cdcee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cdcee-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cdcee-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cdcee-106">マイクロソフト チーム アプリケーション カタログに[アプリケーション](../resources/teamsapp.md)を発行します。</span><span class="sxs-lookup"><span data-stu-id="cdcee-106">Publish an [app](../resources/teamsapp.md) to the Microsoft Teams apps catalog.</span></span> <span data-ttu-id="cdcee-107">この API が、アプリケーションを公開して、組織のカタログ (テナント アプリケーション カタログ) に具体的には、作成されたリソースがある`distributionMethod`  =  `organization`。</span><span class="sxs-lookup"><span data-stu-id="cdcee-107">Specifically, this API publishes the app to your organization's catalog (the tenant app catalog); the created resource will have `distributionMethod` = `organization`.</span></span>

## <a name="permissions"></a><span data-ttu-id="cdcee-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cdcee-108">Permissions</span></span>

<span data-ttu-id="cdcee-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cdcee-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="cdcee-111">**注:** グローバル管理者だけでは、この API を呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="cdcee-111">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="cdcee-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cdcee-112">Permission Type</span></span>                        | <span data-ttu-id="cdcee-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cdcee-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="cdcee-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cdcee-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="cdcee-115">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdcee-115">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="cdcee-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cdcee-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cdcee-117">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="cdcee-117">Not supported</span></span>|
| <span data-ttu-id="cdcee-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cdcee-118">Application</span></span>                            | <span data-ttu-id="cdcee-119">非サポート</span><span class="sxs-lookup"><span data-stu-id="cdcee-119">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="cdcee-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cdcee-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /appCatalogs/teamsApps
```

## <a name="request-headers"></a><span data-ttu-id="cdcee-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cdcee-121">Request headers</span></span>

| <span data-ttu-id="cdcee-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cdcee-122">Header</span></span>        | <span data-ttu-id="cdcee-123">値</span><span class="sxs-lookup"><span data-stu-id="cdcee-123">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="cdcee-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cdcee-124">Authorization</span></span> | <span data-ttu-id="cdcee-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cdcee-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cdcee-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cdcee-127">Content-Type</span></span>  | <span data-ttu-id="cdcee-128">アプリケーション/zip</span><span class="sxs-lookup"><span data-stu-id="cdcee-128">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="cdcee-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="cdcee-129">Request body</span></span>

<span data-ttu-id="cdcee-130">チーム Zip のマニフェスト ペイロード。</span><span class="sxs-lookup"><span data-stu-id="cdcee-130">Teams Zip Manifest Payload.</span></span> <span data-ttu-id="cdcee-131">チームのアプリケーションのファイルは[、アプリケーション パッケージの作成を参照してください](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)zip 形式で圧縮します。</span><span class="sxs-lookup"><span data-stu-id="cdcee-131">For Teams application zip file [see Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> <span data-ttu-id="cdcee-132">その組織の別のアプリケーションと同じマニフェスト ID を持つ組織のアプリケーションを作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="cdcee-132">You can't create an app for an organization that has the same manifest ID as another app in that organization.</span></span>

## <a name="response"></a><span data-ttu-id="cdcee-133">応答</span><span class="sxs-lookup"><span data-stu-id="cdcee-133">Response</span></span>

<span data-ttu-id="cdcee-134">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードと[teamsCatalogApp](../resources/teamsapp.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="cdcee-134">If successful, this method returns a `200 OK` response code and a [teamsCatalogApp](../resources/teamsapp.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="cdcee-135">例</span><span class="sxs-lookup"><span data-stu-id="cdcee-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="cdcee-136">要求</span><span class="sxs-lookup"><span data-stu-id="cdcee-136">Request</span></span>

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="cdcee-137">マイクロソフト チームのアプリケーションの zip ファイルを作成する方法の詳細については、[作成されたアプリケーション パッケージ](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cdcee-137">For information about how to create a Microsoft Teams application zip file, see [Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> 

### <a name="response"></a><span data-ttu-id="cdcee-138">応答</span><span class="sxs-lookup"><span data-stu-id="cdcee-138">Response</span></span>

```
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "e3e29acb-8c79-412b-b746-e6c39ff4cd22",
  "externalId": "b5561ec9-8cab-4aa3-8aa2-d8d7172e4311",
  "name": "Test App",
  "version": "1.0.0",
  "distributionMethod": "organization"
}
```
