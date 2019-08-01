---
title: iosHomeScreenFolder リソースの種類
description: ホーム画面上のアプリのページが含まれるフォルダー
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5a22b20049c886b7cb1de2f7737b269fbd411749
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031521"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="743c9-103">iosHomeScreenFolder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="743c9-103">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="743c9-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="743c9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="743c9-105">ホーム画面上のアプリのページが含まれるフォルダー</span><span class="sxs-lookup"><span data-stu-id="743c9-105">A folder containing pages of apps on the Home Screen</span></span>


<span data-ttu-id="743c9-106">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="743c9-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="743c9-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="743c9-107">Properties</span></span>
|<span data-ttu-id="743c9-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="743c9-108">Property</span></span>|<span data-ttu-id="743c9-109">型</span><span class="sxs-lookup"><span data-stu-id="743c9-109">Type</span></span>|<span data-ttu-id="743c9-110">説明</span><span class="sxs-lookup"><span data-stu-id="743c9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="743c9-111">displayName</span><span class="sxs-lookup"><span data-stu-id="743c9-111">displayName</span></span>|<span data-ttu-id="743c9-112">String</span><span class="sxs-lookup"><span data-stu-id="743c9-112">String</span></span>|<span data-ttu-id="743c9-113">アプリの名前。[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) から継承</span><span class="sxs-lookup"><span data-stu-id="743c9-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="743c9-114">pages</span><span class="sxs-lookup"><span data-stu-id="743c9-114">pages</span></span>|<span data-ttu-id="743c9-115">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="743c9-115">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="743c9-116">アプリケーションの種類にする必要がある、ホーム画面レイアウト アイコンで構成されるページ。</span><span class="sxs-lookup"><span data-stu-id="743c9-116">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="743c9-117">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="743c9-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="743c9-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="743c9-118">Relationships</span></span>
<span data-ttu-id="743c9-119">なし</span><span class="sxs-lookup"><span data-stu-id="743c9-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="743c9-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="743c9-120">JSON Representation</span></span>
<span data-ttu-id="743c9-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="743c9-121">Here is a JSON representation of the resource.</span></span>
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



