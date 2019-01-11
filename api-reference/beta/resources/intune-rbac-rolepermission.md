---
title: rolePermission リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0669a0e169a71ea3806b21a125a4921b5161d516
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855574"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="40df9-103">rolePermission リソースの種類</span><span class="sxs-lookup"><span data-stu-id="40df9-103">rolePermission resource type</span></span>

> <span data-ttu-id="40df9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="40df9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="40df9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40df9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="40df9-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="40df9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="40df9-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="40df9-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="40df9-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="40df9-108">Properties</span></span>
|<span data-ttu-id="40df9-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="40df9-109">Property</span></span>|<span data-ttu-id="40df9-110">種類</span><span class="sxs-lookup"><span data-stu-id="40df9-110">Type</span></span>|<span data-ttu-id="40df9-111">説明</span><span class="sxs-lookup"><span data-stu-id="40df9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40df9-112">actions</span><span class="sxs-lookup"><span data-stu-id="40df9-112">actions</span></span>|<span data-ttu-id="40df9-113">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="40df9-113">String collection</span></span>|<span data-ttu-id="40df9-114">許可されるアクション</span><span class="sxs-lookup"><span data-stu-id="40df9-114">Allowed Actions</span></span>|
|<span data-ttu-id="40df9-115">resourceActions</span><span class="sxs-lookup"><span data-stu-id="40df9-115">resourceActions</span></span>|<span data-ttu-id="40df9-116">[resourceAction](../resources/intune-rbac-resourceaction.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="40df9-116">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="40df9-117">アクション</span><span class="sxs-lookup"><span data-stu-id="40df9-117">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="40df9-118">関係</span><span class="sxs-lookup"><span data-stu-id="40df9-118">Relationships</span></span>
<span data-ttu-id="40df9-119">なし</span><span class="sxs-lookup"><span data-stu-id="40df9-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="40df9-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="40df9-120">JSON Representation</span></span>
<span data-ttu-id="40df9-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="40df9-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rolePermission"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rolePermission",
  "actions": [
    "String"
  ],
  "resourceActions": [
    {
      "@odata.type": "microsoft.graph.resourceAction",
      "allowedResourceActions": [
        "String"
      ],
      "notAllowedResourceActions": [
        "String"
      ]
    }
  ]
}
```





