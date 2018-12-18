---
title: resourceAction リソースの種類
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: c373cc15b1dfce1ca3cede9fa1c7a642da48f5bf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319160"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="7f8ae-103">resourceAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7f8ae-103">resourceAction resource type</span></span>

> <span data-ttu-id="7f8ae-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7f8ae-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7f8ae-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f8ae-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7f8ae-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7f8ae-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7f8ae-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7f8ae-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="7f8ae-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f8ae-108">Properties</span></span>
|<span data-ttu-id="7f8ae-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f8ae-109">Property</span></span>|<span data-ttu-id="7f8ae-110">種類</span><span class="sxs-lookup"><span data-stu-id="7f8ae-110">Type</span></span>|<span data-ttu-id="7f8ae-111">説明</span><span class="sxs-lookup"><span data-stu-id="7f8ae-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f8ae-112">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="7f8ae-112">allowedResourceActions</span></span>|<span data-ttu-id="7f8ae-113">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="7f8ae-113">String collection</span></span>|<span data-ttu-id="7f8ae-114">許可されるアクション</span><span class="sxs-lookup"><span data-stu-id="7f8ae-114">Allowed Actions</span></span>|
|<span data-ttu-id="7f8ae-115">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="7f8ae-115">notAllowedResourceActions</span></span>|<span data-ttu-id="7f8ae-116">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="7f8ae-116">String collection</span></span>|<span data-ttu-id="7f8ae-117">許可されていないアクション</span><span class="sxs-lookup"><span data-stu-id="7f8ae-117">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f8ae-118">関係</span><span class="sxs-lookup"><span data-stu-id="7f8ae-118">Relationships</span></span>
<span data-ttu-id="7f8ae-119">なし</span><span class="sxs-lookup"><span data-stu-id="7f8ae-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7f8ae-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7f8ae-120">JSON Representation</span></span>
<span data-ttu-id="7f8ae-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7f8ae-121">Here is a JSON representation of the resource.</span></span>
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





