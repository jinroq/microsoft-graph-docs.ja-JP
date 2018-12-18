---
title: iosHomeScreenItem リソースの種類
description: IOS ホーム画面上のアイテムを表します
author: tfitzmac
ms.openlocfilehash: 168214da57f2cc903bac110709d721061d4298cd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362518"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="67657-103">iosHomeScreenItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="67657-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="67657-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="67657-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="67657-105">IOS ホーム画面上のアイテムを表します</span><span class="sxs-lookup"><span data-stu-id="67657-105">Represents an item on the iOS Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="67657-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="67657-106">Properties</span></span>
|<span data-ttu-id="67657-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="67657-107">Property</span></span>|<span data-ttu-id="67657-108">種類</span><span class="sxs-lookup"><span data-stu-id="67657-108">Type</span></span>|<span data-ttu-id="67657-109">説明</span><span class="sxs-lookup"><span data-stu-id="67657-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67657-110">displayName</span><span class="sxs-lookup"><span data-stu-id="67657-110">displayName</span></span>|<span data-ttu-id="67657-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="67657-111">String</span></span>|<span data-ttu-id="67657-112">アプリの名前</span><span class="sxs-lookup"><span data-stu-id="67657-112">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="67657-113">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="67657-113">Relationships</span></span>
<span data-ttu-id="67657-114">なし</span><span class="sxs-lookup"><span data-stu-id="67657-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="67657-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="67657-115">JSON Representation</span></span>
<span data-ttu-id="67657-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="67657-116">Here is a JSON representation of the resource.</span></span>
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



