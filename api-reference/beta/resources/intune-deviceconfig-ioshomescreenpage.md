---
title: iosHomeScreenPage リソースの種類
description: ホーム画面上のアプリとフォルダーが含まれるページ
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8b2b6e4ba9cc70253e929a0f434a292aeafd24bd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398549"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="14ec1-103">iosHomeScreenPage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="14ec1-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="14ec1-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="14ec1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="14ec1-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="14ec1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="14ec1-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="14ec1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14ec1-107">ホーム画面上のアプリとフォルダーが含まれるページ</span><span class="sxs-lookup"><span data-stu-id="14ec1-107">A page containing apps and folders on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="14ec1-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="14ec1-108">Properties</span></span>
|<span data-ttu-id="14ec1-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="14ec1-109">Property</span></span>|<span data-ttu-id="14ec1-110">型</span><span class="sxs-lookup"><span data-stu-id="14ec1-110">Type</span></span>|<span data-ttu-id="14ec1-111">説明</span><span class="sxs-lookup"><span data-stu-id="14ec1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14ec1-112">displayName</span><span class="sxs-lookup"><span data-stu-id="14ec1-112">displayName</span></span>|<span data-ttu-id="14ec1-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="14ec1-113">String</span></span>|<span data-ttu-id="14ec1-114">ページの名前</span><span class="sxs-lookup"><span data-stu-id="14ec1-114">Name of the page</span></span>|
|<span data-ttu-id="14ec1-115">アイコン</span><span class="sxs-lookup"><span data-stu-id="14ec1-115">icons</span></span>|<span data-ttu-id="14ec1-116">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="14ec1-116">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="14ec1-117">特定ページに表示されるアプリとフォルダーの一覧。</span><span class="sxs-lookup"><span data-stu-id="14ec1-117">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="14ec1-118">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="14ec1-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="14ec1-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="14ec1-119">Relationships</span></span>
<span data-ttu-id="14ec1-120">なし</span><span class="sxs-lookup"><span data-stu-id="14ec1-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="14ec1-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="14ec1-121">JSON Representation</span></span>
<span data-ttu-id="14ec1-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="14ec1-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenPage",
  "displayName": "String",
  "icons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
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
  ]
}
```




