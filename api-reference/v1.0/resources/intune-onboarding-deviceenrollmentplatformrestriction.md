---
title: deviceEnrollmentPlatformRestriction リソースの種類
description: プラットフォーム固有の登録の制限
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 380e40f04c21bb4276c859597610fa3af769fd11
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037521"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="ada35-103">deviceEnrollmentPlatformRestriction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ada35-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="ada35-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ada35-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ada35-105">プラットフォーム固有の登録の制限</span><span class="sxs-lookup"><span data-stu-id="ada35-105">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="ada35-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ada35-106">Properties</span></span>
|<span data-ttu-id="ada35-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ada35-107">Property</span></span>|<span data-ttu-id="ada35-108">型</span><span class="sxs-lookup"><span data-stu-id="ada35-108">Type</span></span>|<span data-ttu-id="ada35-109">説明</span><span class="sxs-lookup"><span data-stu-id="ada35-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ada35-110">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="ada35-110">platformBlocked</span></span>|<span data-ttu-id="ada35-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="ada35-111">Boolean</span></span>|<span data-ttu-id="ada35-112">登録で対象プラットフォームをブロックします</span><span class="sxs-lookup"><span data-stu-id="ada35-112">Block the platform from enrolling</span></span>|
|<span data-ttu-id="ada35-113">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="ada35-113">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="ada35-114">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="ada35-114">Boolean</span></span>|<span data-ttu-id="ada35-115">個人所有のデバイスの登録をブロックします</span><span class="sxs-lookup"><span data-stu-id="ada35-115">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="ada35-116">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="ada35-116">osMinimumVersion</span></span>|<span data-ttu-id="ada35-117">String</span><span class="sxs-lookup"><span data-stu-id="ada35-117">String</span></span>|<span data-ttu-id="ada35-118">サポートされる最小 OS バージョン</span><span class="sxs-lookup"><span data-stu-id="ada35-118">Min OS version supported</span></span>|
|<span data-ttu-id="ada35-119">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="ada35-119">osMaximumVersion</span></span>|<span data-ttu-id="ada35-120">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ada35-120">String</span></span>|<span data-ttu-id="ada35-121">サポートされる最大 OS バージョン</span><span class="sxs-lookup"><span data-stu-id="ada35-121">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="ada35-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ada35-122">Relationships</span></span>
<span data-ttu-id="ada35-123">なし</span><span class="sxs-lookup"><span data-stu-id="ada35-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ada35-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ada35-124">JSON Representation</span></span>
<span data-ttu-id="ada35-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ada35-125">Here is a JSON representation of the resource.</span></span>
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



