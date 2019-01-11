---
title: iPv4Range リソースの種類
description: IP V4 範囲
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a1f76fcd99663fe7ddd34263c8304b5597e6941c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888292"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="7bb7c-103">iPv4Range リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7bb7c-103">iPv4Range resource type</span></span>

> <span data-ttu-id="7bb7c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7bb7c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7bb7c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7bb7c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7bb7c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7bb7c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7bb7c-107">IP V4 範囲</span><span class="sxs-lookup"><span data-stu-id="7bb7c-107">IP V4 range</span></span>

<span data-ttu-id="7bb7c-108">[ipRange](../resources/intune-shared-iprange.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="7bb7c-108">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7bb7c-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7bb7c-109">Properties</span></span>
|<span data-ttu-id="7bb7c-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7bb7c-110">Property</span></span>|<span data-ttu-id="7bb7c-111">種類</span><span class="sxs-lookup"><span data-stu-id="7bb7c-111">Type</span></span>|<span data-ttu-id="7bb7c-112">説明</span><span class="sxs-lookup"><span data-stu-id="7bb7c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bb7c-113">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="7bb7c-113">lowerAddress</span></span>|<span data-ttu-id="7bb7c-114">文字列</span><span class="sxs-lookup"><span data-stu-id="7bb7c-114">String</span></span>|<span data-ttu-id="7bb7c-115">低い番号の IP アドレス</span><span class="sxs-lookup"><span data-stu-id="7bb7c-115">Lower IP Address</span></span>|
|<span data-ttu-id="7bb7c-116">upperAddress</span><span class="sxs-lookup"><span data-stu-id="7bb7c-116">upperAddress</span></span>|<span data-ttu-id="7bb7c-117">文字列</span><span class="sxs-lookup"><span data-stu-id="7bb7c-117">String</span></span>|<span data-ttu-id="7bb7c-118">高い番号の IP アドレス</span><span class="sxs-lookup"><span data-stu-id="7bb7c-118">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="7bb7c-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7bb7c-119">Relationships</span></span>
<span data-ttu-id="7bb7c-120">なし</span><span class="sxs-lookup"><span data-stu-id="7bb7c-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7bb7c-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7bb7c-121">JSON Representation</span></span>
<span data-ttu-id="7bb7c-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7bb7c-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iPv4Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv4Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```



