---
title: deviceEnrollmentPlatformRestriction リソースの種類
description: プラットフォーム固有の登録の制限
ms.openlocfilehash: 823eecc37dc8ee4536d5cb63213f2bb80ca5138d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072607"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="8fbed-103">deviceEnrollmentPlatformRestriction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8fbed-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="8fbed-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8fbed-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8fbed-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8fbed-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8fbed-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8fbed-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8fbed-107">プラットフォーム固有の登録の制限</span><span class="sxs-lookup"><span data-stu-id="8fbed-107">Platform specific enrollment restrictions</span></span>
## <a name="properties"></a><span data-ttu-id="8fbed-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8fbed-108">Properties</span></span>
|<span data-ttu-id="8fbed-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8fbed-109">Property</span></span>|<span data-ttu-id="8fbed-110">型</span><span class="sxs-lookup"><span data-stu-id="8fbed-110">Type</span></span>|<span data-ttu-id="8fbed-111">説明</span><span class="sxs-lookup"><span data-stu-id="8fbed-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fbed-112">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="8fbed-112">platformBlocked</span></span>|<span data-ttu-id="8fbed-113">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="8fbed-113">Boolean</span></span>|<span data-ttu-id="8fbed-114">登録で対象プラットフォームをブロックします</span><span class="sxs-lookup"><span data-stu-id="8fbed-114">Block the platform from enrolling</span></span>|
|<span data-ttu-id="8fbed-115">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="8fbed-115">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="8fbed-116">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="8fbed-116">Boolean</span></span>|<span data-ttu-id="8fbed-117">個人所有のデバイスの登録をブロックします</span><span class="sxs-lookup"><span data-stu-id="8fbed-117">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="8fbed-118">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="8fbed-118">osMinimumVersion</span></span>|<span data-ttu-id="8fbed-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="8fbed-119">String</span></span>|<span data-ttu-id="8fbed-120">サポートされる最小 OS バージョン</span><span class="sxs-lookup"><span data-stu-id="8fbed-120">Min OS version supported</span></span>|
|<span data-ttu-id="8fbed-121">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="8fbed-121">osMaximumVersion</span></span>|<span data-ttu-id="8fbed-122">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="8fbed-122">String</span></span>|<span data-ttu-id="8fbed-123">サポートされる最大 OS バージョン</span><span class="sxs-lookup"><span data-stu-id="8fbed-123">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="8fbed-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8fbed-124">Relationships</span></span>
<span data-ttu-id="8fbed-125">なし</span><span class="sxs-lookup"><span data-stu-id="8fbed-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8fbed-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8fbed-126">JSON Representation</span></span>
<span data-ttu-id="8fbed-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8fbed-127">Here is a JSON representation of the resource.</span></span>
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





