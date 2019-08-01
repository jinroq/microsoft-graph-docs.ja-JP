---
title: vppLicensingType リソースの種類
description: iOS Volume-Purchase Program (VPP) ライセンスの種類のプロパティが含まれます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 831961fd9e04bff577fe986a2e6309d1cdfbcca0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032131"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="2e444-103">vppLicensingType リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2e444-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="2e444-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2e444-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e444-105">iOS Volume-Purchase Program (VPP) ライセンスの種類のプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="2e444-105">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="2e444-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2e444-106">Properties</span></span>
|<span data-ttu-id="2e444-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2e444-107">Property</span></span>|<span data-ttu-id="2e444-108">型</span><span class="sxs-lookup"><span data-stu-id="2e444-108">Type</span></span>|<span data-ttu-id="2e444-109">説明</span><span class="sxs-lookup"><span data-stu-id="2e444-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e444-110">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="2e444-110">supportsUserLicensing</span></span>|<span data-ttu-id="2e444-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e444-111">Boolean</span></span>|<span data-ttu-id="2e444-112">プログラムがユーザー ライセンスの種類をサポートするかどうか。</span><span class="sxs-lookup"><span data-stu-id="2e444-112">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="2e444-113">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="2e444-113">supportsDeviceLicensing</span></span>|<span data-ttu-id="2e444-114">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="2e444-114">Boolean</span></span>|<span data-ttu-id="2e444-115">プログラムがデバイス ライセンスの種類をサポートするかどうか。</span><span class="sxs-lookup"><span data-stu-id="2e444-115">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e444-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2e444-116">Relationships</span></span>
<span data-ttu-id="2e444-117">なし</span><span class="sxs-lookup"><span data-stu-id="2e444-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2e444-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2e444-118">JSON Representation</span></span>
<span data-ttu-id="2e444-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2e444-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppLicensingType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppLicensingType",
  "supportsUserLicensing": true,
  "supportsDeviceLicensing": true
}
```



