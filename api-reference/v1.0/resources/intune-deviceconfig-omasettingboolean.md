---
title: omaSettingBoolean リソースの種類
description: OMA 設定のブール定義。
author: tfitzmac
ms.openlocfilehash: 10101217d1c0f07931cb847e1c14f36844c8dc9b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323283"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="0755a-103">omaSettingBoolean リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0755a-103">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="0755a-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0755a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0755a-105">OMA 設定のブール定義。</span><span class="sxs-lookup"><span data-stu-id="0755a-105">OMA Settings Boolean definition.</span></span>

<span data-ttu-id="0755a-106">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="0755a-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0755a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0755a-107">Properties</span></span>
|<span data-ttu-id="0755a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0755a-108">Property</span></span>|<span data-ttu-id="0755a-109">種類</span><span class="sxs-lookup"><span data-stu-id="0755a-109">Type</span></span>|<span data-ttu-id="0755a-110">説明</span><span class="sxs-lookup"><span data-stu-id="0755a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0755a-111">displayName</span><span class="sxs-lookup"><span data-stu-id="0755a-111">displayName</span></span>|<span data-ttu-id="0755a-112">文字列</span><span class="sxs-lookup"><span data-stu-id="0755a-112">String</span></span>|<span data-ttu-id="0755a-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="0755a-113">Display Name.</span></span> <span data-ttu-id="0755a-114">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="0755a-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0755a-115">説明</span><span class="sxs-lookup"><span data-stu-id="0755a-115">description</span></span>|<span data-ttu-id="0755a-116">String</span><span class="sxs-lookup"><span data-stu-id="0755a-116">String</span></span>|<span data-ttu-id="0755a-117">説明。</span><span class="sxs-lookup"><span data-stu-id="0755a-117">Description.</span></span> <span data-ttu-id="0755a-118">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="0755a-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0755a-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="0755a-119">omaUri</span></span>|<span data-ttu-id="0755a-120">文字列</span><span class="sxs-lookup"><span data-stu-id="0755a-120">String</span></span>|<span data-ttu-id="0755a-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="0755a-121">OMA.</span></span> <span data-ttu-id="0755a-122">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="0755a-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0755a-123">value</span><span class="sxs-lookup"><span data-stu-id="0755a-123">value</span></span>|<span data-ttu-id="0755a-124">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="0755a-124">Boolean</span></span>|<span data-ttu-id="0755a-125">値。</span><span class="sxs-lookup"><span data-stu-id="0755a-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0755a-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0755a-126">Relationships</span></span>
<span data-ttu-id="0755a-127">なし</span><span class="sxs-lookup"><span data-stu-id="0755a-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0755a-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0755a-128">JSON Representation</span></span>
<span data-ttu-id="0755a-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0755a-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBoolean"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBoolean",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": true
}
```



