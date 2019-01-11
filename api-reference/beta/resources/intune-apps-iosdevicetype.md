---
title: iosDeviceType リソースの種類
description: モバイル アプリを実行できる iOS デバイスの種類のプロパティが含まれます。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8d475b129fa74439c1d5876b96579d556540177f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884883"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="f89bb-103">iosDeviceType リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f89bb-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="f89bb-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f89bb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f89bb-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f89bb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f89bb-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f89bb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f89bb-107">モバイル アプリを実行できる iOS デバイスの種類のプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="f89bb-107">Contains properties of the possible iOS device types the mobile app can run on.</span></span>
## <a name="properties"></a><span data-ttu-id="f89bb-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f89bb-108">Properties</span></span>
|<span data-ttu-id="f89bb-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f89bb-109">Property</span></span>|<span data-ttu-id="f89bb-110">種類</span><span class="sxs-lookup"><span data-stu-id="f89bb-110">Type</span></span>|<span data-ttu-id="f89bb-111">説明</span><span class="sxs-lookup"><span data-stu-id="f89bb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f89bb-112">iPad</span><span class="sxs-lookup"><span data-stu-id="f89bb-112">iPad</span></span>|<span data-ttu-id="f89bb-113">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="f89bb-113">Boolean</span></span>|<span data-ttu-id="f89bb-114">アプリを iPad で実行できるかどうか。</span><span class="sxs-lookup"><span data-stu-id="f89bb-114">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="f89bb-115">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="f89bb-115">iPhoneAndIPod</span></span>|<span data-ttu-id="f89bb-116">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="f89bb-116">Boolean</span></span>|<span data-ttu-id="f89bb-117">アプリを iPhone および iPod で実行できるかどうか。</span><span class="sxs-lookup"><span data-stu-id="f89bb-117">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f89bb-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f89bb-118">Relationships</span></span>
<span data-ttu-id="f89bb-119">なし</span><span class="sxs-lookup"><span data-stu-id="f89bb-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f89bb-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f89bb-120">JSON Representation</span></span>
<span data-ttu-id="f89bb-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f89bb-121">Here is a JSON representation of the resource.</span></span>
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





