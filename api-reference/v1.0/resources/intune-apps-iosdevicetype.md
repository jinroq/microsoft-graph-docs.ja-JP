---
title: iosDeviceType リソースの種類
description: モバイル アプリを実行できる iOS デバイスの種類のプロパティが含まれます。
author: tfitzmac
ms.openlocfilehash: 3111bc4b5fc78f6ed60b4a241b48e443923f7159
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313602"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="3251c-103">iosDeviceType リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3251c-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="3251c-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3251c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3251c-105">モバイル アプリを実行できる iOS デバイスの種類のプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="3251c-105">Contains properties of the possible iOS device types the mobile app can run on.</span></span>
## <a name="properties"></a><span data-ttu-id="3251c-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3251c-106">Properties</span></span>
|<span data-ttu-id="3251c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3251c-107">Property</span></span>|<span data-ttu-id="3251c-108">種類</span><span class="sxs-lookup"><span data-stu-id="3251c-108">Type</span></span>|<span data-ttu-id="3251c-109">説明</span><span class="sxs-lookup"><span data-stu-id="3251c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3251c-110">iPad</span><span class="sxs-lookup"><span data-stu-id="3251c-110">iPad</span></span>|<span data-ttu-id="3251c-111">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="3251c-111">Boolean</span></span>|<span data-ttu-id="3251c-112">アプリを iPad で実行できるかどうか。</span><span class="sxs-lookup"><span data-stu-id="3251c-112">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="3251c-113">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="3251c-113">iPhoneAndIPod</span></span>|<span data-ttu-id="3251c-114">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="3251c-114">Boolean</span></span>|<span data-ttu-id="3251c-115">アプリを iPhone および iPod で実行できるかどうか。</span><span class="sxs-lookup"><span data-stu-id="3251c-115">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3251c-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3251c-116">Relationships</span></span>
<span data-ttu-id="3251c-117">なし</span><span class="sxs-lookup"><span data-stu-id="3251c-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3251c-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3251c-118">JSON Representation</span></span>
<span data-ttu-id="3251c-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3251c-119">Here is a JSON representation of the resource.</span></span>
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



