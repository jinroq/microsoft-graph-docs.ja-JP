---
title: resourceAction リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 17d8bd52996ca9b129292c204dd498fcc5a65ac6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963242"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="c22bf-103">resourceAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c22bf-103">resourceAction resource type</span></span>

> <span data-ttu-id="c22bf-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c22bf-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c22bf-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c22bf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c22bf-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c22bf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c22bf-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c22bf-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="c22bf-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c22bf-108">Properties</span></span>
|<span data-ttu-id="c22bf-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c22bf-109">Property</span></span>|<span data-ttu-id="c22bf-110">種類</span><span class="sxs-lookup"><span data-stu-id="c22bf-110">Type</span></span>|<span data-ttu-id="c22bf-111">説明</span><span class="sxs-lookup"><span data-stu-id="c22bf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c22bf-112">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="c22bf-112">allowedResourceActions</span></span>|<span data-ttu-id="c22bf-113">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="c22bf-113">String collection</span></span>|<span data-ttu-id="c22bf-114">許可されるアクション</span><span class="sxs-lookup"><span data-stu-id="c22bf-114">Allowed Actions</span></span>|
|<span data-ttu-id="c22bf-115">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="c22bf-115">notAllowedResourceActions</span></span>|<span data-ttu-id="c22bf-116">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="c22bf-116">String collection</span></span>|<span data-ttu-id="c22bf-117">許可されていないアクション</span><span class="sxs-lookup"><span data-stu-id="c22bf-117">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="c22bf-118">関係</span><span class="sxs-lookup"><span data-stu-id="c22bf-118">Relationships</span></span>
<span data-ttu-id="c22bf-119">なし</span><span class="sxs-lookup"><span data-stu-id="c22bf-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c22bf-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c22bf-120">JSON Representation</span></span>
<span data-ttu-id="c22bf-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c22bf-121">Here is a JSON representation of the resource.</span></span>
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





