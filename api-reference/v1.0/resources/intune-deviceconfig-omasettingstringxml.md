---
title: omaSettingStringXml リソースの種類
description: OMA 設定文字列の XML 定義です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e34dc1ebdfff2692d35d258492bc58cb26282198
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911484"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="44f47-103">omaSettingStringXml リソースの種類</span><span class="sxs-lookup"><span data-stu-id="44f47-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="44f47-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="44f47-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="44f47-105">OMA 設定文字列の XML 定義です。</span><span class="sxs-lookup"><span data-stu-id="44f47-105">OMA Settings StringXML definition.</span></span>

<span data-ttu-id="44f47-106">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="44f47-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="44f47-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="44f47-107">Properties</span></span>
|<span data-ttu-id="44f47-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="44f47-108">Property</span></span>|<span data-ttu-id="44f47-109">型</span><span class="sxs-lookup"><span data-stu-id="44f47-109">Type</span></span>|<span data-ttu-id="44f47-110">説明</span><span class="sxs-lookup"><span data-stu-id="44f47-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44f47-111">displayName</span><span class="sxs-lookup"><span data-stu-id="44f47-111">displayName</span></span>|<span data-ttu-id="44f47-112">文字列</span><span class="sxs-lookup"><span data-stu-id="44f47-112">String</span></span>|<span data-ttu-id="44f47-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="44f47-113">Display Name.</span></span> <span data-ttu-id="44f47-114">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="44f47-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="44f47-115">説明</span><span class="sxs-lookup"><span data-stu-id="44f47-115">description</span></span>|<span data-ttu-id="44f47-116">String</span><span class="sxs-lookup"><span data-stu-id="44f47-116">String</span></span>|<span data-ttu-id="44f47-117">説明。</span><span class="sxs-lookup"><span data-stu-id="44f47-117">Description.</span></span> <span data-ttu-id="44f47-118">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="44f47-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="44f47-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="44f47-119">omaUri</span></span>|<span data-ttu-id="44f47-120">文字列</span><span class="sxs-lookup"><span data-stu-id="44f47-120">String</span></span>|<span data-ttu-id="44f47-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="44f47-121">OMA.</span></span> <span data-ttu-id="44f47-122">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="44f47-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="44f47-123">fileName</span><span class="sxs-lookup"><span data-stu-id="44f47-123">fileName</span></span>|<span data-ttu-id="44f47-124">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="44f47-124">String</span></span>|<span data-ttu-id="44f47-125">Value プロパティに関連付けられているファイル名 (\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="44f47-125">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="44f47-126">value</span><span class="sxs-lookup"><span data-stu-id="44f47-126">value</span></span>|<span data-ttu-id="44f47-127">バイナリ型 (Binary)</span><span class="sxs-lookup"><span data-stu-id="44f47-127">Binary</span></span>|<span data-ttu-id="44f47-128">値。</span><span class="sxs-lookup"><span data-stu-id="44f47-128">Value.</span></span> <span data-ttu-id="44f47-129">(UTF8 でエンコードされたバイト配列)</span><span class="sxs-lookup"><span data-stu-id="44f47-129">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="44f47-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="44f47-130">Relationships</span></span>
<span data-ttu-id="44f47-131">なし</span><span class="sxs-lookup"><span data-stu-id="44f47-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="44f47-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="44f47-132">JSON Representation</span></span>
<span data-ttu-id="44f47-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="44f47-133">Here is a JSON representation of the resource.</span></span>
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



