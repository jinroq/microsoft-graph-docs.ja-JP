---
title: iPv4Range リソースの種類
description: IP V4 範囲
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 57bcaabfc5155e6b6733de2dc228dd240515281b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980182"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="f10bc-103">iPv4Range リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f10bc-103">iPv4Range resource type</span></span>

> <span data-ttu-id="f10bc-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f10bc-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f10bc-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f10bc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f10bc-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f10bc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f10bc-107">IP V4 範囲</span><span class="sxs-lookup"><span data-stu-id="f10bc-107">IP V4 range</span></span>

<span data-ttu-id="f10bc-108">[ipRange](../resources/intune-shared-iprange.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="f10bc-108">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f10bc-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f10bc-109">Properties</span></span>
|<span data-ttu-id="f10bc-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f10bc-110">Property</span></span>|<span data-ttu-id="f10bc-111">種類</span><span class="sxs-lookup"><span data-stu-id="f10bc-111">Type</span></span>|<span data-ttu-id="f10bc-112">説明</span><span class="sxs-lookup"><span data-stu-id="f10bc-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f10bc-113">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="f10bc-113">lowerAddress</span></span>|<span data-ttu-id="f10bc-114">文字列</span><span class="sxs-lookup"><span data-stu-id="f10bc-114">String</span></span>|<span data-ttu-id="f10bc-115">低い番号の IP アドレス</span><span class="sxs-lookup"><span data-stu-id="f10bc-115">Lower IP Address</span></span>|
|<span data-ttu-id="f10bc-116">upperAddress</span><span class="sxs-lookup"><span data-stu-id="f10bc-116">upperAddress</span></span>|<span data-ttu-id="f10bc-117">文字列</span><span class="sxs-lookup"><span data-stu-id="f10bc-117">String</span></span>|<span data-ttu-id="f10bc-118">高い番号の IP アドレス</span><span class="sxs-lookup"><span data-stu-id="f10bc-118">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="f10bc-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f10bc-119">Relationships</span></span>
<span data-ttu-id="f10bc-120">なし</span><span class="sxs-lookup"><span data-stu-id="f10bc-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f10bc-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f10bc-121">JSON Representation</span></span>
<span data-ttu-id="f10bc-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f10bc-122">Here is a JSON representation of the resource.</span></span>
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



