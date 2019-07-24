---
title: PublishedResource の更新
description: '[Publishedresource](../resources/publishedresource.md)オブジェクトのプロパティを更新します。'
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3e0492116ad0d012846fe1ac531ddcbf4bb77b95
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840983"
---
# <a name="update-publishedresource"></a><span data-ttu-id="b8188-103">PublishedResource の更新</span><span class="sxs-lookup"><span data-stu-id="b8188-103">Update publishedResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8188-104">Publishedresource [Publishedresource](../resources/publishedresource.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b8188-104">Update the properties of publishedresource  [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8188-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b8188-105">Permissions</span></span>

<span data-ttu-id="b8188-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b8188-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b8188-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b8188-108">Permission type</span></span>                        | <span data-ttu-id="b8188-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b8188-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="b8188-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b8188-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b8188-111">OnPremisesPublishingProfiles</span><span class="sxs-lookup"><span data-stu-id="b8188-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="b8188-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b8188-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8188-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b8188-113">Not supported.</span></span> |
| <span data-ttu-id="b8188-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b8188-114">Application</span></span>                            | <span data-ttu-id="b8188-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b8188-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8188-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b8188-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}
```

## <a name="request-headers"></a><span data-ttu-id="b8188-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b8188-117">Request headers</span></span>

| <span data-ttu-id="b8188-118">名前</span><span class="sxs-lookup"><span data-stu-id="b8188-118">Name</span></span>       | <span data-ttu-id="b8188-119">説明</span><span class="sxs-lookup"><span data-stu-id="b8188-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b8188-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8188-120">Authorization</span></span> | <span data-ttu-id="b8188-121">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="b8188-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8188-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="b8188-122">Request body</span></span>

<span data-ttu-id="b8188-123">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="b8188-123">In the request body, supply the values for relevant fields to update.</span></span> <span data-ttu-id="b8188-124">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="b8188-124">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b8188-125">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="b8188-125">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="b8188-126">次の表に、更新できるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b8188-126">The following table lists the properties that can be updated.</span></span>

| <span data-ttu-id="b8188-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b8188-127">Property</span></span>     | <span data-ttu-id="b8188-128">型</span><span class="sxs-lookup"><span data-stu-id="b8188-128">Type</span></span>        | <span data-ttu-id="b8188-129">説明</span><span class="sxs-lookup"><span data-stu-id="b8188-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b8188-130">displayName</span><span class="sxs-lookup"><span data-stu-id="b8188-130">displayName</span></span>|<span data-ttu-id="b8188-131">String</span><span class="sxs-lookup"><span data-stu-id="b8188-131">String</span></span>|<span data-ttu-id="b8188-132">オンプレミスで発行されたリソース名を表します。</span><span class="sxs-lookup"><span data-stu-id="b8188-132">Represents an on-premises published resource name.</span></span>|

## <a name="response"></a><span data-ttu-id="b8188-133">応答</span><span class="sxs-lookup"><span data-stu-id="b8188-133">Response</span></span>

<span data-ttu-id="b8188-134">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="b8188-134">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b8188-135">例</span><span class="sxs-lookup"><span data-stu-id="b8188-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b8188-136">要求</span><span class="sxs-lookup"><span data-stu-id="b8188-136">Request</span></span>

<span data-ttu-id="b8188-137">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b8188-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_publishedresource"
}-->

```http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/1234b780-965f-4149-85c5-a8c73e58b67d

{
    "displayName": "Demo provisioning (updated)"
}
```

### <a name="response"></a><span data-ttu-id="b8188-138">応答</span><span class="sxs-lookup"><span data-stu-id="b8188-138">Response</span></span>

<span data-ttu-id="b8188-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b8188-139">The following is an example of the response.</span></span>

> <span data-ttu-id="b8188-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b8188-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.publishedResource"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update publishedresource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->