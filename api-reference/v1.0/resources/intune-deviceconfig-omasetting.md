---
title: omaSetting リソースの種類
description: OMA 設定の定義。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 42b6d5fcea7b3b46acf8d0a119213f679d99aed6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961485"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="c4c16-103">omaSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c4c16-103">omaSetting resource type</span></span>

> <span data-ttu-id="c4c16-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c4c16-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c4c16-105">OMA 設定の定義。</span><span class="sxs-lookup"><span data-stu-id="c4c16-105">OMA Settings definition.</span></span>
## <a name="properties"></a><span data-ttu-id="c4c16-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c4c16-106">Properties</span></span>
|<span data-ttu-id="c4c16-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c4c16-107">Property</span></span>|<span data-ttu-id="c4c16-108">種類</span><span class="sxs-lookup"><span data-stu-id="c4c16-108">Type</span></span>|<span data-ttu-id="c4c16-109">説明</span><span class="sxs-lookup"><span data-stu-id="c4c16-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4c16-110">displayName</span><span class="sxs-lookup"><span data-stu-id="c4c16-110">displayName</span></span>|<span data-ttu-id="c4c16-111">文字列</span><span class="sxs-lookup"><span data-stu-id="c4c16-111">String</span></span>|<span data-ttu-id="c4c16-112">表示名。</span><span class="sxs-lookup"><span data-stu-id="c4c16-112">Display Name.</span></span>|
|<span data-ttu-id="c4c16-113">説明</span><span class="sxs-lookup"><span data-stu-id="c4c16-113">description</span></span>|<span data-ttu-id="c4c16-114">String</span><span class="sxs-lookup"><span data-stu-id="c4c16-114">String</span></span>|<span data-ttu-id="c4c16-115">説明。</span><span class="sxs-lookup"><span data-stu-id="c4c16-115">Description.</span></span>|
|<span data-ttu-id="c4c16-116">omaUri</span><span class="sxs-lookup"><span data-stu-id="c4c16-116">omaUri</span></span>|<span data-ttu-id="c4c16-117">文字列</span><span class="sxs-lookup"><span data-stu-id="c4c16-117">String</span></span>|<span data-ttu-id="c4c16-118">OMA。</span><span class="sxs-lookup"><span data-stu-id="c4c16-118">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c4c16-119">関係</span><span class="sxs-lookup"><span data-stu-id="c4c16-119">Relationships</span></span>
<span data-ttu-id="c4c16-120">なし</span><span class="sxs-lookup"><span data-stu-id="c4c16-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c4c16-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c4c16-121">JSON Representation</span></span>
<span data-ttu-id="c4c16-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c4c16-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String"
}
```



