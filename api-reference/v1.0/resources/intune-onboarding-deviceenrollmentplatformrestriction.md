---
title: deviceEnrollmentPlatformRestriction リソースの種類
description: プラットフォーム固有の登録の制限
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7879b7f6585908aa760c3169e950cc5257bf49a7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929068"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="da0f1-103">deviceEnrollmentPlatformRestriction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="da0f1-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="da0f1-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="da0f1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="da0f1-105">プラットフォーム固有の登録の制限</span><span class="sxs-lookup"><span data-stu-id="da0f1-105">Platform specific enrollment restrictions</span></span>
## <a name="properties"></a><span data-ttu-id="da0f1-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="da0f1-106">Properties</span></span>
|<span data-ttu-id="da0f1-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="da0f1-107">Property</span></span>|<span data-ttu-id="da0f1-108">種類</span><span class="sxs-lookup"><span data-stu-id="da0f1-108">Type</span></span>|<span data-ttu-id="da0f1-109">説明</span><span class="sxs-lookup"><span data-stu-id="da0f1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da0f1-110">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="da0f1-110">platformBlocked</span></span>|<span data-ttu-id="da0f1-111">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="da0f1-111">Boolean</span></span>|<span data-ttu-id="da0f1-112">登録で対象プラットフォームをブロックします</span><span class="sxs-lookup"><span data-stu-id="da0f1-112">Block the platform from enrolling</span></span>|
|<span data-ttu-id="da0f1-113">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="da0f1-113">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="da0f1-114">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="da0f1-114">Boolean</span></span>|<span data-ttu-id="da0f1-115">個人所有のデバイスの登録をブロックします</span><span class="sxs-lookup"><span data-stu-id="da0f1-115">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="da0f1-116">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="da0f1-116">osMinimumVersion</span></span>|<span data-ttu-id="da0f1-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="da0f1-117">String</span></span>|<span data-ttu-id="da0f1-118">サポートされる最小 OS バージョン</span><span class="sxs-lookup"><span data-stu-id="da0f1-118">Min OS version supported</span></span>|
|<span data-ttu-id="da0f1-119">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="da0f1-119">osMaximumVersion</span></span>|<span data-ttu-id="da0f1-120">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="da0f1-120">String</span></span>|<span data-ttu-id="da0f1-121">サポートされる最大 OS バージョン</span><span class="sxs-lookup"><span data-stu-id="da0f1-121">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="da0f1-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="da0f1-122">Relationships</span></span>
<span data-ttu-id="da0f1-123">なし</span><span class="sxs-lookup"><span data-stu-id="da0f1-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="da0f1-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="da0f1-124">JSON Representation</span></span>
<span data-ttu-id="da0f1-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="da0f1-125">Here is a JSON representation of the resource.</span></span>
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



