---
title: iosHomeScreenPage リソースの種類
description: ホーム画面上のアプリとフォルダーが含まれるページ
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2dab636fb4e1793916b1408007bc56aaaa3933a1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855231"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="80dae-103">iosHomeScreenPage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="80dae-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="80dae-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="80dae-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="80dae-105">ホーム画面上のアプリとフォルダーが含まれるページ</span><span class="sxs-lookup"><span data-stu-id="80dae-105">A page containing apps and folders on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="80dae-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="80dae-106">Properties</span></span>
|<span data-ttu-id="80dae-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="80dae-107">Property</span></span>|<span data-ttu-id="80dae-108">種類</span><span class="sxs-lookup"><span data-stu-id="80dae-108">Type</span></span>|<span data-ttu-id="80dae-109">説明</span><span class="sxs-lookup"><span data-stu-id="80dae-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80dae-110">displayName</span><span class="sxs-lookup"><span data-stu-id="80dae-110">displayName</span></span>|<span data-ttu-id="80dae-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="80dae-111">String</span></span>|<span data-ttu-id="80dae-112">ページの名前</span><span class="sxs-lookup"><span data-stu-id="80dae-112">Name of the page</span></span>|
|<span data-ttu-id="80dae-113">アイコン</span><span class="sxs-lookup"><span data-stu-id="80dae-113">icons</span></span>|<span data-ttu-id="80dae-114">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="80dae-114">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="80dae-115">特定ページに表示されるアプリとフォルダーの一覧。</span><span class="sxs-lookup"><span data-stu-id="80dae-115">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="80dae-116">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="80dae-116">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="80dae-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="80dae-117">Relationships</span></span>
<span data-ttu-id="80dae-118">なし</span><span class="sxs-lookup"><span data-stu-id="80dae-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="80dae-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="80dae-119">JSON Representation</span></span>
<span data-ttu-id="80dae-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="80dae-120">Here is a JSON representation of the resource.</span></span>
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



