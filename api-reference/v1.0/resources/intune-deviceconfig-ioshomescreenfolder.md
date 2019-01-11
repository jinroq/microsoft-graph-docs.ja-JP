---
title: iosHomeScreenFolder リソースの種類
description: ホーム画面上のアプリのページが含まれるフォルダー
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1a4f7f4180bce05d331fcc116826956f4feed70c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844577"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="3e8d5-103">iosHomeScreenFolder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3e8d5-103">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="3e8d5-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3e8d5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3e8d5-105">ホーム画面上のアプリのページが含まれるフォルダー</span><span class="sxs-lookup"><span data-stu-id="3e8d5-105">A folder containing pages of apps on the Home Screen</span></span>

<span data-ttu-id="3e8d5-106">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="3e8d5-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3e8d5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3e8d5-107">Properties</span></span>
|<span data-ttu-id="3e8d5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3e8d5-108">Property</span></span>|<span data-ttu-id="3e8d5-109">種類</span><span class="sxs-lookup"><span data-stu-id="3e8d5-109">Type</span></span>|<span data-ttu-id="3e8d5-110">説明</span><span class="sxs-lookup"><span data-stu-id="3e8d5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e8d5-111">displayName</span><span class="sxs-lookup"><span data-stu-id="3e8d5-111">displayName</span></span>|<span data-ttu-id="3e8d5-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="3e8d5-112">String</span></span>|<span data-ttu-id="3e8d5-113">アプリの名前。[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) から継承</span><span class="sxs-lookup"><span data-stu-id="3e8d5-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="3e8d5-114">pages</span><span class="sxs-lookup"><span data-stu-id="3e8d5-114">pages</span></span>|<span data-ttu-id="3e8d5-115">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3e8d5-115">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="3e8d5-116">アプリケーションの種類にする必要がある、ホーム画面レイアウト アイコンで構成されるページ。</span><span class="sxs-lookup"><span data-stu-id="3e8d5-116">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="3e8d5-117">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="3e8d5-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e8d5-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3e8d5-118">Relationships</span></span>
<span data-ttu-id="3e8d5-119">なし</span><span class="sxs-lookup"><span data-stu-id="3e8d5-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3e8d5-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3e8d5-120">JSON Representation</span></span>
<span data-ttu-id="3e8d5-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3e8d5-121">Here is a JSON representation of the resource.</span></span>
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



