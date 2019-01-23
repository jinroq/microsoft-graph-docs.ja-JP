---
title: iosHomeScreenFolder リソースの種類
description: ホーム画面上のアプリのページが含まれるフォルダー
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 36ea4a00b9310623027179e1d6d2e1c64888c470
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407509"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="79ec1-103">iosHomeScreenFolder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="79ec1-103">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="79ec1-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="79ec1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="79ec1-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79ec1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="79ec1-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="79ec1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79ec1-107">ホーム画面上のアプリのページが含まれるフォルダー</span><span class="sxs-lookup"><span data-stu-id="79ec1-107">A folder containing pages of apps on the Home Screen</span></span>


<span data-ttu-id="79ec1-108">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="79ec1-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="79ec1-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="79ec1-109">Properties</span></span>
|<span data-ttu-id="79ec1-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="79ec1-110">Property</span></span>|<span data-ttu-id="79ec1-111">型</span><span class="sxs-lookup"><span data-stu-id="79ec1-111">Type</span></span>|<span data-ttu-id="79ec1-112">説明</span><span class="sxs-lookup"><span data-stu-id="79ec1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79ec1-113">displayName</span><span class="sxs-lookup"><span data-stu-id="79ec1-113">displayName</span></span>|<span data-ttu-id="79ec1-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="79ec1-114">String</span></span>|<span data-ttu-id="79ec1-115">アプリの名前。[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) から継承</span><span class="sxs-lookup"><span data-stu-id="79ec1-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="79ec1-116">pages</span><span class="sxs-lookup"><span data-stu-id="79ec1-116">pages</span></span>|<span data-ttu-id="79ec1-117">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="79ec1-117">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="79ec1-118">アプリケーションの種類にする必要がある、ホーム画面レイアウト アイコンで構成されるページ。</span><span class="sxs-lookup"><span data-stu-id="79ec1-118">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="79ec1-119">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="79ec1-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="79ec1-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="79ec1-120">Relationships</span></span>
<span data-ttu-id="79ec1-121">なし</span><span class="sxs-lookup"><span data-stu-id="79ec1-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="79ec1-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="79ec1-122">JSON Representation</span></span>
<span data-ttu-id="79ec1-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="79ec1-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolder"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolder",
  "displayName": "String",
  "pages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
      "displayName": "String",
      "apps": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenApp",
          "displayName": "String",
          "bundleID": "String"
        }
      ]
    }
  ]
}
```




