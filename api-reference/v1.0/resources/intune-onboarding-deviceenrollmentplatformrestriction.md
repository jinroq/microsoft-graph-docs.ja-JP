---
title: deviceEnrollmentPlatformRestriction リソースの種類
description: プラットフォーム固有の登録の制限
ms.openlocfilehash: b6d4ea3acf4995548fce7f2c86b3c95c444b59b5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024235"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="2d2b0-103">deviceEnrollmentPlatformRestriction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2d2b0-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="2d2b0-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2d2b0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2d2b0-105">プラットフォーム固有の登録の制限</span><span class="sxs-lookup"><span data-stu-id="2d2b0-105">Platform specific enrollment restrictions</span></span>
## <a name="properties"></a><span data-ttu-id="2d2b0-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2d2b0-106">Properties</span></span>
|<span data-ttu-id="2d2b0-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2d2b0-107">Property</span></span>|<span data-ttu-id="2d2b0-108">型</span><span class="sxs-lookup"><span data-stu-id="2d2b0-108">Type</span></span>|<span data-ttu-id="2d2b0-109">説明</span><span class="sxs-lookup"><span data-stu-id="2d2b0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d2b0-110">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="2d2b0-110">platformBlocked</span></span>|<span data-ttu-id="2d2b0-111">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="2d2b0-111">Boolean</span></span>|<span data-ttu-id="2d2b0-112">登録で対象プラットフォームをブロックします</span><span class="sxs-lookup"><span data-stu-id="2d2b0-112">Block the platform from enrolling</span></span>|
|<span data-ttu-id="2d2b0-113">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="2d2b0-113">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="2d2b0-114">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="2d2b0-114">Boolean</span></span>|<span data-ttu-id="2d2b0-115">個人所有のデバイスの登録をブロックします</span><span class="sxs-lookup"><span data-stu-id="2d2b0-115">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="2d2b0-116">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="2d2b0-116">osMinimumVersion</span></span>|<span data-ttu-id="2d2b0-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="2d2b0-117">String</span></span>|<span data-ttu-id="2d2b0-118">サポートされる最小 OS バージョン</span><span class="sxs-lookup"><span data-stu-id="2d2b0-118">Min OS version supported</span></span>|
|<span data-ttu-id="2d2b0-119">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="2d2b0-119">osMaximumVersion</span></span>|<span data-ttu-id="2d2b0-120">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="2d2b0-120">String</span></span>|<span data-ttu-id="2d2b0-121">サポートされる最大 OS バージョン</span><span class="sxs-lookup"><span data-stu-id="2d2b0-121">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d2b0-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2d2b0-122">Relationships</span></span>
<span data-ttu-id="2d2b0-123">なし</span><span class="sxs-lookup"><span data-stu-id="2d2b0-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2d2b0-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2d2b0-124">JSON Representation</span></span>
<span data-ttu-id="2d2b0-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2d2b0-125">Here is a JSON representation of the resource.</span></span>
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



