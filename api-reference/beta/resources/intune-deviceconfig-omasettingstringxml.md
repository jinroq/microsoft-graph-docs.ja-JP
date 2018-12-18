---
title: omaSettingStringXml リソースの種類
description: OMA 設定文字列の XML 定義です。
author: tfitzmac
ms.openlocfilehash: 5582ca84a9d6c918ce7b8dea5a21f616804da4ca
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323787"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="31dab-103">omaSettingStringXml リソースの種類</span><span class="sxs-lookup"><span data-stu-id="31dab-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="31dab-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="31dab-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="31dab-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31dab-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="31dab-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="31dab-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="31dab-107">OMA 設定文字列の XML 定義です。</span><span class="sxs-lookup"><span data-stu-id="31dab-107">OMA Settings StringXML definition.</span></span>

<span data-ttu-id="31dab-108">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="31dab-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="31dab-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31dab-109">Properties</span></span>
|<span data-ttu-id="31dab-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31dab-110">Property</span></span>|<span data-ttu-id="31dab-111">種類</span><span class="sxs-lookup"><span data-stu-id="31dab-111">Type</span></span>|<span data-ttu-id="31dab-112">説明</span><span class="sxs-lookup"><span data-stu-id="31dab-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31dab-113">displayName</span><span class="sxs-lookup"><span data-stu-id="31dab-113">displayName</span></span>|<span data-ttu-id="31dab-114">文字列</span><span class="sxs-lookup"><span data-stu-id="31dab-114">String</span></span>|<span data-ttu-id="31dab-115">表示名。</span><span class="sxs-lookup"><span data-stu-id="31dab-115">Display Name.</span></span> <span data-ttu-id="31dab-116">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="31dab-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="31dab-117">説明</span><span class="sxs-lookup"><span data-stu-id="31dab-117">description</span></span>|<span data-ttu-id="31dab-118">String</span><span class="sxs-lookup"><span data-stu-id="31dab-118">String</span></span>|<span data-ttu-id="31dab-119">説明。</span><span class="sxs-lookup"><span data-stu-id="31dab-119">Description.</span></span> <span data-ttu-id="31dab-120">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="31dab-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="31dab-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="31dab-121">omaUri</span></span>|<span data-ttu-id="31dab-122">文字列</span><span class="sxs-lookup"><span data-stu-id="31dab-122">String</span></span>|<span data-ttu-id="31dab-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="31dab-123">OMA.</span></span> <span data-ttu-id="31dab-124">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="31dab-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="31dab-125">fileName</span><span class="sxs-lookup"><span data-stu-id="31dab-125">fileName</span></span>|<span data-ttu-id="31dab-126">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="31dab-126">String</span></span>|<span data-ttu-id="31dab-127">Value プロパティに関連付けられているファイル名 (\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="31dab-127">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="31dab-128">value</span><span class="sxs-lookup"><span data-stu-id="31dab-128">value</span></span>|<span data-ttu-id="31dab-129">バイナリ型 (Binary)</span><span class="sxs-lookup"><span data-stu-id="31dab-129">Binary</span></span>|<span data-ttu-id="31dab-130">値。</span><span class="sxs-lookup"><span data-stu-id="31dab-130">Value.</span></span> <span data-ttu-id="31dab-131">(UTF8 でエンコードされたバイト配列)</span><span class="sxs-lookup"><span data-stu-id="31dab-131">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="31dab-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="31dab-132">Relationships</span></span>
<span data-ttu-id="31dab-133">なし</span><span class="sxs-lookup"><span data-stu-id="31dab-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="31dab-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="31dab-134">JSON Representation</span></span>
<span data-ttu-id="31dab-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="31dab-135">Here is a JSON representation of the resource.</span></span>
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





