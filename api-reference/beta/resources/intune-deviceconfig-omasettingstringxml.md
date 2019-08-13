---
title: omaSettingStringXml リソースの種類
description: OMA 設定文字列の XML 定義です。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ddce8acb059ff28ad37bce284efc6f3fd29f0224
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36368444"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="198bf-103">omaSettingStringXml リソースの種類</span><span class="sxs-lookup"><span data-stu-id="198bf-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="198bf-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="198bf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="198bf-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="198bf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="198bf-106">OMA 設定文字列の XML 定義です。</span><span class="sxs-lookup"><span data-stu-id="198bf-106">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="198bf-107">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="198bf-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="198bf-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="198bf-108">Properties</span></span>
|<span data-ttu-id="198bf-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="198bf-109">Property</span></span>|<span data-ttu-id="198bf-110">型</span><span class="sxs-lookup"><span data-stu-id="198bf-110">Type</span></span>|<span data-ttu-id="198bf-111">説明</span><span class="sxs-lookup"><span data-stu-id="198bf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="198bf-112">displayName</span><span class="sxs-lookup"><span data-stu-id="198bf-112">displayName</span></span>|<span data-ttu-id="198bf-113">String</span><span class="sxs-lookup"><span data-stu-id="198bf-113">String</span></span>|<span data-ttu-id="198bf-114">表示名。</span><span class="sxs-lookup"><span data-stu-id="198bf-114">Display Name.</span></span> <span data-ttu-id="198bf-115">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="198bf-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="198bf-116">description</span><span class="sxs-lookup"><span data-stu-id="198bf-116">description</span></span>|<span data-ttu-id="198bf-117">String</span><span class="sxs-lookup"><span data-stu-id="198bf-117">String</span></span>|<span data-ttu-id="198bf-118">説明。</span><span class="sxs-lookup"><span data-stu-id="198bf-118">Description.</span></span> <span data-ttu-id="198bf-119">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="198bf-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="198bf-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="198bf-120">omaUri</span></span>|<span data-ttu-id="198bf-121">文字列</span><span class="sxs-lookup"><span data-stu-id="198bf-121">String</span></span>|<span data-ttu-id="198bf-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="198bf-122">OMA.</span></span> <span data-ttu-id="198bf-123">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="198bf-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="198bf-124">fileName</span><span class="sxs-lookup"><span data-stu-id="198bf-124">fileName</span></span>|<span data-ttu-id="198bf-125">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="198bf-125">String</span></span>|<span data-ttu-id="198bf-126">Value プロパティに関連付けられているファイル名 (\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="198bf-126">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="198bf-127">value</span><span class="sxs-lookup"><span data-stu-id="198bf-127">value</span></span>|<span data-ttu-id="198bf-128">バイナリ型 (Binary)</span><span class="sxs-lookup"><span data-stu-id="198bf-128">Binary</span></span>|<span data-ttu-id="198bf-129">値。</span><span class="sxs-lookup"><span data-stu-id="198bf-129">Value.</span></span> <span data-ttu-id="198bf-130">(UTF8 でエンコードされたバイト配列)</span><span class="sxs-lookup"><span data-stu-id="198bf-130">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="198bf-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="198bf-131">Relationships</span></span>
<span data-ttu-id="198bf-132">なし</span><span class="sxs-lookup"><span data-stu-id="198bf-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="198bf-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="198bf-133">JSON Representation</span></span>
<span data-ttu-id="198bf-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="198bf-134">Here is a JSON representation of the resource.</span></span>
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



