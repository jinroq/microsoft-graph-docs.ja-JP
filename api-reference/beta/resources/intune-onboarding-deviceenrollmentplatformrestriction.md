---
title: deviceEnrollmentPlatformRestriction リソースの種類
description: プラットフォーム固有の登録の制限
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 009485c2051c47209074ae8b938e6b1b06de9eac
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843863"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="2fe57-103">deviceEnrollmentPlatformRestriction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2fe57-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="2fe57-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2fe57-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2fe57-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2fe57-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2fe57-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2fe57-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2fe57-107">プラットフォーム固有の登録の制限</span><span class="sxs-lookup"><span data-stu-id="2fe57-107">Platform specific enrollment restrictions</span></span>
## <a name="properties"></a><span data-ttu-id="2fe57-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2fe57-108">Properties</span></span>
|<span data-ttu-id="2fe57-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2fe57-109">Property</span></span>|<span data-ttu-id="2fe57-110">種類</span><span class="sxs-lookup"><span data-stu-id="2fe57-110">Type</span></span>|<span data-ttu-id="2fe57-111">説明</span><span class="sxs-lookup"><span data-stu-id="2fe57-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fe57-112">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="2fe57-112">platformBlocked</span></span>|<span data-ttu-id="2fe57-113">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="2fe57-113">Boolean</span></span>|<span data-ttu-id="2fe57-114">登録で対象プラットフォームをブロックします</span><span class="sxs-lookup"><span data-stu-id="2fe57-114">Block the platform from enrolling</span></span>|
|<span data-ttu-id="2fe57-115">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="2fe57-115">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="2fe57-116">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="2fe57-116">Boolean</span></span>|<span data-ttu-id="2fe57-117">個人所有のデバイスの登録をブロックします</span><span class="sxs-lookup"><span data-stu-id="2fe57-117">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="2fe57-118">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="2fe57-118">osMinimumVersion</span></span>|<span data-ttu-id="2fe57-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="2fe57-119">String</span></span>|<span data-ttu-id="2fe57-120">サポートされる最小 OS バージョン</span><span class="sxs-lookup"><span data-stu-id="2fe57-120">Min OS version supported</span></span>|
|<span data-ttu-id="2fe57-121">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="2fe57-121">osMaximumVersion</span></span>|<span data-ttu-id="2fe57-122">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="2fe57-122">String</span></span>|<span data-ttu-id="2fe57-123">サポートされる最大 OS バージョン</span><span class="sxs-lookup"><span data-stu-id="2fe57-123">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="2fe57-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2fe57-124">Relationships</span></span>
<span data-ttu-id="2fe57-125">なし</span><span class="sxs-lookup"><span data-stu-id="2fe57-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2fe57-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2fe57-126">JSON Representation</span></span>
<span data-ttu-id="2fe57-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2fe57-127">Here is a JSON representation of the resource.</span></span>
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





