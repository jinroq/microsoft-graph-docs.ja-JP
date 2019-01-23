---
title: iosHomeScreenApp リソースの種類
description: ホーム画面上のアプリのアイコンを表します
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dcc90e774f8d032d46968fc4f751923bcc52e559
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412325"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="3816d-103">iosHomeScreenApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3816d-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="3816d-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3816d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3816d-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3816d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3816d-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3816d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3816d-107">ホーム画面上のアプリのアイコンを表します</span><span class="sxs-lookup"><span data-stu-id="3816d-107">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="3816d-108">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="3816d-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3816d-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3816d-109">Properties</span></span>
|<span data-ttu-id="3816d-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3816d-110">Property</span></span>|<span data-ttu-id="3816d-111">型</span><span class="sxs-lookup"><span data-stu-id="3816d-111">Type</span></span>|<span data-ttu-id="3816d-112">説明</span><span class="sxs-lookup"><span data-stu-id="3816d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3816d-113">displayName</span><span class="sxs-lookup"><span data-stu-id="3816d-113">displayName</span></span>|<span data-ttu-id="3816d-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="3816d-114">String</span></span>|<span data-ttu-id="3816d-115">アプリの名前。[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) から継承</span><span class="sxs-lookup"><span data-stu-id="3816d-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="3816d-116">bundleID</span><span class="sxs-lookup"><span data-stu-id="3816d-116">bundleID</span></span>|<span data-ttu-id="3816d-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="3816d-117">String</span></span>|<span data-ttu-id="3816d-118">アプリの BundleID</span><span class="sxs-lookup"><span data-stu-id="3816d-118">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="3816d-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3816d-119">Relationships</span></span>
<span data-ttu-id="3816d-120">なし</span><span class="sxs-lookup"><span data-stu-id="3816d-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3816d-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3816d-121">JSON Representation</span></span>
<span data-ttu-id="3816d-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3816d-122">Here is a JSON representation of the resource.</span></span>
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




