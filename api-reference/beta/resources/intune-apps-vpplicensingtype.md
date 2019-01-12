---
title: vppLicensingType リソースの種類
description: iOS Volume-Purchase Program (VPP) ライセンスの種類のプロパティが含まれます。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 47ee634c8fa488bb27c6c0a4beb7728fc7e427cb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948682"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="2ab34-103">vppLicensingType リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2ab34-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="2ab34-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2ab34-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2ab34-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ab34-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2ab34-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2ab34-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2ab34-107">iOS Volume-Purchase Program (VPP) ライセンスの種類のプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="2ab34-107">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>
## <a name="properties"></a><span data-ttu-id="2ab34-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ab34-108">Properties</span></span>
|<span data-ttu-id="2ab34-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ab34-109">Property</span></span>|<span data-ttu-id="2ab34-110">種類</span><span class="sxs-lookup"><span data-stu-id="2ab34-110">Type</span></span>|<span data-ttu-id="2ab34-111">説明</span><span class="sxs-lookup"><span data-stu-id="2ab34-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ab34-112">supportUserLicensing</span><span class="sxs-lookup"><span data-stu-id="2ab34-112">supportUserLicensing</span></span>|<span data-ttu-id="2ab34-113">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="2ab34-113">Boolean</span></span>|<span data-ttu-id="2ab34-114">プログラムがユーザー ライセンスの種類をサポートするかどうか。</span><span class="sxs-lookup"><span data-stu-id="2ab34-114">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="2ab34-115">supportDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="2ab34-115">supportDeviceLicensing</span></span>|<span data-ttu-id="2ab34-116">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="2ab34-116">Boolean</span></span>|<span data-ttu-id="2ab34-117">プログラムがデバイス ライセンスの種類をサポートするかどうか。</span><span class="sxs-lookup"><span data-stu-id="2ab34-117">Whether the program supports the device licensing type.</span></span>|
|<span data-ttu-id="2ab34-118">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="2ab34-118">supportsUserLicensing</span></span>|<span data-ttu-id="2ab34-119">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="2ab34-119">Boolean</span></span>|<span data-ttu-id="2ab34-120">プログラムがユーザー ライセンスの種類をサポートするかどうか。</span><span class="sxs-lookup"><span data-stu-id="2ab34-120">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="2ab34-121">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="2ab34-121">supportsDeviceLicensing</span></span>|<span data-ttu-id="2ab34-122">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="2ab34-122">Boolean</span></span>|<span data-ttu-id="2ab34-123">プログラムがデバイス ライセンスの種類をサポートするかどうか。</span><span class="sxs-lookup"><span data-stu-id="2ab34-123">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ab34-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2ab34-124">Relationships</span></span>
<span data-ttu-id="2ab34-125">なし</span><span class="sxs-lookup"><span data-stu-id="2ab34-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2ab34-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2ab34-126">JSON Representation</span></span>
<span data-ttu-id="2ab34-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2ab34-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppLicensingType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppLicensingType",
  "supportUserLicensing": true,
  "supportDeviceLicensing": true,
  "supportsUserLicensing": true,
  "supportsDeviceLicensing": true
}
```





