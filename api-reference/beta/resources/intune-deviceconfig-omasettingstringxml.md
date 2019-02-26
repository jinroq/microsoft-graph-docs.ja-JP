---
title: omaSettingStringXml リソースの種類
description: OMA 設定文字列の XML 定義です。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 846ed1c9bb17065b82f2663e7f4276b34442f9bd
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164534"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="0f4f6-103">omaSettingStringXml リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0f4f6-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="0f4f6-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0f4f6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f4f6-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0f4f6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f4f6-106">OMA 設定文字列の XML 定義です。</span><span class="sxs-lookup"><span data-stu-id="0f4f6-106">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="0f4f6-107">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="0f4f6-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0f4f6-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0f4f6-108">Properties</span></span>
|<span data-ttu-id="0f4f6-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0f4f6-109">Property</span></span>|<span data-ttu-id="0f4f6-110">型</span><span class="sxs-lookup"><span data-stu-id="0f4f6-110">Type</span></span>|<span data-ttu-id="0f4f6-111">説明</span><span class="sxs-lookup"><span data-stu-id="0f4f6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f4f6-112">displayName</span><span class="sxs-lookup"><span data-stu-id="0f4f6-112">displayName</span></span>|<span data-ttu-id="0f4f6-113">String</span><span class="sxs-lookup"><span data-stu-id="0f4f6-113">String</span></span>|<span data-ttu-id="0f4f6-114">表示名。</span><span class="sxs-lookup"><span data-stu-id="0f4f6-114">Display Name.</span></span> <span data-ttu-id="0f4f6-115">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="0f4f6-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0f4f6-116">説明</span><span class="sxs-lookup"><span data-stu-id="0f4f6-116">description</span></span>|<span data-ttu-id="0f4f6-117">String</span><span class="sxs-lookup"><span data-stu-id="0f4f6-117">String</span></span>|<span data-ttu-id="0f4f6-118">説明。</span><span class="sxs-lookup"><span data-stu-id="0f4f6-118">Description.</span></span> <span data-ttu-id="0f4f6-119">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="0f4f6-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0f4f6-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="0f4f6-120">omaUri</span></span>|<span data-ttu-id="0f4f6-121">文字列</span><span class="sxs-lookup"><span data-stu-id="0f4f6-121">String</span></span>|<span data-ttu-id="0f4f6-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="0f4f6-122">OMA.</span></span> <span data-ttu-id="0f4f6-123">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="0f4f6-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0f4f6-124">fileName</span><span class="sxs-lookup"><span data-stu-id="0f4f6-124">fileName</span></span>|<span data-ttu-id="0f4f6-125">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="0f4f6-125">String</span></span>|<span data-ttu-id="0f4f6-126">Value プロパティに関連付けられているファイル名 (\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="0f4f6-126">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="0f4f6-127">value</span><span class="sxs-lookup"><span data-stu-id="0f4f6-127">value</span></span>|<span data-ttu-id="0f4f6-128">バイナリ型 (Binary)</span><span class="sxs-lookup"><span data-stu-id="0f4f6-128">Binary</span></span>|<span data-ttu-id="0f4f6-129">値。</span><span class="sxs-lookup"><span data-stu-id="0f4f6-129">Value.</span></span> <span data-ttu-id="0f4f6-130">(UTF8 でエンコードされたバイト配列)</span><span class="sxs-lookup"><span data-stu-id="0f4f6-130">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f4f6-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0f4f6-131">Relationships</span></span>
<span data-ttu-id="0f4f6-132">なし</span><span class="sxs-lookup"><span data-stu-id="0f4f6-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f4f6-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0f4f6-133">JSON Representation</span></span>
<span data-ttu-id="0f4f6-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0f4f6-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingStringXml"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingStringXml",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "binary"
}
```




