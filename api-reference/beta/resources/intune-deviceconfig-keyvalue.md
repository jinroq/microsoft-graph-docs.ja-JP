---
title: keyValue リソースの種類
description: キー値の定義。
ms.openlocfilehash: 7279b48243139b9234b737ceb7d7fb1ad7232451
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068907"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="98867-103">keyValue リソースの種類</span><span class="sxs-lookup"><span data-stu-id="98867-103">keyValue resource type</span></span>

> <span data-ttu-id="98867-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="98867-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="98867-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="98867-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="98867-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="98867-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="98867-107">キー値の定義。</span><span class="sxs-lookup"><span data-stu-id="98867-107">Key Value definition.</span></span>
## <a name="properties"></a><span data-ttu-id="98867-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="98867-108">Properties</span></span>
|<span data-ttu-id="98867-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="98867-109">Property</span></span>|<span data-ttu-id="98867-110">型</span><span class="sxs-lookup"><span data-stu-id="98867-110">Type</span></span>|<span data-ttu-id="98867-111">説明</span><span class="sxs-lookup"><span data-stu-id="98867-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98867-112">Key</span><span class="sxs-lookup"><span data-stu-id="98867-112">key</span></span>|<span data-ttu-id="98867-113">String</span><span class="sxs-lookup"><span data-stu-id="98867-113">String</span></span>|<span data-ttu-id="98867-114">キー。</span><span class="sxs-lookup"><span data-stu-id="98867-114">Key.</span></span>|
|<span data-ttu-id="98867-115">value</span><span class="sxs-lookup"><span data-stu-id="98867-115">value</span></span>|<span data-ttu-id="98867-116">文字列</span><span class="sxs-lookup"><span data-stu-id="98867-116">String</span></span>|<span data-ttu-id="98867-117">値。</span><span class="sxs-lookup"><span data-stu-id="98867-117">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="98867-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="98867-118">Relationships</span></span>
<span data-ttu-id="98867-119">なし</span><span class="sxs-lookup"><span data-stu-id="98867-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="98867-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="98867-120">JSON Representation</span></span>
<span data-ttu-id="98867-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="98867-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValue",
  "key": "String",
  "value": "String"
}
```





