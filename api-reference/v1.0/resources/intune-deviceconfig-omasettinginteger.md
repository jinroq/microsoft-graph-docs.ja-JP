---
title: omaSettingInteger リソースの種類
description: OMA 設定の整数の定義。
author: tfitzmac
ms.openlocfilehash: 6a2e6fe6e6782159afa99d91785ae9e854a2e99c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306553"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="6ff4b-103">omaSettingInteger リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6ff4b-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="6ff4b-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6ff4b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6ff4b-105">OMA 設定の整数の定義。</span><span class="sxs-lookup"><span data-stu-id="6ff4b-105">OMA Settings Integer definition.</span></span>

<span data-ttu-id="6ff4b-106">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="6ff4b-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6ff4b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ff4b-107">Properties</span></span>
|<span data-ttu-id="6ff4b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ff4b-108">Property</span></span>|<span data-ttu-id="6ff4b-109">種類</span><span class="sxs-lookup"><span data-stu-id="6ff4b-109">Type</span></span>|<span data-ttu-id="6ff4b-110">説明</span><span class="sxs-lookup"><span data-stu-id="6ff4b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ff4b-111">displayName</span><span class="sxs-lookup"><span data-stu-id="6ff4b-111">displayName</span></span>|<span data-ttu-id="6ff4b-112">文字列</span><span class="sxs-lookup"><span data-stu-id="6ff4b-112">String</span></span>|<span data-ttu-id="6ff4b-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="6ff4b-113">Display Name.</span></span> <span data-ttu-id="6ff4b-114">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="6ff4b-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="6ff4b-115">説明</span><span class="sxs-lookup"><span data-stu-id="6ff4b-115">description</span></span>|<span data-ttu-id="6ff4b-116">String</span><span class="sxs-lookup"><span data-stu-id="6ff4b-116">String</span></span>|<span data-ttu-id="6ff4b-117">説明。</span><span class="sxs-lookup"><span data-stu-id="6ff4b-117">Description.</span></span> <span data-ttu-id="6ff4b-118">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="6ff4b-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="6ff4b-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="6ff4b-119">omaUri</span></span>|<span data-ttu-id="6ff4b-120">文字列</span><span class="sxs-lookup"><span data-stu-id="6ff4b-120">String</span></span>|<span data-ttu-id="6ff4b-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="6ff4b-121">OMA.</span></span> <span data-ttu-id="6ff4b-122">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="6ff4b-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="6ff4b-123">値</span><span class="sxs-lookup"><span data-stu-id="6ff4b-123">value</span></span>|<span data-ttu-id="6ff4b-124">Int32</span><span class="sxs-lookup"><span data-stu-id="6ff4b-124">Int32</span></span>|<span data-ttu-id="6ff4b-125">値。</span><span class="sxs-lookup"><span data-stu-id="6ff4b-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ff4b-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6ff4b-126">Relationships</span></span>
<span data-ttu-id="6ff4b-127">なし</span><span class="sxs-lookup"><span data-stu-id="6ff4b-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6ff4b-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6ff4b-128">JSON Representation</span></span>
<span data-ttu-id="6ff4b-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6ff4b-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingInteger"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingInteger",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": 1024
}
```



