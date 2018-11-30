---
title: auditProperty リソースの種類
description: 監査のプロパティのプロパティが含まれるクラス。
ms.openlocfilehash: eaffa5552d611ac2ef8bb236009b9520d1134586
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023655"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="f1171-103">auditProperty リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f1171-103">auditProperty resource type</span></span>

> <span data-ttu-id="f1171-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f1171-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1171-105">監査のプロパティのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="f1171-105">A class containing the properties for Audit Property.</span></span>
## <a name="properties"></a><span data-ttu-id="f1171-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f1171-106">Properties</span></span>
|<span data-ttu-id="f1171-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f1171-107">Property</span></span>|<span data-ttu-id="f1171-108">型</span><span class="sxs-lookup"><span data-stu-id="f1171-108">Type</span></span>|<span data-ttu-id="f1171-109">説明</span><span class="sxs-lookup"><span data-stu-id="f1171-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1171-110">displayName</span><span class="sxs-lookup"><span data-stu-id="f1171-110">displayName</span></span>|<span data-ttu-id="f1171-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f1171-111">String</span></span>|<span data-ttu-id="f1171-112">表示名。</span><span class="sxs-lookup"><span data-stu-id="f1171-112">Display name.</span></span>|
|<span data-ttu-id="f1171-113">oldValue</span><span class="sxs-lookup"><span data-stu-id="f1171-113">oldValue</span></span>|<span data-ttu-id="f1171-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f1171-114">String</span></span>|<span data-ttu-id="f1171-115">以前の値。</span><span class="sxs-lookup"><span data-stu-id="f1171-115">Old value.</span></span>|
|<span data-ttu-id="f1171-116">newValue</span><span class="sxs-lookup"><span data-stu-id="f1171-116">newValue</span></span>|<span data-ttu-id="f1171-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f1171-117">String</span></span>|<span data-ttu-id="f1171-118">新しい値。</span><span class="sxs-lookup"><span data-stu-id="f1171-118">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1171-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f1171-119">Relationships</span></span>
<span data-ttu-id="f1171-120">なし</span><span class="sxs-lookup"><span data-stu-id="f1171-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f1171-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f1171-121">JSON Representation</span></span>
<span data-ttu-id="f1171-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f1171-122">Here is a JSON representation of the resource.</span></span>
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



