---
title: マイクロソフト チーム アプリケーション カタログから公開されているアプリケーションを一覧表示します。
description: 'マイクロソフト チーム アプリケーション カタログからアプリケーションを一覧表示します。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 884fd932acddb1352c48e82302a6c345fadf90b7
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/13/2019
ms.locfileid: "29967313"
---
# <a name="list-the-published-apps-from-the-microsoft-teams-app-catalog"></a><span data-ttu-id="d9228-103">マイクロソフト チーム アプリケーション カタログから公開されているアプリケーションを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="d9228-103">List the published apps from the Microsoft Teams app catalog</span></span>

<span data-ttu-id="d9228-104">マイクロソフト チーム アプリケーション カタログから[アプリケーション](../resources/teamsapp.md)を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="d9228-104">List [apps](../resources/teamsapp.md) from the Microsoft Teams app catalog.</span></span>
<span data-ttu-id="d9228-105">これには、組織のアプリケーション カタログ (テナント アプリケーション カタログ) からアプリケーションと同様に、マイクロソフトのチーム ・ ストアからのアプリが含まれます。</span><span class="sxs-lookup"><span data-stu-id="d9228-105">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="d9228-106">組織のアプリケーションのカタログのみからアプリケーションを取得するのには次のように指定します。 `Organization` [teamsCatalogApp](../resources/teamsapp.md)リソースで**distributionMethod**とします。</span><span class="sxs-lookup"><span data-stu-id="d9228-106">To get apps from your organization's app catalog only, specify `Organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9228-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d9228-107">Permissions</span></span>

<span data-ttu-id="d9228-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions_reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d9228-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

> <span data-ttu-id="d9228-110">**注:** グローバル管理者だけでは、この API を呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="d9228-110">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="d9228-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d9228-111">Permission Type</span></span>                        | <span data-ttu-id="d9228-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d9228-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="d9228-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d9228-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="d9228-114">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9228-114">AppCatalog.ReadWrite.All</span></span>            |
| <span data-ttu-id="d9228-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d9228-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9228-116">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="d9228-116">Not supported</span></span>                       |
| <span data-ttu-id="d9228-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d9228-117">Application</span></span>                            | <span data-ttu-id="d9228-118">非サポート</span><span class="sxs-lookup"><span data-stu-id="d9228-118">Not supported</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="d9228-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d9228-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d9228-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d9228-120">Optional query parameters</span></span>

<span data-ttu-id="d9228-121">このメソッドは、応答をカスタマイズするための $filter、$select、および $expand [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d9228-121">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d9228-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d9228-122">Request headers</span></span>

| <span data-ttu-id="d9228-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d9228-123">Header</span></span>        | <span data-ttu-id="d9228-124">値</span><span class="sxs-lookup"><span data-stu-id="d9228-124">Value</span></span>                     |
|:--------------|:--------------------------|
| <span data-ttu-id="d9228-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9228-125">Authorization</span></span> | <span data-ttu-id="d9228-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d9228-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9228-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="d9228-128">Request body</span></span>

<span data-ttu-id="d9228-129">なし。</span><span class="sxs-lookup"><span data-stu-id="d9228-129">None.</span></span>

> <span data-ttu-id="d9228-130">**注:** 任意の結果の一覧を短縮するための[teamsCatalogApp](../resources/teamsapp.md)オブジェクトのフィールドをフィルターできます。</span><span class="sxs-lookup"><span data-stu-id="d9228-130">**Note:** You can filter on any of the fields of the [teamsCatalogApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="d9228-131">次のフィルター操作のいずれかを使用することができます: 等しい、等しくない、またはではなく。</span><span class="sxs-lookup"><span data-stu-id="d9228-131">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="response"></a><span data-ttu-id="d9228-132">応答</span><span class="sxs-lookup"><span data-stu-id="d9228-132">Response</span></span>

<span data-ttu-id="d9228-133">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[teamsCatalogApp](../resources/teamsapp.md)オブジェクトの一覧です。</span><span class="sxs-lookup"><span data-stu-id="d9228-133">If successful, this method returns a `200 OK` response code and a list of [teamsCatalogApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d9228-134">例</span><span class="sxs-lookup"><span data-stu-id="d9228-134">Examples</span></span>

### <a name="example-1-list-all-applications"></a><span data-ttu-id="d9228-135">例 1: すべてのアプリケーションを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="d9228-135">Example 1: List all applications</span></span>

<span data-ttu-id="d9228-136">次の例では、テナントに固有のすべてのアプリケーションが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="d9228-136">The following example lists all applications that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="d9228-137">要求</span><span class="sxs-lookup"><span data-stu-id="d9228-137">Request</span></span>

```http
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="d9228-138">応答</span><span class="sxs-lookup"><span data-stu-id="d9228-138">Response</span></span>

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

### <a name="example-2-list-applications-with-a-given-id"></a><span data-ttu-id="d9228-139">例 2: 特定の ID を使用してアプリケーションを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="d9228-139">Example 2: List applications with a given ID</span></span>

<span data-ttu-id="d9228-140">次の使用例は指定された ID を使用してアプリケーションを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="d9228-140">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="d9228-141">要求</span><span class="sxs-lookup"><span data-stu-id="d9228-141">Request</span></span>

```http
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a><span data-ttu-id="d9228-142">応答</span><span class="sxs-lookup"><span data-stu-id="d9228-142">Response</span></span>

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
