---
title: windowsInformationProtectionResourceCollection リソースの種類
description: Windows 情報保護のリソース コレクション
author: tfitzmac
ms.openlocfilehash: 8e037ff53e11566aee7d79d2c3bbe5b1075b83a6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327833"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="7f49a-103">windowsInformationProtectionResourceCollection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7f49a-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="7f49a-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7f49a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7f49a-105">Windows 情報保護のリソース コレクション</span><span class="sxs-lookup"><span data-stu-id="7f49a-105">Windows Information Protection Resource Collection</span></span>
## <a name="properties"></a><span data-ttu-id="7f49a-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f49a-106">Properties</span></span>
|<span data-ttu-id="7f49a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f49a-107">Property</span></span>|<span data-ttu-id="7f49a-108">種類</span><span class="sxs-lookup"><span data-stu-id="7f49a-108">Type</span></span>|<span data-ttu-id="7f49a-109">説明</span><span class="sxs-lookup"><span data-stu-id="7f49a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f49a-110">displayName</span><span class="sxs-lookup"><span data-stu-id="7f49a-110">displayName</span></span>|<span data-ttu-id="7f49a-111">文字列</span><span class="sxs-lookup"><span data-stu-id="7f49a-111">String</span></span>|<span data-ttu-id="7f49a-112">表示名</span><span class="sxs-lookup"><span data-stu-id="7f49a-112">Display name</span></span>|
|<span data-ttu-id="7f49a-113">リソース</span><span class="sxs-lookup"><span data-stu-id="7f49a-113">resources</span></span>|<span data-ttu-id="7f49a-114">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="7f49a-114">String collection</span></span>|<span data-ttu-id="7f49a-115">リソースのコレクション</span><span class="sxs-lookup"><span data-stu-id="7f49a-115">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f49a-116">関係</span><span class="sxs-lookup"><span data-stu-id="7f49a-116">Relationships</span></span>
<span data-ttu-id="7f49a-117">なし</span><span class="sxs-lookup"><span data-stu-id="7f49a-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7f49a-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7f49a-118">JSON Representation</span></span>
<span data-ttu-id="7f49a-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7f49a-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionResourceCollection",
  "displayName": "String",
  "resources": [
    "String"
  ]
}
```



