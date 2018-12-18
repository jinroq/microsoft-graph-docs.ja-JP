---
title: iPv4Range リソースの種類
description: IP V4 範囲
author: tfitzmac
ms.openlocfilehash: eae240d185a6cf0dc2fc7d0d83194dc9f3f6f00d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314771"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="91fd7-103">iPv4Range リソースの種類</span><span class="sxs-lookup"><span data-stu-id="91fd7-103">iPv4Range resource type</span></span>

> <span data-ttu-id="91fd7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="91fd7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91fd7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91fd7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="91fd7-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="91fd7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="91fd7-107">IP V4 範囲</span><span class="sxs-lookup"><span data-stu-id="91fd7-107">IP V4 range</span></span>

<span data-ttu-id="91fd7-108">[ipRange](../resources/intune-shared-iprange.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="91fd7-108">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="91fd7-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91fd7-109">Properties</span></span>
|<span data-ttu-id="91fd7-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91fd7-110">Property</span></span>|<span data-ttu-id="91fd7-111">種類</span><span class="sxs-lookup"><span data-stu-id="91fd7-111">Type</span></span>|<span data-ttu-id="91fd7-112">説明</span><span class="sxs-lookup"><span data-stu-id="91fd7-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91fd7-113">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="91fd7-113">lowerAddress</span></span>|<span data-ttu-id="91fd7-114">文字列</span><span class="sxs-lookup"><span data-stu-id="91fd7-114">String</span></span>|<span data-ttu-id="91fd7-115">低い番号の IP アドレス</span><span class="sxs-lookup"><span data-stu-id="91fd7-115">Lower IP Address</span></span>|
|<span data-ttu-id="91fd7-116">upperAddress</span><span class="sxs-lookup"><span data-stu-id="91fd7-116">upperAddress</span></span>|<span data-ttu-id="91fd7-117">文字列</span><span class="sxs-lookup"><span data-stu-id="91fd7-117">String</span></span>|<span data-ttu-id="91fd7-118">高い番号の IP アドレス</span><span class="sxs-lookup"><span data-stu-id="91fd7-118">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="91fd7-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="91fd7-119">Relationships</span></span>
<span data-ttu-id="91fd7-120">なし</span><span class="sxs-lookup"><span data-stu-id="91fd7-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="91fd7-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="91fd7-121">JSON Representation</span></span>
<span data-ttu-id="91fd7-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="91fd7-122">Here is a JSON representation of the resource.</span></span>
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



