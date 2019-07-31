---
title: vppLicensingType リソースの種類
description: iOS Volume-Purchase Program (VPP) ライセンスの種類のプロパティが含まれます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fe6e59ba5703d5c069781db6331f0ea6dbbfa240
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012381"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="ccab7-103">vppLicensingType リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ccab7-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="ccab7-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ccab7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ccab7-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ccab7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccab7-106">iOS Volume-Purchase Program (VPP) ライセンスの種類のプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="ccab7-106">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="ccab7-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ccab7-107">Properties</span></span>
|<span data-ttu-id="ccab7-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ccab7-108">Property</span></span>|<span data-ttu-id="ccab7-109">型</span><span class="sxs-lookup"><span data-stu-id="ccab7-109">Type</span></span>|<span data-ttu-id="ccab7-110">説明</span><span class="sxs-lookup"><span data-stu-id="ccab7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccab7-111">supportUserLicensing</span><span class="sxs-lookup"><span data-stu-id="ccab7-111">supportUserLicensing</span></span>|<span data-ttu-id="ccab7-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="ccab7-112">Boolean</span></span>|<span data-ttu-id="ccab7-113">プログラムがユーザー ライセンスの種類をサポートするかどうか。</span><span class="sxs-lookup"><span data-stu-id="ccab7-113">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="ccab7-114">supportdevicelicenel</span><span class="sxs-lookup"><span data-stu-id="ccab7-114">supportDeviceLicensing</span></span>|<span data-ttu-id="ccab7-115">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="ccab7-115">Boolean</span></span>|<span data-ttu-id="ccab7-116">プログラムがデバイス ライセンスの種類をサポートするかどうか。</span><span class="sxs-lookup"><span data-stu-id="ccab7-116">Whether the program supports the device licensing type.</span></span>|
|<span data-ttu-id="ccab7-117">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="ccab7-117">supportsUserLicensing</span></span>|<span data-ttu-id="ccab7-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="ccab7-118">Boolean</span></span>|<span data-ttu-id="ccab7-119">プログラムがユーザー ライセンスの種類をサポートするかどうか。</span><span class="sxs-lookup"><span data-stu-id="ccab7-119">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="ccab7-120">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="ccab7-120">supportsDeviceLicensing</span></span>|<span data-ttu-id="ccab7-121">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="ccab7-121">Boolean</span></span>|<span data-ttu-id="ccab7-122">プログラムがデバイス ライセンスの種類をサポートするかどうか。</span><span class="sxs-lookup"><span data-stu-id="ccab7-122">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ccab7-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ccab7-123">Relationships</span></span>
<span data-ttu-id="ccab7-124">なし</span><span class="sxs-lookup"><span data-stu-id="ccab7-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ccab7-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ccab7-125">JSON Representation</span></span>
<span data-ttu-id="ccab7-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ccab7-126">Here is a JSON representation of the resource.</span></span>
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





