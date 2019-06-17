---
title: iosHomeScreenPage リソースの種類
description: ホーム画面上のアプリとフォルダーが含まれるページ
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7a3ce2a6ac9cacffb2dc5ac2cc4ad3c5fced14d2
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34978221"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="54c8f-103">iosHomeScreenPage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="54c8f-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="54c8f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="54c8f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54c8f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="54c8f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54c8f-106">ホーム画面上のアプリとフォルダーが含まれるページ</span><span class="sxs-lookup"><span data-stu-id="54c8f-106">A page containing apps and folders on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="54c8f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="54c8f-107">Properties</span></span>
|<span data-ttu-id="54c8f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="54c8f-108">Property</span></span>|<span data-ttu-id="54c8f-109">型</span><span class="sxs-lookup"><span data-stu-id="54c8f-109">Type</span></span>|<span data-ttu-id="54c8f-110">説明</span><span class="sxs-lookup"><span data-stu-id="54c8f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54c8f-111">displayName</span><span class="sxs-lookup"><span data-stu-id="54c8f-111">displayName</span></span>|<span data-ttu-id="54c8f-112">String</span><span class="sxs-lookup"><span data-stu-id="54c8f-112">String</span></span>|<span data-ttu-id="54c8f-113">ページの名前</span><span class="sxs-lookup"><span data-stu-id="54c8f-113">Name of the page</span></span>|
|<span data-ttu-id="54c8f-114">アイコン</span><span class="sxs-lookup"><span data-stu-id="54c8f-114">icons</span></span>|<span data-ttu-id="54c8f-115">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="54c8f-115">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="54c8f-116">特定ページに表示されるアプリとフォルダーの一覧。</span><span class="sxs-lookup"><span data-stu-id="54c8f-116">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="54c8f-117">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="54c8f-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="54c8f-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="54c8f-118">Relationships</span></span>
<span data-ttu-id="54c8f-119">なし</span><span class="sxs-lookup"><span data-stu-id="54c8f-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="54c8f-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="54c8f-120">JSON Representation</span></span>
<span data-ttu-id="54c8f-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="54c8f-121">Here is a JSON representation of the resource.</span></span>
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





