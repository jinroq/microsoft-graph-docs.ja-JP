---
title: deviceEnrollmentPlatformRestriction リソースの種類
description: プラットフォーム固有の登録の制限
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ce30b9ff24067fb2bfec17ad85d3c8827cc6b798
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816003"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="8dd0b-103">deviceEnrollmentPlatformRestriction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8dd0b-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="8dd0b-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8dd0b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8dd0b-105">プラットフォーム固有の登録の制限</span><span class="sxs-lookup"><span data-stu-id="8dd0b-105">Platform specific enrollment restrictions</span></span>
## <a name="properties"></a><span data-ttu-id="8dd0b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8dd0b-106">Properties</span></span>
|<span data-ttu-id="8dd0b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8dd0b-107">Property</span></span>|<span data-ttu-id="8dd0b-108">種類</span><span class="sxs-lookup"><span data-stu-id="8dd0b-108">Type</span></span>|<span data-ttu-id="8dd0b-109">説明</span><span class="sxs-lookup"><span data-stu-id="8dd0b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8dd0b-110">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="8dd0b-110">platformBlocked</span></span>|<span data-ttu-id="8dd0b-111">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="8dd0b-111">Boolean</span></span>|<span data-ttu-id="8dd0b-112">登録で対象プラットフォームをブロックします</span><span class="sxs-lookup"><span data-stu-id="8dd0b-112">Block the platform from enrolling</span></span>|
|<span data-ttu-id="8dd0b-113">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="8dd0b-113">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="8dd0b-114">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="8dd0b-114">Boolean</span></span>|<span data-ttu-id="8dd0b-115">個人所有のデバイスの登録をブロックします</span><span class="sxs-lookup"><span data-stu-id="8dd0b-115">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="8dd0b-116">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="8dd0b-116">osMinimumVersion</span></span>|<span data-ttu-id="8dd0b-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="8dd0b-117">String</span></span>|<span data-ttu-id="8dd0b-118">サポートされる最小 OS バージョン</span><span class="sxs-lookup"><span data-stu-id="8dd0b-118">Min OS version supported</span></span>|
|<span data-ttu-id="8dd0b-119">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="8dd0b-119">osMaximumVersion</span></span>|<span data-ttu-id="8dd0b-120">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="8dd0b-120">String</span></span>|<span data-ttu-id="8dd0b-121">サポートされる最大 OS バージョン</span><span class="sxs-lookup"><span data-stu-id="8dd0b-121">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="8dd0b-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8dd0b-122">Relationships</span></span>
<span data-ttu-id="8dd0b-123">なし</span><span class="sxs-lookup"><span data-stu-id="8dd0b-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8dd0b-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8dd0b-124">JSON Representation</span></span>
<span data-ttu-id="8dd0b-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8dd0b-125">Here is a JSON representation of the resource.</span></span>
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



