---
title: auditProperty リソースの種類
description: 監査のプロパティのプロパティが含まれるクラス。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 290aae8c245fd09c17fc766cedd7c2e253626943
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912030"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="90ec7-103">auditProperty リソースの種類</span><span class="sxs-lookup"><span data-stu-id="90ec7-103">auditProperty resource type</span></span>

> <span data-ttu-id="90ec7-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="90ec7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="90ec7-105">監査のプロパティのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="90ec7-105">A class containing the properties for Audit Property.</span></span>
## <a name="properties"></a><span data-ttu-id="90ec7-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="90ec7-106">Properties</span></span>
|<span data-ttu-id="90ec7-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="90ec7-107">Property</span></span>|<span data-ttu-id="90ec7-108">種類</span><span class="sxs-lookup"><span data-stu-id="90ec7-108">Type</span></span>|<span data-ttu-id="90ec7-109">説明</span><span class="sxs-lookup"><span data-stu-id="90ec7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90ec7-110">displayName</span><span class="sxs-lookup"><span data-stu-id="90ec7-110">displayName</span></span>|<span data-ttu-id="90ec7-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="90ec7-111">String</span></span>|<span data-ttu-id="90ec7-112">表示名。</span><span class="sxs-lookup"><span data-stu-id="90ec7-112">Display name.</span></span>|
|<span data-ttu-id="90ec7-113">oldValue</span><span class="sxs-lookup"><span data-stu-id="90ec7-113">oldValue</span></span>|<span data-ttu-id="90ec7-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="90ec7-114">String</span></span>|<span data-ttu-id="90ec7-115">以前の値。</span><span class="sxs-lookup"><span data-stu-id="90ec7-115">Old value.</span></span>|
|<span data-ttu-id="90ec7-116">newValue</span><span class="sxs-lookup"><span data-stu-id="90ec7-116">newValue</span></span>|<span data-ttu-id="90ec7-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="90ec7-117">String</span></span>|<span data-ttu-id="90ec7-118">新しい値。</span><span class="sxs-lookup"><span data-stu-id="90ec7-118">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="90ec7-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="90ec7-119">Relationships</span></span>
<span data-ttu-id="90ec7-120">なし</span><span class="sxs-lookup"><span data-stu-id="90ec7-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="90ec7-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="90ec7-121">JSON Representation</span></span>
<span data-ttu-id="90ec7-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="90ec7-122">Here is a JSON representation of the resource.</span></span>
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



