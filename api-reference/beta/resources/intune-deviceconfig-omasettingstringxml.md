---
title: omaSettingStringXml リソースの種類
description: OMA 設定文字列の XML 定義です。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: efc9a2ddd996088f88b85be55c9c7d6bfe62b86a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000789"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="319c4-103">omaSettingStringXml リソースの種類</span><span class="sxs-lookup"><span data-stu-id="319c4-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="319c4-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="319c4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="319c4-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="319c4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="319c4-106">OMA 設定文字列の XML 定義です。</span><span class="sxs-lookup"><span data-stu-id="319c4-106">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="319c4-107">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="319c4-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="319c4-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="319c4-108">Properties</span></span>
|<span data-ttu-id="319c4-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="319c4-109">Property</span></span>|<span data-ttu-id="319c4-110">型</span><span class="sxs-lookup"><span data-stu-id="319c4-110">Type</span></span>|<span data-ttu-id="319c4-111">説明</span><span class="sxs-lookup"><span data-stu-id="319c4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="319c4-112">displayName</span><span class="sxs-lookup"><span data-stu-id="319c4-112">displayName</span></span>|<span data-ttu-id="319c4-113">String</span><span class="sxs-lookup"><span data-stu-id="319c4-113">String</span></span>|<span data-ttu-id="319c4-114">表示名。</span><span class="sxs-lookup"><span data-stu-id="319c4-114">Display Name.</span></span> <span data-ttu-id="319c4-115">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="319c4-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="319c4-116">description</span><span class="sxs-lookup"><span data-stu-id="319c4-116">description</span></span>|<span data-ttu-id="319c4-117">String</span><span class="sxs-lookup"><span data-stu-id="319c4-117">String</span></span>|<span data-ttu-id="319c4-118">説明。</span><span class="sxs-lookup"><span data-stu-id="319c4-118">Description.</span></span> <span data-ttu-id="319c4-119">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="319c4-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="319c4-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="319c4-120">omaUri</span></span>|<span data-ttu-id="319c4-121">文字列</span><span class="sxs-lookup"><span data-stu-id="319c4-121">String</span></span>|<span data-ttu-id="319c4-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="319c4-122">OMA.</span></span> <span data-ttu-id="319c4-123">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="319c4-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="319c4-124">fileName</span><span class="sxs-lookup"><span data-stu-id="319c4-124">fileName</span></span>|<span data-ttu-id="319c4-125">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="319c4-125">String</span></span>|<span data-ttu-id="319c4-126">Value プロパティに関連付けられているファイル名 (\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="319c4-126">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="319c4-127">value</span><span class="sxs-lookup"><span data-stu-id="319c4-127">value</span></span>|<span data-ttu-id="319c4-128">バイナリ型 (Binary)</span><span class="sxs-lookup"><span data-stu-id="319c4-128">Binary</span></span>|<span data-ttu-id="319c4-129">値。</span><span class="sxs-lookup"><span data-stu-id="319c4-129">Value.</span></span> <span data-ttu-id="319c4-130">(UTF8 でエンコードされたバイト配列)</span><span class="sxs-lookup"><span data-stu-id="319c4-130">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="319c4-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="319c4-131">Relationships</span></span>
<span data-ttu-id="319c4-132">なし</span><span class="sxs-lookup"><span data-stu-id="319c4-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="319c4-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="319c4-133">JSON Representation</span></span>
<span data-ttu-id="319c4-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="319c4-134">Here is a JSON representation of the resource.</span></span>
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





