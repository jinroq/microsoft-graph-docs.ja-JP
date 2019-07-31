---
title: deviceEnrollmentPlatformRestriction リソースの種類
description: プラットフォーム固有の登録の制限
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3d0e881053d3b24bbfa12e627a4f21ded4049747
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998192"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="7094e-103">deviceEnrollmentPlatformRestriction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7094e-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="7094e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7094e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7094e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7094e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7094e-106">プラットフォーム固有の登録の制限</span><span class="sxs-lookup"><span data-stu-id="7094e-106">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="7094e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7094e-107">Properties</span></span>
|<span data-ttu-id="7094e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7094e-108">Property</span></span>|<span data-ttu-id="7094e-109">型</span><span class="sxs-lookup"><span data-stu-id="7094e-109">Type</span></span>|<span data-ttu-id="7094e-110">説明</span><span class="sxs-lookup"><span data-stu-id="7094e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7094e-111">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="7094e-111">platformBlocked</span></span>|<span data-ttu-id="7094e-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="7094e-112">Boolean</span></span>|<span data-ttu-id="7094e-113">登録で対象プラットフォームをブロックします</span><span class="sxs-lookup"><span data-stu-id="7094e-113">Block the platform from enrolling</span></span>|
|<span data-ttu-id="7094e-114">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="7094e-114">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="7094e-115">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="7094e-115">Boolean</span></span>|<span data-ttu-id="7094e-116">個人所有のデバイスの登録をブロックします</span><span class="sxs-lookup"><span data-stu-id="7094e-116">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="7094e-117">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="7094e-117">osMinimumVersion</span></span>|<span data-ttu-id="7094e-118">String</span><span class="sxs-lookup"><span data-stu-id="7094e-118">String</span></span>|<span data-ttu-id="7094e-119">サポートされる最小 OS バージョン</span><span class="sxs-lookup"><span data-stu-id="7094e-119">Min OS version supported</span></span>|
|<span data-ttu-id="7094e-120">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="7094e-120">osMaximumVersion</span></span>|<span data-ttu-id="7094e-121">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="7094e-121">String</span></span>|<span data-ttu-id="7094e-122">サポートされる最大 OS バージョン</span><span class="sxs-lookup"><span data-stu-id="7094e-122">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="7094e-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7094e-123">Relationships</span></span>
<span data-ttu-id="7094e-124">なし</span><span class="sxs-lookup"><span data-stu-id="7094e-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7094e-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7094e-125">JSON Representation</span></span>
<span data-ttu-id="7094e-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7094e-126">Here is a JSON representation of the resource.</span></span>
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





