---
title: auditResource リソースの種類
description: 監査のリソースのプロパティが含まれるクラス。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7f8fc3a96b3d17759e1e65eaa17c6571e4cec347
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844738"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="867d1-103">auditResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="867d1-103">auditResource resource type</span></span>

> <span data-ttu-id="867d1-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="867d1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="867d1-105">監査のリソースのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="867d1-105">A class containing the properties for Audit Resource.</span></span>
## <a name="properties"></a><span data-ttu-id="867d1-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="867d1-106">Properties</span></span>
|<span data-ttu-id="867d1-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="867d1-107">Property</span></span>|<span data-ttu-id="867d1-108">種類</span><span class="sxs-lookup"><span data-stu-id="867d1-108">Type</span></span>|<span data-ttu-id="867d1-109">説明</span><span class="sxs-lookup"><span data-stu-id="867d1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="867d1-110">displayName</span><span class="sxs-lookup"><span data-stu-id="867d1-110">displayName</span></span>|<span data-ttu-id="867d1-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="867d1-111">String</span></span>|<span data-ttu-id="867d1-112">表示名。</span><span class="sxs-lookup"><span data-stu-id="867d1-112">Display name.</span></span>|
|<span data-ttu-id="867d1-113">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="867d1-113">modifiedProperties</span></span>|<span data-ttu-id="867d1-114">[auditProperty](../resources/intune-auditing-auditproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="867d1-114">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="867d1-115">変更されたプロパティの一覧。</span><span class="sxs-lookup"><span data-stu-id="867d1-115">List of modified properties.</span></span>|
|<span data-ttu-id="867d1-116">type</span><span class="sxs-lookup"><span data-stu-id="867d1-116">type</span></span>|<span data-ttu-id="867d1-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="867d1-117">String</span></span>|<span data-ttu-id="867d1-118">監査のリソースの種類。</span><span class="sxs-lookup"><span data-stu-id="867d1-118">Audit resource's type.</span></span>|
|<span data-ttu-id="867d1-119">resourceId</span><span class="sxs-lookup"><span data-stu-id="867d1-119">resourceId</span></span>|<span data-ttu-id="867d1-120">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="867d1-120">String</span></span>|<span data-ttu-id="867d1-121">監査のリソースの ID。</span><span class="sxs-lookup"><span data-stu-id="867d1-121">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="867d1-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="867d1-122">Relationships</span></span>
<span data-ttu-id="867d1-123">なし</span><span class="sxs-lookup"><span data-stu-id="867d1-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="867d1-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="867d1-124">JSON Representation</span></span>
<span data-ttu-id="867d1-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="867d1-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditResource",
  "displayName": "String",
  "modifiedProperties": [
    {
      "@odata.type": "microsoft.graph.auditProperty",
      "displayName": "String",
      "oldValue": "String",
      "newValue": "String"
    }
  ],
  "type": "String",
  "resourceId": "String"
}
```



