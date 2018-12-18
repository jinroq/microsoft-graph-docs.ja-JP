---
title: auditProperty リソースの種類
description: 監査のプロパティのプロパティが含まれるクラス。
author: tfitzmac
ms.openlocfilehash: 2d7cd7f1fbbf9f813cf447ca53e0d4652eb0feda
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312902"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="115b5-103">auditProperty リソースの種類</span><span class="sxs-lookup"><span data-stu-id="115b5-103">auditProperty resource type</span></span>

> <span data-ttu-id="115b5-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="115b5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="115b5-105">監査のプロパティのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="115b5-105">A class containing the properties for Audit Property.</span></span>
## <a name="properties"></a><span data-ttu-id="115b5-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="115b5-106">Properties</span></span>
|<span data-ttu-id="115b5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="115b5-107">Property</span></span>|<span data-ttu-id="115b5-108">種類</span><span class="sxs-lookup"><span data-stu-id="115b5-108">Type</span></span>|<span data-ttu-id="115b5-109">説明</span><span class="sxs-lookup"><span data-stu-id="115b5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="115b5-110">displayName</span><span class="sxs-lookup"><span data-stu-id="115b5-110">displayName</span></span>|<span data-ttu-id="115b5-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="115b5-111">String</span></span>|<span data-ttu-id="115b5-112">表示名。</span><span class="sxs-lookup"><span data-stu-id="115b5-112">Display name.</span></span>|
|<span data-ttu-id="115b5-113">oldValue</span><span class="sxs-lookup"><span data-stu-id="115b5-113">oldValue</span></span>|<span data-ttu-id="115b5-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="115b5-114">String</span></span>|<span data-ttu-id="115b5-115">以前の値。</span><span class="sxs-lookup"><span data-stu-id="115b5-115">Old value.</span></span>|
|<span data-ttu-id="115b5-116">newValue</span><span class="sxs-lookup"><span data-stu-id="115b5-116">newValue</span></span>|<span data-ttu-id="115b5-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="115b5-117">String</span></span>|<span data-ttu-id="115b5-118">新しい値。</span><span class="sxs-lookup"><span data-stu-id="115b5-118">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="115b5-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="115b5-119">Relationships</span></span>
<span data-ttu-id="115b5-120">なし</span><span class="sxs-lookup"><span data-stu-id="115b5-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="115b5-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="115b5-121">JSON Representation</span></span>
<span data-ttu-id="115b5-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="115b5-122">Here is a JSON representation of the resource.</span></span>
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



