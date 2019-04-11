---
title: vppLicensingType リソースの種類
description: iOS Volume-Purchase Program (VPP) ライセンスの種類のプロパティが含まれます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2f4966b6608bcd96720c4260191388979e811061
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31796466"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="5411f-103">vppLicensingType リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5411f-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="5411f-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5411f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5411f-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5411f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5411f-106">iOS Volume-Purchase Program (VPP) ライセンスの種類のプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="5411f-106">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="5411f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5411f-107">Properties</span></span>
|<span data-ttu-id="5411f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5411f-108">Property</span></span>|<span data-ttu-id="5411f-109">型</span><span class="sxs-lookup"><span data-stu-id="5411f-109">Type</span></span>|<span data-ttu-id="5411f-110">説明</span><span class="sxs-lookup"><span data-stu-id="5411f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5411f-111">supportuserlicensing</span><span class="sxs-lookup"><span data-stu-id="5411f-111">supportUserLicensing</span></span>|<span data-ttu-id="5411f-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="5411f-112">Boolean</span></span>|<span data-ttu-id="5411f-113">プログラムがユーザー ライセンスの種類をサポートするかどうか。</span><span class="sxs-lookup"><span data-stu-id="5411f-113">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="5411f-114">supportdevicelicenel</span><span class="sxs-lookup"><span data-stu-id="5411f-114">supportDeviceLicensing</span></span>|<span data-ttu-id="5411f-115">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="5411f-115">Boolean</span></span>|<span data-ttu-id="5411f-116">プログラムがデバイス ライセンスの種類をサポートするかどうか。</span><span class="sxs-lookup"><span data-stu-id="5411f-116">Whether the program supports the device licensing type.</span></span>|
|<span data-ttu-id="5411f-117">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="5411f-117">supportsUserLicensing</span></span>|<span data-ttu-id="5411f-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="5411f-118">Boolean</span></span>|<span data-ttu-id="5411f-119">プログラムがユーザー ライセンスの種類をサポートするかどうか。</span><span class="sxs-lookup"><span data-stu-id="5411f-119">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="5411f-120">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="5411f-120">supportsDeviceLicensing</span></span>|<span data-ttu-id="5411f-121">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="5411f-121">Boolean</span></span>|<span data-ttu-id="5411f-122">プログラムがデバイス ライセンスの種類をサポートするかどうか。</span><span class="sxs-lookup"><span data-stu-id="5411f-122">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5411f-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5411f-123">Relationships</span></span>
<span data-ttu-id="5411f-124">なし</span><span class="sxs-lookup"><span data-stu-id="5411f-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5411f-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5411f-125">JSON Representation</span></span>
<span data-ttu-id="5411f-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5411f-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppLicensingType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppLicensingType",
  "supportUserLicensing": true,
  "supportDeviceLicensing": true,
  "supportsUserLicensing": true,
  "supportsDeviceLicensing": true
}
```





