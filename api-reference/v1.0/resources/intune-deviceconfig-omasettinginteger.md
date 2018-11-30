---
title: omaSettingInteger リソースの種類
description: OMA 設定の整数の定義。
ms.openlocfilehash: 36c22b423161d9f3c58c3085fb7b040c663d460b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023703"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="f089b-103">omaSettingInteger リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f089b-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="f089b-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f089b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f089b-105">OMA 設定の整数の定義。</span><span class="sxs-lookup"><span data-stu-id="f089b-105">OMA Settings Integer definition.</span></span>

<span data-ttu-id="f089b-106">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="f089b-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f089b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f089b-107">Properties</span></span>
|<span data-ttu-id="f089b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f089b-108">Property</span></span>|<span data-ttu-id="f089b-109">型</span><span class="sxs-lookup"><span data-stu-id="f089b-109">Type</span></span>|<span data-ttu-id="f089b-110">説明</span><span class="sxs-lookup"><span data-stu-id="f089b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f089b-111">displayName</span><span class="sxs-lookup"><span data-stu-id="f089b-111">displayName</span></span>|<span data-ttu-id="f089b-112">文字列</span><span class="sxs-lookup"><span data-stu-id="f089b-112">String</span></span>|<span data-ttu-id="f089b-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="f089b-113">Display Name.</span></span> <span data-ttu-id="f089b-114">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="f089b-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f089b-115">説明</span><span class="sxs-lookup"><span data-stu-id="f089b-115">description</span></span>|<span data-ttu-id="f089b-116">String</span><span class="sxs-lookup"><span data-stu-id="f089b-116">String</span></span>|<span data-ttu-id="f089b-117">説明。</span><span class="sxs-lookup"><span data-stu-id="f089b-117">Description.</span></span> <span data-ttu-id="f089b-118">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="f089b-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f089b-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="f089b-119">omaUri</span></span>|<span data-ttu-id="f089b-120">文字列</span><span class="sxs-lookup"><span data-stu-id="f089b-120">String</span></span>|<span data-ttu-id="f089b-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="f089b-121">OMA.</span></span> <span data-ttu-id="f089b-122">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="f089b-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f089b-123">値</span><span class="sxs-lookup"><span data-stu-id="f089b-123">value</span></span>|<span data-ttu-id="f089b-124">Int32</span><span class="sxs-lookup"><span data-stu-id="f089b-124">Int32</span></span>|<span data-ttu-id="f089b-125">値。</span><span class="sxs-lookup"><span data-stu-id="f089b-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f089b-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f089b-126">Relationships</span></span>
<span data-ttu-id="f089b-127">なし</span><span class="sxs-lookup"><span data-stu-id="f089b-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f089b-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f089b-128">JSON Representation</span></span>
<span data-ttu-id="f089b-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f089b-129">Here is a JSON representation of the resource.</span></span>
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



