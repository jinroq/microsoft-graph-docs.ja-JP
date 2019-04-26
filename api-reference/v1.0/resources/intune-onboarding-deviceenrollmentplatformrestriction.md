---
title: deviceEnrollmentPlatformRestriction リソースの種類
description: プラットフォーム固有の登録の制限
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 306f280928c843b596c57e7bdab454fd138851cc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571199"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="c3cd9-103">deviceEnrollmentPlatformRestriction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c3cd9-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="c3cd9-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c3cd9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3cd9-105">プラットフォーム固有の登録の制限</span><span class="sxs-lookup"><span data-stu-id="c3cd9-105">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="c3cd9-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c3cd9-106">Properties</span></span>
|<span data-ttu-id="c3cd9-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c3cd9-107">Property</span></span>|<span data-ttu-id="c3cd9-108">型</span><span class="sxs-lookup"><span data-stu-id="c3cd9-108">Type</span></span>|<span data-ttu-id="c3cd9-109">説明</span><span class="sxs-lookup"><span data-stu-id="c3cd9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3cd9-110">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="c3cd9-110">platformBlocked</span></span>|<span data-ttu-id="c3cd9-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3cd9-111">Boolean</span></span>|<span data-ttu-id="c3cd9-112">登録で対象プラットフォームをブロックします</span><span class="sxs-lookup"><span data-stu-id="c3cd9-112">Block the platform from enrolling</span></span>|
|<span data-ttu-id="c3cd9-113">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="c3cd9-113">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="c3cd9-114">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="c3cd9-114">Boolean</span></span>|<span data-ttu-id="c3cd9-115">個人所有のデバイスの登録をブロックします</span><span class="sxs-lookup"><span data-stu-id="c3cd9-115">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="c3cd9-116">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="c3cd9-116">osMinimumVersion</span></span>|<span data-ttu-id="c3cd9-117">String</span><span class="sxs-lookup"><span data-stu-id="c3cd9-117">String</span></span>|<span data-ttu-id="c3cd9-118">サポートされる最小 OS バージョン</span><span class="sxs-lookup"><span data-stu-id="c3cd9-118">Min OS version supported</span></span>|
|<span data-ttu-id="c3cd9-119">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="c3cd9-119">osMaximumVersion</span></span>|<span data-ttu-id="c3cd9-120">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c3cd9-120">String</span></span>|<span data-ttu-id="c3cd9-121">サポートされる最大 OS バージョン</span><span class="sxs-lookup"><span data-stu-id="c3cd9-121">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3cd9-122">関係</span><span class="sxs-lookup"><span data-stu-id="c3cd9-122">Relationships</span></span>
<span data-ttu-id="c3cd9-123">なし</span><span class="sxs-lookup"><span data-stu-id="c3cd9-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3cd9-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c3cd9-124">JSON Representation</span></span>
<span data-ttu-id="c3cd9-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c3cd9-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestriction",
  "platformBlocked": true,
  "personalDeviceEnrollmentBlocked": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String"
}
```



