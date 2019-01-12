---
title: iosDeviceType リソースの種類
description: モバイル アプリを実行できる iOS デバイスの種類のプロパティが含まれます。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2fe1f686052468bbab5d7115541a631b77073d6e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977165"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="c8ff1-103">iosDeviceType リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c8ff1-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="c8ff1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c8ff1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c8ff1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8ff1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c8ff1-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c8ff1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c8ff1-107">モバイル アプリを実行できる iOS デバイスの種類のプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="c8ff1-107">Contains properties of the possible iOS device types the mobile app can run on.</span></span>
## <a name="properties"></a><span data-ttu-id="c8ff1-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8ff1-108">Properties</span></span>
|<span data-ttu-id="c8ff1-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8ff1-109">Property</span></span>|<span data-ttu-id="c8ff1-110">種類</span><span class="sxs-lookup"><span data-stu-id="c8ff1-110">Type</span></span>|<span data-ttu-id="c8ff1-111">説明</span><span class="sxs-lookup"><span data-stu-id="c8ff1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8ff1-112">iPad</span><span class="sxs-lookup"><span data-stu-id="c8ff1-112">iPad</span></span>|<span data-ttu-id="c8ff1-113">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="c8ff1-113">Boolean</span></span>|<span data-ttu-id="c8ff1-114">アプリを iPad で実行できるかどうか。</span><span class="sxs-lookup"><span data-stu-id="c8ff1-114">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="c8ff1-115">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="c8ff1-115">iPhoneAndIPod</span></span>|<span data-ttu-id="c8ff1-116">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="c8ff1-116">Boolean</span></span>|<span data-ttu-id="c8ff1-117">アプリを iPhone および iPod で実行できるかどうか。</span><span class="sxs-lookup"><span data-stu-id="c8ff1-117">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8ff1-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c8ff1-118">Relationships</span></span>
<span data-ttu-id="c8ff1-119">なし</span><span class="sxs-lookup"><span data-stu-id="c8ff1-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c8ff1-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c8ff1-120">JSON Representation</span></span>
<span data-ttu-id="c8ff1-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c8ff1-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosDeviceType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosDeviceType",
  "iPad": true,
  "iPhoneAndIPod": true
}
```





