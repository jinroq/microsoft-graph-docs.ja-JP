---
title: resourceAction リソースの種類
description: まだ文書化されていません
ms.openlocfilehash: d4f585ec52096cc9bd6d1430825d61426df644fe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070900"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="f9adf-103">resourceAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f9adf-103">resourceAction resource type</span></span>

> <span data-ttu-id="f9adf-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f9adf-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9adf-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f9adf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f9adf-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f9adf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f9adf-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f9adf-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="f9adf-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f9adf-108">Properties</span></span>
|<span data-ttu-id="f9adf-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f9adf-109">Property</span></span>|<span data-ttu-id="f9adf-110">型</span><span class="sxs-lookup"><span data-stu-id="f9adf-110">Type</span></span>|<span data-ttu-id="f9adf-111">説明</span><span class="sxs-lookup"><span data-stu-id="f9adf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9adf-112">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="f9adf-112">allowedResourceActions</span></span>|<span data-ttu-id="f9adf-113">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="f9adf-113">String collection</span></span>|<span data-ttu-id="f9adf-114">許可されるアクション</span><span class="sxs-lookup"><span data-stu-id="f9adf-114">Allowed Actions</span></span>|
|<span data-ttu-id="f9adf-115">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="f9adf-115">notAllowedResourceActions</span></span>|<span data-ttu-id="f9adf-116">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="f9adf-116">String collection</span></span>|<span data-ttu-id="f9adf-117">許可されていないアクション</span><span class="sxs-lookup"><span data-stu-id="f9adf-117">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9adf-118">関係</span><span class="sxs-lookup"><span data-stu-id="f9adf-118">Relationships</span></span>
<span data-ttu-id="f9adf-119">なし</span><span class="sxs-lookup"><span data-stu-id="f9adf-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f9adf-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f9adf-120">JSON Representation</span></span>
<span data-ttu-id="f9adf-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f9adf-121">Here is a JSON representation of the resource.</span></span>
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





