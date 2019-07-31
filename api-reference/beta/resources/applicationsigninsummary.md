---
title: applicationSignInDetailedSummary リソースの種類
description: アプリケーションサインインの概要を表します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType_
ms.openlocfilehash: d169755679cd60285808c1c93cb31810b1d1939d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013340"
---
# <a name="applicationsigninsummary-resource-type"></a><span data-ttu-id="da50d-103">applicationSignInSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="da50d-103">applicationSignInSummary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da50d-104">アプリケーションサインインの概要を表します。</span><span class="sxs-lookup"><span data-stu-id="da50d-104">Represents an application sign-in summary.</span></span>

## <a name="methods"></a><span data-ttu-id="da50d-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="da50d-105">Methods</span></span>

| <span data-ttu-id="da50d-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="da50d-106">Method</span></span>       | <span data-ttu-id="da50d-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="da50d-107">Return Type</span></span> | <span data-ttu-id="da50d-108">説明</span><span class="sxs-lookup"><span data-stu-id="da50d-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="da50d-109">ApplicationSignInSummary を取得する</span><span class="sxs-lookup"><span data-stu-id="da50d-109">Get applicationSignInSummary</span></span>](../api/applicationsigninsummary-get.md) | [<span data-ttu-id="da50d-110">applicationSignInSummary</span><span class="sxs-lookup"><span data-stu-id="da50d-110">applicationSignInSummary</span></span>](applicationsigninsummary.md) | <span data-ttu-id="da50d-111">**ApplicationSignInSummary**オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="da50d-111">Read the properties and relationships of an **applicationSignInSummary** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="da50d-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="da50d-112">Properties</span></span>
| <span data-ttu-id="da50d-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="da50d-113">Property</span></span>     | <span data-ttu-id="da50d-114">型</span><span class="sxs-lookup"><span data-stu-id="da50d-114">Type</span></span>        | <span data-ttu-id="da50d-115">説明</span><span class="sxs-lookup"><span data-stu-id="da50d-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="da50d-116">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="da50d-116">appDisplayName</span></span>|<span data-ttu-id="da50d-117">String</span><span class="sxs-lookup"><span data-stu-id="da50d-117">String</span></span>|<span data-ttu-id="da50d-118">ユーザーがサインインしたアプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="da50d-118">Name of the application that the user signed in to.</span></span>|
|<span data-ttu-id="da50d-119">appId</span><span class="sxs-lookup"><span data-stu-id="da50d-119">appId</span></span>|<span data-ttu-id="da50d-120">String</span><span class="sxs-lookup"><span data-stu-id="da50d-120">String</span></span>|  <span data-ttu-id="da50d-121">ユーザーがサインアウトしたアプリケーションの ID。</span><span class="sxs-lookup"><span data-stu-id="da50d-121">ID of the application that the user signed i nto.</span></span>|
|<span data-ttu-id="da50d-122">failedSignInCount</span><span class="sxs-lookup"><span data-stu-id="da50d-122">failedSignInCount</span></span>|<span data-ttu-id="da50d-123">Int64</span><span class="sxs-lookup"><span data-stu-id="da50d-123">Int64</span></span>|<span data-ttu-id="da50d-124">アプリケーションによって実行された、失敗したサインインの数。</span><span class="sxs-lookup"><span data-stu-id="da50d-124">Count of failed sign-ins made by the application.</span></span>|
|<span data-ttu-id="da50d-125">successPercentage</span><span class="sxs-lookup"><span data-stu-id="da50d-125">successPercentage</span></span>|<span data-ttu-id="da50d-126">Int32</span><span class="sxs-lookup"><span data-stu-id="da50d-126">Int32</span></span>|<span data-ttu-id="da50d-127">アプリケーションによって行われたサインインの成功率。</span><span class="sxs-lookup"><span data-stu-id="da50d-127">Percentage of successful sign-ins made by the application.</span></span>|
|<span data-ttu-id="da50d-128">successfulSignInCount</span><span class="sxs-lookup"><span data-stu-id="da50d-128">successfulSignInCount</span></span>|<span data-ttu-id="da50d-129">Int64</span><span class="sxs-lookup"><span data-stu-id="da50d-129">Int64</span></span>|<span data-ttu-id="da50d-130">アプリケーションによって作成された成功したサインインの数。</span><span class="sxs-lookup"><span data-stu-id="da50d-130">Count of successful sign-ins made by the application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="da50d-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="da50d-131">Relationships</span></span>
<span data-ttu-id="da50d-132">なし</span><span class="sxs-lookup"><span data-stu-id="da50d-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="da50d-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="da50d-133">JSON representation</span></span>

<span data-ttu-id="da50d-134">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="da50d-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationSignInSummary"
}-->

```json
{
  "appDisplayName": "String",
  "appId": "String (identifier)",
  "failedSignInCount": 1024,
  "successPercentage": 1024,
  "successfulSignInCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationSignInSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
