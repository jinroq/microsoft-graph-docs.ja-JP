---
title: iosHomeScreenFolder リソースの種類
description: ホーム画面上のアプリのページが含まれるフォルダー
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1cf7ef74b12efbe81503ad46f1a9c766fcc996c5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36357041"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="33628-103">iosHomeScreenFolder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="33628-103">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="33628-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="33628-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33628-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="33628-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33628-106">ホーム画面上のアプリのページが含まれるフォルダー</span><span class="sxs-lookup"><span data-stu-id="33628-106">A folder containing pages of apps on the Home Screen</span></span>


<span data-ttu-id="33628-107">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="33628-107">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="33628-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="33628-108">Properties</span></span>
|<span data-ttu-id="33628-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="33628-109">Property</span></span>|<span data-ttu-id="33628-110">型</span><span class="sxs-lookup"><span data-stu-id="33628-110">Type</span></span>|<span data-ttu-id="33628-111">説明</span><span class="sxs-lookup"><span data-stu-id="33628-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33628-112">displayName</span><span class="sxs-lookup"><span data-stu-id="33628-112">displayName</span></span>|<span data-ttu-id="33628-113">String</span><span class="sxs-lookup"><span data-stu-id="33628-113">String</span></span>|<span data-ttu-id="33628-114">アプリの名前。[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) から継承</span><span class="sxs-lookup"><span data-stu-id="33628-114">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="33628-115">pages</span><span class="sxs-lookup"><span data-stu-id="33628-115">pages</span></span>|<span data-ttu-id="33628-116">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="33628-116">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="33628-117">アプリケーションの種類にする必要がある、ホーム画面レイアウト アイコンで構成されるページ。</span><span class="sxs-lookup"><span data-stu-id="33628-117">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="33628-118">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="33628-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="33628-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="33628-119">Relationships</span></span>
<span data-ttu-id="33628-120">なし</span><span class="sxs-lookup"><span data-stu-id="33628-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="33628-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="33628-121">JSON Representation</span></span>
<span data-ttu-id="33628-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="33628-122">Here is a JSON representation of the resource.</span></span>
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



