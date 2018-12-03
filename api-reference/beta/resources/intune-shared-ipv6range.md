---
title: iPv6Range リソースの種類
description: IP V6 の範囲
ms.openlocfilehash: ac2834ea68e1ce4aa7e28f7b421ff4e3d031f8fa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074212"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="a4db0-103">iPv6Range リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a4db0-103">iPv6Range resource type</span></span>

> <span data-ttu-id="a4db0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a4db0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a4db0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4db0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a4db0-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a4db0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a4db0-107">IP V6 の範囲</span><span class="sxs-lookup"><span data-stu-id="a4db0-107">IP V6 range</span></span>

<span data-ttu-id="a4db0-108">[ipRange](../resources/intune-shared-iprange.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="a4db0-108">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a4db0-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4db0-109">Properties</span></span>
|<span data-ttu-id="a4db0-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4db0-110">Property</span></span>|<span data-ttu-id="a4db0-111">型</span><span class="sxs-lookup"><span data-stu-id="a4db0-111">Type</span></span>|<span data-ttu-id="a4db0-112">説明</span><span class="sxs-lookup"><span data-stu-id="a4db0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4db0-113">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="a4db0-113">lowerAddress</span></span>|<span data-ttu-id="a4db0-114">文字列</span><span class="sxs-lookup"><span data-stu-id="a4db0-114">String</span></span>|<span data-ttu-id="a4db0-115">低い番号の IP アドレス</span><span class="sxs-lookup"><span data-stu-id="a4db0-115">Lower IP Address</span></span>|
|<span data-ttu-id="a4db0-116">upperAddress</span><span class="sxs-lookup"><span data-stu-id="a4db0-116">upperAddress</span></span>|<span data-ttu-id="a4db0-117">文字列</span><span class="sxs-lookup"><span data-stu-id="a4db0-117">String</span></span>|<span data-ttu-id="a4db0-118">高い番号の IP アドレス</span><span class="sxs-lookup"><span data-stu-id="a4db0-118">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4db0-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a4db0-119">Relationships</span></span>
<span data-ttu-id="a4db0-120">なし</span><span class="sxs-lookup"><span data-stu-id="a4db0-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a4db0-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a4db0-121">JSON Representation</span></span>
<span data-ttu-id="a4db0-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a4db0-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iPv6Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv6Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```



