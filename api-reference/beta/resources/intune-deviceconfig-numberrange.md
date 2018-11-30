---
title: numberRange リソースの種類
description: 番号範囲の定義です。
ms.openlocfilehash: ef4b24e3034414221365d81c40b453e7ca66a94b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066814"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="4a604-103">numberRange リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4a604-103">numberRange resource type</span></span>

> <span data-ttu-id="4a604-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4a604-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4a604-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a604-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4a604-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4a604-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4a604-107">番号範囲の定義です。</span><span class="sxs-lookup"><span data-stu-id="4a604-107">Number Range definition.</span></span>
## <a name="properties"></a><span data-ttu-id="4a604-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4a604-108">Properties</span></span>
|<span data-ttu-id="4a604-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4a604-109">Property</span></span>|<span data-ttu-id="4a604-110">型</span><span class="sxs-lookup"><span data-stu-id="4a604-110">Type</span></span>|<span data-ttu-id="4a604-111">説明</span><span class="sxs-lookup"><span data-stu-id="4a604-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a604-112">lowerNumber</span><span class="sxs-lookup"><span data-stu-id="4a604-112">lowerNumber</span></span>|<span data-ttu-id="4a604-113">Int32</span><span class="sxs-lookup"><span data-stu-id="4a604-113">Int32</span></span>|<span data-ttu-id="4a604-114">下の数です。</span><span class="sxs-lookup"><span data-stu-id="4a604-114">Lower number.</span></span>|
|<span data-ttu-id="4a604-115">upperNumber</span><span class="sxs-lookup"><span data-stu-id="4a604-115">upperNumber</span></span>|<span data-ttu-id="4a604-116">Int32</span><span class="sxs-lookup"><span data-stu-id="4a604-116">Int32</span></span>|<span data-ttu-id="4a604-117">上の数です。</span><span class="sxs-lookup"><span data-stu-id="4a604-117">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a604-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4a604-118">Relationships</span></span>
<span data-ttu-id="4a604-119">なし</span><span class="sxs-lookup"><span data-stu-id="4a604-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4a604-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4a604-120">JSON Representation</span></span>
<span data-ttu-id="4a604-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4a604-121">Here is a JSON representation of the resource.</span></span>
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





