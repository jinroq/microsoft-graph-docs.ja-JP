---
title: iosMobileAppIdentifier リソースの種類
description: iOS アプリの識別子。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 134f6e27b6fb113516fd119211e245fd77b2ae75
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919527"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="f2601-103">iosMobileAppIdentifier リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f2601-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="f2601-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f2601-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2601-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f2601-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f2601-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f2601-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f2601-107">iOS アプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="f2601-107">The identifier for an iOS app.</span></span>

<span data-ttu-id="f2601-108">[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="f2601-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f2601-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f2601-109">Properties</span></span>
|<span data-ttu-id="f2601-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f2601-110">Property</span></span>|<span data-ttu-id="f2601-111">種類</span><span class="sxs-lookup"><span data-stu-id="f2601-111">Type</span></span>|<span data-ttu-id="f2601-112">説明</span><span class="sxs-lookup"><span data-stu-id="f2601-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2601-113">bundleId</span><span class="sxs-lookup"><span data-stu-id="f2601-113">bundleId</span></span>|<span data-ttu-id="f2601-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f2601-114">String</span></span>|<span data-ttu-id="f2601-115">App Store で指定されている、アプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="f2601-115">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2601-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f2601-116">Relationships</span></span>
<span data-ttu-id="f2601-117">なし</span><span class="sxs-lookup"><span data-stu-id="f2601-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f2601-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f2601-118">JSON Representation</span></span>
<span data-ttu-id="f2601-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f2601-119">Here is a JSON representation of the resource.</span></span>
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





