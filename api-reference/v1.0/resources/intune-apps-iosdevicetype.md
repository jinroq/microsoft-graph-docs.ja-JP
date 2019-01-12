---
title: iosDeviceType リソースの種類
description: モバイル アプリを実行できる iOS デバイスの種類のプロパティが含まれます。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b541310ced9c9aaa781077639203950d00f56f27
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976752"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="84466-103">iosDeviceType リソースの種類</span><span class="sxs-lookup"><span data-stu-id="84466-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="84466-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="84466-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84466-105">モバイル アプリを実行できる iOS デバイスの種類のプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="84466-105">Contains properties of the possible iOS device types the mobile app can run on.</span></span>
## <a name="properties"></a><span data-ttu-id="84466-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="84466-106">Properties</span></span>
|<span data-ttu-id="84466-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="84466-107">Property</span></span>|<span data-ttu-id="84466-108">型</span><span class="sxs-lookup"><span data-stu-id="84466-108">Type</span></span>|<span data-ttu-id="84466-109">説明</span><span class="sxs-lookup"><span data-stu-id="84466-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84466-110">iPad</span><span class="sxs-lookup"><span data-stu-id="84466-110">iPad</span></span>|<span data-ttu-id="84466-111">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="84466-111">Boolean</span></span>|<span data-ttu-id="84466-112">アプリを iPad で実行できるかどうか。</span><span class="sxs-lookup"><span data-stu-id="84466-112">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="84466-113">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="84466-113">iPhoneAndIPod</span></span>|<span data-ttu-id="84466-114">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="84466-114">Boolean</span></span>|<span data-ttu-id="84466-115">アプリを iPhone および iPod で実行できるかどうか。</span><span class="sxs-lookup"><span data-stu-id="84466-115">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="84466-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="84466-116">Relationships</span></span>
<span data-ttu-id="84466-117">なし</span><span class="sxs-lookup"><span data-stu-id="84466-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="84466-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="84466-118">JSON Representation</span></span>
<span data-ttu-id="84466-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="84466-119">Here is a JSON representation of the resource.</span></span>
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



