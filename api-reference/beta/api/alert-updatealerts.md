---
title: '通知: updatealerts'
description: 複数の要求ではなく1つの要求で複数の通知を更新します。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: ad43cf3488ff0661a4b22130ae8728a00c3ea17d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322731"
---
# <a name="alert-updatealerts"></a><span data-ttu-id="5eca6-103">通知: updatealerts</span><span class="sxs-lookup"><span data-stu-id="5eca6-103">alert: updateAlerts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5eca6-104">複数の要求ではなく1つの要求で複数の通知を更新します。</span><span class="sxs-lookup"><span data-stu-id="5eca6-104">Update multiple alerts in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="5eca6-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5eca6-105">Permissions</span></span>

<span data-ttu-id="5eca6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5eca6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5eca6-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5eca6-108">Permission type</span></span>                        | <span data-ttu-id="5eca6-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5eca6-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="5eca6-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5eca6-110">Delegated (work or school account)</span></span> |   <span data-ttu-id="5eca6-111">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5eca6-111">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="5eca6-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5eca6-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5eca6-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5eca6-113">Not supported.</span></span>  |
|<span data-ttu-id="5eca6-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5eca6-114">Application</span></span> | <span data-ttu-id="5eca6-115">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5eca6-115">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5eca6-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5eca6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/alerts/updateAlerts
```

## <a name="request-headers"></a><span data-ttu-id="5eca6-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5eca6-117">Request headers</span></span>

| <span data-ttu-id="5eca6-118">名前</span><span class="sxs-lookup"><span data-stu-id="5eca6-118">Name</span></span>          | <span data-ttu-id="5eca6-119">説明</span><span class="sxs-lookup"><span data-stu-id="5eca6-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="5eca6-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="5eca6-120">Authorization</span></span> | <span data-ttu-id="5eca6-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="5eca6-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="5eca6-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="5eca6-122">Request body</span></span>

<span data-ttu-id="5eca6-123">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="5eca6-123">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="5eca6-124">各エンティティには、 **id**プロパティと**vendorInformation**プロパティが必要です。</span><span class="sxs-lookup"><span data-stu-id="5eca6-124">Each entity must have **id** and **vendorInformation** properties.</span></span> <span data-ttu-id="5eca6-125">更新できるプロパティの詳細については、「 [update alert](alert-update.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5eca6-125">For details about properties that can be updated, see [update alert](alert-update.md).</span></span>

| <span data-ttu-id="5eca6-126">パラメーター</span><span class="sxs-lookup"><span data-stu-id="5eca6-126">Parameter</span></span>    | <span data-ttu-id="5eca6-127">型</span><span class="sxs-lookup"><span data-stu-id="5eca6-127">Type</span></span>        | <span data-ttu-id="5eca6-128">説明</span><span class="sxs-lookup"><span data-stu-id="5eca6-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5eca6-129">value</span><span class="sxs-lookup"><span data-stu-id="5eca6-129">value</span></span>|<span data-ttu-id="5eca6-130">[alert](../resources/alert.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="5eca6-130">[alert](../resources/alert.md) collection</span></span>| <span data-ttu-id="5eca6-131">更新する通知のコレクション。</span><span class="sxs-lookup"><span data-stu-id="5eca6-131">Collection of alerts to update.</span></span> <span data-ttu-id="5eca6-132">各エンティティには、更新する**id**、 **vendorInformation**、およびその他の編集可能なプロパティが必要です。</span><span class="sxs-lookup"><span data-stu-id="5eca6-132">Each entity must have **id**, **vendorInformation**, and other editable properties to be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="5eca6-133">応答</span><span class="sxs-lookup"><span data-stu-id="5eca6-133">Response</span></span>

<span data-ttu-id="5eca6-134">成功した場合、この`200, OK`メソッドは応答コードと、応答本文で[通知](../resources/alert.md)コレクションオブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5eca6-134">If successful, this method returns `200, OK` response code and [alert](../resources/alert.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5eca6-135">例</span><span class="sxs-lookup"><span data-stu-id="5eca6-135">Examples</span></span>

<span data-ttu-id="5eca6-136">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="5eca6-136">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="5eca6-137">要求</span><span class="sxs-lookup"><span data-stu-id="5eca6-137">Request</span></span>

<span data-ttu-id="5eca6-138">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5eca6-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "alert_updatealerts",
   "isCollection": "true"
}-->

```http
POST https://graph.microsoft.com/beta/security/alerts/updateAlerts
Content-type: application/json

{
  "value": [
    {
      "assignedTo": "String",
      "closedDateTime": "String (timestamp)",
      "comments": ["String"],
      "feedback": {"@odata.type": "microsoft.graph.alertFeedback"},
      "id": "String (identifier)",
      "status": {"@odata.type": "microsoft.graph.alertStatus"},
      "tags": ["String"],
      "vendorInformation":
        {
          "provider": "String",
          "vendor": "String"
        }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="5eca6-139">応答</span><span class="sxs-lookup"><span data-stu-id="5eca6-139">Response</span></span>

<span data-ttu-id="5eca6-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5eca6-140">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="5eca6-141">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="5eca6-141">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5eca6-142">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="5eca6-142">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "activityGroupName": "activityGroupName-value",
      "assignedTo": "assignedTo-value",
      "azureSubscriptionId": "azureSubscriptionId-value",
      "azureTenantId": "azureTenantId-value",
      "category": "category-value",
      "closedDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alert: updateAlerts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
