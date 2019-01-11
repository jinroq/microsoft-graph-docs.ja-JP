---
title: マイクロソフト チーム アプリケーション カタログから公開されているアプリケーションを一覧表示します。
description: 'マイクロソフト チーム アプリケーション カタログからアプリケーションを一覧表示します。 '
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 4cd3d8d66caa384a064711987f4fcd7473083089
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863456"
---
# <a name="list-the-published-apps-from-the-microsoft-teams-app-catalog"></a><span data-ttu-id="4a79d-103">マイクロソフト チーム アプリケーション カタログから公開されているアプリケーションを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="4a79d-103">List the published apps from the Microsoft Teams app catalog</span></span>

> <span data-ttu-id="4a79d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4a79d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4a79d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a79d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4a79d-106">マイクロソフト チーム アプリケーション カタログから[アプリケーション](../resources/teamsapp.md)を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="4a79d-106">List [apps](../resources/teamsapp.md) from the Microsoft Teams app catalog.</span></span> <span data-ttu-id="4a79d-107">これには、組織のアプリケーション カタログ (テナント アプリケーション カタログ) からアプリケーションと同様に、マイクロソフトのチーム ・ ストアからのアプリが含まれます。</span><span class="sxs-lookup"><span data-stu-id="4a79d-107">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="4a79d-108">組織のアプリケーションのカタログのみからアプリケーションを取得するのには次のように指定します。 `Organization` [teamsCatalogApp](../resources/teamsapp.md)リソースで**distributionMethod**とします。</span><span class="sxs-lookup"><span data-stu-id="4a79d-108">To get apps from your organization's app catalog only, specify `Organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a79d-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4a79d-109">Permissions</span></span>

<span data-ttu-id="4a79d-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4a79d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="4a79d-112">**注:** グローバル管理者だけでは、この API を呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="4a79d-112">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="4a79d-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4a79d-113">Permission Type</span></span>                        | <span data-ttu-id="4a79d-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4a79d-114">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="4a79d-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4a79d-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="4a79d-116">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a79d-116">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="4a79d-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4a79d-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a79d-118">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="4a79d-118">Not supported</span></span>|
| <span data-ttu-id="4a79d-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4a79d-119">Application</span></span>                            | <span data-ttu-id="4a79d-120">非サポート</span><span class="sxs-lookup"><span data-stu-id="4a79d-120">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a79d-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4a79d-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4a79d-122">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="4a79d-122">Optional query parameters</span></span>
<span data-ttu-id="4a79d-123">このメソッドは、$filter、$select をサポートしていて、$ は、応答をカスタマイズするために[OData クエリ パラメーター](/graph/query-parameters)を展開します。</span><span class="sxs-lookup"><span data-stu-id="4a79d-123">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4a79d-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4a79d-124">Request headers</span></span>

| <span data-ttu-id="4a79d-125">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4a79d-125">Header</span></span>        | <span data-ttu-id="4a79d-126">値</span><span class="sxs-lookup"><span data-stu-id="4a79d-126">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="4a79d-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a79d-127">Authorization</span></span> | <span data-ttu-id="4a79d-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4a79d-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4a79d-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="4a79d-130">Request body</span></span>
<span data-ttu-id="4a79d-131">なし。</span><span class="sxs-lookup"><span data-stu-id="4a79d-131">None.</span></span>

><span data-ttu-id="4a79d-132">**注:** 任意の結果の一覧を短縮するための[teamsCatalogApp](../resources/teamsapp.md)オブジェクトのフィールドをフィルターできます。</span><span class="sxs-lookup"><span data-stu-id="4a79d-132">**Note:** You can filter on any of the fields of the [teamsCatalogApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="4a79d-133">次のフィルター操作のいずれかを使用することができます: 等しい、等しくない、またはではなく。</span><span class="sxs-lookup"><span data-stu-id="4a79d-133">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="response"></a><span data-ttu-id="4a79d-134">応答</span><span class="sxs-lookup"><span data-stu-id="4a79d-134">Response</span></span>
<span data-ttu-id="4a79d-135">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[teamsCatalogApp](../resources/teamsapp.md)オブジェクトの一覧です。</span><span class="sxs-lookup"><span data-stu-id="4a79d-135">If successful, this method returns a `200 OK` response code and a list of [teamsCatalogApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4a79d-136">例</span><span class="sxs-lookup"><span data-stu-id="4a79d-136">Examples</span></span>
### <a name="example-1"></a><span data-ttu-id="4a79d-137">例 1</span><span class="sxs-lookup"><span data-stu-id="4a79d-137">Example 1</span></span>
<span data-ttu-id="4a79d-138">次の例では、テナントに固有のすべてのアプリケーションが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="4a79d-138">The following example lists all applications that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="4a79d-139">要求</span><span class="sxs-lookup"><span data-stu-id="4a79d-139">Request</span></span>
```
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```

#### <a name="response"></a><span data-ttu-id="4a79d-140">応答</span><span class="sxs-lookup"><span data-stu-id="4a79d-140">Response</span></span>
```
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod":"Organization"
    }
  ]
}
```

### <a name="example-2"></a><span data-ttu-id="4a79d-141">例 2</span><span class="sxs-lookup"><span data-stu-id="4a79d-141">Example 2</span></span>

<span data-ttu-id="4a79d-142">次の使用例は指定された ID を使用してアプリケーションを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="4a79d-142">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="4a79d-143">要求</span><span class="sxs-lookup"><span data-stu-id="4a79d-143">Request</span></span>
```
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a><span data-ttu-id="4a79d-144">応答</span><span class="sxs-lookup"><span data-stu-id="4a79d-144">Response</span></span>
```
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod":"Organization"
    }
  ]
}
```

