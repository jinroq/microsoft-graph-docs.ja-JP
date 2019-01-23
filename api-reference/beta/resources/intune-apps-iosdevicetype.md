---
title: iosDeviceType リソースの種類
description: モバイル アプリを実行できる iOS デバイスの種類のプロパティが含まれます。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b68c7ce163dbf0f9232bf53d919ae84c7906c997
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395385"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="6c3d2-103">iosDeviceType リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6c3d2-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="6c3d2-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6c3d2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6c3d2-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c3d2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6c3d2-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6c3d2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c3d2-107">モバイル アプリを実行できる iOS デバイスの種類のプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="6c3d2-107">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="6c3d2-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c3d2-108">Properties</span></span>
|<span data-ttu-id="6c3d2-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c3d2-109">Property</span></span>|<span data-ttu-id="6c3d2-110">型</span><span class="sxs-lookup"><span data-stu-id="6c3d2-110">Type</span></span>|<span data-ttu-id="6c3d2-111">説明</span><span class="sxs-lookup"><span data-stu-id="6c3d2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c3d2-112">iPad</span><span class="sxs-lookup"><span data-stu-id="6c3d2-112">iPad</span></span>|<span data-ttu-id="6c3d2-113">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="6c3d2-113">Boolean</span></span>|<span data-ttu-id="6c3d2-114">アプリを iPad で実行できるかどうか。</span><span class="sxs-lookup"><span data-stu-id="6c3d2-114">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="6c3d2-115">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="6c3d2-115">iPhoneAndIPod</span></span>|<span data-ttu-id="6c3d2-116">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="6c3d2-116">Boolean</span></span>|<span data-ttu-id="6c3d2-117">アプリを iPhone および iPod で実行できるかどうか。</span><span class="sxs-lookup"><span data-stu-id="6c3d2-117">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c3d2-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6c3d2-118">Relationships</span></span>
<span data-ttu-id="6c3d2-119">なし</span><span class="sxs-lookup"><span data-stu-id="6c3d2-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c3d2-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6c3d2-120">JSON Representation</span></span>
<span data-ttu-id="6c3d2-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6c3d2-121">Here is a JSON representation of the resource.</span></span>
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




