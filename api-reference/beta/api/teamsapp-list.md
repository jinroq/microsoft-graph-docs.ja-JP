---
title: Microsoft Teams アプリカタログから発行されたアプリを一覧表示する
description: 'Microsoft Teams アプリカタログのアプリを一覧表示します。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 229d91768f222a6bfc4bbf0de726a2f6d40c0da4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33330131"
---
# <a name="list-the-published-apps-from-the-microsoft-teams-app-catalog"></a><span data-ttu-id="1e440-103">Microsoft Teams アプリカタログから発行されたアプリを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1e440-103">List the published apps from the Microsoft Teams app catalog</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e440-104">Microsoft Teams アプリカタログの[アプリ](../resources/teamsapp.md)を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="1e440-104">List [apps](../resources/teamsapp.md) from the Microsoft Teams app catalog.</span></span>
<span data-ttu-id="1e440-105">これには、Microsoft Teams ストアからのアプリや、組織のアプリカタログ (テナントのアプリカタログ) からのアプリが含まれます。</span><span class="sxs-lookup"><span data-stu-id="1e440-105">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="1e440-106">組織のアプリカタログからアプリのみを取得するには`Organization` 、 [teamsCatalogApp](../resources/teamsapp.md)リソースの "の" として、を指定します。 \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="1e440-106">To get apps from your organization's app catalog only, specify `Organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e440-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1e440-107">Permissions</span></span>

<span data-ttu-id="1e440-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions_reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1e440-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

> <span data-ttu-id="1e440-110">**注:** この API は、グローバル管理者のみが呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="1e440-110">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="1e440-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1e440-111">Permission Type</span></span>                        | <span data-ttu-id="1e440-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1e440-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="1e440-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1e440-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="1e440-114">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e440-114">AppCatalog.ReadWrite.All</span></span>            |
| <span data-ttu-id="1e440-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1e440-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e440-116">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="1e440-116">Not supported</span></span>                       |
| <span data-ttu-id="1e440-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1e440-117">Application</span></span>                            | <span data-ttu-id="1e440-118">非サポート</span><span class="sxs-lookup"><span data-stu-id="1e440-118">Not supported</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="1e440-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1e440-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1e440-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="1e440-120">Optional query parameters</span></span>

<span data-ttu-id="1e440-121">このメソッドは、応答をカスタマイズするための $filter、$select、および $expand [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="1e440-121">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1e440-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1e440-122">Request headers</span></span>

| <span data-ttu-id="1e440-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1e440-123">Header</span></span>        | <span data-ttu-id="1e440-124">値</span><span class="sxs-lookup"><span data-stu-id="1e440-124">Value</span></span>                     |
|:--------------|:--------------------------|
| <span data-ttu-id="1e440-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e440-125">Authorization</span></span> | <span data-ttu-id="1e440-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1e440-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e440-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="1e440-128">Request body</span></span>

<span data-ttu-id="1e440-129">なし。</span><span class="sxs-lookup"><span data-stu-id="1e440-129">None.</span></span>

> <span data-ttu-id="1e440-130">**注:**[teamsCatalogApp](../resources/teamsapp.md)オブジェクトの任意のフィールドでフィルター処理して、結果の一覧を短縮できます。</span><span class="sxs-lookup"><span data-stu-id="1e440-130">**Note:** You can filter on any of the fields of the [teamsCatalogApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="1e440-131">次のいずれかのフィルター操作を使用できます: equal、not equal、and、or not。</span><span class="sxs-lookup"><span data-stu-id="1e440-131">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="response"></a><span data-ttu-id="1e440-132">応答</span><span class="sxs-lookup"><span data-stu-id="1e440-132">Response</span></span>

<span data-ttu-id="1e440-133">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[teamsCatalogApp](../resources/teamsapp.md)オブジェクトのリストを返します。</span><span class="sxs-lookup"><span data-stu-id="1e440-133">If successful, this method returns a `200 OK` response code and a list of [teamsCatalogApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1e440-134">例</span><span class="sxs-lookup"><span data-stu-id="1e440-134">Examples</span></span>

### <a name="example-1-list-all-applications"></a><span data-ttu-id="1e440-135">例 1: すべてのアプリケーションを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1e440-135">Example 1: List all applications</span></span>

<span data-ttu-id="1e440-136">次の例では、テナント固有のすべてのアプリケーションを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="1e440-136">The following example lists all applications that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="1e440-137">要求</span><span class="sxs-lookup"><span data-stu-id="1e440-137">Request</span></span>

```http
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="1e440-138">応答</span><span class="sxs-lookup"><span data-stu-id="1e440-138">Response</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod": "Organization"
    }
  ]
}
```

### <a name="example-2-list-applications-with-a-given-id"></a><span data-ttu-id="1e440-139">例 2: 指定された ID を持つアプリケーションを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1e440-139">Example 2: List applications with a given ID</span></span>

<span data-ttu-id="1e440-140">次の例では、指定された ID を持つアプリケーションを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="1e440-140">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="1e440-141">要求</span><span class="sxs-lookup"><span data-stu-id="1e440-141">Request</span></span>

```http
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a><span data-ttu-id="1e440-142">応答</span><span class="sxs-lookup"><span data-stu-id="1e440-142">Response</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod": "Organization"
    }
  ]
}
```

