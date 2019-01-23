---
title: iPv4Range リソースの種類
description: Intune は、複数のワークフローをサポートする Microsoft グラフ API の iPv4Range リソースについて説明します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9ac2656b7c79cceba70879fe478aec65a5bd7250
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425226"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="a177f-103">iPv4Range リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a177f-103">iPv4Range resource type</span></span>

> <span data-ttu-id="a177f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a177f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a177f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a177f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a177f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a177f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a177f-107">IP V4 範囲</span><span class="sxs-lookup"><span data-stu-id="a177f-107">IP V4 range</span></span>

<span data-ttu-id="a177f-108">[ipRange](../resources/intune-shared-iprange.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="a177f-108">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a177f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a177f-109">Properties</span></span>
|<span data-ttu-id="a177f-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a177f-110">Property</span></span>|<span data-ttu-id="a177f-111">型</span><span class="sxs-lookup"><span data-stu-id="a177f-111">Type</span></span>|<span data-ttu-id="a177f-112">説明</span><span class="sxs-lookup"><span data-stu-id="a177f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a177f-113">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="a177f-113">lowerAddress</span></span>|<span data-ttu-id="a177f-114">文字列</span><span class="sxs-lookup"><span data-stu-id="a177f-114">String</span></span>|<span data-ttu-id="a177f-115">低い番号の IP アドレス</span><span class="sxs-lookup"><span data-stu-id="a177f-115">Lower IP Address</span></span>|
|<span data-ttu-id="a177f-116">upperAddress</span><span class="sxs-lookup"><span data-stu-id="a177f-116">upperAddress</span></span>|<span data-ttu-id="a177f-117">文字列</span><span class="sxs-lookup"><span data-stu-id="a177f-117">String</span></span>|<span data-ttu-id="a177f-118">高い番号の IP アドレス</span><span class="sxs-lookup"><span data-stu-id="a177f-118">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="a177f-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a177f-119">Relationships</span></span>
<span data-ttu-id="a177f-120">なし</span><span class="sxs-lookup"><span data-stu-id="a177f-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a177f-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a177f-121">JSON Representation</span></span>
<span data-ttu-id="a177f-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a177f-122">Here is a JSON representation of the resource.</span></span>
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



