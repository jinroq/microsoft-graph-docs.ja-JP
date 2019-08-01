---
title: アクセス許可
description: '組織のアプリカタログ (テナントのアプリカタログ) からアプリを削除します。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7fa273be1265c4e0a236688cc4af4a3f695a1477
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36021141"
---
# <a name="remove-an-app-from-your-organizations-app-catalog"></a><span data-ttu-id="1a37e-103">組織のアプリカタログからアプリを削除する</span><span class="sxs-lookup"><span data-stu-id="1a37e-103">Remove an app from your organization's app catalog</span></span>



<span data-ttu-id="1a37e-104">組織のアプリカタログ (テナントのアプリカタログ) から[アプリ](../resources/teamsapp.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="1a37e-104">Remove the [app](../resources/teamsapp.md) from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="1a37e-105">組織のアプリカタログからアプリを削除するには、 `organization` teamsCatalogApp リソース\*\*\*\* で、を " [](../resources/teamsapp.md) " として指定します。</span><span class="sxs-lookup"><span data-stu-id="1a37e-105">To remove your app from your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a37e-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1a37e-106">Permissions</span></span>

<span data-ttu-id="1a37e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1a37e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="1a37e-109">**注:** この API は、グローバル管理者のみが呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="1a37e-109">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="1a37e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1a37e-110">Permission Type</span></span>                        | <span data-ttu-id="1a37e-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1a37e-111">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="1a37e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1a37e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="1a37e-113">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a37e-113">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="1a37e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1a37e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a37e-115">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="1a37e-115">Not supported</span></span>|
| <span data-ttu-id="1a37e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1a37e-116">Application</span></span>                            | <span data-ttu-id="1a37e-117">非サポート</span><span class="sxs-lookup"><span data-stu-id="1a37e-117">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a37e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1a37e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1a37e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1a37e-119">Request headers</span></span>

| <span data-ttu-id="1a37e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1a37e-120">Header</span></span>        | <span data-ttu-id="1a37e-121">値</span><span class="sxs-lookup"><span data-stu-id="1a37e-121">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="1a37e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a37e-122">Authorization</span></span> | <span data-ttu-id="1a37e-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1a37e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1a37e-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="1a37e-125">Request body</span></span>

<span data-ttu-id="1a37e-126">なし。</span><span class="sxs-lookup"><span data-stu-id="1a37e-126">None.</span></span>

><span data-ttu-id="1a37e-127">**注:** の[発行済みアプリの一覧](./teamsapp-list.md)から返された ID を使用して、更新するアプリを参照します。</span><span class="sxs-lookup"><span data-stu-id="1a37e-127">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="1a37e-128">Zip アプリパッケージのマニフェストからの ID は使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="1a37e-128">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="1a37e-129">応答</span><span class="sxs-lookup"><span data-stu-id="1a37e-129">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="1a37e-130">例</span><span class="sxs-lookup"><span data-stu-id="1a37e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a37e-131">要求</span><span class="sxs-lookup"><span data-stu-id="1a37e-131">Request</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```

### <a name="response"></a><span data-ttu-id="1a37e-132">応答</span><span class="sxs-lookup"><span data-stu-id="1a37e-132">Response</span></span>

```http
HTTP/1.1 204 No Content
```
