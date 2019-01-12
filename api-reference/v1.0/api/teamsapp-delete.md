---
title: アクセス許可
description: '組織のアプリケーション カタログ (テナント アプリケーション カタログ) からアプリケーションを削除します。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 58984044ea59bd38f0232bfa9407c01f97f22708
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943607"
---
# <a name="remove-an-app-from-your-organizations-app-catalog"></a><span data-ttu-id="32d52-103">組織のアプリケーションのカタログからアプリケーションを削除します。</span><span class="sxs-lookup"><span data-stu-id="32d52-103">Remove an app from your organization's app catalog</span></span>



<span data-ttu-id="32d52-104">組織のアプリケーション カタログ (テナント アプリケーション カタログ) から[アプリケーション](../resources/teamsapp.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="32d52-104">Remove the [app](../resources/teamsapp.md) from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="32d52-105">組織のアプリケーションのカタログからアプリケーションを削除するのには次のように指定します。 `organization` [teamsCatalogApp](../resources/teamsapp.md)リソースで**distributionMethod**とします。</span><span class="sxs-lookup"><span data-stu-id="32d52-105">To remove your app from your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="32d52-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="32d52-106">Permissions</span></span>

<span data-ttu-id="32d52-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="32d52-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="32d52-109">**注:** グローバル管理者だけでは、この API を呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="32d52-109">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="32d52-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="32d52-110">Permission Type</span></span>                        | <span data-ttu-id="32d52-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="32d52-111">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="32d52-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="32d52-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="32d52-113">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32d52-113">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="32d52-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="32d52-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32d52-115">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="32d52-115">Not supported</span></span>|
| <span data-ttu-id="32d52-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="32d52-116">Application</span></span>                            | <span data-ttu-id="32d52-117">非サポート</span><span class="sxs-lookup"><span data-stu-id="32d52-117">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="32d52-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="32d52-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="32d52-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="32d52-119">Request headers</span></span>

| <span data-ttu-id="32d52-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="32d52-120">Header</span></span>        | <span data-ttu-id="32d52-121">値</span><span class="sxs-lookup"><span data-stu-id="32d52-121">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="32d52-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="32d52-122">Authorization</span></span> | <span data-ttu-id="32d52-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="32d52-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="32d52-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="32d52-125">Request body</span></span>

<span data-ttu-id="32d52-126">なし。</span><span class="sxs-lookup"><span data-stu-id="32d52-126">None.</span></span>

><span data-ttu-id="32d52-127">**注:** 更新するにはアプリケーションを参照するための[リストには、アプリケーションが公開されて](./teamsapp-list.md)呼び出しから返された ID を使用します。</span><span class="sxs-lookup"><span data-stu-id="32d52-127">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="32d52-128">Zip アプリケーション パッケージのマニフェストの ID を使用しません。</span><span class="sxs-lookup"><span data-stu-id="32d52-128">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="32d52-129">応答</span><span class="sxs-lookup"><span data-stu-id="32d52-129">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="32d52-130">例</span><span class="sxs-lookup"><span data-stu-id="32d52-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="32d52-131">要求</span><span class="sxs-lookup"><span data-stu-id="32d52-131">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```

### <a name="response"></a><span data-ttu-id="32d52-132">応答</span><span class="sxs-lookup"><span data-stu-id="32d52-132">Response</span></span>

```http
HTTP/1.1 204 No Content
```
