---
title: resourceAction リソースの種類
description: まだ文書化されていません
ms.openlocfilehash: 4cbfc149207f2f7589bd7e05075326641d4e8b67
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020297"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="3d203-103">resourceAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3d203-103">resourceAction resource type</span></span>

> <span data-ttu-id="3d203-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3d203-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3d203-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3d203-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="3d203-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3d203-106">Properties</span></span>
|<span data-ttu-id="3d203-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3d203-107">Property</span></span>|<span data-ttu-id="3d203-108">型</span><span class="sxs-lookup"><span data-stu-id="3d203-108">Type</span></span>|<span data-ttu-id="3d203-109">説明</span><span class="sxs-lookup"><span data-stu-id="3d203-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d203-110">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="3d203-110">allowedResourceActions</span></span>|<span data-ttu-id="3d203-111">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="3d203-111">String collection</span></span>|<span data-ttu-id="3d203-112">許可されるアクション</span><span class="sxs-lookup"><span data-stu-id="3d203-112">Allowed Actions</span></span>|
|<span data-ttu-id="3d203-113">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="3d203-113">notAllowedResourceActions</span></span>|<span data-ttu-id="3d203-114">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="3d203-114">String collection</span></span>|<span data-ttu-id="3d203-115">許可されていないアクション</span><span class="sxs-lookup"><span data-stu-id="3d203-115">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d203-116">関係</span><span class="sxs-lookup"><span data-stu-id="3d203-116">Relationships</span></span>
<span data-ttu-id="3d203-117">なし</span><span class="sxs-lookup"><span data-stu-id="3d203-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3d203-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3d203-118">JSON Representation</span></span>
<span data-ttu-id="3d203-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3d203-119">Here is a JSON representation of the resource.</span></span>
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



