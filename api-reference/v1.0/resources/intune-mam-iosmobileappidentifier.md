---
title: iosMobileAppIdentifier リソースの種類
description: iOS アプリの識別子。
author: tfitzmac
ms.openlocfilehash: 7d668d6b1751b125fc3cb4f5e2bb74d481aca9f2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303347"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="756b0-103">iosMobileAppIdentifier リソースの種類</span><span class="sxs-lookup"><span data-stu-id="756b0-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="756b0-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="756b0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="756b0-105">iOS アプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="756b0-105">The identifier for an iOS app.</span></span>

<span data-ttu-id="756b0-106">[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="756b0-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="756b0-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="756b0-107">Properties</span></span>
|<span data-ttu-id="756b0-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="756b0-108">Property</span></span>|<span data-ttu-id="756b0-109">種類</span><span class="sxs-lookup"><span data-stu-id="756b0-109">Type</span></span>|<span data-ttu-id="756b0-110">説明</span><span class="sxs-lookup"><span data-stu-id="756b0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="756b0-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="756b0-111">bundleId</span></span>|<span data-ttu-id="756b0-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="756b0-112">String</span></span>|<span data-ttu-id="756b0-113">App Store で指定されている、アプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="756b0-113">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="756b0-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="756b0-114">Relationships</span></span>
<span data-ttu-id="756b0-115">なし</span><span class="sxs-lookup"><span data-stu-id="756b0-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="756b0-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="756b0-116">JSON Representation</span></span>
<span data-ttu-id="756b0-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="756b0-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMobileAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMobileAppIdentifier",
  "bundleId": "String"
}
```



