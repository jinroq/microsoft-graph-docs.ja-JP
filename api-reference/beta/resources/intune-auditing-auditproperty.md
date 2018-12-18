---
title: auditProperty リソースの種類
description: 監査のプロパティのプロパティが含まれるクラス。
author: tfitzmac
ms.openlocfilehash: 801ac78cb81e126ff49c4c680fc0624611a9f6d6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316318"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="c732d-103">auditProperty リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c732d-103">auditProperty resource type</span></span>

> <span data-ttu-id="c732d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c732d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c732d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c732d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c732d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c732d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c732d-107">監査のプロパティのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="c732d-107">A class containing the properties for Audit Property.</span></span>
## <a name="properties"></a><span data-ttu-id="c732d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c732d-108">Properties</span></span>
|<span data-ttu-id="c732d-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c732d-109">Property</span></span>|<span data-ttu-id="c732d-110">種類</span><span class="sxs-lookup"><span data-stu-id="c732d-110">Type</span></span>|<span data-ttu-id="c732d-111">説明</span><span class="sxs-lookup"><span data-stu-id="c732d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c732d-112">displayName</span><span class="sxs-lookup"><span data-stu-id="c732d-112">displayName</span></span>|<span data-ttu-id="c732d-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c732d-113">String</span></span>|<span data-ttu-id="c732d-114">表示名。</span><span class="sxs-lookup"><span data-stu-id="c732d-114">Display name.</span></span>|
|<span data-ttu-id="c732d-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="c732d-115">oldValue</span></span>|<span data-ttu-id="c732d-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c732d-116">String</span></span>|<span data-ttu-id="c732d-117">以前の値。</span><span class="sxs-lookup"><span data-stu-id="c732d-117">Old value.</span></span>|
|<span data-ttu-id="c732d-118">newValue</span><span class="sxs-lookup"><span data-stu-id="c732d-118">newValue</span></span>|<span data-ttu-id="c732d-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c732d-119">String</span></span>|<span data-ttu-id="c732d-120">新しい値。</span><span class="sxs-lookup"><span data-stu-id="c732d-120">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c732d-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c732d-121">Relationships</span></span>
<span data-ttu-id="c732d-122">なし</span><span class="sxs-lookup"><span data-stu-id="c732d-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c732d-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c732d-123">JSON Representation</span></span>
<span data-ttu-id="c732d-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c732d-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditProperty"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditProperty",
  "displayName": "String",
  "oldValue": "String",
  "newValue": "String"
}
```





