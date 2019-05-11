---
title: iosHomeScreenPage リソースの種類
description: ホーム画面上のアプリとフォルダーが含まれるページ
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 570dcf430824601383ba9348b721df7862f6eef6
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946547"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="7498c-103">iosHomeScreenPage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7498c-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="7498c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7498c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7498c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7498c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7498c-106">ホーム画面上のアプリとフォルダーが含まれるページ</span><span class="sxs-lookup"><span data-stu-id="7498c-106">A page containing apps and folders on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="7498c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7498c-107">Properties</span></span>
|<span data-ttu-id="7498c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7498c-108">Property</span></span>|<span data-ttu-id="7498c-109">型</span><span class="sxs-lookup"><span data-stu-id="7498c-109">Type</span></span>|<span data-ttu-id="7498c-110">説明</span><span class="sxs-lookup"><span data-stu-id="7498c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7498c-111">displayName</span><span class="sxs-lookup"><span data-stu-id="7498c-111">displayName</span></span>|<span data-ttu-id="7498c-112">String</span><span class="sxs-lookup"><span data-stu-id="7498c-112">String</span></span>|<span data-ttu-id="7498c-113">ページの名前</span><span class="sxs-lookup"><span data-stu-id="7498c-113">Name of the page</span></span>|
|<span data-ttu-id="7498c-114">アイコン</span><span class="sxs-lookup"><span data-stu-id="7498c-114">icons</span></span>|<span data-ttu-id="7498c-115">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7498c-115">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="7498c-116">特定ページに表示されるアプリとフォルダーの一覧。</span><span class="sxs-lookup"><span data-stu-id="7498c-116">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="7498c-117">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="7498c-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7498c-118">関係</span><span class="sxs-lookup"><span data-stu-id="7498c-118">Relationships</span></span>
<span data-ttu-id="7498c-119">なし</span><span class="sxs-lookup"><span data-stu-id="7498c-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7498c-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7498c-120">JSON Representation</span></span>
<span data-ttu-id="7498c-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7498c-121">Here is a JSON representation of the resource.</span></span>
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




