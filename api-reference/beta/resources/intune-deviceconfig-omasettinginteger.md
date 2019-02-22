---
title: omaSettingInteger リソースの種類
description: OMA 設定の整数の定義。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cb87ecf7f658e9eb6ed19904a09460d2b2695be4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172325"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="0ab38-103">omaSettingInteger リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0ab38-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="0ab38-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0ab38-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ab38-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0ab38-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ab38-106">OMA 設定の整数の定義。</span><span class="sxs-lookup"><span data-stu-id="0ab38-106">OMA Settings Integer definition.</span></span>


<span data-ttu-id="0ab38-107">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="0ab38-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0ab38-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0ab38-108">Properties</span></span>
|<span data-ttu-id="0ab38-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0ab38-109">Property</span></span>|<span data-ttu-id="0ab38-110">型</span><span class="sxs-lookup"><span data-stu-id="0ab38-110">Type</span></span>|<span data-ttu-id="0ab38-111">説明</span><span class="sxs-lookup"><span data-stu-id="0ab38-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ab38-112">displayName</span><span class="sxs-lookup"><span data-stu-id="0ab38-112">displayName</span></span>|<span data-ttu-id="0ab38-113">String</span><span class="sxs-lookup"><span data-stu-id="0ab38-113">String</span></span>|<span data-ttu-id="0ab38-114">表示名。</span><span class="sxs-lookup"><span data-stu-id="0ab38-114">Display Name.</span></span> <span data-ttu-id="0ab38-115">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="0ab38-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0ab38-116">説明</span><span class="sxs-lookup"><span data-stu-id="0ab38-116">description</span></span>|<span data-ttu-id="0ab38-117">String</span><span class="sxs-lookup"><span data-stu-id="0ab38-117">String</span></span>|<span data-ttu-id="0ab38-118">説明。</span><span class="sxs-lookup"><span data-stu-id="0ab38-118">Description.</span></span> <span data-ttu-id="0ab38-119">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="0ab38-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0ab38-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="0ab38-120">omaUri</span></span>|<span data-ttu-id="0ab38-121">文字列</span><span class="sxs-lookup"><span data-stu-id="0ab38-121">String</span></span>|<span data-ttu-id="0ab38-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="0ab38-122">OMA.</span></span> <span data-ttu-id="0ab38-123">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="0ab38-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0ab38-124">値</span><span class="sxs-lookup"><span data-stu-id="0ab38-124">value</span></span>|<span data-ttu-id="0ab38-125">Int32</span><span class="sxs-lookup"><span data-stu-id="0ab38-125">Int32</span></span>|<span data-ttu-id="0ab38-126">値。</span><span class="sxs-lookup"><span data-stu-id="0ab38-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ab38-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0ab38-127">Relationships</span></span>
<span data-ttu-id="0ab38-128">なし</span><span class="sxs-lookup"><span data-stu-id="0ab38-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0ab38-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0ab38-129">JSON Representation</span></span>
<span data-ttu-id="0ab38-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0ab38-130">Here is a JSON representation of the resource.</span></span>
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




