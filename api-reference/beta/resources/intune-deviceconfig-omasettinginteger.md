---
title: omaSettingInteger リソースの種類
description: OMA 設定の整数の定義。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 800c36cf769def2f040376c8c580f361cd52cde0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397863"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="b98ee-103">omaSettingInteger リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b98ee-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="b98ee-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b98ee-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b98ee-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b98ee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b98ee-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b98ee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b98ee-107">OMA 設定の整数の定義。</span><span class="sxs-lookup"><span data-stu-id="b98ee-107">OMA Settings Integer definition.</span></span>


<span data-ttu-id="b98ee-108">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="b98ee-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b98ee-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b98ee-109">Properties</span></span>
|<span data-ttu-id="b98ee-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b98ee-110">Property</span></span>|<span data-ttu-id="b98ee-111">型</span><span class="sxs-lookup"><span data-stu-id="b98ee-111">Type</span></span>|<span data-ttu-id="b98ee-112">説明</span><span class="sxs-lookup"><span data-stu-id="b98ee-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b98ee-113">displayName</span><span class="sxs-lookup"><span data-stu-id="b98ee-113">displayName</span></span>|<span data-ttu-id="b98ee-114">文字列</span><span class="sxs-lookup"><span data-stu-id="b98ee-114">String</span></span>|<span data-ttu-id="b98ee-115">表示名。</span><span class="sxs-lookup"><span data-stu-id="b98ee-115">Display Name.</span></span> <span data-ttu-id="b98ee-116">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="b98ee-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b98ee-117">説明</span><span class="sxs-lookup"><span data-stu-id="b98ee-117">description</span></span>|<span data-ttu-id="b98ee-118">String</span><span class="sxs-lookup"><span data-stu-id="b98ee-118">String</span></span>|<span data-ttu-id="b98ee-119">説明。</span><span class="sxs-lookup"><span data-stu-id="b98ee-119">Description.</span></span> <span data-ttu-id="b98ee-120">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="b98ee-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b98ee-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="b98ee-121">omaUri</span></span>|<span data-ttu-id="b98ee-122">文字列</span><span class="sxs-lookup"><span data-stu-id="b98ee-122">String</span></span>|<span data-ttu-id="b98ee-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="b98ee-123">OMA.</span></span> <span data-ttu-id="b98ee-124">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="b98ee-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b98ee-125">値</span><span class="sxs-lookup"><span data-stu-id="b98ee-125">value</span></span>|<span data-ttu-id="b98ee-126">Int32</span><span class="sxs-lookup"><span data-stu-id="b98ee-126">Int32</span></span>|<span data-ttu-id="b98ee-127">値。</span><span class="sxs-lookup"><span data-stu-id="b98ee-127">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b98ee-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b98ee-128">Relationships</span></span>
<span data-ttu-id="b98ee-129">なし</span><span class="sxs-lookup"><span data-stu-id="b98ee-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b98ee-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b98ee-130">JSON Representation</span></span>
<span data-ttu-id="b98ee-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b98ee-131">Here is a JSON representation of the resource.</span></span>
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




