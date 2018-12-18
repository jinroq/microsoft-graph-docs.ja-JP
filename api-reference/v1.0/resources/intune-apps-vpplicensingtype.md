---
title: vppLicensingType リソースの種類
description: iOS Volume-Purchase Program (VPP) ライセンスの種類のプロパティが含まれます。
author: tfitzmac
ms.openlocfilehash: 7958266fe208e0a04bc72ab658291c58455c763b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322562"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="22d27-103">vppLicensingType リソースの種類</span><span class="sxs-lookup"><span data-stu-id="22d27-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="22d27-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="22d27-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="22d27-105">iOS Volume-Purchase Program (VPP) ライセンスの種類のプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="22d27-105">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>
## <a name="properties"></a><span data-ttu-id="22d27-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22d27-106">Properties</span></span>
|<span data-ttu-id="22d27-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22d27-107">Property</span></span>|<span data-ttu-id="22d27-108">種類</span><span class="sxs-lookup"><span data-stu-id="22d27-108">Type</span></span>|<span data-ttu-id="22d27-109">説明</span><span class="sxs-lookup"><span data-stu-id="22d27-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22d27-110">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="22d27-110">supportsUserLicensing</span></span>|<span data-ttu-id="22d27-111">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="22d27-111">Boolean</span></span>|<span data-ttu-id="22d27-112">プログラムがユーザー ライセンスの種類をサポートするかどうか。</span><span class="sxs-lookup"><span data-stu-id="22d27-112">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="22d27-113">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="22d27-113">supportsDeviceLicensing</span></span>|<span data-ttu-id="22d27-114">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="22d27-114">Boolean</span></span>|<span data-ttu-id="22d27-115">プログラムがデバイス ライセンスの種類をサポートするかどうか。</span><span class="sxs-lookup"><span data-stu-id="22d27-115">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="22d27-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="22d27-116">Relationships</span></span>
<span data-ttu-id="22d27-117">なし</span><span class="sxs-lookup"><span data-stu-id="22d27-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="22d27-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="22d27-118">JSON Representation</span></span>
<span data-ttu-id="22d27-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="22d27-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppLicensingType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppLicensingType",
  "supportsUserLicensing": true,
  "supportsDeviceLicensing": true
}
```



