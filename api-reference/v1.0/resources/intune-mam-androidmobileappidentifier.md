---
title: androidMobileAppIdentifier リソースの種類
description: Android アプリの識別子。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9cc203cc9268849e8b7b46d994c166378252df59
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871744"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="414e3-103">androidMobileAppIdentifier リソースの種類</span><span class="sxs-lookup"><span data-stu-id="414e3-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="414e3-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="414e3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="414e3-105">Android アプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="414e3-105">The identifier for an Android app.</span></span>

<span data-ttu-id="414e3-106">[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="414e3-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="414e3-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="414e3-107">Properties</span></span>
|<span data-ttu-id="414e3-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="414e3-108">Property</span></span>|<span data-ttu-id="414e3-109">種類</span><span class="sxs-lookup"><span data-stu-id="414e3-109">Type</span></span>|<span data-ttu-id="414e3-110">説明</span><span class="sxs-lookup"><span data-stu-id="414e3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="414e3-111">packageId</span><span class="sxs-lookup"><span data-stu-id="414e3-111">packageId</span></span>|<span data-ttu-id="414e3-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="414e3-112">String</span></span>|<span data-ttu-id="414e3-113">Play ストアで指定されている、アプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="414e3-113">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="414e3-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="414e3-114">Relationships</span></span>
<span data-ttu-id="414e3-115">なし</span><span class="sxs-lookup"><span data-stu-id="414e3-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="414e3-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="414e3-116">JSON Representation</span></span>
<span data-ttu-id="414e3-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="414e3-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidMobileAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidMobileAppIdentifier",
  "packageId": "String"
}
```



