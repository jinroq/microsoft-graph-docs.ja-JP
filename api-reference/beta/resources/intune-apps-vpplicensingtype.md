---
title: vppLicensingType リソースの種類
description: iOS Volume-Purchase Program (VPP) ライセンスの種類のプロパティが含まれます。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5d4b7983d20f22be5f8cce24a5c362926d00de55
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851598"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="a3230-103">vppLicensingType リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a3230-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="a3230-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a3230-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a3230-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3230-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a3230-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a3230-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a3230-107">iOS Volume-Purchase Program (VPP) ライセンスの種類のプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="a3230-107">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>
## <a name="properties"></a><span data-ttu-id="a3230-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a3230-108">Properties</span></span>
|<span data-ttu-id="a3230-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a3230-109">Property</span></span>|<span data-ttu-id="a3230-110">種類</span><span class="sxs-lookup"><span data-stu-id="a3230-110">Type</span></span>|<span data-ttu-id="a3230-111">説明</span><span class="sxs-lookup"><span data-stu-id="a3230-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3230-112">supportUserLicensing</span><span class="sxs-lookup"><span data-stu-id="a3230-112">supportUserLicensing</span></span>|<span data-ttu-id="a3230-113">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="a3230-113">Boolean</span></span>|<span data-ttu-id="a3230-114">プログラムがユーザー ライセンスの種類をサポートするかどうか。</span><span class="sxs-lookup"><span data-stu-id="a3230-114">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="a3230-115">supportDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="a3230-115">supportDeviceLicensing</span></span>|<span data-ttu-id="a3230-116">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="a3230-116">Boolean</span></span>|<span data-ttu-id="a3230-117">プログラムがデバイス ライセンスの種類をサポートするかどうか。</span><span class="sxs-lookup"><span data-stu-id="a3230-117">Whether the program supports the device licensing type.</span></span>|
|<span data-ttu-id="a3230-118">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="a3230-118">supportsUserLicensing</span></span>|<span data-ttu-id="a3230-119">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="a3230-119">Boolean</span></span>|<span data-ttu-id="a3230-120">プログラムがユーザー ライセンスの種類をサポートするかどうか。</span><span class="sxs-lookup"><span data-stu-id="a3230-120">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="a3230-121">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="a3230-121">supportsDeviceLicensing</span></span>|<span data-ttu-id="a3230-122">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="a3230-122">Boolean</span></span>|<span data-ttu-id="a3230-123">プログラムがデバイス ライセンスの種類をサポートするかどうか。</span><span class="sxs-lookup"><span data-stu-id="a3230-123">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3230-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a3230-124">Relationships</span></span>
<span data-ttu-id="a3230-125">なし</span><span class="sxs-lookup"><span data-stu-id="a3230-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a3230-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a3230-126">JSON Representation</span></span>
<span data-ttu-id="a3230-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a3230-127">Here is a JSON representation of the resource.</span></span>
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





