---
title: omaSettingFloatingPoint リソースの種類
description: OMA 設定の浮動小数点の定義です。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7105cf54323a76f2d08552b18dbb04d623e800b7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36368486"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="393c0-103">omaSettingFloatingPoint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="393c0-103">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="393c0-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="393c0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="393c0-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="393c0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="393c0-106">OMA 設定の浮動小数点の定義です。</span><span class="sxs-lookup"><span data-stu-id="393c0-106">OMA Settings Floating Point definition.</span></span>


<span data-ttu-id="393c0-107">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="393c0-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="393c0-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="393c0-108">Properties</span></span>
|<span data-ttu-id="393c0-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="393c0-109">Property</span></span>|<span data-ttu-id="393c0-110">型</span><span class="sxs-lookup"><span data-stu-id="393c0-110">Type</span></span>|<span data-ttu-id="393c0-111">説明</span><span class="sxs-lookup"><span data-stu-id="393c0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="393c0-112">displayName</span><span class="sxs-lookup"><span data-stu-id="393c0-112">displayName</span></span>|<span data-ttu-id="393c0-113">String</span><span class="sxs-lookup"><span data-stu-id="393c0-113">String</span></span>|<span data-ttu-id="393c0-114">表示名。</span><span class="sxs-lookup"><span data-stu-id="393c0-114">Display Name.</span></span> <span data-ttu-id="393c0-115">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="393c0-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="393c0-116">description</span><span class="sxs-lookup"><span data-stu-id="393c0-116">description</span></span>|<span data-ttu-id="393c0-117">String</span><span class="sxs-lookup"><span data-stu-id="393c0-117">String</span></span>|<span data-ttu-id="393c0-118">説明。</span><span class="sxs-lookup"><span data-stu-id="393c0-118">Description.</span></span> <span data-ttu-id="393c0-119">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="393c0-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="393c0-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="393c0-120">omaUri</span></span>|<span data-ttu-id="393c0-121">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="393c0-121">String</span></span>|<span data-ttu-id="393c0-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="393c0-122">OMA.</span></span> <span data-ttu-id="393c0-123">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="393c0-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="393c0-124">値</span><span class="sxs-lookup"><span data-stu-id="393c0-124">value</span></span>|<span data-ttu-id="393c0-125">単精度浮動小数点型 (Single)</span><span class="sxs-lookup"><span data-stu-id="393c0-125">Single</span></span>|<span data-ttu-id="393c0-126">値。</span><span class="sxs-lookup"><span data-stu-id="393c0-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="393c0-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="393c0-127">Relationships</span></span>
<span data-ttu-id="393c0-128">なし</span><span class="sxs-lookup"><span data-stu-id="393c0-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="393c0-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="393c0-129">JSON Representation</span></span>
<span data-ttu-id="393c0-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="393c0-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingFloatingPoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingFloatingPoint",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "<Unknown Primitive Type Edm.Single>"
}
```



