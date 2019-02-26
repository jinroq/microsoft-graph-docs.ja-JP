---
title: iosHomeScreenPage リソースの種類
description: ホーム画面上のアプリとフォルダーが含まれるページ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f4317ac80e7ff6273b809eb747da745f5cf5edb6
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254388"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="d5c6c-103">iosHomeScreenPage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d5c6c-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="d5c6c-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d5c6c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5c6c-105">ホーム画面上のアプリとフォルダーが含まれるページ</span><span class="sxs-lookup"><span data-stu-id="d5c6c-105">A page containing apps and folders on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="d5c6c-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d5c6c-106">Properties</span></span>
|<span data-ttu-id="d5c6c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d5c6c-107">Property</span></span>|<span data-ttu-id="d5c6c-108">型</span><span class="sxs-lookup"><span data-stu-id="d5c6c-108">Type</span></span>|<span data-ttu-id="d5c6c-109">説明</span><span class="sxs-lookup"><span data-stu-id="d5c6c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5c6c-110">displayName</span><span class="sxs-lookup"><span data-stu-id="d5c6c-110">displayName</span></span>|<span data-ttu-id="d5c6c-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="d5c6c-111">String</span></span>|<span data-ttu-id="d5c6c-112">ページの名前</span><span class="sxs-lookup"><span data-stu-id="d5c6c-112">Name of the page</span></span>|
|<span data-ttu-id="d5c6c-113">アイコン</span><span class="sxs-lookup"><span data-stu-id="d5c6c-113">icons</span></span>|<span data-ttu-id="d5c6c-114">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d5c6c-114">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="d5c6c-115">特定ページに表示されるアプリとフォルダーの一覧。</span><span class="sxs-lookup"><span data-stu-id="d5c6c-115">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="d5c6c-116">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="d5c6c-116">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5c6c-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d5c6c-117">Relationships</span></span>
<span data-ttu-id="d5c6c-118">なし</span><span class="sxs-lookup"><span data-stu-id="d5c6c-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5c6c-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d5c6c-119">JSON Representation</span></span>
<span data-ttu-id="d5c6c-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d5c6c-120">Here is a JSON representation of the resource.</span></span>
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



