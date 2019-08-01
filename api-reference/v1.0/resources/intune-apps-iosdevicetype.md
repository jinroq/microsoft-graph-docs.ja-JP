---
title: iosDeviceType リソースの種類
description: モバイル アプリを実行できる iOS デバイスの種類のプロパティが含まれます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 23d38faeafd9aac0d0e547596de51507b6932c20
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029164"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="cee85-103">iosDeviceType リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cee85-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="cee85-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cee85-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cee85-105">モバイル アプリを実行できる iOS デバイスの種類のプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="cee85-105">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="cee85-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cee85-106">Properties</span></span>
|<span data-ttu-id="cee85-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cee85-107">Property</span></span>|<span data-ttu-id="cee85-108">型</span><span class="sxs-lookup"><span data-stu-id="cee85-108">Type</span></span>|<span data-ttu-id="cee85-109">説明</span><span class="sxs-lookup"><span data-stu-id="cee85-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cee85-110">iPad</span><span class="sxs-lookup"><span data-stu-id="cee85-110">iPad</span></span>|<span data-ttu-id="cee85-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="cee85-111">Boolean</span></span>|<span data-ttu-id="cee85-112">アプリを iPad で実行できるかどうか。</span><span class="sxs-lookup"><span data-stu-id="cee85-112">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="cee85-113">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="cee85-113">iPhoneAndIPod</span></span>|<span data-ttu-id="cee85-114">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="cee85-114">Boolean</span></span>|<span data-ttu-id="cee85-115">アプリを iPhone および iPod で実行できるかどうか。</span><span class="sxs-lookup"><span data-stu-id="cee85-115">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cee85-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cee85-116">Relationships</span></span>
<span data-ttu-id="cee85-117">なし</span><span class="sxs-lookup"><span data-stu-id="cee85-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cee85-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cee85-118">JSON Representation</span></span>
<span data-ttu-id="cee85-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cee85-119">Here is a JSON representation of the resource.</span></span>
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



