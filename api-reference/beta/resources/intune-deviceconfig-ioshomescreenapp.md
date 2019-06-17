---
title: iosHomeScreenApp リソースの種類
description: ホーム画面上のアプリのアイコンを表します
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 279ec6fb424653cbe9247e57881a6a60d96025d4
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34992411"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="ca706-103">iosHomeScreenApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ca706-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="ca706-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ca706-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca706-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ca706-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca706-106">ホーム画面上のアプリのアイコンを表します</span><span class="sxs-lookup"><span data-stu-id="ca706-106">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="ca706-107">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="ca706-107">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ca706-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ca706-108">Properties</span></span>
|<span data-ttu-id="ca706-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ca706-109">Property</span></span>|<span data-ttu-id="ca706-110">型</span><span class="sxs-lookup"><span data-stu-id="ca706-110">Type</span></span>|<span data-ttu-id="ca706-111">説明</span><span class="sxs-lookup"><span data-stu-id="ca706-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca706-112">displayName</span><span class="sxs-lookup"><span data-stu-id="ca706-112">displayName</span></span>|<span data-ttu-id="ca706-113">String</span><span class="sxs-lookup"><span data-stu-id="ca706-113">String</span></span>|<span data-ttu-id="ca706-114">アプリの名前。[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) から継承</span><span class="sxs-lookup"><span data-stu-id="ca706-114">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="ca706-115">bundleID</span><span class="sxs-lookup"><span data-stu-id="ca706-115">bundleID</span></span>|<span data-ttu-id="ca706-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ca706-116">String</span></span>|<span data-ttu-id="ca706-117">アプリの BundleID</span><span class="sxs-lookup"><span data-stu-id="ca706-117">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca706-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ca706-118">Relationships</span></span>
<span data-ttu-id="ca706-119">なし</span><span class="sxs-lookup"><span data-stu-id="ca706-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ca706-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ca706-120">JSON Representation</span></span>
<span data-ttu-id="ca706-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ca706-121">Here is a JSON representation of the resource.</span></span>
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





