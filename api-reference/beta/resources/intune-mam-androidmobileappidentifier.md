---
title: androidMobileAppIdentifier リソースの種類
description: Android アプリの識別子。
author: tfitzmac
ms.openlocfilehash: c8f590deb33faf1782e3e2ad38f0b65ab4f58eed
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306882"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="8ff50-103">androidMobileAppIdentifier リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8ff50-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="8ff50-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8ff50-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8ff50-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ff50-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8ff50-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8ff50-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8ff50-107">Android アプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="8ff50-107">The identifier for an Android app.</span></span>

<span data-ttu-id="8ff50-108">[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="8ff50-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8ff50-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8ff50-109">Properties</span></span>
|<span data-ttu-id="8ff50-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8ff50-110">Property</span></span>|<span data-ttu-id="8ff50-111">種類</span><span class="sxs-lookup"><span data-stu-id="8ff50-111">Type</span></span>|<span data-ttu-id="8ff50-112">説明</span><span class="sxs-lookup"><span data-stu-id="8ff50-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ff50-113">packageId</span><span class="sxs-lookup"><span data-stu-id="8ff50-113">packageId</span></span>|<span data-ttu-id="8ff50-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="8ff50-114">String</span></span>|<span data-ttu-id="8ff50-115">Play ストアで指定されている、アプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="8ff50-115">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ff50-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8ff50-116">Relationships</span></span>
<span data-ttu-id="8ff50-117">なし</span><span class="sxs-lookup"><span data-stu-id="8ff50-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8ff50-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8ff50-118">JSON Representation</span></span>
<span data-ttu-id="8ff50-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8ff50-119">Here is a JSON representation of the resource.</span></span>
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





