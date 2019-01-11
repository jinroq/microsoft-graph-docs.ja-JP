---
title: numberRange リソースの種類
description: 番号範囲の定義です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5b428320fd66263149b6d443a15c6a0e1eee744a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845704"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="162c6-103">numberRange リソースの種類</span><span class="sxs-lookup"><span data-stu-id="162c6-103">numberRange resource type</span></span>

> <span data-ttu-id="162c6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="162c6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="162c6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="162c6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="162c6-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="162c6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="162c6-107">番号範囲の定義です。</span><span class="sxs-lookup"><span data-stu-id="162c6-107">Number Range definition.</span></span>
## <a name="properties"></a><span data-ttu-id="162c6-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="162c6-108">Properties</span></span>
|<span data-ttu-id="162c6-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="162c6-109">Property</span></span>|<span data-ttu-id="162c6-110">種類</span><span class="sxs-lookup"><span data-stu-id="162c6-110">Type</span></span>|<span data-ttu-id="162c6-111">説明</span><span class="sxs-lookup"><span data-stu-id="162c6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="162c6-112">lowerNumber</span><span class="sxs-lookup"><span data-stu-id="162c6-112">lowerNumber</span></span>|<span data-ttu-id="162c6-113">Int32</span><span class="sxs-lookup"><span data-stu-id="162c6-113">Int32</span></span>|<span data-ttu-id="162c6-114">下の数です。</span><span class="sxs-lookup"><span data-stu-id="162c6-114">Lower number.</span></span>|
|<span data-ttu-id="162c6-115">upperNumber</span><span class="sxs-lookup"><span data-stu-id="162c6-115">upperNumber</span></span>|<span data-ttu-id="162c6-116">Int32</span><span class="sxs-lookup"><span data-stu-id="162c6-116">Int32</span></span>|<span data-ttu-id="162c6-117">上の数です。</span><span class="sxs-lookup"><span data-stu-id="162c6-117">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="162c6-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="162c6-118">Relationships</span></span>
<span data-ttu-id="162c6-119">なし</span><span class="sxs-lookup"><span data-stu-id="162c6-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="162c6-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="162c6-120">JSON Representation</span></span>
<span data-ttu-id="162c6-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="162c6-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.numberRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.numberRange",
  "lowerNumber": 1024,
  "upperNumber": 1024
}
```





