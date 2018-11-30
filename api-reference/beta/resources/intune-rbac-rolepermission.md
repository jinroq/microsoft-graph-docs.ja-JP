---
title: rolePermission リソースの種類
description: まだ文書化されていません
ms.openlocfilehash: 350cfe6c220d73b14464a761c3b8a469f57ab352
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071699"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="1e021-103">rolePermission リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1e021-103">rolePermission resource type</span></span>

> <span data-ttu-id="1e021-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1e021-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e021-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e021-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1e021-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1e021-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1e021-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1e021-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="1e021-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e021-108">Properties</span></span>
|<span data-ttu-id="1e021-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e021-109">Property</span></span>|<span data-ttu-id="1e021-110">型</span><span class="sxs-lookup"><span data-stu-id="1e021-110">Type</span></span>|<span data-ttu-id="1e021-111">説明</span><span class="sxs-lookup"><span data-stu-id="1e021-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e021-112">actions</span><span class="sxs-lookup"><span data-stu-id="1e021-112">actions</span></span>|<span data-ttu-id="1e021-113">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="1e021-113">String collection</span></span>|<span data-ttu-id="1e021-114">許可されるアクション</span><span class="sxs-lookup"><span data-stu-id="1e021-114">Allowed Actions</span></span>|
|<span data-ttu-id="1e021-115">resourceActions</span><span class="sxs-lookup"><span data-stu-id="1e021-115">resourceActions</span></span>|<span data-ttu-id="1e021-116">[resourceAction](../resources/intune-rbac-resourceaction.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1e021-116">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="1e021-117">アクション</span><span class="sxs-lookup"><span data-stu-id="1e021-117">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e021-118">関係</span><span class="sxs-lookup"><span data-stu-id="1e021-118">Relationships</span></span>
<span data-ttu-id="1e021-119">なし</span><span class="sxs-lookup"><span data-stu-id="1e021-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1e021-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1e021-120">JSON Representation</span></span>
<span data-ttu-id="1e021-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1e021-121">Here is a JSON representation of the resource.</span></span>
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





