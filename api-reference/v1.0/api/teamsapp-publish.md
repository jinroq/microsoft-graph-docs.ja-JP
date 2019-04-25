---
title: アクセス許可
description: 'Microsoft Teams アプリカタログにアプリを発行します。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0c8093092a6a5dfc6d8c97df372832f15cc8eb20
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521762"
---
# <a name="publish-apps-to-your-organizations-app-catalog"></a><span data-ttu-id="8ae5c-103">組織のアプリカタログにアプリを発行する</span><span class="sxs-lookup"><span data-stu-id="8ae5c-103">Publish apps to your organization's app catalog</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ae5c-104">Microsoft Teams アプリカタログに[アプリ](../resources/teamsapp.md)を発行します。</span><span class="sxs-lookup"><span data-stu-id="8ae5c-104">Publish an [app](../resources/teamsapp.md) to the Microsoft Teams apps catalog.</span></span> <span data-ttu-id="8ae5c-105">具体的には、この API は、アプリを組織のカタログ (テナントのアプリカタログ) に公開します。作成されたリソース`distributionMethod`  =  `organization`には、があります。</span><span class="sxs-lookup"><span data-stu-id="8ae5c-105">Specifically, this API publishes the app to your organization's catalog (the tenant app catalog); the created resource will have `distributionMethod` = `organization`.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ae5c-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8ae5c-106">Permissions</span></span>

<span data-ttu-id="8ae5c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8ae5c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="8ae5c-109">**注:** この API は、グローバル管理者のみが呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="8ae5c-109">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="8ae5c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8ae5c-110">Permission Type</span></span>                        | <span data-ttu-id="8ae5c-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8ae5c-111">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="8ae5c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8ae5c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="8ae5c-113">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ae5c-113">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="8ae5c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8ae5c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ae5c-115">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="8ae5c-115">Not supported</span></span>|
| <span data-ttu-id="8ae5c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8ae5c-116">Application</span></span>                            | <span data-ttu-id="8ae5c-117">非サポート</span><span class="sxs-lookup"><span data-stu-id="8ae5c-117">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ae5c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8ae5c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /appCatalogs/teamsApps
```

## <a name="request-headers"></a><span data-ttu-id="8ae5c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8ae5c-119">Request headers</span></span>

| <span data-ttu-id="8ae5c-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8ae5c-120">Header</span></span>        | <span data-ttu-id="8ae5c-121">値</span><span class="sxs-lookup"><span data-stu-id="8ae5c-121">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="8ae5c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ae5c-122">Authorization</span></span> | <span data-ttu-id="8ae5c-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8ae5c-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8ae5c-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8ae5c-125">Content-Type</span></span>  | <span data-ttu-id="8ae5c-126">アプリケーション/zip</span><span class="sxs-lookup"><span data-stu-id="8ae5c-126">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ae5c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="8ae5c-127">Request body</span></span>

<span data-ttu-id="8ae5c-128">Teams の Zip マニフェストのペイロード。</span><span class="sxs-lookup"><span data-stu-id="8ae5c-128">Teams Zip Manifest Payload.</span></span> <span data-ttu-id="8ae5c-129">Teams アプリケーションの zip ファイルについ[ては、「アプリパッケージを作成する」を参照してください](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)。</span><span class="sxs-lookup"><span data-stu-id="8ae5c-129">For Teams application zip file [see Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> <span data-ttu-id="8ae5c-130">その組織の別のアプリと同じマニフェスト ID を持つ組織に対してアプリを作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="8ae5c-130">You can't create an app for an organization that has the same manifest ID as another app in that organization.</span></span>

## <a name="response"></a><span data-ttu-id="8ae5c-131">応答</span><span class="sxs-lookup"><span data-stu-id="8ae5c-131">Response</span></span>

<span data-ttu-id="8ae5c-132">成功した場合、このメソッド`200 OK`は応答コードと、 [teamsCatalogApp](../resources/teamsapp.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8ae5c-132">If successful, this method returns a `200 OK` response code and a [teamsCatalogApp](../resources/teamsapp.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="8ae5c-133">例</span><span class="sxs-lookup"><span data-stu-id="8ae5c-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ae5c-134">要求</span><span class="sxs-lookup"><span data-stu-id="8ae5c-134">Request</span></span>

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="8ae5c-135">Microsoft Teams アプリケーション zip ファイルを作成する方法については、「[アプリパッケージを作成](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8ae5c-135">For information about how to create a Microsoft Teams application zip file, see [Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> 

### <a name="response"></a><span data-ttu-id="8ae5c-136">応答</span><span class="sxs-lookup"><span data-stu-id="8ae5c-136">Response</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/teamsapp-publish.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
