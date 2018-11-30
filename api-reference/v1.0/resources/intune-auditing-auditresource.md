---
title: auditResource リソースの種類
description: 監査のリソースのプロパティが含まれるクラス。
ms.openlocfilehash: 452df4cb27dba5de04022c6ba7be08471286d866
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023203"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="b5576-103">auditResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b5576-103">auditResource resource type</span></span>

> <span data-ttu-id="b5576-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b5576-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b5576-105">監査のリソースのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="b5576-105">A class containing the properties for Audit Resource.</span></span>
## <a name="properties"></a><span data-ttu-id="b5576-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b5576-106">Properties</span></span>
|<span data-ttu-id="b5576-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b5576-107">Property</span></span>|<span data-ttu-id="b5576-108">型</span><span class="sxs-lookup"><span data-stu-id="b5576-108">Type</span></span>|<span data-ttu-id="b5576-109">説明</span><span class="sxs-lookup"><span data-stu-id="b5576-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5576-110">displayName</span><span class="sxs-lookup"><span data-stu-id="b5576-110">displayName</span></span>|<span data-ttu-id="b5576-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b5576-111">String</span></span>|<span data-ttu-id="b5576-112">表示名。</span><span class="sxs-lookup"><span data-stu-id="b5576-112">Display name.</span></span>|
|<span data-ttu-id="b5576-113">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="b5576-113">modifiedProperties</span></span>|<span data-ttu-id="b5576-114">[auditProperty](../resources/intune-auditing-auditproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b5576-114">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="b5576-115">変更されたプロパティの一覧。</span><span class="sxs-lookup"><span data-stu-id="b5576-115">List of modified properties.</span></span>|
|<span data-ttu-id="b5576-116">type</span><span class="sxs-lookup"><span data-stu-id="b5576-116">type</span></span>|<span data-ttu-id="b5576-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b5576-117">String</span></span>|<span data-ttu-id="b5576-118">監査のリソースの種類。</span><span class="sxs-lookup"><span data-stu-id="b5576-118">Audit resource's type.</span></span>|
|<span data-ttu-id="b5576-119">resourceId</span><span class="sxs-lookup"><span data-stu-id="b5576-119">resourceId</span></span>|<span data-ttu-id="b5576-120">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b5576-120">String</span></span>|<span data-ttu-id="b5576-121">監査のリソースの ID。</span><span class="sxs-lookup"><span data-stu-id="b5576-121">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5576-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b5576-122">Relationships</span></span>
<span data-ttu-id="b5576-123">なし</span><span class="sxs-lookup"><span data-stu-id="b5576-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b5576-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b5576-124">JSON Representation</span></span>
<span data-ttu-id="b5576-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b5576-125">Here is a JSON representation of the resource.</span></span>
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



