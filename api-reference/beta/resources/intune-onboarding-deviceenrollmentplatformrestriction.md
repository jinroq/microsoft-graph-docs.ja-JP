---
title: deviceEnrollmentPlatformRestriction リソースの種類
description: プラットフォーム固有の登録の制限
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eecbc405fd56d21f7be1c7b9bccd5254db89c8d1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140601"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="e204c-103">deviceEnrollmentPlatformRestriction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e204c-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="e204c-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e204c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e204c-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e204c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e204c-106">プラットフォーム固有の登録の制限</span><span class="sxs-lookup"><span data-stu-id="e204c-106">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="e204c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e204c-107">Properties</span></span>
|<span data-ttu-id="e204c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e204c-108">Property</span></span>|<span data-ttu-id="e204c-109">型</span><span class="sxs-lookup"><span data-stu-id="e204c-109">Type</span></span>|<span data-ttu-id="e204c-110">説明</span><span class="sxs-lookup"><span data-stu-id="e204c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e204c-111">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="e204c-111">platformBlocked</span></span>|<span data-ttu-id="e204c-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="e204c-112">Boolean</span></span>|<span data-ttu-id="e204c-113">登録で対象プラットフォームをブロックします</span><span class="sxs-lookup"><span data-stu-id="e204c-113">Block the platform from enrolling</span></span>|
|<span data-ttu-id="e204c-114">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="e204c-114">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="e204c-115">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="e204c-115">Boolean</span></span>|<span data-ttu-id="e204c-116">個人所有のデバイスの登録をブロックします</span><span class="sxs-lookup"><span data-stu-id="e204c-116">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="e204c-117">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="e204c-117">osMinimumVersion</span></span>|<span data-ttu-id="e204c-118">String</span><span class="sxs-lookup"><span data-stu-id="e204c-118">String</span></span>|<span data-ttu-id="e204c-119">サポートされる最小 OS バージョン</span><span class="sxs-lookup"><span data-stu-id="e204c-119">Min OS version supported</span></span>|
|<span data-ttu-id="e204c-120">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="e204c-120">osMaximumVersion</span></span>|<span data-ttu-id="e204c-121">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e204c-121">String</span></span>|<span data-ttu-id="e204c-122">サポートされる最大 OS バージョン</span><span class="sxs-lookup"><span data-stu-id="e204c-122">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="e204c-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e204c-123">Relationships</span></span>
<span data-ttu-id="e204c-124">なし</span><span class="sxs-lookup"><span data-stu-id="e204c-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e204c-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e204c-125">JSON Representation</span></span>
<span data-ttu-id="e204c-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e204c-126">Here is a JSON representation of the resource.</span></span>
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




