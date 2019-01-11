---
title: auditProperty リソースの種類
description: 監査のプロパティのプロパティが含まれるクラス。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e91f3771be981f6ff410e8774f6a8ac9fbc121dd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870918"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="ceb09-103">auditProperty リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ceb09-103">auditProperty resource type</span></span>

> <span data-ttu-id="ceb09-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ceb09-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ceb09-105">監査のプロパティのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="ceb09-105">A class containing the properties for Audit Property.</span></span>
## <a name="properties"></a><span data-ttu-id="ceb09-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ceb09-106">Properties</span></span>
|<span data-ttu-id="ceb09-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ceb09-107">Property</span></span>|<span data-ttu-id="ceb09-108">種類</span><span class="sxs-lookup"><span data-stu-id="ceb09-108">Type</span></span>|<span data-ttu-id="ceb09-109">説明</span><span class="sxs-lookup"><span data-stu-id="ceb09-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ceb09-110">displayName</span><span class="sxs-lookup"><span data-stu-id="ceb09-110">displayName</span></span>|<span data-ttu-id="ceb09-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ceb09-111">String</span></span>|<span data-ttu-id="ceb09-112">表示名。</span><span class="sxs-lookup"><span data-stu-id="ceb09-112">Display name.</span></span>|
|<span data-ttu-id="ceb09-113">oldValue</span><span class="sxs-lookup"><span data-stu-id="ceb09-113">oldValue</span></span>|<span data-ttu-id="ceb09-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ceb09-114">String</span></span>|<span data-ttu-id="ceb09-115">以前の値。</span><span class="sxs-lookup"><span data-stu-id="ceb09-115">Old value.</span></span>|
|<span data-ttu-id="ceb09-116">newValue</span><span class="sxs-lookup"><span data-stu-id="ceb09-116">newValue</span></span>|<span data-ttu-id="ceb09-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ceb09-117">String</span></span>|<span data-ttu-id="ceb09-118">新しい値。</span><span class="sxs-lookup"><span data-stu-id="ceb09-118">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ceb09-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ceb09-119">Relationships</span></span>
<span data-ttu-id="ceb09-120">なし</span><span class="sxs-lookup"><span data-stu-id="ceb09-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ceb09-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ceb09-121">JSON Representation</span></span>
<span data-ttu-id="ceb09-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ceb09-122">Here is a JSON representation of the resource.</span></span>
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



