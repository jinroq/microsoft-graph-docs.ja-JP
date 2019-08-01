---
title: iosHomeScreenPage リソースの種類
description: ホーム画面上のアプリとフォルダーが含まれるページ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d898a1611c05b156ee4b16d042175b6b5c33284d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028176"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="8657b-103">iosHomeScreenPage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8657b-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="8657b-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8657b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8657b-105">ホーム画面上のアプリとフォルダーが含まれるページ</span><span class="sxs-lookup"><span data-stu-id="8657b-105">A page containing apps and folders on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="8657b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8657b-106">Properties</span></span>
|<span data-ttu-id="8657b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8657b-107">Property</span></span>|<span data-ttu-id="8657b-108">型</span><span class="sxs-lookup"><span data-stu-id="8657b-108">Type</span></span>|<span data-ttu-id="8657b-109">説明</span><span class="sxs-lookup"><span data-stu-id="8657b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8657b-110">displayName</span><span class="sxs-lookup"><span data-stu-id="8657b-110">displayName</span></span>|<span data-ttu-id="8657b-111">String</span><span class="sxs-lookup"><span data-stu-id="8657b-111">String</span></span>|<span data-ttu-id="8657b-112">ページの名前</span><span class="sxs-lookup"><span data-stu-id="8657b-112">Name of the page</span></span>|
|<span data-ttu-id="8657b-113">アイコン</span><span class="sxs-lookup"><span data-stu-id="8657b-113">icons</span></span>|<span data-ttu-id="8657b-114">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8657b-114">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="8657b-115">特定ページに表示されるアプリとフォルダーの一覧。</span><span class="sxs-lookup"><span data-stu-id="8657b-115">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="8657b-116">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="8657b-116">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8657b-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8657b-117">Relationships</span></span>
<span data-ttu-id="8657b-118">なし</span><span class="sxs-lookup"><span data-stu-id="8657b-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8657b-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8657b-119">JSON Representation</span></span>
<span data-ttu-id="8657b-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8657b-120">Here is a JSON representation of the resource.</span></span>
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
      "@odata.type": "microsoft.graph.iosHomeScreenItem",
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



