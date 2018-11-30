---
title: Permissions
description: 'マイクロソフト チーム アプリケーション カタログにアプリケーションを発行します。 '
ms.openlocfilehash: c33a1d85673b9f59aade253b2ea5fd237eb5fc83
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020960"
---
# <a name="publish-apps-to-your-organizations-app-catalog"></a><span data-ttu-id="f94a7-103">アプリケーションを組織のアプリケーションのカタログに発行します。</span><span class="sxs-lookup"><span data-stu-id="f94a7-103">Publish apps to your organization's app catalog</span></span>



<span data-ttu-id="f94a7-104">マイクロソフト チーム アプリケーション カタログに[アプリケーション](../resources/teamsapp.md)を発行します。</span><span class="sxs-lookup"><span data-stu-id="f94a7-104">Publish an [app](../resources/teamsapp.md) to the Microsoft Teams apps catalog.</span></span> <span data-ttu-id="f94a7-105">この API が、アプリケーションを公開して、組織のカタログ (テナント アプリケーション カタログ) に具体的には、作成されたリソースがある`distributionMethod`  =  `organization`。</span><span class="sxs-lookup"><span data-stu-id="f94a7-105">Specifically, this API publishes the app to your organization's catalog (the tenant app catalog); the created resource will have `distributionMethod` = `organization`.</span></span>

## <a name="permissions"></a><span data-ttu-id="f94a7-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f94a7-106">Permissions</span></span>

<span data-ttu-id="f94a7-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f94a7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="f94a7-109">**注:** グローバル管理者だけでは、この API を呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="f94a7-109">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="f94a7-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f94a7-110">Permission Type</span></span>                        | <span data-ttu-id="f94a7-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f94a7-111">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="f94a7-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f94a7-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f94a7-113">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f94a7-113">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="f94a7-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f94a7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f94a7-115">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="f94a7-115">Not supported</span></span>|
| <span data-ttu-id="f94a7-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f94a7-116">Application</span></span>                            | <span data-ttu-id="f94a7-117">非サポート</span><span class="sxs-lookup"><span data-stu-id="f94a7-117">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="f94a7-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f94a7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /appCatalogs/teamsApps
```

## <a name="request-headers"></a><span data-ttu-id="f94a7-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f94a7-119">Request headers</span></span>

| <span data-ttu-id="f94a7-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f94a7-120">Header</span></span>        | <span data-ttu-id="f94a7-121">値</span><span class="sxs-lookup"><span data-stu-id="f94a7-121">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="f94a7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f94a7-122">Authorization</span></span> | <span data-ttu-id="f94a7-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f94a7-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f94a7-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f94a7-125">Content-Type</span></span>  | <span data-ttu-id="f94a7-126">アプリケーション/zip</span><span class="sxs-lookup"><span data-stu-id="f94a7-126">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="f94a7-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f94a7-127">Request body</span></span>

<span data-ttu-id="f94a7-128">チーム Zip のマニフェスト ペイロード。</span><span class="sxs-lookup"><span data-stu-id="f94a7-128">Teams Zip Manifest Payload.</span></span> <span data-ttu-id="f94a7-129">チームのアプリケーションのファイルは[、アプリケーション パッケージの作成を参照してください](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)zip 形式で圧縮します。</span><span class="sxs-lookup"><span data-stu-id="f94a7-129">For Teams application zip file [see Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> <span data-ttu-id="f94a7-130">その組織の別のアプリケーションと同じマニフェスト ID を持つ組織のアプリケーションを作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="f94a7-130">You can't create an app for an organization that has the same manifest ID as another app in that organization.</span></span>

## <a name="response"></a><span data-ttu-id="f94a7-131">応答</span><span class="sxs-lookup"><span data-stu-id="f94a7-131">Response</span></span>

<span data-ttu-id="f94a7-132">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードと[teamsCatalogApp](../resources/teamsapp.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="f94a7-132">If successful, this method returns a `200 OK` response code and a [teamsCatalogApp](../resources/teamsapp.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="f94a7-133">例</span><span class="sxs-lookup"><span data-stu-id="f94a7-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="f94a7-134">要求</span><span class="sxs-lookup"><span data-stu-id="f94a7-134">Request</span></span>

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="f94a7-135">マイクロソフト チームのアプリケーションの zip ファイルを作成する方法の詳細については、[作成されたアプリケーション パッケージ](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f94a7-135">For information about how to create a Microsoft Teams application zip file, see [Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> 

### <a name="response"></a><span data-ttu-id="f94a7-136">応答</span><span class="sxs-lookup"><span data-stu-id="f94a7-136">Response</span></span>

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
