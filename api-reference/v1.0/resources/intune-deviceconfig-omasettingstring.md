---
title: omaSettingString リソースの種類
description: OMA 設定の文字列の定義です。
author: tfitzmac
ms.openlocfilehash: a62f6dee2bf0f5a9ca96488625a84ceef5f7c785
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311201"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="ecad4-103">omaSettingString リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ecad4-103">omaSettingString resource type</span></span>

> <span data-ttu-id="ecad4-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ecad4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ecad4-105">OMA 設定の文字列の定義です。</span><span class="sxs-lookup"><span data-stu-id="ecad4-105">OMA Settings String definition.</span></span>

<span data-ttu-id="ecad4-106">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="ecad4-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ecad4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ecad4-107">Properties</span></span>
|<span data-ttu-id="ecad4-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ecad4-108">Property</span></span>|<span data-ttu-id="ecad4-109">種類</span><span class="sxs-lookup"><span data-stu-id="ecad4-109">Type</span></span>|<span data-ttu-id="ecad4-110">説明</span><span class="sxs-lookup"><span data-stu-id="ecad4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ecad4-111">displayName</span><span class="sxs-lookup"><span data-stu-id="ecad4-111">displayName</span></span>|<span data-ttu-id="ecad4-112">文字列</span><span class="sxs-lookup"><span data-stu-id="ecad4-112">String</span></span>|<span data-ttu-id="ecad4-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="ecad4-113">Display Name.</span></span> <span data-ttu-id="ecad4-114">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="ecad4-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ecad4-115">説明</span><span class="sxs-lookup"><span data-stu-id="ecad4-115">description</span></span>|<span data-ttu-id="ecad4-116">String</span><span class="sxs-lookup"><span data-stu-id="ecad4-116">String</span></span>|<span data-ttu-id="ecad4-117">説明。</span><span class="sxs-lookup"><span data-stu-id="ecad4-117">Description.</span></span> <span data-ttu-id="ecad4-118">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="ecad4-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ecad4-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="ecad4-119">omaUri</span></span>|<span data-ttu-id="ecad4-120">文字列</span><span class="sxs-lookup"><span data-stu-id="ecad4-120">String</span></span>|<span data-ttu-id="ecad4-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="ecad4-121">OMA.</span></span> <span data-ttu-id="ecad4-122">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="ecad4-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ecad4-123">value</span><span class="sxs-lookup"><span data-stu-id="ecad4-123">value</span></span>|<span data-ttu-id="ecad4-124">文字列</span><span class="sxs-lookup"><span data-stu-id="ecad4-124">String</span></span>|<span data-ttu-id="ecad4-125">値。</span><span class="sxs-lookup"><span data-stu-id="ecad4-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ecad4-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ecad4-126">Relationships</span></span>
<span data-ttu-id="ecad4-127">なし</span><span class="sxs-lookup"><span data-stu-id="ecad4-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ecad4-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ecad4-128">JSON Representation</span></span>
<span data-ttu-id="ecad4-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ecad4-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingString",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String"
}
```



