---
title: omaSettingStringXml リソースの種類
description: OMA 設定文字列の XML 定義です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3c0e47ba7fce929e114282c6aa88605d9f185618
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419437"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="1d432-103">omaSettingStringXml リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1d432-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="1d432-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1d432-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1d432-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d432-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1d432-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1d432-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d432-107">OMA 設定文字列の XML 定義です。</span><span class="sxs-lookup"><span data-stu-id="1d432-107">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="1d432-108">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="1d432-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1d432-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d432-109">Properties</span></span>
|<span data-ttu-id="1d432-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d432-110">Property</span></span>|<span data-ttu-id="1d432-111">型</span><span class="sxs-lookup"><span data-stu-id="1d432-111">Type</span></span>|<span data-ttu-id="1d432-112">説明</span><span class="sxs-lookup"><span data-stu-id="1d432-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d432-113">displayName</span><span class="sxs-lookup"><span data-stu-id="1d432-113">displayName</span></span>|<span data-ttu-id="1d432-114">文字列</span><span class="sxs-lookup"><span data-stu-id="1d432-114">String</span></span>|<span data-ttu-id="1d432-115">表示名。</span><span class="sxs-lookup"><span data-stu-id="1d432-115">Display Name.</span></span> <span data-ttu-id="1d432-116">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="1d432-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="1d432-117">説明</span><span class="sxs-lookup"><span data-stu-id="1d432-117">description</span></span>|<span data-ttu-id="1d432-118">String</span><span class="sxs-lookup"><span data-stu-id="1d432-118">String</span></span>|<span data-ttu-id="1d432-119">説明。</span><span class="sxs-lookup"><span data-stu-id="1d432-119">Description.</span></span> <span data-ttu-id="1d432-120">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="1d432-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="1d432-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="1d432-121">omaUri</span></span>|<span data-ttu-id="1d432-122">文字列</span><span class="sxs-lookup"><span data-stu-id="1d432-122">String</span></span>|<span data-ttu-id="1d432-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="1d432-123">OMA.</span></span> <span data-ttu-id="1d432-124">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="1d432-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="1d432-125">fileName</span><span class="sxs-lookup"><span data-stu-id="1d432-125">fileName</span></span>|<span data-ttu-id="1d432-126">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="1d432-126">String</span></span>|<span data-ttu-id="1d432-127">Value プロパティに関連付けられているファイル名 (\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="1d432-127">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="1d432-128">value</span><span class="sxs-lookup"><span data-stu-id="1d432-128">value</span></span>|<span data-ttu-id="1d432-129">バイナリ型 (Binary)</span><span class="sxs-lookup"><span data-stu-id="1d432-129">Binary</span></span>|<span data-ttu-id="1d432-130">値。</span><span class="sxs-lookup"><span data-stu-id="1d432-130">Value.</span></span> <span data-ttu-id="1d432-131">(UTF8 でエンコードされたバイト配列)</span><span class="sxs-lookup"><span data-stu-id="1d432-131">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d432-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1d432-132">Relationships</span></span>
<span data-ttu-id="1d432-133">なし</span><span class="sxs-lookup"><span data-stu-id="1d432-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d432-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1d432-134">JSON Representation</span></span>
<span data-ttu-id="1d432-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1d432-135">Here is a JSON representation of the resource.</span></span>
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




