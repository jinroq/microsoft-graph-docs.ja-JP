---
title: iosHomeScreenFolder リソースの種類
description: ホーム画面上のアプリのページが含まれるフォルダー
author: tfitzmac
ms.openlocfilehash: 251f854a0038c905175b863e2c19dd638c49b452
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302801"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="2ab75-103">iosHomeScreenFolder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2ab75-103">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="2ab75-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2ab75-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2ab75-105">ホーム画面上のアプリのページが含まれるフォルダー</span><span class="sxs-lookup"><span data-stu-id="2ab75-105">A folder containing pages of apps on the Home Screen</span></span>

<span data-ttu-id="2ab75-106">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="2ab75-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2ab75-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ab75-107">Properties</span></span>
|<span data-ttu-id="2ab75-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ab75-108">Property</span></span>|<span data-ttu-id="2ab75-109">種類</span><span class="sxs-lookup"><span data-stu-id="2ab75-109">Type</span></span>|<span data-ttu-id="2ab75-110">説明</span><span class="sxs-lookup"><span data-stu-id="2ab75-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ab75-111">displayName</span><span class="sxs-lookup"><span data-stu-id="2ab75-111">displayName</span></span>|<span data-ttu-id="2ab75-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="2ab75-112">String</span></span>|<span data-ttu-id="2ab75-113">アプリの名前。[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) から継承</span><span class="sxs-lookup"><span data-stu-id="2ab75-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="2ab75-114">pages</span><span class="sxs-lookup"><span data-stu-id="2ab75-114">pages</span></span>|<span data-ttu-id="2ab75-115">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2ab75-115">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="2ab75-116">アプリケーションの種類にする必要がある、ホーム画面レイアウト アイコンで構成されるページ。</span><span class="sxs-lookup"><span data-stu-id="2ab75-116">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="2ab75-117">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="2ab75-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ab75-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2ab75-118">Relationships</span></span>
<span data-ttu-id="2ab75-119">なし</span><span class="sxs-lookup"><span data-stu-id="2ab75-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2ab75-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2ab75-120">JSON Representation</span></span>
<span data-ttu-id="2ab75-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2ab75-121">Here is a JSON representation of the resource.</span></span>
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



