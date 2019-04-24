---
title: iosDeviceType リソースの種類
description: モバイル アプリを実行できる iOS デバイスの種類のプロパティが含まれます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5f3bd1d0aff7e09d5828496de348805075d0b330
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503528"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="95836-103">iosDeviceType リソースの種類</span><span class="sxs-lookup"><span data-stu-id="95836-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="95836-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="95836-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95836-105">モバイル アプリを実行できる iOS デバイスの種類のプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="95836-105">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="95836-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95836-106">Properties</span></span>
|<span data-ttu-id="95836-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95836-107">Property</span></span>|<span data-ttu-id="95836-108">型</span><span class="sxs-lookup"><span data-stu-id="95836-108">Type</span></span>|<span data-ttu-id="95836-109">説明</span><span class="sxs-lookup"><span data-stu-id="95836-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95836-110">iPad</span><span class="sxs-lookup"><span data-stu-id="95836-110">iPad</span></span>|<span data-ttu-id="95836-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="95836-111">Boolean</span></span>|<span data-ttu-id="95836-112">アプリを iPad で実行できるかどうか。</span><span class="sxs-lookup"><span data-stu-id="95836-112">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="95836-113">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="95836-113">iPhoneAndIPod</span></span>|<span data-ttu-id="95836-114">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="95836-114">Boolean</span></span>|<span data-ttu-id="95836-115">アプリを iPhone および iPod で実行できるかどうか。</span><span class="sxs-lookup"><span data-stu-id="95836-115">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95836-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="95836-116">Relationships</span></span>
<span data-ttu-id="95836-117">なし</span><span class="sxs-lookup"><span data-stu-id="95836-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="95836-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="95836-118">JSON Representation</span></span>
<span data-ttu-id="95836-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="95836-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosDeviceType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosDeviceType",
  "iPad": true,
  "iPhoneAndIPod": true
}
```



