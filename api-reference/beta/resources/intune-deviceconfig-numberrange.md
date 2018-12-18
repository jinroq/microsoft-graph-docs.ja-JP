---
title: numberRange リソースの種類
description: 番号範囲の定義です。
author: tfitzmac
ms.openlocfilehash: 7b9703524e1562a7367a3c5b9bf0212e29620429
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314659"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="9e54a-103">numberRange リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9e54a-103">numberRange resource type</span></span>

> <span data-ttu-id="9e54a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9e54a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9e54a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e54a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9e54a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9e54a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9e54a-107">番号範囲の定義です。</span><span class="sxs-lookup"><span data-stu-id="9e54a-107">Number Range definition.</span></span>
## <a name="properties"></a><span data-ttu-id="9e54a-108">Properties</span><span class="sxs-lookup"><span data-stu-id="9e54a-108">Properties</span></span>
|<span data-ttu-id="9e54a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9e54a-109">Property</span></span>|<span data-ttu-id="9e54a-110">種類</span><span class="sxs-lookup"><span data-stu-id="9e54a-110">Type</span></span>|<span data-ttu-id="9e54a-111">説明</span><span class="sxs-lookup"><span data-stu-id="9e54a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e54a-112">lowerNumber</span><span class="sxs-lookup"><span data-stu-id="9e54a-112">lowerNumber</span></span>|<span data-ttu-id="9e54a-113">Int32</span><span class="sxs-lookup"><span data-stu-id="9e54a-113">Int32</span></span>|<span data-ttu-id="9e54a-114">下の数です。</span><span class="sxs-lookup"><span data-stu-id="9e54a-114">Lower number.</span></span>|
|<span data-ttu-id="9e54a-115">upperNumber</span><span class="sxs-lookup"><span data-stu-id="9e54a-115">upperNumber</span></span>|<span data-ttu-id="9e54a-116">Int32</span><span class="sxs-lookup"><span data-stu-id="9e54a-116">Int32</span></span>|<span data-ttu-id="9e54a-117">上の数です。</span><span class="sxs-lookup"><span data-stu-id="9e54a-117">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e54a-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9e54a-118">Relationships</span></span>
<span data-ttu-id="9e54a-119">なし</span><span class="sxs-lookup"><span data-stu-id="9e54a-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9e54a-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9e54a-120">JSON Representation</span></span>
<span data-ttu-id="9e54a-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9e54a-121">Here is a JSON representation of the resource.</span></span>
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





