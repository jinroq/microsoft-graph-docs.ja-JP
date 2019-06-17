---
title: iosDeviceType リソースの種類
description: モバイル アプリを実行できる iOS デバイスの種類のプロパティが含まれます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d9751d541b0bcb64b68673aa8ca646fb85e70b5f
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991304"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="c1df0-103">iosDeviceType リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c1df0-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="c1df0-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c1df0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1df0-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c1df0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1df0-106">モバイル アプリを実行できる iOS デバイスの種類のプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="c1df0-106">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="c1df0-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1df0-107">Properties</span></span>
|<span data-ttu-id="c1df0-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1df0-108">Property</span></span>|<span data-ttu-id="c1df0-109">型</span><span class="sxs-lookup"><span data-stu-id="c1df0-109">Type</span></span>|<span data-ttu-id="c1df0-110">説明</span><span class="sxs-lookup"><span data-stu-id="c1df0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1df0-111">iPad</span><span class="sxs-lookup"><span data-stu-id="c1df0-111">iPad</span></span>|<span data-ttu-id="c1df0-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1df0-112">Boolean</span></span>|<span data-ttu-id="c1df0-113">アプリを iPad で実行できるかどうか。</span><span class="sxs-lookup"><span data-stu-id="c1df0-113">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="c1df0-114">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="c1df0-114">iPhoneAndIPod</span></span>|<span data-ttu-id="c1df0-115">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="c1df0-115">Boolean</span></span>|<span data-ttu-id="c1df0-116">アプリを iPhone および iPod で実行できるかどうか。</span><span class="sxs-lookup"><span data-stu-id="c1df0-116">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1df0-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c1df0-117">Relationships</span></span>
<span data-ttu-id="c1df0-118">なし</span><span class="sxs-lookup"><span data-stu-id="c1df0-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1df0-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c1df0-119">JSON Representation</span></span>
<span data-ttu-id="c1df0-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c1df0-120">Here is a JSON representation of the resource.</span></span>
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





