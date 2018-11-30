---
title: omaSettingStringXml リソースの種類
description: OMA 設定文字列の XML 定義です。
ms.openlocfilehash: ecdc22f698479ba25a2cce4ce822cda633c582ab
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020336"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="c54b2-103">omaSettingStringXml リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c54b2-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="c54b2-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c54b2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c54b2-105">OMA 設定文字列の XML 定義です。</span><span class="sxs-lookup"><span data-stu-id="c54b2-105">OMA Settings StringXML definition.</span></span>

<span data-ttu-id="c54b2-106">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="c54b2-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c54b2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c54b2-107">Properties</span></span>
|<span data-ttu-id="c54b2-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c54b2-108">Property</span></span>|<span data-ttu-id="c54b2-109">型</span><span class="sxs-lookup"><span data-stu-id="c54b2-109">Type</span></span>|<span data-ttu-id="c54b2-110">説明</span><span class="sxs-lookup"><span data-stu-id="c54b2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c54b2-111">displayName</span><span class="sxs-lookup"><span data-stu-id="c54b2-111">displayName</span></span>|<span data-ttu-id="c54b2-112">文字列</span><span class="sxs-lookup"><span data-stu-id="c54b2-112">String</span></span>|<span data-ttu-id="c54b2-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="c54b2-113">Display Name.</span></span> <span data-ttu-id="c54b2-114">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="c54b2-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c54b2-115">説明</span><span class="sxs-lookup"><span data-stu-id="c54b2-115">description</span></span>|<span data-ttu-id="c54b2-116">String</span><span class="sxs-lookup"><span data-stu-id="c54b2-116">String</span></span>|<span data-ttu-id="c54b2-117">説明。</span><span class="sxs-lookup"><span data-stu-id="c54b2-117">Description.</span></span> <span data-ttu-id="c54b2-118">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="c54b2-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c54b2-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="c54b2-119">omaUri</span></span>|<span data-ttu-id="c54b2-120">文字列</span><span class="sxs-lookup"><span data-stu-id="c54b2-120">String</span></span>|<span data-ttu-id="c54b2-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="c54b2-121">OMA.</span></span> <span data-ttu-id="c54b2-122">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="c54b2-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c54b2-123">fileName</span><span class="sxs-lookup"><span data-stu-id="c54b2-123">fileName</span></span>|<span data-ttu-id="c54b2-124">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c54b2-124">String</span></span>|<span data-ttu-id="c54b2-125">Value プロパティに関連付けられているファイル名 (\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="c54b2-125">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="c54b2-126">value</span><span class="sxs-lookup"><span data-stu-id="c54b2-126">value</span></span>|<span data-ttu-id="c54b2-127">バイナリ型 (Binary)</span><span class="sxs-lookup"><span data-stu-id="c54b2-127">Binary</span></span>|<span data-ttu-id="c54b2-128">値。</span><span class="sxs-lookup"><span data-stu-id="c54b2-128">Value.</span></span> <span data-ttu-id="c54b2-129">(UTF8 でエンコードされたバイト配列)</span><span class="sxs-lookup"><span data-stu-id="c54b2-129">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="c54b2-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c54b2-130">Relationships</span></span>
<span data-ttu-id="c54b2-131">なし</span><span class="sxs-lookup"><span data-stu-id="c54b2-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c54b2-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c54b2-132">JSON Representation</span></span>
<span data-ttu-id="c54b2-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c54b2-133">Here is a JSON representation of the resource.</span></span>
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



