---
title: deviceEnrollmentPlatformRestriction リソースの種類
description: プラットフォーム固有の登録の制限
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e8ba3306c5a4af4dfbb8b97e4d4794b917ebbf64
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31806455"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="fadf4-103">deviceEnrollmentPlatformRestriction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fadf4-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="fadf4-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fadf4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fadf4-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fadf4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fadf4-106">プラットフォーム固有の登録の制限</span><span class="sxs-lookup"><span data-stu-id="fadf4-106">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="fadf4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fadf4-107">Properties</span></span>
|<span data-ttu-id="fadf4-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fadf4-108">Property</span></span>|<span data-ttu-id="fadf4-109">型</span><span class="sxs-lookup"><span data-stu-id="fadf4-109">Type</span></span>|<span data-ttu-id="fadf4-110">説明</span><span class="sxs-lookup"><span data-stu-id="fadf4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fadf4-111">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="fadf4-111">platformBlocked</span></span>|<span data-ttu-id="fadf4-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="fadf4-112">Boolean</span></span>|<span data-ttu-id="fadf4-113">登録で対象プラットフォームをブロックします</span><span class="sxs-lookup"><span data-stu-id="fadf4-113">Block the platform from enrolling</span></span>|
|<span data-ttu-id="fadf4-114">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="fadf4-114">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="fadf4-115">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="fadf4-115">Boolean</span></span>|<span data-ttu-id="fadf4-116">個人所有のデバイスの登録をブロックします</span><span class="sxs-lookup"><span data-stu-id="fadf4-116">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="fadf4-117">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="fadf4-117">osMinimumVersion</span></span>|<span data-ttu-id="fadf4-118">文字列</span><span class="sxs-lookup"><span data-stu-id="fadf4-118">String</span></span>|<span data-ttu-id="fadf4-119">サポートされる最小 OS バージョン</span><span class="sxs-lookup"><span data-stu-id="fadf4-119">Min OS version supported</span></span>|
|<span data-ttu-id="fadf4-120">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="fadf4-120">osMaximumVersion</span></span>|<span data-ttu-id="fadf4-121">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="fadf4-121">String</span></span>|<span data-ttu-id="fadf4-122">サポートされる最大 OS バージョン</span><span class="sxs-lookup"><span data-stu-id="fadf4-122">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="fadf4-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fadf4-123">Relationships</span></span>
<span data-ttu-id="fadf4-124">なし</span><span class="sxs-lookup"><span data-stu-id="fadf4-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fadf4-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fadf4-125">JSON Representation</span></span>
<span data-ttu-id="fadf4-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fadf4-126">Here is a JSON representation of the resource.</span></span>
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





