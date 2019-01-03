---
title: iosHomeScreenApp リソースの種類
description: ホーム画面上のアプリのアイコンを表します
author: tfitzmac
ms.openlocfilehash: 68fe4e7b5a226422cc0aaf980ac7fb0421a9bfc0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350373"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="781e8-103">iosHomeScreenApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="781e8-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="781e8-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="781e8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="781e8-105">ホーム画面上のアプリのアイコンを表します</span><span class="sxs-lookup"><span data-stu-id="781e8-105">Represents an icon for an app on the Home Screen</span></span>

<span data-ttu-id="781e8-106">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="781e8-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="781e8-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="781e8-107">Properties</span></span>
|<span data-ttu-id="781e8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="781e8-108">Property</span></span>|<span data-ttu-id="781e8-109">種類</span><span class="sxs-lookup"><span data-stu-id="781e8-109">Type</span></span>|<span data-ttu-id="781e8-110">説明</span><span class="sxs-lookup"><span data-stu-id="781e8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="781e8-111">displayName</span><span class="sxs-lookup"><span data-stu-id="781e8-111">displayName</span></span>|<span data-ttu-id="781e8-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="781e8-112">String</span></span>|<span data-ttu-id="781e8-113">アプリの名前。[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) から継承</span><span class="sxs-lookup"><span data-stu-id="781e8-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="781e8-114">bundleID</span><span class="sxs-lookup"><span data-stu-id="781e8-114">bundleID</span></span>|<span data-ttu-id="781e8-115">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="781e8-115">String</span></span>|<span data-ttu-id="781e8-116">アプリの BundleID</span><span class="sxs-lookup"><span data-stu-id="781e8-116">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="781e8-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="781e8-117">Relationships</span></span>
<span data-ttu-id="781e8-118">なし</span><span class="sxs-lookup"><span data-stu-id="781e8-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="781e8-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="781e8-119">JSON Representation</span></span>
<span data-ttu-id="781e8-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="781e8-120">Here is a JSON representation of the resource.</span></span>
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


