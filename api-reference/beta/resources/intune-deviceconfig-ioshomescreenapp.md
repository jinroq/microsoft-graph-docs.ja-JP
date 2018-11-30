---
title: iosHomeScreenApp リソースの種類
description: ホーム画面上のアプリのアイコンを表します
ms.openlocfilehash: 5c8700e0164bebbe6e930ebbd07a01c27c0f2495
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067377"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="49d0d-103">iosHomeScreenApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="49d0d-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="49d0d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="49d0d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="49d0d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="49d0d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="49d0d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="49d0d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="49d0d-107">ホーム画面上のアプリのアイコンを表します</span><span class="sxs-lookup"><span data-stu-id="49d0d-107">Represents an icon for an app on the Home Screen</span></span>

<span data-ttu-id="49d0d-108">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="49d0d-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="49d0d-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="49d0d-109">Properties</span></span>
|<span data-ttu-id="49d0d-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="49d0d-110">Property</span></span>|<span data-ttu-id="49d0d-111">型</span><span class="sxs-lookup"><span data-stu-id="49d0d-111">Type</span></span>|<span data-ttu-id="49d0d-112">説明</span><span class="sxs-lookup"><span data-stu-id="49d0d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49d0d-113">displayName</span><span class="sxs-lookup"><span data-stu-id="49d0d-113">displayName</span></span>|<span data-ttu-id="49d0d-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="49d0d-114">String</span></span>|<span data-ttu-id="49d0d-115">アプリの名前。[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) から継承</span><span class="sxs-lookup"><span data-stu-id="49d0d-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="49d0d-116">bundleID</span><span class="sxs-lookup"><span data-stu-id="49d0d-116">bundleID</span></span>|<span data-ttu-id="49d0d-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="49d0d-117">String</span></span>|<span data-ttu-id="49d0d-118">アプリの BundleID</span><span class="sxs-lookup"><span data-stu-id="49d0d-118">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="49d0d-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="49d0d-119">Relationships</span></span>
<span data-ttu-id="49d0d-120">なし</span><span class="sxs-lookup"><span data-stu-id="49d0d-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="49d0d-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="49d0d-121">JSON Representation</span></span>
<span data-ttu-id="49d0d-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="49d0d-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenApp",
  "displayName": "String",
  "bundleID": "String"
}
```





