---
title: omaSettingDateTime リソースの種類
description: OMA 設定の DateTime の定義です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 34c19caee6bab30dbfe0e82abf1a55f20bb5d3b4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932295"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="d6f6a-103">omaSettingDateTime リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d6f6a-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="d6f6a-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d6f6a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d6f6a-105">OMA 設定の DateTime の定義です。</span><span class="sxs-lookup"><span data-stu-id="d6f6a-105">OMA Settings DateTime definition.</span></span>

<span data-ttu-id="d6f6a-106">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="d6f6a-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d6f6a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d6f6a-107">Properties</span></span>
|<span data-ttu-id="d6f6a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d6f6a-108">Property</span></span>|<span data-ttu-id="d6f6a-109">種類</span><span class="sxs-lookup"><span data-stu-id="d6f6a-109">Type</span></span>|<span data-ttu-id="d6f6a-110">説明</span><span class="sxs-lookup"><span data-stu-id="d6f6a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6f6a-111">displayName</span><span class="sxs-lookup"><span data-stu-id="d6f6a-111">displayName</span></span>|<span data-ttu-id="d6f6a-112">文字列</span><span class="sxs-lookup"><span data-stu-id="d6f6a-112">String</span></span>|<span data-ttu-id="d6f6a-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="d6f6a-113">Display Name.</span></span> <span data-ttu-id="d6f6a-114">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="d6f6a-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d6f6a-115">説明</span><span class="sxs-lookup"><span data-stu-id="d6f6a-115">description</span></span>|<span data-ttu-id="d6f6a-116">String</span><span class="sxs-lookup"><span data-stu-id="d6f6a-116">String</span></span>|<span data-ttu-id="d6f6a-117">説明。</span><span class="sxs-lookup"><span data-stu-id="d6f6a-117">Description.</span></span> <span data-ttu-id="d6f6a-118">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="d6f6a-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d6f6a-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="d6f6a-119">omaUri</span></span>|<span data-ttu-id="d6f6a-120">文字列</span><span class="sxs-lookup"><span data-stu-id="d6f6a-120">String</span></span>|<span data-ttu-id="d6f6a-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="d6f6a-121">OMA.</span></span> <span data-ttu-id="d6f6a-122">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="d6f6a-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d6f6a-123">値</span><span class="sxs-lookup"><span data-stu-id="d6f6a-123">value</span></span>|<span data-ttu-id="d6f6a-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6f6a-124">DateTimeOffset</span></span>|<span data-ttu-id="d6f6a-125">値。</span><span class="sxs-lookup"><span data-stu-id="d6f6a-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6f6a-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d6f6a-126">Relationships</span></span>
<span data-ttu-id="d6f6a-127">なし</span><span class="sxs-lookup"><span data-stu-id="d6f6a-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d6f6a-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d6f6a-128">JSON Representation</span></span>
<span data-ttu-id="d6f6a-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d6f6a-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingDateTime"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingDateTime",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String (timestamp)"
}
```



