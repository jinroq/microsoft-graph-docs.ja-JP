---
title: iosHomeScreenItem リソースの種類
description: IOS ホーム画面上のアイテムを表します
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ff573a6f7ae0d78113a32514bc312c3920b216f1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987623"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="91f9f-103">iosHomeScreenItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="91f9f-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="91f9f-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="91f9f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="91f9f-105">IOS ホーム画面上のアイテムを表します</span><span class="sxs-lookup"><span data-stu-id="91f9f-105">Represents an item on the iOS Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="91f9f-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91f9f-106">Properties</span></span>
|<span data-ttu-id="91f9f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91f9f-107">Property</span></span>|<span data-ttu-id="91f9f-108">種類</span><span class="sxs-lookup"><span data-stu-id="91f9f-108">Type</span></span>|<span data-ttu-id="91f9f-109">説明</span><span class="sxs-lookup"><span data-stu-id="91f9f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91f9f-110">displayName</span><span class="sxs-lookup"><span data-stu-id="91f9f-110">displayName</span></span>|<span data-ttu-id="91f9f-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="91f9f-111">String</span></span>|<span data-ttu-id="91f9f-112">アプリの名前</span><span class="sxs-lookup"><span data-stu-id="91f9f-112">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="91f9f-113">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="91f9f-113">Relationships</span></span>
<span data-ttu-id="91f9f-114">なし</span><span class="sxs-lookup"><span data-stu-id="91f9f-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="91f9f-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="91f9f-115">JSON Representation</span></span>
<span data-ttu-id="91f9f-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="91f9f-116">Here is a JSON representation of the resource.</span></span>
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



