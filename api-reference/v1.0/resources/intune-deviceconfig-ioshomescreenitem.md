---
title: iosHomeScreenItem リソースの種類
description: IOS ホーム画面上のアイテムを表します
ms.openlocfilehash: 57d6e3c748b99dce88f195ed6906e14fdf80157f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020223"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="13067-103">iosHomeScreenItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="13067-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="13067-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="13067-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="13067-105">IOS ホーム画面上のアイテムを表します</span><span class="sxs-lookup"><span data-stu-id="13067-105">Represents an item on the iOS Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="13067-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13067-106">Properties</span></span>
|<span data-ttu-id="13067-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13067-107">Property</span></span>|<span data-ttu-id="13067-108">型</span><span class="sxs-lookup"><span data-stu-id="13067-108">Type</span></span>|<span data-ttu-id="13067-109">説明</span><span class="sxs-lookup"><span data-stu-id="13067-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13067-110">displayName</span><span class="sxs-lookup"><span data-stu-id="13067-110">displayName</span></span>|<span data-ttu-id="13067-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="13067-111">String</span></span>|<span data-ttu-id="13067-112">アプリの名前</span><span class="sxs-lookup"><span data-stu-id="13067-112">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="13067-113">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="13067-113">Relationships</span></span>
<span data-ttu-id="13067-114">なし</span><span class="sxs-lookup"><span data-stu-id="13067-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="13067-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="13067-115">JSON Representation</span></span>
<span data-ttu-id="13067-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="13067-116">Here is a JSON representation of the resource.</span></span>
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



