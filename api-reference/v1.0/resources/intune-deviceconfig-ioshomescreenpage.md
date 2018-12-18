---
title: iosHomeScreenPage リソースの種類
description: ホーム画面上のアプリとフォルダーが含まれるページ
author: tfitzmac
ms.openlocfilehash: b8aca5c671d0c8521cdf8a870a2f0ad3cd35ba1b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321463"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="58b6d-103">iosHomeScreenPage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="58b6d-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="58b6d-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="58b6d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="58b6d-105">ホーム画面上のアプリとフォルダーが含まれるページ</span><span class="sxs-lookup"><span data-stu-id="58b6d-105">A page containing apps and folders on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="58b6d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="58b6d-106">Properties</span></span>
|<span data-ttu-id="58b6d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="58b6d-107">Property</span></span>|<span data-ttu-id="58b6d-108">種類</span><span class="sxs-lookup"><span data-stu-id="58b6d-108">Type</span></span>|<span data-ttu-id="58b6d-109">説明</span><span class="sxs-lookup"><span data-stu-id="58b6d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58b6d-110">displayName</span><span class="sxs-lookup"><span data-stu-id="58b6d-110">displayName</span></span>|<span data-ttu-id="58b6d-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="58b6d-111">String</span></span>|<span data-ttu-id="58b6d-112">ページの名前</span><span class="sxs-lookup"><span data-stu-id="58b6d-112">Name of the page</span></span>|
|<span data-ttu-id="58b6d-113">アイコン</span><span class="sxs-lookup"><span data-stu-id="58b6d-113">icons</span></span>|<span data-ttu-id="58b6d-114">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="58b6d-114">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="58b6d-115">特定ページに表示されるアプリとフォルダーの一覧。</span><span class="sxs-lookup"><span data-stu-id="58b6d-115">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="58b6d-116">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="58b6d-116">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="58b6d-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="58b6d-117">Relationships</span></span>
<span data-ttu-id="58b6d-118">なし</span><span class="sxs-lookup"><span data-stu-id="58b6d-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="58b6d-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="58b6d-119">JSON Representation</span></span>
<span data-ttu-id="58b6d-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="58b6d-120">Here is a JSON representation of the resource.</span></span>
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



