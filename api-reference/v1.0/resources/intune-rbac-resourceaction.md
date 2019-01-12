---
title: resourceAction リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f1db2a1db2c76829ddd39438ed40cd1086fe4e17
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932714"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="afbce-103">resourceAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="afbce-103">resourceAction resource type</span></span>

> <span data-ttu-id="afbce-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="afbce-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="afbce-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="afbce-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="afbce-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="afbce-106">Properties</span></span>
|<span data-ttu-id="afbce-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="afbce-107">Property</span></span>|<span data-ttu-id="afbce-108">種類</span><span class="sxs-lookup"><span data-stu-id="afbce-108">Type</span></span>|<span data-ttu-id="afbce-109">説明</span><span class="sxs-lookup"><span data-stu-id="afbce-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afbce-110">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="afbce-110">allowedResourceActions</span></span>|<span data-ttu-id="afbce-111">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="afbce-111">String collection</span></span>|<span data-ttu-id="afbce-112">許可されるアクション</span><span class="sxs-lookup"><span data-stu-id="afbce-112">Allowed Actions</span></span>|
|<span data-ttu-id="afbce-113">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="afbce-113">notAllowedResourceActions</span></span>|<span data-ttu-id="afbce-114">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="afbce-114">String collection</span></span>|<span data-ttu-id="afbce-115">許可されていないアクション</span><span class="sxs-lookup"><span data-stu-id="afbce-115">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="afbce-116">関係</span><span class="sxs-lookup"><span data-stu-id="afbce-116">Relationships</span></span>
<span data-ttu-id="afbce-117">なし</span><span class="sxs-lookup"><span data-stu-id="afbce-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="afbce-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="afbce-118">JSON Representation</span></span>
<span data-ttu-id="afbce-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="afbce-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```



