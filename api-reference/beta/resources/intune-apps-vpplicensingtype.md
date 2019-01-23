---
title: vppLicensingType リソースの種類
description: iOS Volume-Purchase Program (VPP) ライセンスの種類のプロパティが含まれます。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 42bb678077781309b9e06c339112537bc2e48bde
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399676"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="bf180-103">vppLicensingType リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bf180-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="bf180-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bf180-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bf180-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bf180-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bf180-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bf180-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf180-107">iOS Volume-Purchase Program (VPP) ライセンスの種類のプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="bf180-107">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="bf180-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf180-108">Properties</span></span>
|<span data-ttu-id="bf180-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf180-109">Property</span></span>|<span data-ttu-id="bf180-110">型</span><span class="sxs-lookup"><span data-stu-id="bf180-110">Type</span></span>|<span data-ttu-id="bf180-111">説明</span><span class="sxs-lookup"><span data-stu-id="bf180-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf180-112">supportUserLicensing</span><span class="sxs-lookup"><span data-stu-id="bf180-112">supportUserLicensing</span></span>|<span data-ttu-id="bf180-113">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="bf180-113">Boolean</span></span>|<span data-ttu-id="bf180-114">プログラムがユーザー ライセンスの種類をサポートするかどうか。</span><span class="sxs-lookup"><span data-stu-id="bf180-114">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="bf180-115">supportDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="bf180-115">supportDeviceLicensing</span></span>|<span data-ttu-id="bf180-116">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="bf180-116">Boolean</span></span>|<span data-ttu-id="bf180-117">プログラムがデバイス ライセンスの種類をサポートするかどうか。</span><span class="sxs-lookup"><span data-stu-id="bf180-117">Whether the program supports the device licensing type.</span></span>|
|<span data-ttu-id="bf180-118">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="bf180-118">supportsUserLicensing</span></span>|<span data-ttu-id="bf180-119">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="bf180-119">Boolean</span></span>|<span data-ttu-id="bf180-120">プログラムがユーザー ライセンスの種類をサポートするかどうか。</span><span class="sxs-lookup"><span data-stu-id="bf180-120">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="bf180-121">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="bf180-121">supportsDeviceLicensing</span></span>|<span data-ttu-id="bf180-122">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="bf180-122">Boolean</span></span>|<span data-ttu-id="bf180-123">プログラムがデバイス ライセンスの種類をサポートするかどうか。</span><span class="sxs-lookup"><span data-stu-id="bf180-123">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf180-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bf180-124">Relationships</span></span>
<span data-ttu-id="bf180-125">なし</span><span class="sxs-lookup"><span data-stu-id="bf180-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf180-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bf180-126">JSON Representation</span></span>
<span data-ttu-id="bf180-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bf180-127">Here is a JSON representation of the resource.</span></span>
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




