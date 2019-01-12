---
title: auditProperty リソースの種類
description: 監査のプロパティのプロパティが含まれるクラス。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: bd251fa942d526b01abca4191f041eb5a76745e5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952266"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="b0cdd-103">auditProperty リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b0cdd-103">auditProperty resource type</span></span>

> <span data-ttu-id="b0cdd-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b0cdd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b0cdd-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b0cdd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b0cdd-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b0cdd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b0cdd-107">監査のプロパティのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="b0cdd-107">A class containing the properties for Audit Property.</span></span>
## <a name="properties"></a><span data-ttu-id="b0cdd-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b0cdd-108">Properties</span></span>
|<span data-ttu-id="b0cdd-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b0cdd-109">Property</span></span>|<span data-ttu-id="b0cdd-110">種類</span><span class="sxs-lookup"><span data-stu-id="b0cdd-110">Type</span></span>|<span data-ttu-id="b0cdd-111">説明</span><span class="sxs-lookup"><span data-stu-id="b0cdd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0cdd-112">displayName</span><span class="sxs-lookup"><span data-stu-id="b0cdd-112">displayName</span></span>|<span data-ttu-id="b0cdd-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b0cdd-113">String</span></span>|<span data-ttu-id="b0cdd-114">表示名。</span><span class="sxs-lookup"><span data-stu-id="b0cdd-114">Display name.</span></span>|
|<span data-ttu-id="b0cdd-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="b0cdd-115">oldValue</span></span>|<span data-ttu-id="b0cdd-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b0cdd-116">String</span></span>|<span data-ttu-id="b0cdd-117">以前の値。</span><span class="sxs-lookup"><span data-stu-id="b0cdd-117">Old value.</span></span>|
|<span data-ttu-id="b0cdd-118">newValue</span><span class="sxs-lookup"><span data-stu-id="b0cdd-118">newValue</span></span>|<span data-ttu-id="b0cdd-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b0cdd-119">String</span></span>|<span data-ttu-id="b0cdd-120">新しい値。</span><span class="sxs-lookup"><span data-stu-id="b0cdd-120">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0cdd-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b0cdd-121">Relationships</span></span>
<span data-ttu-id="b0cdd-122">なし</span><span class="sxs-lookup"><span data-stu-id="b0cdd-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b0cdd-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b0cdd-123">JSON Representation</span></span>
<span data-ttu-id="b0cdd-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b0cdd-124">Here is a JSON representation of the resource.</span></span>
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





