---
title: omaSettingDateTime リソースの種類
description: OMA 設定の DateTime の定義です。
ms.openlocfilehash: b4ea11c22acb2a4119c2de1934f1ae66c2310658
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020918"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="b7559-103">omaSettingDateTime リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b7559-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="b7559-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b7559-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b7559-105">OMA 設定の DateTime の定義です。</span><span class="sxs-lookup"><span data-stu-id="b7559-105">OMA Settings DateTime definition.</span></span>

<span data-ttu-id="b7559-106">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="b7559-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b7559-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b7559-107">Properties</span></span>
|<span data-ttu-id="b7559-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b7559-108">Property</span></span>|<span data-ttu-id="b7559-109">型</span><span class="sxs-lookup"><span data-stu-id="b7559-109">Type</span></span>|<span data-ttu-id="b7559-110">説明</span><span class="sxs-lookup"><span data-stu-id="b7559-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7559-111">displayName</span><span class="sxs-lookup"><span data-stu-id="b7559-111">displayName</span></span>|<span data-ttu-id="b7559-112">文字列</span><span class="sxs-lookup"><span data-stu-id="b7559-112">String</span></span>|<span data-ttu-id="b7559-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="b7559-113">Display Name.</span></span> <span data-ttu-id="b7559-114">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="b7559-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b7559-115">説明</span><span class="sxs-lookup"><span data-stu-id="b7559-115">description</span></span>|<span data-ttu-id="b7559-116">String</span><span class="sxs-lookup"><span data-stu-id="b7559-116">String</span></span>|<span data-ttu-id="b7559-117">説明。</span><span class="sxs-lookup"><span data-stu-id="b7559-117">Description.</span></span> <span data-ttu-id="b7559-118">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="b7559-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b7559-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="b7559-119">omaUri</span></span>|<span data-ttu-id="b7559-120">文字列</span><span class="sxs-lookup"><span data-stu-id="b7559-120">String</span></span>|<span data-ttu-id="b7559-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="b7559-121">OMA.</span></span> <span data-ttu-id="b7559-122">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="b7559-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b7559-123">値</span><span class="sxs-lookup"><span data-stu-id="b7559-123">value</span></span>|<span data-ttu-id="b7559-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7559-124">DateTimeOffset</span></span>|<span data-ttu-id="b7559-125">値。</span><span class="sxs-lookup"><span data-stu-id="b7559-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b7559-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b7559-126">Relationships</span></span>
<span data-ttu-id="b7559-127">なし</span><span class="sxs-lookup"><span data-stu-id="b7559-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b7559-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b7559-128">JSON Representation</span></span>
<span data-ttu-id="b7559-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b7559-129">Here is a JSON representation of the resource.</span></span>
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



