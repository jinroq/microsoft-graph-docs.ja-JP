---
title: iosHomeScreenPage リソースの種類
description: ホーム画面上のアプリとフォルダーが含まれるページ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2c726d751d81277a4f1b79a33606e1a2ec3eaede
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521608"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="23296-103">iosHomeScreenPage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="23296-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="23296-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="23296-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23296-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="23296-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23296-106">ホーム画面上のアプリとフォルダーが含まれるページ</span><span class="sxs-lookup"><span data-stu-id="23296-106">A page containing apps and folders on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="23296-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="23296-107">Properties</span></span>
|<span data-ttu-id="23296-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="23296-108">Property</span></span>|<span data-ttu-id="23296-109">型</span><span class="sxs-lookup"><span data-stu-id="23296-109">Type</span></span>|<span data-ttu-id="23296-110">説明</span><span class="sxs-lookup"><span data-stu-id="23296-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23296-111">displayName</span><span class="sxs-lookup"><span data-stu-id="23296-111">displayName</span></span>|<span data-ttu-id="23296-112">String</span><span class="sxs-lookup"><span data-stu-id="23296-112">String</span></span>|<span data-ttu-id="23296-113">ページの名前</span><span class="sxs-lookup"><span data-stu-id="23296-113">Name of the page</span></span>|
|<span data-ttu-id="23296-114">アイコン</span><span class="sxs-lookup"><span data-stu-id="23296-114">icons</span></span>|<span data-ttu-id="23296-115">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="23296-115">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="23296-116">特定ページに表示されるアプリとフォルダーの一覧。</span><span class="sxs-lookup"><span data-stu-id="23296-116">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="23296-117">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="23296-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23296-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="23296-118">Relationships</span></span>
<span data-ttu-id="23296-119">なし</span><span class="sxs-lookup"><span data-stu-id="23296-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23296-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="23296-120">JSON Representation</span></span>
<span data-ttu-id="23296-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="23296-121">Here is a JSON representation of the resource.</span></span>
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





