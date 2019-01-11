---
title: omaSettingBoolean リソースの種類
description: OMA 設定のブール定義。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 46bca1f6052dae3f4699b88258abce4b346c67bb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868209"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="a6391-103">omaSettingBoolean リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a6391-103">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="a6391-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a6391-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a6391-105">OMA 設定のブール定義。</span><span class="sxs-lookup"><span data-stu-id="a6391-105">OMA Settings Boolean definition.</span></span>

<span data-ttu-id="a6391-106">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="a6391-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a6391-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6391-107">Properties</span></span>
|<span data-ttu-id="a6391-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6391-108">Property</span></span>|<span data-ttu-id="a6391-109">種類</span><span class="sxs-lookup"><span data-stu-id="a6391-109">Type</span></span>|<span data-ttu-id="a6391-110">説明</span><span class="sxs-lookup"><span data-stu-id="a6391-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6391-111">displayName</span><span class="sxs-lookup"><span data-stu-id="a6391-111">displayName</span></span>|<span data-ttu-id="a6391-112">文字列</span><span class="sxs-lookup"><span data-stu-id="a6391-112">String</span></span>|<span data-ttu-id="a6391-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="a6391-113">Display Name.</span></span> <span data-ttu-id="a6391-114">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="a6391-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="a6391-115">説明</span><span class="sxs-lookup"><span data-stu-id="a6391-115">description</span></span>|<span data-ttu-id="a6391-116">String</span><span class="sxs-lookup"><span data-stu-id="a6391-116">String</span></span>|<span data-ttu-id="a6391-117">説明。</span><span class="sxs-lookup"><span data-stu-id="a6391-117">Description.</span></span> <span data-ttu-id="a6391-118">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="a6391-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="a6391-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="a6391-119">omaUri</span></span>|<span data-ttu-id="a6391-120">文字列</span><span class="sxs-lookup"><span data-stu-id="a6391-120">String</span></span>|<span data-ttu-id="a6391-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="a6391-121">OMA.</span></span> <span data-ttu-id="a6391-122">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="a6391-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="a6391-123">value</span><span class="sxs-lookup"><span data-stu-id="a6391-123">value</span></span>|<span data-ttu-id="a6391-124">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="a6391-124">Boolean</span></span>|<span data-ttu-id="a6391-125">値。</span><span class="sxs-lookup"><span data-stu-id="a6391-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6391-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a6391-126">Relationships</span></span>
<span data-ttu-id="a6391-127">なし</span><span class="sxs-lookup"><span data-stu-id="a6391-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a6391-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a6391-128">JSON Representation</span></span>
<span data-ttu-id="a6391-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a6391-129">Here is a JSON representation of the resource.</span></span>
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



