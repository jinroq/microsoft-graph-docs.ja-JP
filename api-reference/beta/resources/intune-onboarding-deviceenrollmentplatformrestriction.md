---
title: deviceEnrollmentPlatformRestriction リソースの種類
description: プラットフォーム固有の登録の制限
author: tfitzmac
ms.openlocfilehash: 22401c83b3e68d66a2bd7a39359602e2aca0a932
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304124"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="1a645-103">deviceEnrollmentPlatformRestriction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1a645-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="1a645-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1a645-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1a645-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a645-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1a645-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1a645-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1a645-107">プラットフォーム固有の登録の制限</span><span class="sxs-lookup"><span data-stu-id="1a645-107">Platform specific enrollment restrictions</span></span>
## <a name="properties"></a><span data-ttu-id="1a645-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1a645-108">Properties</span></span>
|<span data-ttu-id="1a645-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1a645-109">Property</span></span>|<span data-ttu-id="1a645-110">種類</span><span class="sxs-lookup"><span data-stu-id="1a645-110">Type</span></span>|<span data-ttu-id="1a645-111">説明</span><span class="sxs-lookup"><span data-stu-id="1a645-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a645-112">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="1a645-112">platformBlocked</span></span>|<span data-ttu-id="1a645-113">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="1a645-113">Boolean</span></span>|<span data-ttu-id="1a645-114">登録で対象プラットフォームをブロックします</span><span class="sxs-lookup"><span data-stu-id="1a645-114">Block the platform from enrolling</span></span>|
|<span data-ttu-id="1a645-115">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="1a645-115">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="1a645-116">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="1a645-116">Boolean</span></span>|<span data-ttu-id="1a645-117">個人所有のデバイスの登録をブロックします</span><span class="sxs-lookup"><span data-stu-id="1a645-117">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="1a645-118">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="1a645-118">osMinimumVersion</span></span>|<span data-ttu-id="1a645-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="1a645-119">String</span></span>|<span data-ttu-id="1a645-120">サポートされる最小 OS バージョン</span><span class="sxs-lookup"><span data-stu-id="1a645-120">Min OS version supported</span></span>|
|<span data-ttu-id="1a645-121">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="1a645-121">osMaximumVersion</span></span>|<span data-ttu-id="1a645-122">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="1a645-122">String</span></span>|<span data-ttu-id="1a645-123">サポートされる最大 OS バージョン</span><span class="sxs-lookup"><span data-stu-id="1a645-123">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a645-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1a645-124">Relationships</span></span>
<span data-ttu-id="1a645-125">なし</span><span class="sxs-lookup"><span data-stu-id="1a645-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1a645-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1a645-126">JSON Representation</span></span>
<span data-ttu-id="1a645-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1a645-127">Here is a JSON representation of the resource.</span></span>
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





