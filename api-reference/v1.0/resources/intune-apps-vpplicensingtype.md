---
title: vppLicensingType リソースの種類
description: iOS Volume-Purchase Program (VPP) ライセンスの種類のプロパティが含まれます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 73b46c9bcd8680ffbd78c1cfc85cc6dec85126e6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32557930"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="60aca-103">vppLicensingType リソースの種類</span><span class="sxs-lookup"><span data-stu-id="60aca-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="60aca-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="60aca-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60aca-105">iOS Volume-Purchase Program (VPP) ライセンスの種類のプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="60aca-105">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="60aca-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="60aca-106">Properties</span></span>
|<span data-ttu-id="60aca-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="60aca-107">Property</span></span>|<span data-ttu-id="60aca-108">型</span><span class="sxs-lookup"><span data-stu-id="60aca-108">Type</span></span>|<span data-ttu-id="60aca-109">説明</span><span class="sxs-lookup"><span data-stu-id="60aca-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60aca-110">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="60aca-110">supportsUserLicensing</span></span>|<span data-ttu-id="60aca-111">ブール値</span><span class="sxs-lookup"><span data-stu-id="60aca-111">Boolean</span></span>|<span data-ttu-id="60aca-112">プログラムがユーザー ライセンスの種類をサポートするかどうか。</span><span class="sxs-lookup"><span data-stu-id="60aca-112">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="60aca-113">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="60aca-113">supportsDeviceLicensing</span></span>|<span data-ttu-id="60aca-114">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="60aca-114">Boolean</span></span>|<span data-ttu-id="60aca-115">プログラムがデバイス ライセンスの種類をサポートするかどうか。</span><span class="sxs-lookup"><span data-stu-id="60aca-115">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="60aca-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="60aca-116">Relationships</span></span>
<span data-ttu-id="60aca-117">なし</span><span class="sxs-lookup"><span data-stu-id="60aca-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="60aca-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="60aca-118">JSON Representation</span></span>
<span data-ttu-id="60aca-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="60aca-119">Here is a JSON representation of the resource.</span></span>
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



