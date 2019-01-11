---
title: iosHomeScreenItem リソースの種類
description: IOS ホーム画面上のアイテムを表します
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bbde13f06df55b984aed8f2e0920a6ec3e3ce158
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835806"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="842ed-103">iosHomeScreenItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="842ed-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="842ed-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="842ed-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="842ed-105">IOS ホーム画面上のアイテムを表します</span><span class="sxs-lookup"><span data-stu-id="842ed-105">Represents an item on the iOS Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="842ed-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="842ed-106">Properties</span></span>
|<span data-ttu-id="842ed-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="842ed-107">Property</span></span>|<span data-ttu-id="842ed-108">種類</span><span class="sxs-lookup"><span data-stu-id="842ed-108">Type</span></span>|<span data-ttu-id="842ed-109">説明</span><span class="sxs-lookup"><span data-stu-id="842ed-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="842ed-110">displayName</span><span class="sxs-lookup"><span data-stu-id="842ed-110">displayName</span></span>|<span data-ttu-id="842ed-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="842ed-111">String</span></span>|<span data-ttu-id="842ed-112">アプリの名前</span><span class="sxs-lookup"><span data-stu-id="842ed-112">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="842ed-113">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="842ed-113">Relationships</span></span>
<span data-ttu-id="842ed-114">なし</span><span class="sxs-lookup"><span data-stu-id="842ed-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="842ed-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="842ed-115">JSON Representation</span></span>
<span data-ttu-id="842ed-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="842ed-116">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenItem",
  "displayName": "String"
}
```



