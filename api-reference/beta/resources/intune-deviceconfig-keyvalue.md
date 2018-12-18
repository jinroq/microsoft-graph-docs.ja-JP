---
title: keyValue リソースの種類
description: キー値の定義。
author: tfitzmac
ms.openlocfilehash: 5e5754657e679f3a703c2b5dec7cea36d1bad860
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302640"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="4a56a-103">keyValue リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4a56a-103">keyValue resource type</span></span>

> <span data-ttu-id="4a56a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4a56a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4a56a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a56a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4a56a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4a56a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4a56a-107">キー値の定義。</span><span class="sxs-lookup"><span data-stu-id="4a56a-107">Key Value definition.</span></span>
## <a name="properties"></a><span data-ttu-id="4a56a-108">Properties</span><span class="sxs-lookup"><span data-stu-id="4a56a-108">Properties</span></span>
|<span data-ttu-id="4a56a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4a56a-109">Property</span></span>|<span data-ttu-id="4a56a-110">種類</span><span class="sxs-lookup"><span data-stu-id="4a56a-110">Type</span></span>|<span data-ttu-id="4a56a-111">説明</span><span class="sxs-lookup"><span data-stu-id="4a56a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a56a-112">Key</span><span class="sxs-lookup"><span data-stu-id="4a56a-112">key</span></span>|<span data-ttu-id="4a56a-113">String</span><span class="sxs-lookup"><span data-stu-id="4a56a-113">String</span></span>|<span data-ttu-id="4a56a-114">キー。</span><span class="sxs-lookup"><span data-stu-id="4a56a-114">Key.</span></span>|
|<span data-ttu-id="4a56a-115">value</span><span class="sxs-lookup"><span data-stu-id="4a56a-115">value</span></span>|<span data-ttu-id="4a56a-116">文字列</span><span class="sxs-lookup"><span data-stu-id="4a56a-116">String</span></span>|<span data-ttu-id="4a56a-117">値。</span><span class="sxs-lookup"><span data-stu-id="4a56a-117">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a56a-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4a56a-118">Relationships</span></span>
<span data-ttu-id="4a56a-119">なし</span><span class="sxs-lookup"><span data-stu-id="4a56a-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4a56a-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4a56a-120">JSON Representation</span></span>
<span data-ttu-id="4a56a-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4a56a-121">Here is a JSON representation of the resource.</span></span>
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





