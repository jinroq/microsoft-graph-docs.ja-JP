---
title: iosHomeScreenApp リソースの種類
description: ホーム画面上のアプリのアイコンを表します
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cc4e94071e7b81fab82044f65da809f7b17e5b3f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028218"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="d5b5c-103">iosHomeScreenApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d5b5c-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="d5b5c-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d5b5c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5b5c-105">ホーム画面上のアプリのアイコンを表します</span><span class="sxs-lookup"><span data-stu-id="d5b5c-105">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="d5b5c-106">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="d5b5c-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d5b5c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d5b5c-107">Properties</span></span>
|<span data-ttu-id="d5b5c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d5b5c-108">Property</span></span>|<span data-ttu-id="d5b5c-109">型</span><span class="sxs-lookup"><span data-stu-id="d5b5c-109">Type</span></span>|<span data-ttu-id="d5b5c-110">説明</span><span class="sxs-lookup"><span data-stu-id="d5b5c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5b5c-111">displayName</span><span class="sxs-lookup"><span data-stu-id="d5b5c-111">displayName</span></span>|<span data-ttu-id="d5b5c-112">String</span><span class="sxs-lookup"><span data-stu-id="d5b5c-112">String</span></span>|<span data-ttu-id="d5b5c-113">アプリの名前。[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) から継承</span><span class="sxs-lookup"><span data-stu-id="d5b5c-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="d5b5c-114">bundleID</span><span class="sxs-lookup"><span data-stu-id="d5b5c-114">bundleID</span></span>|<span data-ttu-id="d5b5c-115">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="d5b5c-115">String</span></span>|<span data-ttu-id="d5b5c-116">アプリの BundleID</span><span class="sxs-lookup"><span data-stu-id="d5b5c-116">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5b5c-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d5b5c-117">Relationships</span></span>
<span data-ttu-id="d5b5c-118">なし</span><span class="sxs-lookup"><span data-stu-id="d5b5c-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5b5c-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d5b5c-119">JSON Representation</span></span>
<span data-ttu-id="d5b5c-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d5b5c-120">Here is a JSON representation of the resource.</span></span>
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



