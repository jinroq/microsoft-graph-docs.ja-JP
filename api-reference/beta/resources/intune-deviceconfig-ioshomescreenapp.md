---
title: iosHomeScreenApp リソースの種類
description: ホーム画面上のアプリのアイコンを表します
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 964ec12a40a707b96b29c4793e35533995f16eaf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001230"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="a129b-103">iosHomeScreenApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a129b-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="a129b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a129b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a129b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a129b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a129b-106">ホーム画面上のアプリのアイコンを表します</span><span class="sxs-lookup"><span data-stu-id="a129b-106">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="a129b-107">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="a129b-107">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a129b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a129b-108">Properties</span></span>
|<span data-ttu-id="a129b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a129b-109">Property</span></span>|<span data-ttu-id="a129b-110">型</span><span class="sxs-lookup"><span data-stu-id="a129b-110">Type</span></span>|<span data-ttu-id="a129b-111">説明</span><span class="sxs-lookup"><span data-stu-id="a129b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a129b-112">displayName</span><span class="sxs-lookup"><span data-stu-id="a129b-112">displayName</span></span>|<span data-ttu-id="a129b-113">String</span><span class="sxs-lookup"><span data-stu-id="a129b-113">String</span></span>|<span data-ttu-id="a129b-114">アプリの名前。[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) から継承</span><span class="sxs-lookup"><span data-stu-id="a129b-114">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="a129b-115">bundleID</span><span class="sxs-lookup"><span data-stu-id="a129b-115">bundleID</span></span>|<span data-ttu-id="a129b-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="a129b-116">String</span></span>|<span data-ttu-id="a129b-117">アプリの BundleID</span><span class="sxs-lookup"><span data-stu-id="a129b-117">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="a129b-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a129b-118">Relationships</span></span>
<span data-ttu-id="a129b-119">なし</span><span class="sxs-lookup"><span data-stu-id="a129b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a129b-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a129b-120">JSON Representation</span></span>
<span data-ttu-id="a129b-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a129b-121">Here is a JSON representation of the resource.</span></span>
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





