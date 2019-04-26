---
title: applicationSignInDetailedSummary リソースの種類
description: アプリケーションサインインの概要を表します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0329aec304602151a23ff389bc041247f9fb65b7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339071"
---
# <a name="applicationsigninsummary-resource-type"></a><span data-ttu-id="184d8-103">applicationSignInSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="184d8-103">applicationSignInSummary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="184d8-104">アプリケーションサインインの概要を表します。</span><span class="sxs-lookup"><span data-stu-id="184d8-104">Represents an application sign-in summary.</span></span>

## <a name="methods"></a><span data-ttu-id="184d8-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="184d8-105">Methods</span></span>

| <span data-ttu-id="184d8-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="184d8-106">Method</span></span>       | <span data-ttu-id="184d8-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="184d8-107">Return Type</span></span> | <span data-ttu-id="184d8-108">説明</span><span class="sxs-lookup"><span data-stu-id="184d8-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="184d8-109">applicationSignInSummary を取得する</span><span class="sxs-lookup"><span data-stu-id="184d8-109">Get applicationSignInSummary</span></span>](../api/applicationsigninsummary-get.md) | [<span data-ttu-id="184d8-110">applicationSignInSummary</span><span class="sxs-lookup"><span data-stu-id="184d8-110">applicationSignInSummary</span></span>](applicationsigninsummary.md) | <span data-ttu-id="184d8-111">**applicationSignInSummary**オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="184d8-111">Read the properties and relationships of an **applicationSignInSummary** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="184d8-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="184d8-112">Properties</span></span>
| <span data-ttu-id="184d8-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="184d8-113">Property</span></span>     | <span data-ttu-id="184d8-114">型</span><span class="sxs-lookup"><span data-stu-id="184d8-114">Type</span></span>        | <span data-ttu-id="184d8-115">説明</span><span class="sxs-lookup"><span data-stu-id="184d8-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="184d8-116">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="184d8-116">appDisplayName</span></span>|<span data-ttu-id="184d8-117">String</span><span class="sxs-lookup"><span data-stu-id="184d8-117">String</span></span>|<span data-ttu-id="184d8-118">ユーザーがサインインしたアプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="184d8-118">Name of the application that the user signed in to.</span></span>|
|<span data-ttu-id="184d8-119">appId</span><span class="sxs-lookup"><span data-stu-id="184d8-119">appId</span></span>|<span data-ttu-id="184d8-120">String</span><span class="sxs-lookup"><span data-stu-id="184d8-120">String</span></span>|  <span data-ttu-id="184d8-121">ユーザーがサインアウトしたアプリケーションの ID。</span><span class="sxs-lookup"><span data-stu-id="184d8-121">ID of the application that the user signed i nto.</span></span>|
|<span data-ttu-id="184d8-122">failedSignInCount</span><span class="sxs-lookup"><span data-stu-id="184d8-122">failedSignInCount</span></span>|<span data-ttu-id="184d8-123">Int64</span><span class="sxs-lookup"><span data-stu-id="184d8-123">Int64</span></span>|<span data-ttu-id="184d8-124">アプリケーションによって実行された、失敗したサインインの数。</span><span class="sxs-lookup"><span data-stu-id="184d8-124">Count of failed sign-ins made by the application.</span></span>|
|<span data-ttu-id="184d8-125">successPercentage</span><span class="sxs-lookup"><span data-stu-id="184d8-125">successPercentage</span></span>|<span data-ttu-id="184d8-126">Int32</span><span class="sxs-lookup"><span data-stu-id="184d8-126">Int32</span></span>|<span data-ttu-id="184d8-127">アプリケーションによって行われたサインインの成功率。</span><span class="sxs-lookup"><span data-stu-id="184d8-127">Percentage of successful sign-ins made by the application.</span></span>|
|<span data-ttu-id="184d8-128">successfulSignInCount</span><span class="sxs-lookup"><span data-stu-id="184d8-128">successfulSignInCount</span></span>|<span data-ttu-id="184d8-129">Int64</span><span class="sxs-lookup"><span data-stu-id="184d8-129">Int64</span></span>|<span data-ttu-id="184d8-130">アプリケーションによって作成された成功したサインインの数。</span><span class="sxs-lookup"><span data-stu-id="184d8-130">Count of successful sign-ins made by the application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="184d8-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="184d8-131">Relationships</span></span>
<span data-ttu-id="184d8-132">なし</span><span class="sxs-lookup"><span data-stu-id="184d8-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="184d8-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="184d8-133">JSON representation</span></span>

<span data-ttu-id="184d8-134">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="184d8-134">The following is a JSON representation of the resource.</span></span>

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
