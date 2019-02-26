---
title: deviceEnrollmentPlatformRestriction リソースの種類
description: プラットフォーム固有の登録の制限
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 306f280928c843b596c57e7bdab454fd138851cc
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260838"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="2f609-103">deviceEnrollmentPlatformRestriction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2f609-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="2f609-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2f609-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f609-105">プラットフォーム固有の登録の制限</span><span class="sxs-lookup"><span data-stu-id="2f609-105">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="2f609-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2f609-106">Properties</span></span>
|<span data-ttu-id="2f609-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2f609-107">Property</span></span>|<span data-ttu-id="2f609-108">型</span><span class="sxs-lookup"><span data-stu-id="2f609-108">Type</span></span>|<span data-ttu-id="2f609-109">説明</span><span class="sxs-lookup"><span data-stu-id="2f609-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f609-110">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="2f609-110">platformBlocked</span></span>|<span data-ttu-id="2f609-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f609-111">Boolean</span></span>|<span data-ttu-id="2f609-112">登録で対象プラットフォームをブロックします</span><span class="sxs-lookup"><span data-stu-id="2f609-112">Block the platform from enrolling</span></span>|
|<span data-ttu-id="2f609-113">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="2f609-113">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="2f609-114">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="2f609-114">Boolean</span></span>|<span data-ttu-id="2f609-115">個人所有のデバイスの登録をブロックします</span><span class="sxs-lookup"><span data-stu-id="2f609-115">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="2f609-116">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="2f609-116">osMinimumVersion</span></span>|<span data-ttu-id="2f609-117">String</span><span class="sxs-lookup"><span data-stu-id="2f609-117">String</span></span>|<span data-ttu-id="2f609-118">サポートされる最小 OS バージョン</span><span class="sxs-lookup"><span data-stu-id="2f609-118">Min OS version supported</span></span>|
|<span data-ttu-id="2f609-119">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="2f609-119">osMaximumVersion</span></span>|<span data-ttu-id="2f609-120">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="2f609-120">String</span></span>|<span data-ttu-id="2f609-121">サポートされる最大 OS バージョン</span><span class="sxs-lookup"><span data-stu-id="2f609-121">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f609-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2f609-122">Relationships</span></span>
<span data-ttu-id="2f609-123">なし</span><span class="sxs-lookup"><span data-stu-id="2f609-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2f609-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2f609-124">JSON Representation</span></span>
<span data-ttu-id="2f609-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2f609-125">Here is a JSON representation of the resource.</span></span>
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



