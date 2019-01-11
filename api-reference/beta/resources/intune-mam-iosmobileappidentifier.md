---
title: iosMobileAppIdentifier リソースの種類
description: iOS アプリの識別子。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a5540ba03dffe0dcedbfe3e59c6b004434bb0ed4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828358"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="32bbf-103">iosMobileAppIdentifier リソースの種類</span><span class="sxs-lookup"><span data-stu-id="32bbf-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="32bbf-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="32bbf-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="32bbf-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="32bbf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="32bbf-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="32bbf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="32bbf-107">iOS アプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="32bbf-107">The identifier for an iOS app.</span></span>

<span data-ttu-id="32bbf-108">[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="32bbf-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="32bbf-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="32bbf-109">Properties</span></span>
|<span data-ttu-id="32bbf-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="32bbf-110">Property</span></span>|<span data-ttu-id="32bbf-111">種類</span><span class="sxs-lookup"><span data-stu-id="32bbf-111">Type</span></span>|<span data-ttu-id="32bbf-112">説明</span><span class="sxs-lookup"><span data-stu-id="32bbf-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32bbf-113">bundleId</span><span class="sxs-lookup"><span data-stu-id="32bbf-113">bundleId</span></span>|<span data-ttu-id="32bbf-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="32bbf-114">String</span></span>|<span data-ttu-id="32bbf-115">App Store で指定されている、アプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="32bbf-115">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="32bbf-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="32bbf-116">Relationships</span></span>
<span data-ttu-id="32bbf-117">なし</span><span class="sxs-lookup"><span data-stu-id="32bbf-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="32bbf-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="32bbf-118">JSON Representation</span></span>
<span data-ttu-id="32bbf-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="32bbf-119">Here is a JSON representation of the resource.</span></span>
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





