---
title: omaSettingString リソースの種類
description: OMA 設定の文字列の定義です。
author: tfitzmac
ms.openlocfilehash: 34f25d7814c533ddc6d9ffe16ca45487382b4391
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332559"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="59111-103">omaSettingString リソースの種類</span><span class="sxs-lookup"><span data-stu-id="59111-103">omaSettingString resource type</span></span>

> <span data-ttu-id="59111-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="59111-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="59111-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="59111-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="59111-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="59111-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="59111-107">OMA 設定の文字列の定義です。</span><span class="sxs-lookup"><span data-stu-id="59111-107">OMA Settings String definition.</span></span>

<span data-ttu-id="59111-108">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="59111-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="59111-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="59111-109">Properties</span></span>
|<span data-ttu-id="59111-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="59111-110">Property</span></span>|<span data-ttu-id="59111-111">種類</span><span class="sxs-lookup"><span data-stu-id="59111-111">Type</span></span>|<span data-ttu-id="59111-112">説明</span><span class="sxs-lookup"><span data-stu-id="59111-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59111-113">displayName</span><span class="sxs-lookup"><span data-stu-id="59111-113">displayName</span></span>|<span data-ttu-id="59111-114">文字列</span><span class="sxs-lookup"><span data-stu-id="59111-114">String</span></span>|<span data-ttu-id="59111-115">表示名。</span><span class="sxs-lookup"><span data-stu-id="59111-115">Display Name.</span></span> <span data-ttu-id="59111-116">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="59111-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="59111-117">説明</span><span class="sxs-lookup"><span data-stu-id="59111-117">description</span></span>|<span data-ttu-id="59111-118">String</span><span class="sxs-lookup"><span data-stu-id="59111-118">String</span></span>|<span data-ttu-id="59111-119">説明。</span><span class="sxs-lookup"><span data-stu-id="59111-119">Description.</span></span> <span data-ttu-id="59111-120">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="59111-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="59111-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="59111-121">omaUri</span></span>|<span data-ttu-id="59111-122">文字列</span><span class="sxs-lookup"><span data-stu-id="59111-122">String</span></span>|<span data-ttu-id="59111-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="59111-123">OMA.</span></span> <span data-ttu-id="59111-124">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="59111-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="59111-125">value</span><span class="sxs-lookup"><span data-stu-id="59111-125">value</span></span>|<span data-ttu-id="59111-126">文字列</span><span class="sxs-lookup"><span data-stu-id="59111-126">String</span></span>|<span data-ttu-id="59111-127">値。</span><span class="sxs-lookup"><span data-stu-id="59111-127">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="59111-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="59111-128">Relationships</span></span>
<span data-ttu-id="59111-129">なし</span><span class="sxs-lookup"><span data-stu-id="59111-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="59111-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="59111-130">JSON Representation</span></span>
<span data-ttu-id="59111-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="59111-131">Here is a JSON representation of the resource.</span></span>
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





